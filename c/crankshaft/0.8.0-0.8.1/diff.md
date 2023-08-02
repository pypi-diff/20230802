# Comparing `tmp/crankshaft-0.8.0.tar.gz` & `tmp/crankshaft-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crankshaft-0.8.0.tar", max compression
+gzip compressed data, was "crankshaft-0.8.1.tar", max compression
```

## Comparing `crankshaft-0.8.0.tar` & `crankshaft-0.8.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1067 2023-07-16 23:42:31.027788 crankshaft-0.8.0/LICENSE
--rw-r--r--   0        0        0     1564 2023-07-16 23:42:31.027788 crankshaft-0.8.0/README.md
--rw-r--r--   0        0        0      326 2023-07-16 23:43:31.042436 crankshaft-0.8.0/crankshaft/__init__.py
--rw-r--r--   0        0        0      132 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/api.bolt
--rw-r--r--   0        0        0      216 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/config.bolt
--rw-r--r--   0        0        0      513 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/defer.bolt
--rw-r--r--   0        0        0     3872 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/event_handler.bolt
--rw-r--r--   0        0        0     1605 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_entity_attack_player.bolt
--rw-r--r--   0        0        0      207 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_load.bolt
--rw-r--r--   0        0        0      566 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_airborne.bolt
--rw-r--r--   0        0        0      831 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_airborne_end.bolt
--rw-r--r--   0        0        0      646 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_airborne_start.bolt
--rw-r--r--   0        0        0     1605 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_attack_entity.bolt
--rw-r--r--   0        0        0      328 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_burn.bolt
--rw-r--r--   0        0        0      629 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_burn_end.bolt
--rw-r--r--   0        0        0      632 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_burn_start.bolt
--rw-r--r--   0        0        0      589 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_charge_bow.bolt
--rw-r--r--   0        0        0      975 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_charge_bow_end.bolt
--rw-r--r--   0        0        0      665 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_charge_bow_start.bolt
--rw-r--r--   0        0        0      332 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_glide.bolt
--rw-r--r--   0        0        0      632 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_glide_end.bolt
--rw-r--r--   0        0        0      636 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_glide_start.bolt
--rw-r--r--   0        0        0      677 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_inventory_change.bolt
--rw-r--r--   0        0        0      501 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_join.bolt
--rw-r--r--   0        0        0      495 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_jump.bolt
--rw-r--r--   0        0        0      608 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_land.bolt
--rw-r--r--   0        0        0      471 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_load.bolt
--rw-r--r--   0        0        0      748 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_shoot_bow.bolt
--rw-r--r--   0        0        0      335 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_sneak.bolt
--rw-r--r--   0        0        0      635 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_sneak_end.bolt
--rw-r--r--   0        0        0      638 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_sneak_start.bolt
--rw-r--r--   0        0        0      341 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_sprint.bolt
--rw-r--r--   0        0        0      642 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_sprint_end.bolt
--rw-r--r--   0        0        0      644 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_sprint_start.bolt
--rw-r--r--   0        0        0      332 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_swim.bolt
--rw-r--r--   0        0        0      632 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_swim_end.bolt
--rw-r--r--   0        0        0      635 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_swim_start.bolt
--rw-r--r--   0        0        0      263 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_tick.bolt
--rw-r--r--   0        0        0      558 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_use_coas.bolt
--rw-r--r--   0        0        0      573 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_player_use_wfoas.bolt
--rw-r--r--   0        0        0      207 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events/on_tick.bolt
--rw-r--r--   0        0        0     2118 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/events.bolt
--rw-r--r--   0        0        0     3398 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flag.bolt
--rw-r--r--   0        0        0      377 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags/is_airborne.bolt
--rw-r--r--   0        0        0      402 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags/is_baby.bolt
--rw-r--r--   0        0        0      411 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags/is_burning.bolt
--rw-r--r--   0        0        0     1258 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags/is_charging_bow.bolt
--rw-r--r--   0        0        0      377 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags/is_gliding.bolt
--rw-r--r--   0        0        0      379 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags/is_in_ground.bolt
--rw-r--r--   0        0        0      379 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags/is_on_ground.bolt
--rw-r--r--   0        0        0      158 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags/is_player.bolt
--rw-r--r--   0        0        0      414 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags/is_sneaking.bolt
--rw-r--r--   0        0        0      417 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags/is_sprinting.bolt
--rw-r--r--   0        0        0      414 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags/is_swimming.bolt
--rw-r--r--   0        0        0      535 2023-07-16 23:42:31.027788 crankshaft-0.8.0/crankshaft/modules/flags.bolt
--rw-r--r--   0        0        0      443 2023-07-16 23:42:31.031788 crankshaft-0.8.0/crankshaft/modules/lib/entity_hit_matching/api.bolt
--rw-r--r--   0        0        0      124 2023-07-16 23:42:31.031788 crankshaft-0.8.0/crankshaft/modules/lib/entity_hit_matching/credits.txt
--rw-r--r--   0        0        0    58171 2023-07-16 23:42:31.031788 crankshaft-0.8.0/crankshaft/modules/lib/entity_hit_matching/main.bolt
--rw-r--r--   0        0        0      207 2023-07-16 23:42:31.031788 crankshaft-0.8.0/crankshaft/modules/utils.bolt
--rw-r--r--   0        0        0        0 2023-07-16 23:42:31.031788 crankshaft-0.8.0/crankshaft/py.typed
--rw-r--r--   0        0        0     1329 2023-07-16 23:43:31.066437 crankshaft-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 crankshaft-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-02 19:10:02.901745 crankshaft-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1564 2023-08-02 19:10:02.901745 crankshaft-0.8.1/README.md
+-rw-r--r--   0        0        0      326 2023-08-02 19:11:42.863354 crankshaft-0.8.1/crankshaft/__init__.py
+-rw-r--r--   0        0        0      132 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/api.bolt
+-rw-r--r--   0        0        0      216 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/config.bolt
+-rw-r--r--   0        0        0      513 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/defer.bolt
+-rw-r--r--   0        0        0     3872 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/event_handler.bolt
+-rw-r--r--   0        0        0     1603 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_entity_attack_player.bolt
+-rw-r--r--   0        0        0      205 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_load.bolt
+-rw-r--r--   0        0        0      634 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_airborne.bolt
+-rw-r--r--   0        0        0      902 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_airborne_end.bolt
+-rw-r--r--   0        0        0      644 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_airborne_start.bolt
+-rw-r--r--   0        0        0     1603 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_attack_entity.bolt
+-rw-r--r--   0        0        0      327 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_burn.bolt
+-rw-r--r--   0        0        0      627 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_burn_end.bolt
+-rw-r--r--   0        0        0      630 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_burn_start.bolt
+-rw-r--r--   0        0        0      655 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_charge_bow.bolt
+-rw-r--r--   0        0        0     1049 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_charge_bow_end.bolt
+-rw-r--r--   0        0        0      663 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_charge_bow_start.bolt
+-rw-r--r--   0        0        0      330 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_glide.bolt
+-rw-r--r--   0        0        0      630 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_glide_end.bolt
+-rw-r--r--   0        0        0      634 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_glide_start.bolt
+-rw-r--r--   0        0        0      674 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_inventory_change.bolt
+-rw-r--r--   0        0        0      499 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_join.bolt
+-rw-r--r--   0        0        0      493 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_jump.bolt
+-rw-r--r--   0        0        0      606 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_land.bolt
+-rw-r--r--   0        0        0      469 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_load.bolt
+-rw-r--r--   0        0        0      813 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_shoot_bow.bolt
+-rw-r--r--   0        0        0      333 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_sneak.bolt
+-rw-r--r--   0        0        0      633 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_sneak_end.bolt
+-rw-r--r--   0        0        0      636 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_sneak_start.bolt
+-rw-r--r--   0        0        0      339 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_sprint.bolt
+-rw-r--r--   0        0        0      640 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_sprint_end.bolt
+-rw-r--r--   0        0        0      642 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_sprint_start.bolt
+-rw-r--r--   0        0        0      330 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_swim.bolt
+-rw-r--r--   0        0        0      630 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_swim_end.bolt
+-rw-r--r--   0        0        0      634 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_swim_start.bolt
+-rw-r--r--   0        0        0      261 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_tick.bolt
+-rw-r--r--   0        0        0      556 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_use_coas.bolt
+-rw-r--r--   0        0        0      571 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_player_use_wfoas.bolt
+-rw-r--r--   0        0        0      205 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events/on_tick.bolt
+-rw-r--r--   0        0        0     2118 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/events.bolt
+-rw-r--r--   0        0        0     3398 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/flag.bolt
+-rw-r--r--   0        0        0      377 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/flags/is_airborne.bolt
+-rw-r--r--   0        0        0      402 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/flags/is_baby.bolt
+-rw-r--r--   0        0        0      411 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/flags/is_burning.bolt
+-rw-r--r--   0        0        0     1258 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/flags/is_charging_bow.bolt
+-rw-r--r--   0        0        0      377 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/flags/is_gliding.bolt
+-rw-r--r--   0        0        0      379 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/flags/is_in_ground.bolt
+-rw-r--r--   0        0        0      379 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/flags/is_on_ground.bolt
+-rw-r--r--   0        0        0      158 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/flags/is_player.bolt
+-rw-r--r--   0        0        0      414 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/flags/is_sneaking.bolt
+-rw-r--r--   0        0        0      417 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/flags/is_sprinting.bolt
+-rw-r--r--   0        0        0      414 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/flags/is_swimming.bolt
+-rw-r--r--   0        0        0      535 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/flags.bolt
+-rw-r--r--   0        0        0      443 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/lib/entity_hit_matching/api.bolt
+-rw-r--r--   0        0        0      124 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/lib/entity_hit_matching/credits.txt
+-rw-r--r--   0        0        0    58171 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/lib/entity_hit_matching/main.bolt
+-rw-r--r--   0        0        0      207 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/modules/utils.bolt
+-rw-r--r--   0        0        0        0 2023-08-02 19:10:02.901745 crankshaft-0.8.1/crankshaft/py.typed
+-rw-r--r--   0        0        0     1329 2023-08-02 19:11:42.899354 crankshaft-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 crankshaft-0.8.1/PKG-INFO
```

### Comparing `crankshaft-0.8.0/LICENSE` & `crankshaft-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crankshaft-0.8.0/README.md` & `crankshaft-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `crankshaft-0.8.0/crankshaft/modules/defer.bolt` & `crankshaft-0.8.1/crankshaft/modules/defer.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.8.0/crankshaft/modules/event_handler.bolt` & `crankshaft-0.8.1/crankshaft/modules/event_handler.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.8.0/crankshaft/modules/events/on_entity_attack_player.bolt` & `crankshaft-0.8.1/crankshaft/modules/events/on_entity_attack_player.bolt`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from wicked_expressions:nbtlib import Bool
 from lightning_rod:api import tag, untag
 from ../event_handler import BuiltinEvent
 from ../lib/entity_hit_matching/api import append_player_trigger
 from ../config import Config
 from ../utils import selector
 
-
 def handler(event):
     has_owner = StaticVar(Bool)
     victim_tag = f"{Config.TAG_ROOT}.event.{event.id}.victim"
     attacker_tag = f"{Config.TAG_ROOT}.event.{event.id}.attacker"
     direct_tag = f"{Config.TAG_ROOT}.event.{event.id}.direct"
     victim = selector(f"@a[tag={victim_tag}, limit=1]")
     attacker = selector(f"@e[tag={attacker_tag}, limit=1]")
@@ -42,10 +41,9 @@
 
         as attacker:
             untag(attacker_tag)
         
         as direct:
             untag(direct_tag)
 
-
 on_entity_attack_player = BuiltinEvent('on_entity_attack_player')
 on_entity_attack_player.attach_handler(handler)
```

### Comparing `crankshaft-0.8.0/crankshaft/modules/events/on_player_airborne.bolt` & `crankshaft-0.8.1/crankshaft/modules/events/on_player_burn_end.bolt`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from wicked_expressions:api import Scoreboard
+from lightning_rod:api import tag, untag
 from ../event_handler import BuiltinEvent, Entrypoint
-from ../flags/is_airborne import is_airborne
 from ./on_player_tick import on_player_tick
 from ../config import Config
+from ../flags/is_burning import is_burning
 
 def handler(event):
-    air_time = Scoreboard(f"{Config.SCOREBOARD_ROOT}.event.{event.id}.air_time")['@s']
+    event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
-    if is_airborne:
-        air_time += 1
-        event.trigger(air_time)
+    if not is_burning:
+        if entity @s[tag=event_fired_tag] function event.path('nested_0'):
+            untag(event_fired_tag)
+            event.trigger()
     else:
-        air_time = 0
+        tag(event_fired_tag)
 
-on_player_airborne = BuiltinEvent('on_player_airborne')
-on_player_airborne.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
+on_player_burn_end = BuiltinEvent('on_player_burn_end')
+on_player_burn_end.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.8.0/crankshaft/modules/events/on_player_airborne_end.bolt` & `crankshaft-0.8.1/crankshaft/modules/events/on_player_airborne_end.bolt`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from wicked_expressions:api import Scoreboard
+from wicked_expressions:api import Scoreboard, StaticVar, Int
 from lightning_rod:api import tag, untag
 from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../config import Config
 from ../flags/is_airborne import is_airborne
 
-
 def handler(event):
     air_time = Scoreboard(f"{Config.SCOREBOARD_ROOT}.event.{event.id}.air_time")['@s']
     event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
+    output = StaticVar(Int)
 
     if not is_airborne:
         if entity @s[tag=event_fired_tag] function event.path('nested_0'):
             untag(event_fired_tag)
-            event.trigger(air_time)
+            output = air_time
+            event.trigger(output)
             air_time = 0
     else:
         tag(event_fired_tag)
         air_time += 1
 
 on_player_airborne_end = BuiltinEvent('on_player_airborne_end')
 on_player_airborne_end.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.8.0/crankshaft/modules/events/on_player_airborne_start.bolt` & `crankshaft-0.8.1/crankshaft/modules/events/on_player_airborne_start.bolt`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from lightning_rod:api import tag, untag
 from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../config import Config
 from ../flags/is_airborne import is_airborne
 
-
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
     if is_airborne:
         if entity @s[tag=!event_fired_tag] function event.path('nested_0'):
             tag(event_fired_tag)
             event.trigger()
     else:
         untag(event_fired_tag)
 
-
 on_player_airborne_start = BuiltinEvent('on_player_airborne_start')
 on_player_airborne_start.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.8.0/crankshaft/modules/events/on_player_attack_entity.bolt` & `crankshaft-0.8.1/crankshaft/modules/events/on_player_attack_entity.bolt`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from wicked_expressions:nbtlib import Bool
 from lightning_rod:api import tag, untag
 from ../event_handler import BuiltinEvent
 from ../lib/entity_hit_matching/api import append_target_trigger
 from ../config import Config
 from ../utils import selector
 
-
 def handler(event):
     has_owner = StaticVar(Bool)
     victim_tag = f"{Config.TAG_ROOT}.event.{event.id}.victim"
     attacker_tag = f"{Config.TAG_ROOT}.event.{event.id}.attacker"
     direct_tag = f"{Config.TAG_ROOT}.event.{event.id}.direct"
     victim = selector(f"@e[tag={victim_tag}, limit=1]")
     attacker = selector(f"@a[tag={attacker_tag}, limit=1]")
@@ -42,10 +41,9 @@
 
         as attacker:
             untag(attacker_tag)
         
         as direct:
             untag(direct_tag)
 
-
 on_player_attack_entity = BuiltinEvent('on_player_attack_entity')
 on_player_attack_entity.attach_handler(handler)
```

### Comparing `crankshaft-0.8.0/crankshaft/modules/events/on_player_burn_end.bolt` & `crankshaft-0.8.1/crankshaft/modules/events/on_player_charge_bow_start.bolt`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from lightning_rod:api import tag, untag
 from ../event_handler import BuiltinEvent, Entrypoint
-from ./on_player_tick import on_player_tick
 from ../config import Config
-from ../flags/is_burning import is_burning
-
+from ../flags/is_charging_bow import is_charging_bow
+from ./on_player_tick import on_player_tick
 
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
-    if not is_burning:
-        if entity @s[tag=event_fired_tag] function event.path('nested_0'):
-            untag(event_fired_tag)
+    if is_charging_bow:
+        if entity @s[tag=!event_fired_tag] function event.path('nested_0'):
+            tag(event_fired_tag)
             event.trigger()
     else:
-        tag(event_fired_tag)
-
+        untag(event_fired_tag)
 
-on_player_burn_end = BuiltinEvent('on_player_burn_end')
-on_player_burn_end.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
+on_player_charge_bow_start = BuiltinEvent('on_player_charge_bow_start')
+on_player_charge_bow_start.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.8.0/crankshaft/modules/events/on_player_burn_start.bolt` & `crankshaft-0.8.1/crankshaft/modules/events/on_player_sneak_start.bolt`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from lightning_rod:api import tag, untag
 from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../config import Config
-from ../flags/is_burning import is_burning
-
+from ../flags/is_sneaking import is_sneaking
 
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
-    if is_burning:
+    if is_sneaking:
         if entity @s[tag=!event_fired_tag] function event.path('nested_0'):
             tag(event_fired_tag)
             event.trigger()
     else:
         untag(event_fired_tag)
 
-
-on_player_burn_start = BuiltinEvent('on_player_burn_start')
-on_player_burn_start.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
+on_player_sneak_start = BuiltinEvent('on_player_sneak_start')
+on_player_sneak_start.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.8.0/crankshaft/modules/events/on_player_charge_bow.bolt` & `crankshaft-0.8.1/crankshaft/modules/events/on_player_charge_bow.bolt`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from wicked_expressions:api import Scoreboard
+from wicked_expressions:api import Scoreboard, StaticVar, Int
 from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../flags/is_charging_bow import is_charging_bow
 from ../config import Config
 
-
 def handler(event):
     charge_time = Scoreboard(f"{Config.SCOREBOARD_ROOT}.event.{event.id}")['@s']
+    output = StaticVar(Int)
 
     if is_charging_bow:
         charge_time += 1
-        event.trigger(charge_time)
+        output = charge_time
+        event.trigger(output)
     else:
         charge_time = 0
 
-
 on_player_charge_bow = BuiltinEvent('on_player_charge_bow')
 on_player_charge_bow.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.8.0/crankshaft/modules/events/on_player_charge_bow_end.bolt` & `crankshaft-0.8.1/crankshaft/modules/events/on_player_charge_bow_end.bolt`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from wicked_expressions:api import Scoreboard
+from wicked_expressions:api import Scoreboard, StaticVar, Int
 from lightning_rod:api import tag, untag
 from ../event_handler import BuiltinEvent, Entrypoint
 from ../config import Config
 from ../flags/is_charging_bow import is_charging_bow
 from ./on_player_tick import on_player_tick
 
-
 def handler(event):
     charge_time = Scoreboard(f"{Config.SCOREBOARD_ROOT}.event.{event.id}")['@s']
     event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
+    output = StaticVar(Int)
 
     if not is_charging_bow:
         execute function event.path('nested_0'):
             if entity @s[tag=event_fired_tag] function event.path('nested_1'):
                 untag(event_fired_tag)
-                event.trigger(charge_time)
+                output = charge_time
+                event.trigger(output)
                 charge_time = 0
     else:
         execute function event.path('nested_2'):
             tag(event_fired_tag)
             charge_time += 1
 
-
 on_player_charge_bow_end = BuiltinEvent('on_player_charge_bow_end')
 on_player_charge_bow_end.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.8.0/crankshaft/modules/events/on_player_charge_bow_start.bolt` & `crankshaft-0.8.1/crankshaft/modules/events/on_player_burn_start.bolt`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from lightning_rod:api import tag, untag
 from ../event_handler import BuiltinEvent, Entrypoint
-from ../config import Config
-from ../flags/is_charging_bow import is_charging_bow
 from ./on_player_tick import on_player_tick
-
+from ../config import Config
+from ../flags/is_burning import is_burning
 
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
-    if is_charging_bow:
+    if is_burning:
         if entity @s[tag=!event_fired_tag] function event.path('nested_0'):
             tag(event_fired_tag)
             event.trigger()
     else:
         untag(event_fired_tag)
 
-
-on_player_charge_bow_start = BuiltinEvent('on_player_charge_bow_start')
-on_player_charge_bow_start.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
+on_player_burn_start = BuiltinEvent('on_player_burn_start')
+on_player_burn_start.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.8.0/crankshaft/modules/events/on_player_glide_end.bolt` & `crankshaft-0.8.1/crankshaft/modules/events/on_player_glide_end.bolt`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from lightning_rod:api import tag, untag
 from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../config import Config
 from ../flags/is_gliding import is_gliding
 
-
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
     if not is_gliding:
         if entity @s[tag=event_fired_tag] function event.path('nested_0'):
             untag(event_fired_tag)
             event.trigger()
     else:
         tag(event_fired_tag)
 
-
 on_player_glide_end = BuiltinEvent('on_player_glide_end')
 on_player_glide_end.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.8.0/crankshaft/modules/events/on_player_glide_start.bolt` & `crankshaft-0.8.1/crankshaft/modules/events/on_player_glide_start.bolt`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from lightning_rod:api import tag, untag
 from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../config import Config
 from ../flags/is_gliding import is_gliding 
 
-
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
     if is_gliding:
         if entity @s[tag=!event_fired_tag] function event.path('nested_0'):
             tag(event_fired_tag)
             event.trigger()
     else:
         untag(event_fired_tag)
 
-
 on_player_glide_start = BuiltinEvent('on_player_glide_start')
 on_player_glide_start.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.8.0/crankshaft/modules/events/on_player_inventory_change.bolt` & `crankshaft-0.8.1/crankshaft/modules/events/on_player_inventory_change.bolt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from lightning_rod:api import revoke_advancement
 from ../event_handler import BuiltinEvent
 
-
 def handler(event):
     advancement_path = event.path('advancement')
     reward_path = event.path('advancement_reward')
 
     advancement advancement_path {
         "criteria": {
             "requirement": {
@@ -13,15 +12,13 @@
             }
         },
         "rewards": {
             "function": reward_path
         }
     }
 
-
     function reward_path:
         revoke_advancement(advancement_path)
         event.trigger()
 
-
 on_player_inventory_change = BuiltinEvent('on_player_inventory_change')
 on_player_inventory_change.attach_handler(handler)
```

### Comparing `crankshaft-0.8.0/crankshaft/modules/events/on_player_land.bolt` & `crankshaft-0.8.1/crankshaft/modules/events/on_player_land.bolt`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from lightning_rod:api import tag, untag
 from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../config import Config
 from ../flags/is_airborne import is_airborne
 
-
 def handler(event):
     available_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
     if is_airborne:
         tag(available_tag)
     else:
         if entity @s[tag=available_tag] function event.path('nested_0'):
             untag(available_tag)
             event.trigger()
 
-
 on_player_land = BuiltinEvent('on_player_land')
 on_player_land.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.8.0/crankshaft/modules/events/on_player_shoot_bow.bolt` & `crankshaft-0.8.1/crankshaft/modules/events/on_player_shoot_bow.bolt`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-from wicked_expressions:api import Scoreboard
+from wicked_expressions:api import Scoreboard, StaticVar, Int
 from ../event_handler import BuiltinEvent, Entrypoint
 from ../flags/is_charging_bow import is_charging_bow
 from ../config import Config
 from ./on_player_tick import on_player_tick
 
-
-
 def handler(event):
     charge_time = Scoreboard(f"{Config.SCOREBOARD_ROOT}.event.{event.id}.charge_time")['@s']
     shoot_tracker = Scoreboard(f"{Config.SCOREBOARD_ROOT}.event.{event.id}", 'used:bow')['@s']
+    output = StaticVar(Int)
 
     if is_charging_bow:
         charge_time += 1
     else:
         charge_time = 0
 
     if shoot_tracker >= 1:
         shoot_tracker = 0
-        event.trigger(charge_time)
-
+        output = charge_time
+        event.trigger(output)
 
 on_player_shoot_bow = BuiltinEvent('on_player_shoot_bow')
 on_player_shoot_bow.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.8.0/crankshaft/modules/events/on_player_sneak_end.bolt` & `crankshaft-0.8.1/crankshaft/modules/events/on_player_sneak_end.bolt`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from lightning_rod:api import tag, untag
 from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../config import Config
 from ../flags/is_sneaking import is_sneaking
 
-
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
     if not is_sneaking:
         if entity @s[tag=event_fired_tag] function event.path('nested_0'):
             untag(event_fired_tag)
             event.trigger()
     else:
         tag(event_fired_tag)
 
-
 on_player_sneak_end = BuiltinEvent('on_player_sneak_end')
 on_player_sneak_end.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.8.0/crankshaft/modules/events/on_player_sneak_start.bolt` & `crankshaft-0.8.1/crankshaft/modules/events/on_player_swim_start.bolt`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from lightning_rod:api import tag, untag
 from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../config import Config
-from ../flags/is_sneaking import is_sneaking
-
+from ../flags/is_swimming import is_swimming 
 
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
-    if is_sneaking:
+    if is_swimming:
         if entity @s[tag=!event_fired_tag] function event.path('nested_0'):
             tag(event_fired_tag)
             event.trigger()
     else:
         untag(event_fired_tag)
 
-
-on_player_sneak_start = BuiltinEvent('on_player_sneak_start')
-on_player_sneak_start.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
+on_player_swim_start = BuiltinEvent('on_player_swim_start')
+on_player_swim_start.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.8.0/crankshaft/modules/events/on_player_sprint_end.bolt` & `crankshaft-0.8.1/crankshaft/modules/events/on_player_sprint_end.bolt`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from lightning_rod:api import tag, untag
 from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../config import Config
 from ../flags/is_sprinting import is_sprinting 
 
-
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
     if not is_sprinting:
         if entity @s[tag=event_fired_tag] function event.path('nested_0'):
             untag(event_fired_tag)
             event.trigger()
     else:
         tag(event_fired_tag)
 
-
 on_player_sprint_end = BuiltinEvent('on_player_sprint_end')
 on_player_sprint_end.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.8.0/crankshaft/modules/events/on_player_sprint_start.bolt` & `crankshaft-0.8.1/crankshaft/modules/events/on_player_sprint_start.bolt`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from lightning_rod:api import tag, untag
 from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../config import Config
 from ../flags/is_sprinting import is_sprinting
 
-
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
     if is_sprinting:
         if entity @s[tag=!event_fired_tag] function event.path('nested_0'):
             tag(event_fired_tag)
             event.trigger()
     else:
         untag(event_fired_tag)
 
-
 on_player_sprint_start = BuiltinEvent('on_player_sprint_start')
 on_player_sprint_start.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.8.0/crankshaft/modules/events/on_player_swim_end.bolt` & `crankshaft-0.8.1/crankshaft/modules/events/on_player_swim_end.bolt`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from lightning_rod:api import tag, untag
 from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../config import Config
 from ../flags/is_swimming import is_swimming
 
-
 def handler(event):
     event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
     if not is_swimming:
         if entity @s[tag=event_fired_tag] function event.path('nested_0'):
             untag(event_fired_tag)
             event.trigger()
     else:
         tag(event_fired_tag)
 
-
 on_player_swim_end = BuiltinEvent('on_player_swim_end')
 on_player_swim_end.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.8.0/crankshaft/modules/events/on_player_use_coas.bolt` & `crankshaft-0.8.1/crankshaft/modules/events/on_player_use_wfoas.bolt`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from wicked_expressions:api import Scoreboard
 from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../config import Config
 
-
 def handler(event):
-    used_coas = Scoreboard(f"{Config.SCOREBOARD_ROOT}.event.{event.id}", 'used:carrot_on_a_stick')['@s']
+    used_wfoas = Scoreboard(f"{Config.SCOREBOARD_ROOT}.event.{event.id}", 'used:warped_fungus_on_a_stick')['@s']
 
-    if not used_coas.exists():
-        used_coas = 0
+    if not used_wfoas.exists():
+        used_wfoas = 0
 
-    if used_coas > 0:
-        used_coas = 0
+    if used_wfoas > 0:
+        used_wfoas = 0
         event.trigger()
 
-
-on_player_use_coas = BuiltinEvent('on_player_use_coas')
-on_player_use_coas.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
+on_player_use_wfoas = BuiltinEvent('on_player_use_wfoas')
+on_player_use_wfoas.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.8.0/crankshaft/modules/events/on_player_use_wfoas.bolt` & `crankshaft-0.8.1/crankshaft/modules/events/on_player_use_coas.bolt`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from wicked_expressions:api import Scoreboard
 from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../config import Config
 
-
 def handler(event):
-    used_wfoas = Scoreboard(f"{Config.SCOREBOARD_ROOT}.event.{event.id}", 'used:warped_fungus_on_a_stick')['@s']
+    used_coas = Scoreboard(f"{Config.SCOREBOARD_ROOT}.event.{event.id}", 'used:carrot_on_a_stick')['@s']
 
-    if not used_wfoas.exists():
-        used_wfoas = 0
+    if not used_coas.exists():
+        used_coas = 0
 
-    if used_wfoas > 0:
-        used_wfoas = 0
+    if used_coas > 0:
+        used_coas = 0
         event.trigger()
 
-
-on_player_use_wfoas = BuiltinEvent('on_player_use_wfoas')
-on_player_use_wfoas.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
+on_player_use_coas = BuiltinEvent('on_player_use_coas')
+on_player_use_coas.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.8.0/crankshaft/modules/events.bolt` & `crankshaft-0.8.1/crankshaft/modules/events.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.8.0/crankshaft/modules/flag.bolt` & `crankshaft-0.8.1/crankshaft/modules/flag.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.8.0/crankshaft/modules/flags/is_charging_bow.bolt` & `crankshaft-0.8.1/crankshaft/modules/flags/is_charging_bow.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.8.0/crankshaft/modules/flags.bolt` & `crankshaft-0.8.1/crankshaft/modules/flags.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.8.0/crankshaft/modules/lib/entity_hit_matching/main.bolt` & `crankshaft-0.8.1/crankshaft/modules/lib/entity_hit_matching/main.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.8.0/pyproject.toml` & `crankshaft-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crankshaft"
-version = "0.8.0"
+version = "0.8.1"
 description = "Bolt datapack flow control library."
 authors = ["ArcticYeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/crankshaft"
 readme = "README.md"
```

### Comparing `crankshaft-0.8.0/PKG-INFO` & `crankshaft-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crankshaft
-Version: 0.8.0
+Version: 0.8.1
 Summary: Bolt datapack flow control library.
 Home-page: https://github.com/reapermc/crankshaft
 License: MIT
 Keywords: beet,mecha,bolt,python,minecraft,datapack,minecraft-commands,mcfunction,crankshaft,library,reapermc,flow-control,event,event-handler
 Author: ArcticYeti
 Author-email: arcticyeti1@gmail.com
 Requires-Python: >=3.10,<4.0
```

