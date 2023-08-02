# Comparing `tmp/wonda-0.5.7.tar.gz` & `tmp/wonda-0.6.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wonda-0.5.7.tar", max compression
+gzip compressed data, was "wonda-0.6.0a1.tar", max compression
```

## Comparing `wonda-0.5.7.tar` & `wonda-0.6.0a1.tar`

### file list

```diff
@@ -1,92 +1,88 @@
--rw-r--r--   0        0        0     1131 2023-03-09 14:13:36.085239 wonda-0.5.7/LICENSE
--rw-r--r--   0        0        0     2447 2023-03-09 14:13:36.085352 wonda-0.5.7/README.md
--rw-r--r--   0        0        0      770 2023-03-09 19:07:12.840066 wonda-0.5.7/pyproject.toml
--rw-r--r--   0        0        0      371 2023-03-09 14:13:36.088490 wonda-0.5.7/wonda/__init__.py
--rw-r--r--   0        0        0      220 2023-03-09 14:13:36.088650 wonda-0.5.7/wonda/api/__init__.py
--rw-r--r--   0        0        0     2146 2023-03-09 14:13:36.088758 wonda-0.5.7/wonda/api/abc.py
--rw-r--r--   0        0        0     1337 2023-03-09 14:13:36.088856 wonda-0.5.7/wonda/api/api.py
--rw-r--r--   0        0        0       58 2023-03-09 14:13:36.089031 wonda-0.5.7/wonda/api/utils/__init__.py
--rw-r--r--   0        0        0      842 2023-03-09 14:13:36.089143 wonda-0.5.7/wonda/api/utils/file_util.py
--rw-r--r--   0        0        0      350 2023-03-09 14:13:36.089240 wonda-0.5.7/wonda/api/utils/token_util.py
--rw-r--r--   0        0        0      207 2023-03-09 14:13:36.089400 wonda-0.5.7/wonda/api/validators/__init__.py
--rw-r--r--   0        0        0      493 2023-03-09 14:13:36.089503 wonda-0.5.7/wonda/api/validators/abc.py
--rw-r--r--   0        0        0     1153 2023-03-09 14:13:36.089604 wonda-0.5.7/wonda/api/validators/request.py
--rw-r--r--   0        0        0      658 2023-03-09 14:13:36.089699 wonda-0.5.7/wonda/api/validators/response.py
--rw-r--r--   0        0        0      640 2023-03-09 14:13:36.089846 wonda-0.5.7/wonda/bot/__init__.py
--rw-r--r--   0        0        0      452 2023-03-09 14:13:36.089957 wonda-0.5.7/wonda/bot/abc.py
--rw-r--r--   0        0        0       60 2023-03-09 14:13:36.090090 wonda-0.5.7/wonda/bot/blueprint/__init__.py
--rw-r--r--   0        0        0     2450 2023-03-09 14:13:36.090212 wonda-0.5.7/wonda/bot/blueprint/abc.py
--rw-r--r--   0        0        0     1466 2023-03-09 14:13:36.090308 wonda-0.5.7/wonda/bot/blueprint/bot.py
--rw-r--r--   0        0        0     2916 2023-03-09 14:13:36.090417 wonda-0.5.7/wonda/bot/bot.py
--rw-r--r--   0        0        0      268 2023-03-09 14:13:36.090558 wonda-0.5.7/wonda/bot/dispatch/__init__.py
--rw-r--r--   0        0        0       62 2023-03-09 14:13:36.090716 wonda-0.5.7/wonda/bot/dispatch/handlers/__init__.py
--rw-r--r--   0        0        0      399 2023-03-09 14:13:36.090812 wonda-0.5.7/wonda/bot/dispatch/handlers/abc.py
--rw-r--r--   0        0        0     1652 2023-03-09 14:13:36.090911 wonda-0.5.7/wonda/bot/dispatch/handlers/func.py
--rw-r--r--   0        0        0       60 2023-03-09 14:13:36.091054 wonda-0.5.7/wonda/bot/dispatch/labelers/__init__.py
--rw-r--r--   0        0        0     1169 2023-03-09 14:13:36.091150 wonda-0.5.7/wonda/bot/dispatch/labelers/abc.py
--rw-r--r--   0        0        0     4174 2023-03-09 14:13:36.091266 wonda-0.5.7/wonda/bot/dispatch/labelers/default.py
--rw-r--r--   0        0        0       50 2023-03-09 14:13:36.091401 wonda-0.5.7/wonda/bot/dispatch/middlewares/__init__.py
--rw-r--r--   0        0        0     2463 2023-03-09 14:13:36.091502 wonda-0.5.7/wonda/bot/dispatch/middlewares/base.py
--rw-r--r--   0        0        0       76 2023-03-09 14:13:36.091637 wonda-0.5.7/wonda/bot/dispatch/return_manager/__init__.py
--rw-r--r--   0        0        0     1051 2023-03-09 14:13:36.091722 wonda-0.5.7/wonda/bot/dispatch/return_manager/abc.py
--rw-r--r--   0        0        0      749 2023-03-09 14:13:36.091807 wonda-0.5.7/wonda/bot/dispatch/return_manager/message.py
--rw-r--r--   0        0        0       54 2023-03-09 14:13:36.091936 wonda-0.5.7/wonda/bot/dispatch/router/__init__.py
--rw-r--r--   0        0        0     1133 2023-03-09 14:13:36.092022 wonda-0.5.7/wonda/bot/dispatch/router/abc.py
--rw-r--r--   0        0        0     1076 2023-03-09 14:13:36.092100 wonda-0.5.7/wonda/bot/dispatch/router/bot.py
--rw-r--r--   0        0        0      144 2023-03-09 14:13:36.092220 wonda-0.5.7/wonda/bot/dispatch/view/__init__.py
--rw-r--r--   0        0        0     4058 2023-03-09 14:13:36.092329 wonda-0.5.7/wonda/bot/dispatch/view/abc.py
--rw-r--r--   0        0        0     2512 2023-03-09 14:13:36.092485 wonda-0.5.7/wonda/bot/dispatch/view/message.py
--rw-r--r--   0        0        0     2719 2023-03-09 14:13:36.092583 wonda-0.5.7/wonda/bot/dispatch/view/raw.py
--rw-r--r--   0        0        0       56 2023-03-09 14:13:36.092708 wonda-0.5.7/wonda/bot/polling/__init__.py
--rw-r--r--   0        0        0      370 2023-03-09 14:13:36.092794 wonda-0.5.7/wonda/bot/polling/abc.py
--rw-r--r--   0        0        0     2038 2023-03-09 14:13:36.092877 wonda-0.5.7/wonda/bot/polling/bot.py
--rw-r--r--   0        0        0      184 2023-03-09 14:13:36.093016 wonda-0.5.7/wonda/bot/rules/__init__.py
--rw-r--r--   0        0        0     1980 2023-03-09 14:13:36.093110 wonda-0.5.7/wonda/bot/rules/abc.py
--rw-r--r--   0        0        0     4401 2023-03-09 14:13:36.093229 wonda-0.5.7/wonda/bot/rules/base.py
--rw-r--r--   0        0        0     4925 2023-03-09 14:13:36.093340 wonda-0.5.7/wonda/bot/rules/message.py
--rw-r--r--   0        0        0      121 2023-03-09 14:13:36.093469 wonda-0.5.7/wonda/bot/states/__init__.py
--rw-r--r--   0        0        0       74 2023-03-09 14:13:36.093593 wonda-0.5.7/wonda/bot/states/dispenser/__init__.py
--rw-r--r--   0        0        0      834 2023-03-09 14:13:36.093680 wonda-0.5.7/wonda/bot/states/dispenser/abc.py
--rw-r--r--   0        0        0      855 2023-03-09 14:13:36.093769 wonda-0.5.7/wonda/bot/states/dispenser/default.py
--rw-r--r--   0        0        0      803 2023-03-09 14:13:36.093853 wonda-0.5.7/wonda/bot/states/types.py
--rw-r--r--   0        0        0      696 2023-03-09 14:13:36.093987 wonda-0.5.7/wonda/bot/updates/__init__.py
--rw-r--r--   0        0        0      463 2023-03-09 14:13:36.094075 wonda-0.5.7/wonda/bot/updates/base.py
--rw-r--r--   0        0        0     6449 2023-03-09 14:15:17.540335 wonda-0.5.7/wonda/bot/updates/types.py
--rw-r--r--   0        0        0        0 2023-03-09 14:13:36.094271 wonda-0.5.7/wonda/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-03-09 14:13:36.094381 wonda-0.5.7/wonda/contrib/rules/__init__.py
--rw-r--r--   0        0        0        0 2023-03-09 14:13:36.094472 wonda-0.5.7/wonda/contrib/storage/__init__.py
--rw-r--r--   0        0        0      218 2023-03-09 14:13:36.094607 wonda-0.5.7/wonda/errors/__init__.py
--rw-r--r--   0        0        0      331 2023-03-09 14:13:36.094694 wonda-0.5.7/wonda/errors/base_exceptions.py
--rw-r--r--   0        0        0     1687 2023-03-09 14:13:36.094786 wonda-0.5.7/wonda/errors/code_exception.py
--rw-r--r--   0        0        0       73 2023-03-09 14:13:36.094907 wonda-0.5.7/wonda/errors/error_handler/__init__.py
--rw-r--r--   0        0        0      729 2023-03-09 14:13:36.095005 wonda-0.5.7/wonda/errors/error_handler/abc.py
--rw-r--r--   0        0        0     2023 2023-03-09 14:13:36.095097 wonda-0.5.7/wonda/errors/error_handler/error_handler.py
--rw-r--r--   0        0        0       33 2023-03-09 14:13:36.095233 wonda-0.5.7/wonda/errors/swear_handler/__init__.py
--rw-r--r--   0        0        0     2464 2023-03-09 14:13:36.095336 wonda-0.5.7/wonda/errors/swear_handler/swear_handler.py
--rw-r--r--   0        0        0       66 2023-03-09 14:13:36.095464 wonda-0.5.7/wonda/http/__init__.py
--rw-r--r--   0        0        0     1047 2023-03-09 14:13:36.095553 wonda-0.5.7/wonda/http/abc.py
--rw-r--r--   0        0        0     2734 2023-03-09 14:13:36.095656 wonda-0.5.7/wonda/http/aiohttp.py
--rw-r--r--   0        0        0      631 2023-03-09 14:13:36.095752 wonda-0.5.7/wonda/modules.py
--rw-r--r--   0        0        0      224 2023-03-09 14:13:36.095872 wonda-0.5.7/wonda/tools/__init__.py
--rw-r--r--   0        0        0      863 2023-03-09 14:13:36.095965 wonda-0.5.7/wonda/tools/auto_reload.py
--rw-r--r--   0        0        0      562 2023-03-09 14:13:36.096047 wonda-0.5.7/wonda/tools/delayed_task.py
--rw-r--r--   0        0        0      196 2023-03-09 14:13:36.096193 wonda-0.5.7/wonda/tools/keyboard/__init__.py
--rw-r--r--   0        0        0     2136 2023-03-09 14:13:36.096310 wonda-0.5.7/wonda/tools/keyboard/abc.py
--rw-r--r--   0        0        0     2660 2023-03-09 14:13:36.096427 wonda-0.5.7/wonda/tools/keyboard/inline.py
--rw-r--r--   0        0        0     4155 2023-03-09 14:13:36.096554 wonda-0.5.7/wonda/tools/keyboard/reply.py
--rw-r--r--   0        0        0     3743 2023-03-09 14:13:36.096679 wonda-0.5.7/wonda/tools/loop_wrapper.py
--rw-r--r--   0        0        0      135 2023-03-09 14:13:36.096811 wonda-0.5.7/wonda/tools/storage/__init__.py
--rw-r--r--   0        0        0      640 2023-03-09 14:13:36.096903 wonda-0.5.7/wonda/tools/storage/abc.py
--rw-r--r--   0        0        0      931 2023-03-09 14:13:36.096996 wonda-0.5.7/wonda/tools/storage/memory.py
--rw-r--r--   0        0        0      193 2023-03-09 14:13:36.097081 wonda-0.5.7/wonda/tools/storage/types.py
--rw-r--r--   0        0        0       73 2023-03-09 14:13:36.097211 wonda-0.5.7/wonda/tools/text/__init__.py
--rw-r--r--   0        0        0       29 2023-03-09 14:13:36.097346 wonda-0.5.7/wonda/tools/text/formatting/__init__.py
--rw-r--r--   0        0        0     2182 2023-03-09 14:13:36.097459 wonda-0.5.7/wonda/tools/text/formatting/html.py
--rw-r--r--   0        0        0     2761 2023-03-09 14:13:36.097561 wonda-0.5.7/wonda/tools/text/formatting/markdown.py
--rw-r--r--   0        0        0       93 2023-03-09 14:13:36.097655 wonda-0.5.7/wonda/tools/text/parse_mode.py
--rw-r--r--   0        0        0       55 2023-03-09 14:13:36.097808 wonda-0.5.7/wonda/types/__init__.py
--rw-r--r--   0        0        0     4338 2023-03-09 19:04:42.405317 wonda-0.5.7/wonda/types/enums.py
--rw-r--r--   0        0        0    78234 2023-03-09 19:04:42.624651 wonda-0.5.7/wonda/types/methods.py
--rw-r--r--   0        0        0    74651 2023-03-09 19:04:42.922154 wonda-0.5.7/wonda/types/objects.py
--rw-r--r--   0        0        0     4207 2023-03-09 19:07:42.712960 wonda-0.5.7/setup.py
--rw-r--r--   0        0        0     3431 2023-03-09 19:07:42.713247 wonda-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1131 2023-01-08 13:20:34.909130 wonda-0.6.0a1/LICENSE
+-rw-r--r--   0        0        0     2177 2023-08-01 13:12:06.355095 wonda-0.6.0a1/README.md
+-rw-r--r--   0        0        0      542 2023-08-01 14:00:48.639524 wonda-0.6.0a1/pyproject.toml
+-rw-r--r--   0        0        0      356 2023-08-01 13:12:06.359212 wonda-0.6.0a1/wonda/__init__.py
+-rw-r--r--   0        0        0      220 2023-08-01 14:26:17.698469 wonda-0.6.0a1/wonda/api/__init__.py
+-rw-r--r--   0        0        0     1941 2023-08-01 14:34:12.037508 wonda-0.6.0a1/wonda/api/abc.py
+-rw-r--r--   0        0        0     1282 2023-08-01 14:36:44.589394 wonda-0.6.0a1/wonda/api/api.py
+-rw-r--r--   0        0        0       68 2023-08-01 14:15:25.890716 wonda-0.6.0a1/wonda/api/response.py
+-rw-r--r--   0        0        0       58 2023-07-09 17:08:19.452596 wonda-0.6.0a1/wonda/api/utils/__init__.py
+-rw-r--r--   0        0        0      631 2023-08-01 13:12:06.360196 wonda-0.6.0a1/wonda/api/utils/file_util.py
+-rw-r--r--   0        0        0     1076 2023-08-01 14:04:17.058304 wonda-0.6.0a1/wonda/api/utils/token_util.py
+-rw-r--r--   0        0        0      253 2023-08-01 13:32:22.879290 wonda-0.6.0a1/wonda/api/validators/__init__.py
+-rw-r--r--   0        0        0      327 2023-08-01 14:34:07.149011 wonda-0.6.0a1/wonda/api/validators/abc.py
+-rw-r--r--   0        0        0      831 2023-08-01 14:39:32.506796 wonda-0.6.0a1/wonda/api/validators/request.py
+-rw-r--r--   0        0        0      713 2023-08-01 14:20:27.832088 wonda-0.6.0a1/wonda/api/validators/response.py
+-rw-r--r--   0        0        0      559 2023-08-01 13:12:06.361697 wonda-0.6.0a1/wonda/bot/__init__.py
+-rw-r--r--   0        0        0      324 2023-08-01 13:16:13.482655 wonda-0.6.0a1/wonda/bot/abc.py
+-rw-r--r--   0        0        0       68 2023-08-01 13:12:06.362105 wonda-0.6.0a1/wonda/bot/blueprint/__init__.py
+-rw-r--r--   0        0        0      616 2023-08-01 13:19:08.503857 wonda-0.6.0a1/wonda/bot/blueprint/abc.py
+-rw-r--r--   0        0        0      817 2023-08-01 13:16:13.828698 wonda-0.6.0a1/wonda/bot/blueprint/default.py
+-rw-r--r--   0        0        0     2219 2023-08-01 13:16:13.736400 wonda-0.6.0a1/wonda/bot/bot.py
+-rw-r--r--   0        0        0      212 2023-08-01 13:16:13.736421 wonda-0.6.0a1/wonda/bot/dispatch/__init__.py
+-rw-r--r--   0        0        0       70 2023-08-01 13:16:13.828532 wonda-0.6.0a1/wonda/bot/dispatch/dispatcher/__init__.py
+-rw-r--r--   0        0        0      510 2023-08-01 13:16:13.839652 wonda-0.6.0a1/wonda/bot/dispatch/dispatcher/abc.py
+-rw-r--r--   0        0        0     1115 2023-08-01 13:16:13.828518 wonda-0.6.0a1/wonda/bot/dispatch/dispatcher/default.py
+-rw-r--r--   0        0        0       58 2023-08-01 13:12:06.387599 wonda-0.6.0a1/wonda/bot/dispatch/handler/__init__.py
+-rw-r--r--   0        0        0      391 2023-08-01 13:12:06.387736 wonda-0.6.0a1/wonda/bot/dispatch/handler/abc.py
+-rw-r--r--   0        0        0     1219 2023-08-01 13:12:06.387872 wonda-0.6.0a1/wonda/bot/dispatch/handler/func.py
+-rw-r--r--   0        0        0       78 2023-08-01 13:12:06.362854 wonda-0.6.0a1/wonda/bot/dispatch/middlewares/__init__.py
+-rw-r--r--   0        0        0      406 2023-08-01 13:12:06.388025 wonda-0.6.0a1/wonda/bot/dispatch/middlewares/abc.py
+-rw-r--r--   0        0        0       62 2023-08-01 13:12:06.363015 wonda-0.6.0a1/wonda/bot/dispatch/router/__init__.py
+-rw-r--r--   0        0        0      637 2023-08-01 14:10:44.271381 wonda-0.6.0a1/wonda/bot/dispatch/router/abc.py
+-rw-r--r--   0        0        0     1072 2023-08-01 13:12:06.388166 wonda-0.6.0a1/wonda/bot/dispatch/router/default.py
+-rw-r--r--   0        0        0      110 2023-08-01 13:12:06.363412 wonda-0.6.0a1/wonda/bot/dispatch/view/__init__.py
+-rw-r--r--   0        0        0     3533 2023-08-01 13:39:56.214935 wonda-0.6.0a1/wonda/bot/dispatch/view/abc.py
+-rw-r--r--   0        0        0     2103 2023-08-01 13:18:52.420643 wonda-0.6.0a1/wonda/bot/dispatch/view/impl.py
+-rw-r--r--   0        0        0       56 2023-04-21 11:36:28.382086 wonda-0.6.0a1/wonda/bot/polling/__init__.py
+-rw-r--r--   0        0        0      464 2023-08-01 13:12:06.364052 wonda-0.6.0a1/wonda/bot/polling/abc.py
+-rw-r--r--   0        0        0     1211 2023-08-01 13:12:06.364287 wonda-0.6.0a1/wonda/bot/polling/bot.py
+-rw-r--r--   0        0        0      129 2023-08-01 13:12:06.364526 wonda-0.6.0a1/wonda/bot/rules/__init__.py
+-rw-r--r--   0        0        0     1816 2023-08-01 14:48:49.174835 wonda-0.6.0a1/wonda/bot/rules/abc.py
+-rw-r--r--   0        0        0     4437 2023-08-01 13:50:29.499615 wonda-0.6.0a1/wonda/bot/rules/base.py
+-rw-r--r--   0        0        0     5537 2023-08-01 13:12:06.365118 wonda-0.6.0a1/wonda/bot/rules/message.py
+-rw-r--r--   0        0        0      125 2023-08-01 13:12:06.365285 wonda-0.6.0a1/wonda/bot/states/__init__.py
+-rw-r--r--   0        0        0       78 2023-08-01 13:12:06.365455 wonda-0.6.0a1/wonda/bot/states/dispenser/__init__.py
+-rw-r--r--   0        0        0      822 2023-08-01 13:12:06.365624 wonda-0.6.0a1/wonda/bot/states/dispenser/abc.py
+-rw-r--r--   0        0        0      832 2023-08-01 13:12:06.365811 wonda-0.6.0a1/wonda/bot/states/dispenser/default.py
+-rw-r--r--   0        0        0      574 2023-08-01 13:12:06.365978 wonda-0.6.0a1/wonda/bot/states/types.py
+-rw-r--r--   0        0        0      636 2023-08-01 13:12:06.366161 wonda-0.6.0a1/wonda/bot/updates/__init__.py
+-rw-r--r--   0        0        0      135 2023-08-01 13:12:06.366317 wonda-0.6.0a1/wonda/bot/updates/base.py
+-rw-r--r--   0        0        0     5287 2023-08-01 13:12:50.665638 wonda-0.6.0a1/wonda/bot/updates/types.py
+-rw-r--r--   0        0        0        0 2022-12-09 12:31:48.203870 wonda-0.6.0a1/wonda/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:12:06.388351 wonda-0.6.0a1/wonda/contrib/middleware/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-09 12:31:48.204053 wonda-0.6.0a1/wonda/contrib/rules/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-03 19:17:57.296559 wonda-0.6.0a1/wonda/contrib/storage/__init__.py
+-rw-r--r--   0        0        0     1475 2023-08-01 13:12:06.388804 wonda-0.6.0a1/wonda/contrib/storage/redis.py
+-rw-r--r--   0        0        0      298 2023-08-01 13:12:06.366842 wonda-0.6.0a1/wonda/errors/__init__.py
+-rw-r--r--   0        0        0      269 2023-08-01 13:12:06.367058 wonda-0.6.0a1/wonda/errors/base_exceptions.py
+-rw-r--r--   0        0        0     1635 2023-08-01 14:03:19.646417 wonda-0.6.0a1/wonda/errors/code_exception.py
+-rw-r--r--   0        0        0       73 2023-04-21 11:36:28.384533 wonda-0.6.0a1/wonda/errors/error_handler/__init__.py
+-rw-r--r--   0        0        0      704 2023-08-01 13:12:06.367251 wonda-0.6.0a1/wonda/errors/error_handler/abc.py
+-rw-r--r--   0        0        0     2031 2023-08-01 13:12:06.367470 wonda-0.6.0a1/wonda/errors/error_handler/error_handler.py
+-rw-r--r--   0        0        0      533 2023-08-01 14:27:57.256711 wonda-0.6.0a1/wonda/modules.py
+-rw-r--r--   0        0        0       76 2023-08-01 13:12:06.389026 wonda-0.6.0a1/wonda/net/__init__.py
+-rw-r--r--   0        0        0      799 2023-08-01 13:12:06.389181 wonda-0.6.0a1/wonda/net/abc.py
+-rw-r--r--   0        0        0     1960 2023-08-01 14:28:02.359184 wonda-0.6.0a1/wonda/net/default.py
+-rw-r--r--   0        0        0      123 2023-08-01 13:12:06.368301 wonda-0.6.0a1/wonda/tools/__init__.py
+-rw-r--r--   0        0        0      551 2023-08-01 13:12:06.368500 wonda-0.6.0a1/wonda/tools/delayed_task.py
+-rw-r--r--   0        0        0      284 2023-08-01 13:12:06.368688 wonda-0.6.0a1/wonda/tools/keyboard/__init__.py
+-rw-r--r--   0        0        0      704 2023-08-01 13:12:06.368872 wonda-0.6.0a1/wonda/tools/keyboard/abc.py
+-rw-r--r--   0        0        0     2889 2023-08-01 14:46:49.980391 wonda-0.6.0a1/wonda/tools/keyboard/builder.py
+-rw-r--r--   0        0        0     5281 2023-08-01 13:12:06.389685 wonda-0.6.0a1/wonda/tools/keyboard/elements.py
+-rw-r--r--   0        0        0     2603 2023-08-01 14:08:40.080104 wonda-0.6.0a1/wonda/tools/loop_wrapper.py
+-rw-r--r--   0        0        0      174 2023-08-01 13:12:06.369277 wonda-0.6.0a1/wonda/tools/storage/__init__.py
+-rw-r--r--   0        0        0      648 2023-08-01 13:12:06.369452 wonda-0.6.0a1/wonda/tools/storage/abc.py
+-rw-r--r--   0        0        0     1861 2023-08-01 13:12:06.369619 wonda-0.6.0a1/wonda/tools/storage/memory.py
+-rw-r--r--   0        0        0      132 2023-08-01 13:12:06.369784 wonda-0.6.0a1/wonda/tools/storage/types.py
+-rw-r--r--   0        0        0       73 2023-02-27 18:52:52.469528 wonda-0.6.0a1/wonda/tools/text/__init__.py
+-rw-r--r--   0        0        0       29 2023-02-27 18:52:54.495531 wonda-0.6.0a1/wonda/tools/text/formatting/__init__.py
+-rw-r--r--   0        0        0     2182 2023-02-27 18:52:47.941301 wonda-0.6.0a1/wonda/tools/text/formatting/html.py
+-rw-r--r--   0        0        0     2761 2023-02-27 18:52:50.221309 wonda-0.6.0a1/wonda/tools/text/formatting/markdown.py
+-rw-r--r--   0        0        0       93 2022-12-09 12:31:48.210068 wonda-0.6.0a1/wonda/tools/text/parse_mode.py
+-rw-r--r--   0        0        0       55 2023-02-01 05:24:13.893095 wonda-0.6.0a1/wonda/types/__init__.py
+-rw-r--r--   0        0        0     4438 2023-08-01 13:13:03.042503 wonda-0.6.0a1/wonda/types/enums.py
+-rw-r--r--   0        0        0      451 2023-08-01 13:12:06.389838 wonda-0.6.0a1/wonda/types/helper.py
+-rw-r--r--   0        0        0    78297 2023-08-01 14:19:52.164954 wonda-0.6.0a1/wonda/types/methods.py
+-rw-r--r--   0        0        0    59280 2023-08-01 13:13:37.342354 wonda-0.6.0a1/wonda/types/objects.py
+-rw-r--r--   0        0        0     2852 1970-01-01 00:00:00.000000 wonda-0.6.0a1/PKG-INFO
```

### Comparing `wonda-0.5.7/LICENSE` & `wonda-0.6.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `wonda-0.5.7/pyproject.toml` & `wonda-0.6.0a1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 [tool.poetry]
 name = "wonda"
-version = "0.5.7"
-description = "Asynchronous feature-rich Telegram bot framework for building great bots"
+version = "0.6.0a1"
+description = "Asynchronous feature-rich framework for building Telegram bots"
 authors = []
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/wondergram-org/wonda/"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-certifi = "^2022.6.15"
+python = "^3.10"
+certifi = "^2023.7.22"
+aiohttp = "^3.8.5"
+structlog = "^23.1.0"
 choicelib = "^0.1.5"
-aiohttp = "^3.8.1"
-pydantic = "^1.10.4"
-typing-extensions = "^4.3.0"
-uvloop = {version = "^0.16.0", optional = true}
-watchfiles = {version = "^0.16.0", optional = true}
-orjson = {version = "^3.8.5", optional = true}
+msgspec = "^0.17.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.6.0"
-
-[tool.poetry.extras]
-auto-reload = ["watchfiles"]
-power-ups = ["orjson", "uvloop"]
+isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `wonda-0.5.7/wonda/api/abc.py` & `wonda-0.6.0a1/wonda/api/abc.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 import typing
 from abc import ABC, abstractmethod
 
 if typing.TYPE_CHECKING:
     from wonda.api import ABCRequestValidator, ABCResponseValidator, Token
-    from wonda.http import ABCHTTPClient
+    from wonda.net import ABCNetworkClient
 
-APIResponse = typing.NewType(
-    "APIResponse", typing.Union[typing.NoReturn, typing.Dict[str, typing.Any]]
-)
 APIRequest = typing.NamedTuple("APIRequest", [("method", str), ("params", dict)])
 
 
 class ABCAPI(ABC):
     API_URL = "https://api.telegram.org/"
     APIRequest = APIRequest
 
-    response_validators: typing.List["ABCResponseValidator"]
-    request_validators: typing.List["ABCRequestValidator"]
-    http_client: "ABCHTTPClient"
+    response_validators: list["ABCResponseValidator"]
+    request_validators: list["ABCRequestValidator"]
+    http_client: "ABCNetworkClient"
     token: "Token"
 
     @property
     def api_url(self) -> str:
         """
         Address for API requests
         """
@@ -31,42 +28,38 @@
     def file_url(self) -> str:
         """
         Link to the file storage
         """
         return self.API_URL + f"file/bot{self.token}/"
 
     @abstractmethod
-    async def request(
-        self, method: str, params: typing.Optional[dict] = None
-    ) -> APIResponse:
+    async def request(self, method: str, params: dict = {}) -> bytes | None:
         """
         Opens a request session and makes a single API call
         """
         pass
 
     async def request_many(
-        self, requests: typing.Iterable[APIRequest]
-    ) -> typing.AsyncIterator[APIResponse]:
+        self, requests: typing.Iterable[APIRequest]  # type: ignore
+    ) -> typing.AsyncIterator[bytes | None]:
         """
         Makes multiple calls to the API opening session for each
         """
         for request in requests:
-            yield await self.request(request.method, request.params)
+            yield await self.request(request.method, request.params)  # type: ignore
 
-    async def validate_request(self, request: dict) -> dict:
+    async def validate_request(self, params: dict) -> dict | None:
         """
         Performs validation of the request data.
         If necessary, modifies and transforms it.
         """
-        for validator in self.request_validators:
-            request = await validator.validate(request)
-        return request
-
-    async def validate_response(
-        self, method: str, data: dict, response: dict
-    ) -> APIResponse:
+        for v in self.request_validators:
+            params = await v.validate(params)
+        return params
+
+    async def validate_response(self, response: bytes) -> bytes | None:
         """
         Verifies and adapts the response.
         """
-        for validator in self.response_validators:
-            response = await validator.validate(method, data, response, self)
+        for v in self.response_validators:
+            response = await v.validate(response)
         return response
```

### Comparing `wonda-0.5.7/wonda/api/api.py` & `wonda-0.6.0a1/wonda/api/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,37 @@
-from typing import List, Optional
-
-from wonda.api.abc import ABCAPI, APIResponse
+from wonda.api.abc import ABCAPI
 from wonda.api.utils import Token
 from wonda.api.validators import (
     DEFAULT_REQUEST_VALIDATORS,
     DEFAULT_RESPONSE_VALIDATORS,
     ABCRequestValidator,
     ABCResponseValidator,
 )
-from wonda.http.abc import ABCHTTPClient
-from wonda.http.aiohttp import AioHTTPClient
 from wonda.modules import logger
+from wonda.net.abc import ABCNetworkClient
+from wonda.net.default import DefaultNetworkClient
 from wonda.types.methods import APIMethods
 
 
 class API(ABCAPI, APIMethods):
     def __init__(
-        self,
-        token: Token,
-        http_client: Optional[ABCHTTPClient] = None,
+        self, token: Token, http_client: ABCNetworkClient | None = None
     ) -> None:
         super().__init__(self)
 
         self.token = token
-        self.http_client = http_client or AioHTTPClient()
-        self.request_validators: List[ABCRequestValidator] = DEFAULT_REQUEST_VALIDATORS
-        self.response_validators: List[
+        self.http_client = http_client or DefaultNetworkClient()
+        self.request_validators: list[ABCRequestValidator] = DEFAULT_REQUEST_VALIDATORS
+        self.response_validators: list[
             ABCResponseValidator
         ] = DEFAULT_RESPONSE_VALIDATORS
 
-    async def request(self, method: str, params: dict) -> APIResponse:
-        logger.debug(f"Calling {method} with {params}")
+    async def request(self, method: str, params: dict = {}) -> bytes | None:
+        await logger.debug("Calling", method=method, params=params)
 
-        data = await self.validate_request(params)
-        response = await self.http_client.request_json(
-            method="post", url=self.api_url + method, data=data
+        data = await self.validate_request(params or {})
+        response = await self.http_client.request_bytes(
+            self.api_url + method, data=data
         )
 
-        logger.debug(f"Server responded {response}")
-        return await self.validate_response(method, params, response)
+        await logger.debug("Received", response=response)
+        return await self.validate_response(response)
```

### Comparing `wonda-0.5.7/wonda/api/validators/request.py` & `wonda-0.6.0a1/wonda/api/validators/request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,29 @@
-from enum import Enum
 from typing import Any
 
 from aiohttp import FormData
-from pydantic import BaseModel
 
-from wonda.api.utils.file_util import File
+from wonda.api.utils.file_util import InputFile
 from wonda.api.validators.abc import ABCRequestValidator
-from wonda.modules import json
+from wonda.types.helper import Model, json
 
 
-def translate(v: Any, rec: bool = False) -> Any:
-    if isinstance(v, BaseModel):
-        return (
-            v.json(exclude_none=True, encoder=json.dumps)
-            if not rec
-            else v.dict(exclude_none=True)
-        )
+def translate(v: Any) -> Any:
+    if isinstance(v, Model):
+        return json.encode(v).decode()
     elif isinstance(v, dict):
-        return {k: translate(v, rec=True) for k, v in v.items() if v is not None}
+        return {n: translate(p) for n, p in v.items() if v is not None}
     elif isinstance(v, list):
-        return json.dumps([translate(i, rec=True) for i in v])
-    elif isinstance(v, File):
-        return v.content
-    elif isinstance(v, Enum):
-        return v.value
-    elif isinstance(v, int):
-        return str(v)
+        return [translate(i) for i in v]
+    elif isinstance(v, InputFile):
+        return (v.name, v.content)
     elif v is None:
         pass
     return v
 
 
-class TranslateFriendlyTypesRequestValidator(ABCRequestValidator):
+class TranslateTypesValidator(ABCRequestValidator):
     async def validate(self, request: dict) -> FormData:
         return FormData({k: translate(v) for k, v in request.items() if v is not None})
 
 
-__all__ = ("TranslateFriendlyTypesRequestValidator",)
+__all__ = ("TranslateTypesValidator",)
```

### Comparing `wonda-0.5.7/wonda/bot/bot.py` & `wonda-0.6.0a1/wonda/bot/bot.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,87 +1,65 @@
 from asyncio import AbstractEventLoop, get_event_loop
-from typing import List, NoReturn, Optional, Union
 
 from wonda.api import ABCAPI, API, Token
 from wonda.bot.abc import ABCFramework
-from wonda.bot.dispatch import ABCLabeler, ABCRouter, BotLabeler, BotRouter
+from wonda.bot.dispatch import (
+    ABCDispatcher,
+    ABCRouter,
+    DefaultDispatcher,
+    DefaultRouter,
+)
 from wonda.bot.polling import ABCPolling, BotPolling
-from wonda.bot.states import BotStateDispenser
+from wonda.bot.states import ABCStateDispenser, DefaultStateDispenser
 from wonda.errors import ABCErrorHandler, ErrorHandler
 from wonda.modules import logger
 from wonda.tools import LoopWrapper
 
 
 class Bot(ABCFramework):
     def __init__(
         self,
-        token: Optional[Token] = None,
-        api: Optional[ABCAPI] = None,
-        polling: Optional[ABCPolling] = None,
-        router: Optional[ABCRouter] = None,
-        labeler: Optional[ABCLabeler] = None,
-        loop: Optional[AbstractEventLoop] = None,
-        loop_wrapper: Optional[LoopWrapper] = None,
-        error_handler: Optional[ABCErrorHandler] = None,
+        token: Token | None = None,
+        api: API | None = None,
+        dispatcher: DefaultDispatcher | None = None,
+        router: ABCRouter | None = None,
+        polling: ABCPolling | None = None,
+        state_dispenser: ABCStateDispenser | None = None,
+        error_handler: ABCErrorHandler | None = None,
+        loop: AbstractEventLoop | None = None,
+        loop_wrapper: LoopWrapper | None = None,
     ):
-        self.api: Union[ABCAPI, API] = API(token) if token is not None else api  # type: ignore
         self.error_handler = error_handler or ErrorHandler()
         self.loop_wrapper = loop_wrapper or LoopWrapper()
-        self.labeler = labeler or BotLabeler()
-        self.state_dispenser = BotStateDispenser()
-        self._polling = polling or BotPolling(self.api)
-        self._router = router or BotRouter()
-        self._loop = loop
+
+        self.api = api or API(token or Token(""))
+        self.polling = polling or BotPolling(self.api, self.error_handler)
+
+        self.dispatcher = dispatcher or DefaultDispatcher()
+        self.state_dispenser = state_dispenser or DefaultStateDispenser()
+        self.router = router or DefaultRouter(
+            self.state_dispenser, self.error_handler, self.dispatcher.views()
+        )
+        self.loop = loop or get_event_loop()
 
     async def run_polling(
         self,
-        *,
         offset: int = 0,
+        allowed_updates: list[str] = [],
+        *,
         drop_updates: bool = False,
-        allowed_updates: List[str] = [],
-    ) -> NoReturn:
+    ) -> None:
         if drop_updates is True:
             await self.api.delete_webhook(drop_updates)
 
-        self.polling.offset, self.polling.allowed_updates = offset, allowed_updates
-        logger.info("Starting polling")
+        await logger.info("Starting polling")
 
         async for update in self.polling.listen():  # type: ignore
-            self.loop.create_task(self.router.route(update, self.api))
+            await self.router.route(update, self.api)
 
     def run_forever(self, **kwargs) -> None:
         self.loop_wrapper.add_task(self.run_polling(**kwargs))
         self.loop_wrapper.run_forever(self.loop)  # type: ignore
 
     @property
-    def on(self) -> "ABCLabeler":
-        return self.labeler
-
-    @property
-    def polling(self) -> "ABCPolling":
-        return self._polling.construct(self.api)
-
-    @property
-    def router(self) -> "ABCRouter":
-        return self._router.construct(
-            views=self.labeler.views(),
-            state_dispenser=self.state_dispenser,
-            error_handler=self.error_handler,
-        )
-
-    @property
-    def loop(self) -> AbstractEventLoop:
-        if self._loop is None:
-            self._loop = get_event_loop()
-        return self._loop
-
-    @loop.setter
-    def loop(self, new_loop: AbstractEventLoop):
-        self._loop = new_loop
-
-    @router.setter
-    def router(self, new_router: "ABCRouter"):
-        self._router = new_router
-
-    @polling.setter
-    def polling(self, value):
-        self._polling = value
+    def on(self) -> DefaultDispatcher:
+        return self.dispatcher
```

### Comparing `wonda-0.5.7/wonda/bot/dispatch/view/abc.py` & `wonda-0.6.0a1/wonda/bot/dispatch/view/abc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,128 +1,110 @@
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type, Union
+from typing import TYPE_CHECKING, Any, Generic, TypeVar
 
-from wonda.bot.dispatch.middlewares.base import BaseMiddleware
-from wonda.bot.updates import BaseBotUpdate, BotUpdateType
-from wonda.modules import logger
+from wonda.bot.dispatch.handler.func import FuncHandler
+from wonda.bot.dispatch.middlewares.abc import ABCMiddleware
+from wonda.bot.rules.abc import ABCRule
+from wonda.bot.updates.base import BaseUpdate
 
 if TYPE_CHECKING:
     from wonda.api import ABCAPI, API
-    from wonda.bot.dispatch.handlers.abc import ABCHandler
+    from wonda.bot.dispatch.handler.abc import ABCHandler
     from wonda.bot.states.dispenser.abc import ABCStateDispenser
+    from wonda.types.objects import Update
 
 
-class ABCView(ABC):
-    handlers: Union[List["ABCHandler"], Dict[Any, List[Any]]]
-    middlewares: List[Type["BaseMiddleware"]]
+_ = Any
+T = TypeVar("T", bound=BaseUpdate)
 
-    @abstractmethod
-    async def process_update(self, update: dict) -> bool:
-        """
-        Checks if the update is of the type
-        that this view supports
-        """
-        pass
+
+def get_update_type(update: "Update") -> str:
+    for k in update.__struct_fields__:
+        v = getattr(update, k, None)
+
+        # Handle None values and `update_id` field
+        if v is not None and not isinstance(v, int):
+            return k
+
+    return ""
+
+
+class ABCView(ABC, Generic[T]):
+    matches: str | list[str]
+
+    def __init__(self) -> None:
+        self.handlers: list["ABCHandler"] = []
+        self.middlewares: list["ABCMiddleware"] = []
+        self.auto_rules: list["ABCRule"] = []
+
+    def __init_subclass__(cls, matches: str | list[str]) -> None:
+        cls.matches = [matches] if isinstance(matches, str) else matches
+
+    def __call__(self, *rules: "ABCRule", blocking: bool = True):
+        """ """
+        assert all(
+            isinstance(rule, ABCRule) for rule in rules
+        ), "All rules must be subclasses of ABCRule"
+
+        def decorator(func) -> None:
+            self.handlers.append(
+                FuncHandler(func, [*self.auto_rules, *rules], blocking=blocking)
+            )
+
+        return decorator
 
     @abstractmethod
-    async def handle_update(
-        self,
-        update: dict,
-        ctx_api: "ABCAPI",
-        state_dispenser: "ABCStateDispenser",
-    ) -> None:
+    def get_state_key(self, update: T) -> int | None:
         pass
 
-    @staticmethod
-    @abstractmethod
-    def get_update_model(
-        update: dict, ctx_api: Union["ABCAPI", "API"]
-    ) -> "BaseBotUpdate":
+    async def filter(self, update: "Update") -> bool:
         """
-        Performs data validation and parses update
-        into BaseBotUpdate subclass
+        Checks if the update is of the type this view supports.
         """
-        pass
+        return get_update_type(update) in self.matches
 
-    async def pre_middleware(
-        self,
-        update: dict,
-        context_variables: Optional[dict] = None,
-    ) -> Optional[List[BaseMiddleware]]:
+    async def handle(
+        self, update: "Update", ctx_api: "ABCAPI", state_dispenser: "ABCStateDispenser"
+    ) -> None:
         """
-        Runs all of the pre middleware methods
-        and returns an exception if any error occurs
+        Handles the update, casting it into suitable model and saturating it with
+        useful properties like contextual API and FSM representation.
         """
-        mw_instances = []
+
+        upd = self.get_update_model(update)
+        upd.ctx_api, upd.state_repr = ctx_api, await state_dispenser.cast(  # type: ignore
+            self.get_state_key(upd)
+        )
+
+        ctx: dict[str, _] = {}
+        responses: list[_] = []
 
         for middleware in self.middlewares:
-            mw_instance = middleware(update, view=self)
-            await mw_instance.pre()
-            if not mw_instance.can_forward:
-                logger.debug(
-                    f"Pre middleware {mw_instance} "
-                    f"returned error {mw_instance.error}"
-                )
-                return None
-
-            mw_instances.append(mw_instance)
-
-            if context_variables is not None:
-                context_variables.update(mw_instance.context_update)
-
-        return mw_instances
-
-    async def post_middleware(
-        self,
-        mw_instances: List[BaseMiddleware],
-        handle_responses: Optional[List] = None,
-        handlers: Optional[List["ABCHandler"]] = None,
-    ):
-        """
-        Runs all of the post middleware methods
-        and returns an exception if any error occurs
-        """
-        for middleware in mw_instances:
-            middleware.handle_responses = (
-                handle_responses or middleware.handle_responses
-            )
-            middleware.handlers = handlers or middleware.handlers
+            result = await middleware.pre(upd, ctx)
+
+            if result is False:
+                return
+
+        for handler in self.handlers:
+            if not await handler.filter(upd, ctx):
+                continue
 
-            await middleware.post()
-            if not middleware.can_forward:
-                logger.debug(
-                    f"Post middleware {middleware} "
-                    f"returned error {middleware.error!r}"
-                )
-                return middleware.error
+            response = await handler.handle(upd, ctx)
+            responses.append(response)
 
-    def register_middleware(self, middleware: Type[BaseMiddleware]):
+        for middleware in self.middlewares:
+            await middleware.post(upd, ctx, responses)
+
+    def get_update_model(self, update: "Update") -> T:
+        upd = getattr(update, get_update_type(update))
+        return self.__orig_bases__[0].__args__[0](**upd.dict())  # type: ignore
+
+    def register_middleware(self, middleware: ABCMiddleware):
         """
-        Registers an uninitialized middleware.
-        This can also work as a decorator if needed
+        Registers a middleware. You can use this as a decorator.
         """
         try:
-            if not issubclass(middleware, BaseMiddleware):
-                raise ValueError("Argument is not a subclass of BaseMiddleware")
+            if not isinstance(middleware, ABCMiddleware):
+                raise ValueError("Argument is not an instance of ABCMiddleware")
         except TypeError:
             raise ValueError("Argument is not a class")
         self.middlewares.append(middleware)
-
-    @staticmethod
-    def get_update_type(update: dict) -> BotUpdateType:
-        """
-        Extracts the update type assuming that it is
-        always a second field in the object.
-
-        This method is a workaround for getting update types
-        because Telegram does not explicitly return them
-        """
-        update_type = list(update.keys())[1]
-        return BotUpdateType(update_type)
-
-    def __repr__(self) -> str:
-        return (
-            f"<{self.__class__.__name__} "
-            f"handlers={self.handlers} "
-            f"middlewares={self.middlewares} "
-            f"handler_return_manager={self.handler_return_manager}"
-        )
```

### Comparing `wonda-0.5.7/wonda/bot/rules/abc.py` & `wonda-0.6.0a1/wonda/bot/rules/abc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from abc import ABC, abstractmethod
-from typing import Generic, TypeVar, Union
+from typing import Generic, TypeVar
 
 T = TypeVar("T")
 
 
 class ABCRule(ABC, Generic[T]):
     @abstractmethod
-    async def check(self, update: T) -> Union[bool, dict]:
+    async def check(self, update: T, ctx: dict) -> bool:
         pass
 
     def __and__(self, other: "ABCRule") -> "AndRule":
         return AndRule(self, other)
 
     def __or__(self, other: "ABCRule") -> "OrRule":
         return OrRule(self, other)
@@ -22,51 +22,50 @@
         return f"<{self.__class__.__name__}>"
 
 
 class AndRule(ABCRule[T]):
     def __init__(self, *rules: ABCRule[T]) -> None:
         self.rules = rules
 
-    async def check(self, update: T) -> Union[bool, dict]:
-        context = {}
+    async def check(self, update: T, ctx: dict) -> bool:
+        ctx_copy = ctx.copy()
 
         for rule in self.rules:
-            check_response = await rule.check(update)
-            if check_response is False:
-                return check_response
-            elif isinstance(check_response, dict):
-                context.update(check_response)
+            if not await rule.check(update, ctx_copy):
+                return False
 
-        return context
+        ctx |= ctx_copy
+        return True
 
     def __repr__(self):
         return f"<{self.__class__.__qualname__} rules={self.rules}>"
 
 
 class NotRule(ABCRule[T]):
-    def __init__(self, *rules: ABCRule[T]) -> None:
-        self.rules = rules
+    def __init__(self, rule: ABCRule[T]) -> None:
+        self.rule = rule
 
-    async def check(self, update: T) -> bool:
-        for rule in self.rules:
-            check_response = await rule.check(update)
-            if check_response is False:
-                return True
-        return False
+    async def check(self, update: T, ctx: dict) -> bool:
+        ctx_copy = ctx.copy()
+        return not await self.rule.check(update, ctx_copy)
 
     def __repr__(self):
         return f"<{self.__class__.__qualname__} rules={self.rules}>"
 
 
 class OrRule(ABCRule[T]):
     def __init__(self, *rules: ABCRule[T]) -> None:
         self.rules = rules
 
-    async def check(self, update: T) -> None:
+    async def check(self, update: T, ctx: dict) -> bool:
         for rule in self.rules:
-            check_response = await rule.check(update)
-            if check_response is not False:
-                return check_response
+            ctx_copy = ctx.copy()
+
+            if not await rule.check(update, ctx):
+                return False
+
+            ctx |= ctx_copy
+            return True
         return False
 
     def __repr__(self):
         return f"<{self.__class__.__qualname__} rules={self.rules}>"
```

### Comparing `wonda-0.5.7/wonda/bot/rules/base.py` & `wonda-0.6.0a1/wonda/bot/rules/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,142 +1,145 @@
 import re
 from asyncio import iscoroutinefunction
-from typing import Callable, Iterable, List, Optional, Type, Union
+from functools import reduce
+from typing import Callable
 
 from wonda.bot.rules.abc import ABCRule
 from wonda.bot.states.types import BaseStateGroup, get_state_repr
-from wonda.bot.updates import BaseBotUpdate
+from wonda.bot.updates import BaseUpdate
 
 
-class Function(ABCRule[BaseBotUpdate]):
+class Function(ABCRule[BaseUpdate]):
     """
     Calls a function to check whether the update should be handled.
     Accepts any update objects, but always returns a boolean.
     """
 
-    def __init__(self, func: Callable[[BaseBotUpdate], bool]) -> None:
+    def __init__(self, func: Callable[[BaseUpdate], bool]) -> None:
         self.func = func
 
-    async def check(self, upd: BaseBotUpdate) -> bool:
+    async def check(self, upd: BaseUpdate, _) -> bool:
         if iscoroutinefunction(self.func):
             return await self.func(upd)
         return self.func(upd)
 
 
-class Has(ABCRule[BaseBotUpdate]):
+class Has(ABCRule[BaseUpdate]):
     """
-    Checks if the update dataclass has the specified attributes at its upper level.
+    Checks if the specified attributes are present in the update dataclass.
     """
 
-    def __init__(self, attr_names: Union[str, List[str]]) -> None:
+    def __init__(self, attr_names: str | list[str]) -> None:
         self.attr_names = [attr_names] if isinstance(attr_names, str) else attr_names
 
-    async def check(self, upd: BaseBotUpdate) -> bool:
-        return all(bool(getattr(upd, attr, None)) for attr in self.attr_names)
+    async def check(self, upd: BaseUpdate, _) -> bool:
+        return all(
+            bool(reduce(getattr, attr.split("."), upd)) for attr in self.attr_names
+        )
 
 
-class State(ABCRule[BaseBotUpdate]):
+class State(ABCRule[BaseUpdate]):
     """
     Checks that the user's state is currently set to one of the specified values.
     """
 
     def __init__(
-        self,
-        state: Optional[Union[BaseStateGroup, List[BaseStateGroup]]] = None,
-    ):
+        self, state: BaseStateGroup | list[BaseStateGroup] | None = None
+    ) -> None:
         if not isinstance(state, list):
             state = [] if state is None else [state]
         self.state = [get_state_repr(s) for s in state]
 
-    async def check(self, upd: BaseBotUpdate) -> bool:
+    async def check(self, upd: BaseUpdate, _) -> bool:
         if upd.state_repr is None:
             return not self.state
         return upd.state_repr.state in self.state
 
 
-class StateGroup(ABCRule[BaseBotUpdate]):
+class StateGroup(ABCRule[BaseUpdate]):
     """
     Checks that the state set for the current user belongs to one of the specified groups.
     """
 
     def __init__(
         self,
-        state_group: Union[Type[BaseStateGroup], List[Type[BaseStateGroup]]],
-    ):
+        state_group: type[BaseStateGroup] | list[type[BaseStateGroup]],
+    ) -> None:
         if not isinstance(state_group, list):
             state_group = [] if state_group is None else [state_group]
         self.state_group = [group.__name__ for group in state_group]
 
-    async def check(self, upd: BaseBotUpdate) -> bool:
+    async def check(self, upd: BaseUpdate, _) -> bool:
         if upd.state_repr is None:
             return not self.state_group
 
         group_name = upd.state_repr.state.split(":", maxsplit=1)[0]
         return group_name in self.state_group
 
 
-class Text(ABCRule[BaseBotUpdate]):
+class Text(ABCRule[BaseUpdate]):
     """
-    Checks if text/caption/query etc. is equal to one of the specified texts.
+    Checks if text contents of the update are exactly one of the specified variants.
     """
 
-    def __init__(self, texts: Union[str, List[str]], ignore_case: bool = False) -> None:
+    def __init__(self, texts: str | list[str], ignore_case: bool = False) -> None:
         if not isinstance(texts, list):
             texts = [texts]
 
         self.texts = texts
         self.ignore_case = ignore_case
 
-    async def check(self, upd: BaseBotUpdate) -> bool:
+    async def check(self, upd: BaseUpdate, _) -> bool:
         if any(
-            (text := getattr(upd, src, None))
+            (text := getattr(upd, src, ""))
             for src in ("text", "caption", "data", "query", "question")
         ):
-
             return (
                 text in self.texts
                 if not self.ignore_case
                 else text.lower() in list(map(str.lower, self.texts))
             )
+        return False
 
 
 try:
     import vbml
 except ImportError:
     vbml = None
 
 
 if vbml:
+    PatternLike = type[str | vbml.Pattern]
 
-    class Match(ABCRule[BaseBotUpdate]):
+    class Match(ABCRule[BaseUpdate]):
         """
-        Matches text, captions and queries against given patterns.
-        Docs: https://github.com/tesseradecade/vbml
+        Parses and validates text, captions and queries.
+        Learn more at: https://github.com/tesseradecade/vbml
         """
 
-        PatternLike = Union[str, vbml.Pattern]
-
         def __init__(
             self,
-            patterns: Union[PatternLike, Iterable[PatternLike]],
+            patterns: PatternLike | list[PatternLike],
             patcher: vbml.Patcher = vbml.Patcher(),
             flags: re.RegexFlag = re.RegexFlag(0),
         ) -> None:
             if not isinstance(patterns, list):
                 patterns = [patterns]
 
             self.patterns = [
                 vbml.Pattern(p, flags=flags) if isinstance(p, str) else p
                 for p in patterns
             ]
             self.patcher = patcher
 
-        async def check(self, upd: BaseBotUpdate) -> Union[bool, dict]:
+        async def check(self, upd: BaseUpdate, ctx: dict) -> bool:
             if any(
-                (text := getattr(upd, src, None))
+                (text := getattr(upd, src, ""))
                 for src in ("text", "caption", "data", "query", "question")
             ):
                 for pattern in self.patterns:
                     match = self.patcher.check(pattern, text)
 
                     if match not in (None, False):
-                        return match
+                        ctx |= match
+                        return True
+            return False
```

### Comparing `wonda-0.5.7/wonda/bot/rules/message.py` & `wonda-0.6.0a1/wonda/bot/rules/message.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,177 +1,202 @@
-import re
 from difflib import SequenceMatcher
-from typing import List, Tuple, Union
+from re import Pattern, compile, match
 
 from wonda.bot.rules.abc import ABCRule
 from wonda.bot.updates import MessageUpdate
 from wonda.types.enums import ChatType, MessageEntityType
+from wonda.types.objects import User
 
+Message = MessageUpdate
 
-class Command(ABCRule[MessageUpdate]):
+
+class Command(ABCRule[Message]):
     """
     A rule that handles bot commands. It takes in a list of
     valid command texts and checks if the message
     contains one of those commands.
     """
 
-    def __init__(
-        self, texts: Union[str, List[str]], prefixes: Union[str, List[str]] = "/"
-    ) -> None:
+    me: "User | None" = None
+
+    def __init__(self, texts: str | list[str], prefixes: str | list[str] = "/") -> None:
         self.texts = texts if isinstance(texts, list) else [texts]
         self.prefixes = prefixes if isinstance(prefixes, list) else [prefixes]
 
-    async def check(self, msg: MessageUpdate) -> Union[bool, dict]:
-        if text := msg.text or msg.caption:
+    async def check(self, m: Message, ctx: dict) -> bool:
+        if text := m.text or m.caption:
             prefix, text, tag, args = self.parse(text)
 
-            if msg.chat.type in [ChatType.GROUP, ChatType.SUPERGROUP]:
-                bot = await msg.ctx_api.get_me()
+            if m.chat.type in (ChatType.GROUP, ChatType.SUPERGROUP):
+                # Make a one-time request to get the bot info
+                # so we can compare it's short name to the tag
+                # contained in the command.
+                self.me = self.me or await m.ctx_api.get_me()
 
-                if tag and tag.lower() != bot.username.lower():
+                if not tag or tag.lower() != self.me.username.lower():  # type: ignore
                     return False
 
             if prefix not in self.prefixes or text not in self.texts:
                 return False
 
-            return {"args": args}
+            ctx["args"] = args
+            return True
+        return False
 
     @staticmethod
-    def parse(text: str) -> Tuple[str]:
+    def parse(text: str):
         head, *tail = text.split()
         pfx, (cmd, _, tag) = head[0], head[1:].partition("@")
         return pfx, cmd, tag, tail
 
 
-class From(ABCRule[MessageUpdate]):
+class From(ABCRule[Message]):
     """
     Checks if the message was sent from user or public chat
     with given username(-s).
     """
 
-    def __init__(self, chats: Union[str, List[str]]) -> None:
-        self.chats = chats if isinstance(chats, list) else [chats]
+    def __init__(self, usernames: str | list[str]) -> None:
+        self.usernames = usernames if isinstance(usernames, list) else [usernames]
 
-    async def check(self, msg: MessageUpdate) -> bool:
-        return bool(set(self.chats) & {msg.chat.username, msg.from_.username})
+    async def check(self, m: Message, _) -> bool:
+        username = m.from_.username if m.from_ is not None else m.chat.username
+        return username in self.usernames
 
 
-class Fuzzy(ABCRule[MessageUpdate]):
+class Fuzzy(ABCRule[Message]):
     """
     Compares message text with the given text
     and returns the closest match.
     """
 
-    def __init__(self, texts: Union[str, List[str]], min_ratio: int = 0.7) -> None:
+    def __init__(self, texts: str | list[str], min_ratio: float = 0.7) -> None:
         self.texts = texts if isinstance(texts, list) else [texts]
         self.min_ratio = min_ratio
 
-    async def check(self, msg: MessageUpdate) -> bool:
-        text = msg.text or msg.caption
+    async def check(self, m: Message, _) -> bool:
+        text = m.text or m.caption
 
         if not text:
             return False
 
         closest = max(SequenceMatcher(None, t, text).ratio() for t in self.texts)
         return closest >= self.min_ratio
 
 
-class IsReply(ABCRule[MessageUpdate]):
+class IsReply(ABCRule[Message]):
     """
     Checks if the message is a reply.
     """
 
-    async def check(self, msg: MessageUpdate) -> bool:
-        return msg.reply_to_message is not None
+    async def check(self, m: Message, _) -> bool:
+        return m.reply_to_message is not None
 
 
-class IsForward(ABCRule[MessageUpdate]):
+class IsForward(ABCRule[Message]):
     """
     Checks if the message was forwarded.
     """
 
-    async def check(self, msg: MessageUpdate) -> bool:
-        return msg.forward_date is not None
+    async def check(self, m: Message, _) -> bool:
+        return m.forward_date is not None
 
 
-class IsGroup(ABCRule[MessageUpdate]):
+class FromGroup(ABCRule[Message]):
     """
-    Checks if the message was sent in the chat.
+    Checks if the message was sent in a group.
     """
 
-    async def check(self, msg: MessageUpdate) -> bool:
-        return msg.chat.type in [ChatType.GROUP, ChatType.SUPERGROUP]
+    async def check(self, m: Message, _) -> bool:
+        return m.chat.type in (ChatType.GROUP, ChatType.SUPERGROUP)
 
 
-class IsPrivate(ABCRule[MessageUpdate]):
+class IsPrivate(ABCRule[Message]):
     """
     Checks if the message is private.
     """
 
-    async def check(self, msg: MessageUpdate) -> bool:
-        return msg.chat.type == ChatType.PRIVATE
+    async def check(self, m: Message, _) -> bool:
+        return m.chat.type == ChatType.PRIVATE
 
 
-class Length(ABCRule[MessageUpdate]):
+class Length(ABCRule[Message]):
     """
     Checks if the message is longer than or equal to the given length.
     """
 
     def __init__(self, min_length: int) -> None:
         self.min_length = min_length
 
-    async def check(self, msg: MessageUpdate) -> bool:
-        text = msg.text or msg.caption
+    async def check(self, m: Message, _) -> bool:
+        text = m.text or m.caption
 
         if not text:
             return False
 
         return len(text) >= self.min_length
 
 
-class Mention(ABCRule[MessageUpdate]):
+class Mention(ABCRule[Message]):
     """
     Parses message entities and checks if the message contains mention(-s).
     Returns a list of mentioned usernames.
     """
 
-    async def check(self, msg: MessageUpdate) -> Union[bool, dict]:
-        if not msg.entities:
+    async def check(self, m: Message, ctx: dict) -> bool:
+        text = m.text or m.caption
+        entities = m.entities or m.caption_entities
+
+        if entities is None or text is None:
             return False
 
         mentions = [
-            msg.text[e.offset : e.offset + e.length].strip("@")
-            for e in msg.entities
+            text[e.offset : e.offset + e.length].strip("@")
+            for e in entities
             if e.type == MessageEntityType.MENTION
         ]
 
-        return {"mentions": mentions}
+        ctx["mentions"] = mentions
+        return True
+
+
+PatternLike = str | Pattern
 
 
-class Regex(ABCRule[MessageUpdate]):
+class Regex(ABCRule[Message]):
     """
     Checks if the message text matches the given regex.
     """
 
-    PatternLike = Union[str, re.Pattern]
+    def __init__(self, expr: PatternLike | list[PatternLike]) -> None:
+        self.expr: list[Pattern[str]] = []
 
-    def __init__(self, expr: Union[PatternLike, List[PatternLike]]) -> None:
-        if isinstance(expr, re.Pattern):
-            expr = [expr]
-        elif isinstance(expr, str):
-            expr = [compile(expr)]
-        else:
-            expr = [compile(e) if isinstance(e, str) else e for e in expr]
+        match expr:
+            case Pattern() as p:
+                self.expr += [p]
+            case str(p):
+                self.expr += [compile(p)]
+            case _:
+                self.expr += [
+                    compile(expr) if isinstance(expr, str) else e for e in expr  # type: ignore
+                ]
 
-        self.expr = expr
-
-    async def check(self, msg: MessageUpdate) -> bool:
-        text = msg.text or msg.caption
+    async def check(self, m: Message, ctx: dict) -> bool:
+        text = m.text or m.caption
 
         if not text:
             return False
 
         for e in self.expr:
-            if result := re.match(e, text):
-                return {"match": result.groups()}
+            if result := match(e, text):
+                ctx["match"] = result.groups()
+                return True
 
         return False
+
+
+class WasEdited(ABCRule[Message]):
+    """
+    Checks if the message was edited.
+    """
+    async def check(self, m: Message, _) -> bool:
+        return m.edit_date is not None
```

### Comparing `wonda-0.5.7/wonda/bot/states/dispenser/abc.py` & `wonda-0.6.0a1/wonda/bot/states/dispenser/abc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING
 
 from wonda.modules import logger
 
 if TYPE_CHECKING:
     from wonda.bot.states.types import BaseStateGroup, StateRepr
     from wonda.tools.storage.abc import ABCStorage
 
 
 class ABCStateDispenser(ABC):
     storage: "ABCStorage"
 
     @abstractmethod
-    async def get(self, chat_id: int) -> Optional["StateRepr"]:
+    async def get(self, chat_id: int) -> "StateRepr | None":
         pass
 
     @abstractmethod
     async def set(self, chat_id: int, state: "BaseStateGroup", **payload) -> None:
         pass
 
     @abstractmethod
     async def finish(self, chat_id: int) -> None:
         pass
 
-    async def cast(self, chat_id: Optional[int]) -> Optional["StateRepr"]:
+    async def cast(self, chat_id: int | None = None) -> "StateRepr | None":
         if chat_id is None:
             return None
-
-        logger.debug(f"State cast for identifier {chat_id}")
+        
+        await logger.debug("State cast", id=chat_id)
         return await self.get(chat_id)
```

### Comparing `wonda-0.5.7/wonda/bot/states/dispenser/default.py` & `wonda-0.6.0a1/wonda/bot/states/dispenser/default.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from typing import Optional
-
 from wonda.bot.states.dispenser import ABCStateDispenser
 from wonda.bot.states.types import BaseStateGroup, StateRepr
 from wonda.tools.storage import ABCStorage, MemoryStorage
 
 
-class BotStateDispenser(ABCStateDispenser):
-    def __init__(self, storage: Optional[ABCStorage] = None):
+class DefaultStateDispenser(ABCStateDispenser):
+    def __init__(self, storage: ABCStorage | None = None) -> None:
         self.storage = storage or MemoryStorage()
 
-    async def get(self, chat_id: int) -> Optional[StateRepr]:
+    async def get(self, chat_id: int) -> StateRepr | None:
         return await self.storage.get(f"fsm_state:{chat_id}", default=None)
 
     async def set(self, chat_id: int, state: BaseStateGroup, **payload) -> None:
         return await self.storage.put(
             f"fsm_state:{chat_id}",
             StateRepr(chat_id=chat_id, state=state, payload=payload),
         )
```

### Comparing `wonda-0.5.7/wonda/bot/updates/__init__.py` & `wonda-0.6.0a1/wonda/bot/updates/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-from .base import BaseBotUpdate
+from .base import BaseUpdate
 from .types import *
 
 Message = MessageUpdate
 CallbackQuery = CallbackQueryUpdate
 InlineQuery = InlineQueryUpdate
 ChatJoinRequest = ChatJoinRequestUpdate
 ChatMember = ChatMemberUpdate
 ChosenInlineResult = ChosenInlineResultUpdate
-MyChatMember = MyChatMemberUpdate
 PreCheckoutQuery = PreCheckoutQueryUpdate
 ShippingQuery = ShippingQueryUpdate
 PollAnswer = PollAnswerUpdate
 Poll = PollUpdate
 
 __all__ = (
-    "BaseBotUpdate",
+    "BaseUpdate",
     "BotUpdateType",
     "Message",
     "CallbackQuery",
     "InlineQuery",
     "ChatJoinRequest",
     "ChatMember",
     "ChosenInlineResult",
-    "MyChatMember",
     "PreCheckoutQuery",
     "ShippingQuery",
     "PollAnswer",
     "Poll",
 )
```

### Comparing `wonda-0.5.7/wonda/errors/code_exception.py` & `wonda-0.6.0a1/wonda/errors/code_exception.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import Dict, Tuple, Type, TypeVar, Union, cast, no_type_check, overload
+from typing import TypeVar, cast, no_type_check, overload
 
-T = TypeVar("T", bound=Type["CodeException"])
+T = TypeVar("T", bound=type["CodeException"])
 
 
 class CodeException(Exception):
     code: int
     __code_specified__: bool = False
-    __exceptions__: Dict[int, Type["CodeException"]] = {}
+    __exceptions__: dict[int, type["CodeException"]] = {}
 
     @no_type_check
     def __new__(cls, *args, **kwargs):
         if not cls.__code_specified__:
             raise TypeError("exception code is not specified")
 
         return super().__new__(cls, *args, **kwargs)
@@ -21,20 +21,18 @@
         cls.__exceptions__ = {}
 
     @overload
     def __class_getitem__(cls: T, code: int) -> T:
         ...
 
     @overload
-    def __class_getitem__(cls: T, code: Tuple[int, ...]) -> Tuple[T, ...]:
+    def __class_getitem__(cls: T, code: tuple[int, ...]) -> tuple[T, ...]:
         ...
 
-    def __class_getitem__(
-        cls: T, code: Union[int, Tuple[int, ...]]
-    ) -> Union[T, Tuple[T, ...]]:
+    def __class_getitem__(cls: T, code: int | tuple[int, ...]) -> T | tuple[T, ...]:
         if cls.__code_specified__:
             raise TypeError("exception code already specified")
 
         if isinstance(code, tuple):
             return tuple(cls._get_exception(c) for c in code)
 
         return cls._get_exception(code)
```

### Comparing `wonda-0.5.7/wonda/errors/error_handler/abc.py` & `wonda-0.6.0a1/wonda/errors/error_handler/abc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from abc import ABC, abstractmethod
-from typing import Any, Awaitable, Callable, Dict, Optional, Type
+from typing import Any, Awaitable, Callable
 
 AsyncFunc = Callable[..., Awaitable[Any]]
 
 
 class ABCErrorHandler(ABC):
-    error_handlers: Dict[Type[BaseException], AsyncFunc]
-    undefined_error_handler: Optional[AsyncFunc]
+    error_handlers: dict[type[BaseException], AsyncFunc]
+    undefined_error_handler: AsyncFunc | None
 
     @abstractmethod
     def register_error_handler(
-        self, *error_types: Type[BaseException]
+        self, *error_types: type[BaseException]
     ) -> Callable[[AsyncFunc], AsyncFunc]:
         pass
 
     @abstractmethod
     def register_undefined_error_handler(self, handler: AsyncFunc) -> AsyncFunc:
         pass
```

### Comparing `wonda-0.5.7/wonda/errors/error_handler/error_handler.py` & `wonda-0.6.0a1/wonda/errors/error_handler/error_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 from functools import wraps
-from typing import TYPE_CHECKING, Any, Callable, Optional, Type
+from typing import TYPE_CHECKING, Any, Callable
 
 from .abc import ABCErrorHandler
 
 if TYPE_CHECKING:
     from .abc import AsyncFunc
 
 from wonda.modules import logger
 
 
 class ErrorHandler(ABCErrorHandler):
     def __init__(
         self, redirect_arguments: bool = False, raise_exceptions: bool = False
     ):
-        self.redirect_arguments = redirect_arguments
-        self.raise_exceptions = raise_exceptions
         self.error_handlers = {}
         self.undefined_error_handler = None
 
+        self.redirect_arguments = redirect_arguments
+        self.raise_exceptions = raise_exceptions
+
     def register_error_handler(
-        self, *error_types: Type[BaseException]
+        self, *error_types: type[BaseException]
     ) -> Callable[["AsyncFunc"], "AsyncFunc"]:
         def decorator(handler: "AsyncFunc") -> "AsyncFunc":
             for error_type in error_types:
                 self.error_handlers[error_type] = handler
             return handler
 
         return decorator
 
     def register_undefined_error_handler(self, handler: "AsyncFunc") -> "AsyncFunc":
         self.undefined_error_handler = handler
         return handler
 
-    def lookup_handler(self, for_type: Type[BaseException]) -> Optional["AsyncFunc"]:
+    def lookup_handler(self, for_type: type[BaseException]) -> "AsyncFunc | None":
         for error_type in self.error_handlers:
             if issubclass(for_type, error_type):
                 return self.error_handlers[error_type]
+        return None
 
     async def handle(self, error: BaseException, *args, **kwargs) -> Any:
         handler = self.lookup_handler(type(error)) or self.undefined_error_handler
 
         if not handler:
             if self.raise_exceptions:
                 raise error
-            logger.exception(error)
+            await logger.exception(error)
             return
 
         if self.redirect_arguments:
             return await handler(error, *args, **kwargs)
         return await handler(error)
 
     def catch(self, func: "AsyncFunc") -> "AsyncFunc":
```

### Comparing `wonda-0.5.7/wonda/tools/keyboard/abc.py` & `wonda-0.6.0a1/wonda/tools/keyboard/builder.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,87 +1,100 @@
-from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Any, Dict, List, Union
+from typing import Any, Generic, TypeVar
 
-if TYPE_CHECKING:
-    from wonda.types.objects import InlineKeyboardMarkup, ReplyKeyboardMarkup
+from wonda.tools.keyboard.abc import ABCButton, ABCKeyboardBuilder
+from wonda.types.objects import (
+    InlineKeyboardButton,
+    InlineKeyboardMarkup,
+    KeyboardButton,
+    ReplyKeyboardMarkup,
+    ReplyKeyboardRemove,
+)
 
-    AnyMarkup = Union[ReplyKeyboardMarkup, InlineKeyboardMarkup]
+_ = Any
+T = TypeVar("T")
 
 
-class Button:
+class BaseKeyboardBuilder(ABCKeyboardBuilder, Generic[T]):
     """
-    A text-only keyboard button interface. All 
-    other button types should inherit this class.
+    A basic keyboard builder which implements independent logic for
+    `.add()` and `.row()` methods
     """
 
-    def __init__(self, text: str) -> None:
-        self.text = text
+    def __init__(self) -> None:
+        self.rows: list[list[ABCButton]] = [[]]
 
-    def get_data(self) -> dict:
+    @property
+    def keyboard(self) -> list[list[Any]]:
         """
-        Returns the button data.
+        Keyboard markup to be sent.
         """
-        return {k: v for k, v in self.__dict__.items() if v is not None}
-
-
-class ABCBuilder(ABC):
-    """
-    An abstract keyboard builder interface.
-    """
+        type = self.__orig_bases__[0].__args__[0]  # type: ignore
+        return [[type(**button.dict()) for button in row] for row in self.rows]
 
-    buttons: List[List[Button]]
-
-    def add(self, button: Button) -> "ABCBuilder":
+    @property
+    def last_row(self) -> list[ABCButton]:
         """
-        Adds a button to the keyboard.
+        Convenience property to get the last button row.
         """
-        if not len(self.buttons):
+        return self.rows[-1]
+
+    def add(self, button: ABCButton) -> "BaseKeyboardBuilder":
+        if not len(self.rows):
             self.row()
 
         self.last_row.append(button)
         return self
 
-    @abstractmethod
-    def build(self) -> "AnyMarkup":
-        """
-        Builds the keyboard into whatever markup object.
-        """
-        pass
+    def row(self) -> "BaseKeyboardBuilder":
+        if len(self.rows) and not len(self.last_row):
+            raise ValueError("Last row is empty")
 
-    @classmethod
-    def empty(cls) -> str:
-        """
-        Returns an empty keyboard.
-        """
-        return cls().build()
+        self.rows.append([])
+        return self
 
-    @property
-    def keyboard(self) -> List[List[Dict[str, Any]]]:
-        """
-        Convenience property to get the keyboard data.
-        """
-        return [[button.get_data() for button in row] for row in self.buttons]
+    def build(self) -> ReplyKeyboardMarkup | InlineKeyboardMarkup:
+        raise NotImplementedError("`.build()` method implemenation is builder specific")
 
-    @property
-    def last_row(self) -> List[Button]:
-        """
-        Convenience property to get the last button row.
-        """
-        return self.buttons[-1]
 
-    def merge(self, builder: "ABCBuilder") -> "ABCBuilder":
-        self.buttons.extend(builder.buttons)
-        return self
+class InlineKeyboardBuilder(BaseKeyboardBuilder[InlineKeyboardButton]):
+    """
+    A builder for an inline keyboard. No options are available
+    for this type of keyboard.
+    """
 
-    def row(self) -> "ABCBuilder":
-        """
-        Adds a row to the keyboard.
-        Panics if the last row was empty.
-        """
-        if len(self.buttons) and not len(self.last_row):
-            raise ValueError("Last row is empty")
+    def build(self) -> InlineKeyboardMarkup:
+        return InlineKeyboardMarkup(self.keyboard)
 
-        self.buttons.append([])
-        return self
 
-    def __repr__(self) -> str:
-        return self.build().json()
+class ReplyKeyboardBuilder(BaseKeyboardBuilder[KeyboardButton]):
+    """
+    A builder for a keyboard with custom reply options.
+    """
+
+    def __init__(
+        self,
+        is_persistent: bool = False,
+        resize_keyboard: bool = False,
+        one_time_keyboard: bool = False,
+        selective: bool = False,
+    ) -> None:
+        self.is_persistent = is_persistent
+        self.resize_keyboard = resize_keyboard
+        self.one_time_keyboard = one_time_keyboard
+        self.selective = selective
+        self.rows = [[]]
+
+    def build(self) -> ReplyKeyboardMarkup:
+        return ReplyKeyboardMarkup(
+            keyboard=self.keyboard,
+            is_persistent=self.is_persistent,
+            resize_keyboard=self.resize_keyboard,
+            one_time_keyboard=self.one_time_keyboard,
+            selective=self.selective,
+        )
+
+    @staticmethod
+    def remove(selective: bool | None = None) -> ReplyKeyboardRemove:
+        """
+        A shortcut to remove a reply keyboard.
+        """
+        return ReplyKeyboardRemove(selective=selective, remove_keyboard=True)
```

### Comparing `wonda-0.5.7/wonda/tools/keyboard/reply.py` & `wonda-0.6.0a1/wonda/tools/keyboard/elements.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,114 @@
-from wonda.tools.keyboard.abc import ABCBuilder, Button
+from wonda.tools.keyboard.abc import ABCButton
 from wonda.types.objects import (
+    CallbackGame,
     ChatAdministratorRights,
     KeyboardButtonPollType,
     KeyboardButtonRequestChat,
     KeyboardButtonRequestUser,
-    ReplyKeyboardMarkup,
-    ReplyKeyboardRemove,
+    LoginUrl,
     WebAppInfo,
 )
 
 
-class ReplyKeyboard(ABCBuilder):
-    """
-    A builder for reply keyboard markup.
-    """
-
-    def __init__(
-        self,
-        is_persistent: bool = False,
-        resize_keyboard: bool = False,
-        one_time_keyboard: bool = False,
-        selective: bool = False,
-    ) -> None:
-        self.is_persistent = is_persistent
-        self.resize_keyboard = resize_keyboard
-        self.one_time_keyboard = one_time_keyboard
-        self.selective = selective
-        self.buttons = [[]]
-
-    def build(self) -> ReplyKeyboardMarkup:
-        return ReplyKeyboardMarkup(
-            keyboard=self.keyboard,
-            is_persistent=self.is_persistent,
-            resize_keyboard=self.resize_keyboard,
-            one_time_keyboard=self.one_time_keyboard,
-            selective=self.selective,
-        )
+class Button(ABCButton):
+    def __init__(self, text: str) -> None:
+        self.text = text
 
-    @staticmethod
-    def remove(selective: bool = None) -> ReplyKeyboardRemove:
+    def dict(self) -> dict:
         """
-        A shortcut to remove a reply keyboard.
+        Returns the button data.
         """
-        return ReplyKeyboardRemove(selective=selective, remove_keyboard=True)
+        return {k: v for k, v in self.__dict__.items() if v is not None}
 
 
 class App(Button):
     """
-    This button opens specified web app that will be able to send a “web_app_data”
-    service message. Available in private chats only.
+    This button opens specified web app which will be able to send an arbitrary message
+    on behalf of the user using the method `answerWebAppQuery`. Available only
+    in private chats between a user and the bot.
     """
 
     def __init__(self, text: str, web_app: WebAppInfo) -> None:
         super().__init__(text)
         self.web_app = web_app
 
 
+class Callback(Button):
+    """
+    A button that sends a callback query to the bot when pressed.
+    """
+
+    def __init__(self, text: str, data: str) -> None:
+        super().__init__(text)
+        self.callback_data = data
+
+
+class Game(Button):
+    """
+    This button will launch a game in the chat when pressed.
+    This type of button must always be the first button in the first row.
+    """
+
+    def __init__(self, text: str, game: CallbackGame) -> None:
+        super().__init__(text)
+        self.callback_game = game
+
+
+class Login(Button):
+    """
+    A button containing a login URL. This button will open a web page
+    with the specified URL and ask the user to log in. Can be used
+    as a replacement for the Telegram Login Widget.
+    """
+
+    def __init__(self, text: str, login_url: LoginUrl) -> None:
+        super().__init__(text)
+        self.login_url = login_url
+
+
+class Pay(Button):
+    """
+    A pay button. This type of button must always be the first button
+    in the first row and can only be used in invoice messages.
+    """
+
+    def __init__(self, text: str) -> None:
+        super().__init__(text)
+        self.pay = True
+
+
+class Switch(Button):
+    """
+    Pressing the button will open specified inline query in the chat,
+    either current or selected by the user.
+    """
+
+    def __init__(self, text: str, query: str, current_chat: bool = False) -> None:
+        super().__init__(text)
+
+        setattr(
+            self,
+            "switch_inline_query_current_chat"
+            if current_chat
+            else "switch_inline_query",
+            query,
+        )
+
+
+class URL(Button):
+    """
+    When this button is pressed, HTTP or tg:// link is opened.
+    """
+
+    def __init__(self, text: str, url: str) -> None:
+        super().__init__(text)
+        self.url = url
+
+
 class Contact(Button):
     """
     When pressed, the user's phone number will be sent as a contact.
     Available in private chats only.
     """
 
     def __init__(self, text: str) -> None:
@@ -95,17 +144,17 @@
     Tapping on any user will send their identifier to the bot in a "user_shared"
     service message. Available in private chats only.
     """
 
     def __init__(
         self,
         text: str,
-        request_id: int = None,
-        is_bot: bool = None,
-        is_premium: bool = None,
+        request_id: int,
+        is_bot: bool | None = None,
+        is_premium: bool | None = None,
     ) -> None:
         super().__init__(text)
         self.request_user = KeyboardButtonRequestUser(
             request_id=request_id, user_is_bot=is_bot, user_is_premium=is_premium
         )
 
 
@@ -117,20 +166,20 @@
     """
 
     def __init__(
         self,
         text: str,
         request_id: int,
         is_channel: bool,
-        is_forum: bool = None,
-        has_username: bool = None,
-        is_created: bool = None,
-        user_administrator_rights: ChatAdministratorRights = None,
-        bot_administrator_rights: ChatAdministratorRights = None,
-        bot_is_member: bool = None,
+        is_forum: bool | None = None,
+        has_username: bool | None = None,
+        is_created: bool | None = None,
+        user_administrator_rights: ChatAdministratorRights | None = None,
+        bot_administrator_rights: ChatAdministratorRights | None = None,
+        bot_is_member: bool | None = None,
     ) -> None:
         super().__init__(text)
         self.request_chat = KeyboardButtonRequestChat(
             request_id=request_id,
             chat_is_channel=is_channel,
             chat_is_forum=is_forum,
             chat_has_username=has_username,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `wonda-0.5.7/wonda/tools/storage/abc.py` & `wonda-0.6.0a1/wonda/tools/storage/abc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from abc import ABC, abstractmethod
 
-from wonda.tools.storage.types import NO_KEY, TTL, Key, Value
+from wonda.tools.storage.types import Ex, Key, Value
 
 
 class ABCBaseStorage(ABC):
     @abstractmethod
-    def get(self, key: Key, default: Value = NO_KEY) -> Value:
+    async def get(self, key: Key, default: Value = ...) -> Value:
         pass
 
     @abstractmethod
-    def delete(self, key: Key) -> None:
+    async def delete(self, key: Key) -> None:
         pass
 
     @abstractmethod
-    def contains(self, key: Key) -> bool:
+    async def contains(self, key: Key) -> bool:
         pass
 
 
 class ABCStorage(ABCBaseStorage):
     @abstractmethod
     async def put(self, key: Key, value: Value) -> None:
         pass
 
 
-class ABCExpiringStorage(ABCStorage):
+class ABCExpiringStorage(ABCBaseStorage):
     @abstractmethod
-    async def put(self, key: Key, value: Value, ttl: TTL) -> None:
+    async def put(self, key: Key, value: Value, ex: Ex) -> None:
         pass
```

### Comparing `wonda-0.5.7/wonda/tools/text/formatting/html.py` & `wonda-0.6.0a1/wonda/tools/text/formatting/html.py`

 * *Files identical despite different names*

### Comparing `wonda-0.5.7/wonda/tools/text/formatting/markdown.py` & `wonda-0.6.0a1/wonda/tools/text/formatting/markdown.py`

 * *Files identical despite different names*

### Comparing `wonda-0.5.7/wonda/types/enums.py` & `wonda-0.6.0a1/wonda/types/enums.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from enum import Enum
 
 
-class ChatType(Enum):
+class ChatType(str, Enum):
     PRIVATE = "private"
     GROUP = "group"
     SUPERGROUP = "supergroup"
     CHANNEL = "channel"
 
 
-class MessageEntityType(Enum):
+class MessageEntityType(str, Enum):
     MENTION = "mention"
     HASHTAG = "hashtag"
     CASHTAG = "cashtag"
     BOT_COMMAND = "bot_command"
     URL = "url"
     EMAIL = "email"
     PHONE_NUMBER = "phone_number"
@@ -24,69 +24,69 @@
     CODE = "code"
     PRE = "pre"
     TEXT_LINK = "text_link"
     TEXT_MENTION = "text_mention"
     CUSTOM_EMOJI = "custom_emoji"
 
 
-class PollType(Enum):
+class PollType(str, Enum):
     REGULAR = "regular"
     QUIZ = "quiz"
 
 
-class StickerType(Enum):
+class StickerType(str, Enum):
     REGULAR = "regular"
     MASK = "mask"
     CUSTOM_EMOJI = "custom_emoji"
 
 
-class StickerSetStickerType(Enum):
+class StickerSetStickerType(str, Enum):
     REGULAR = "regular"
     MASK = "mask"
     CUSTOM_EMOJI = "custom_emoji"
 
 
-class MaskPositionPoint(Enum):
+class MaskPositionPoint(str, Enum):
     FOREHEAD = "forehead"
     EYES = "eyes"
     MOUTH = "mouth"
     CHIN = "chin"
 
 
-class InlineQueryChatType(Enum):
+class InlineQueryChatType(str, Enum):
     SENDER = "sender"
     PRIVATE = "private"
     GROUP = "group"
     SUPERGROUP = "supergroup"
     CHANNEL = "channel"
 
 
-class InlineQueryResultGifThumbnailMimeType(Enum):
+class InlineQueryResultGifThumbnailMimeType(str, Enum):
     IMAGE_JPEG = "image/jpeg"
     IMAGE_GIF = "image/gif"
     VIDEO_MP4 = "video/mp4"
 
 
-class InlineQueryResultMpeg4GifThumbnailMimeType(Enum):
+class InlineQueryResultMpeg4GifThumbnailMimeType(str, Enum):
     IMAGE_JPEG = "image/jpeg"
     IMAGE_GIF = "image/gif"
     VIDEO_MP4 = "video/mp4"
 
 
-class InlineQueryResultVideoMimeType(Enum):
+class InlineQueryResultVideoMimeType(str, Enum):
     TEXT_HTML = "text/html"
     VIDEO_MP4 = "video/mp4"
 
 
-class InlineQueryResultDocumentMimeType(Enum):
+class InlineQueryResultDocumentMimeType(str, Enum):
     APPLICATION_PDF = "application/pdf"
     APPLICATION_ZIP = "application/zip"
 
 
-class EncryptedPassportElementType(Enum):
+class EncryptedPassportElementType(str, Enum):
     PERSONAL_DETAILS = "personal_details"
     PASSPORT = "passport"
     DRIVER_LICENSE = "driver_license"
     IDENTITY_CARD = "identity_card"
     INTERNAL_PASSPORT = "internal_passport"
     ADDRESS = "address"
     UTILITY_BILL = "utility_bill"
@@ -94,71 +94,71 @@
     RENTAL_AGREEMENT = "rental_agreement"
     PASSPORT_REGISTRATION = "passport_registration"
     TEMPORARY_REGISTRATION = "temporary_registration"
     PHONE_NUMBER = "phone_number"
     EMAIL = "email"
 
 
-class PassportElementErrorDataFieldType(Enum):
+class PassportElementErrorDataFieldType(str, Enum):
     PERSONAL_DETAILS = "personal_details"
     PASSPORT = "passport"
     DRIVER_LICENSE = "driver_license"
     IDENTITY_CARD = "identity_card"
     INTERNAL_PASSPORT = "internal_passport"
     ADDRESS = "address"
 
 
-class PassportElementErrorFrontSideType(Enum):
+class PassportElementErrorFrontSideType(str, Enum):
     PASSPORT = "passport"
     DRIVER_LICENSE = "driver_license"
     IDENTITY_CARD = "identity_card"
     INTERNAL_PASSPORT = "internal_passport"
 
 
-class PassportElementErrorReverseSideType(Enum):
+class PassportElementErrorReverseSideType(str, Enum):
     DRIVER_LICENSE = "driver_license"
     IDENTITY_CARD = "identity_card"
 
 
-class PassportElementErrorSelfieType(Enum):
+class PassportElementErrorSelfieType(str, Enum):
     PASSPORT = "passport"
     DRIVER_LICENSE = "driver_license"
     IDENTITY_CARD = "identity_card"
     INTERNAL_PASSPORT = "internal_passport"
 
 
-class PassportElementErrorFileType(Enum):
+class PassportElementErrorFileType(str, Enum):
     UTILITY_BILL = "utility_bill"
     BANK_STATEMENT = "bank_statement"
     RENTAL_AGREEMENT = "rental_agreement"
     PASSPORT_REGISTRATION = "passport_registration"
     TEMPORARY_REGISTRATION = "temporary_registration"
 
 
-class PassportElementErrorFilesType(Enum):
+class PassportElementErrorFilesType(str, Enum):
     UTILITY_BILL = "utility_bill"
     BANK_STATEMENT = "bank_statement"
     RENTAL_AGREEMENT = "rental_agreement"
     PASSPORT_REGISTRATION = "passport_registration"
     TEMPORARY_REGISTRATION = "temporary_registration"
 
 
-class PassportElementErrorTranslationFileType(Enum):
+class PassportElementErrorTranslationFileType(str, Enum):
     PASSPORT = "passport"
     DRIVER_LICENSE = "driver_license"
     IDENTITY_CARD = "identity_card"
     INTERNAL_PASSPORT = "internal_passport"
     UTILITY_BILL = "utility_bill"
     BANK_STATEMENT = "bank_statement"
     RENTAL_AGREEMENT = "rental_agreement"
     PASSPORT_REGISTRATION = "passport_registration"
     TEMPORARY_REGISTRATION = "temporary_registration"
 
 
-class PassportElementErrorTranslationFilesType(Enum):
+class PassportElementErrorTranslationFilesType(str, Enum):
     PASSPORT = "passport"
     DRIVER_LICENSE = "driver_license"
     IDENTITY_CARD = "identity_card"
     INTERNAL_PASSPORT = "internal_passport"
     UTILITY_BILL = "utility_bill"
     BANK_STATEMENT = "bank_statement"
     RENTAL_AGREEMENT = "rental_agreement"
```

### Comparing `wonda-0.5.7/wonda/types/methods.py` & `wonda-0.6.0a1/wonda/types/methods.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,1935 +1,1912 @@
-from typing import *
-
-from pydantic import parse_obj_as
+import typing
 
 from .objects import *
 
-if TYPE_CHECKING:
+if typing.TYPE_CHECKING:
     from wonda.api import ABCAPI, API
-    from wonda.api import File as InputFile
 
 
 class APIMethods:
-    def __init__(self, api: Union["ABCAPI", "API"]) -> None:
+    def __init__(self, api: "ABCAPI | API") -> None:
         self.api = api
 
-    @staticmethod
-    def get_params(loc: dict) -> dict:
-        n = {
-            k: v
-            for k, v in loc.items()
-            if k not in ("self", "kwargs") and v is not None
-        }
-        n.update(loc["kwargs"])
-        return n
-
     async def get_updates(
         self,
-        timeout: Optional[int] = None,
-        offset: Optional[int] = None,
-        limit: Optional[int] = None,
-        allowed_updates: Optional[List[str]] = None,
+        timeout: int | None = None,
+        offset: int | None = None,
+        limit: int | None = None,
+        allowed_updates: list[str] | None = None,
         **kwargs
-    ) -> List[Update]:
+    ) -> list[Update]:
         """
-        Use this method to receive incoming updates using long polling (wiki). Returns an
-        Array of Update objects.
+        Use this method to receive incoming updates using long polling (wiki).
+        Returns an Array of Update objects.
         """
-        response = await self.api.request("getUpdates", self.get_params(locals()))
-        return parse_obj_as(List[Update], response)
+        response = await self.api.request("getUpdates", get_params(locals()))
+        return json.decode(response, type=list[Update])
 
     async def set_webhook(
         self,
         url: str,
-        secret_token: Optional[str] = None,
-        max_connections: Optional[int] = None,
-        ip_address: Optional[str] = None,
-        drop_pending_updates: Optional[bool] = None,
-        certificate: Optional[InputFile] = None,
-        allowed_updates: Optional[List[str]] = None,
+        secret_token: str | None = None,
+        max_connections: int | None = None,
+        ip_address: str | None = None,
+        drop_pending_updates: bool | None = None,
+        certificate: InputFile | None = None,
+        allowed_updates: list[str] | None = None,
         **kwargs
     ) -> bool:
         """
-        Use this method to specify a URL and receive incoming updates via an outgoing
-        webhook. Whenever there is an update for the bot, we will send an HTTPS POST request
-        to the specified URL, containing a JSON-serialized Update. In case of an
-        unsuccessful request, we will give up after a reasonable amount of attempts. Returns
-        True on success. If you'd like to make sure that the webhook was set by you, you can
-        specify secret data in the parameter secret_token. If specified, the request will
-        contain a header “X-Telegram-Bot-Api-Secret-Token” with the secret token as content.
+        Use this method to specify a URL and receive incoming updates via an
+        outgoing webhook. Whenever there is an update for the bot, we will
+        send an HTTPS POST request to the specified URL, containing a JSON-
+        serialized Update. In case of an unsuccessful request, we will give up
+        after a reasonable amount of attempts. Returns True on success. If
+        you'd like to make sure that the webhook was set by you, you can
+        specify secret data in the parameter secret_token. If specified, the
+        request will contain a header “X-Telegram-Bot-Api-Secret-Token” with
+        the secret token as content.
         """
-        response = await self.api.request("setWebhook", self.get_params(locals()))
-        return response
+        response = await self.api.request("setWebhook", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def delete_webhook(
-        self, drop_pending_updates: Optional[bool] = None, **kwargs
+        self, drop_pending_updates: bool | None = None, **kwargs
     ) -> bool:
         """
-        Use this method to remove webhook integration if you decide to switch back to
-        getUpdates. Returns True on success.
+        Use this method to remove webhook integration if you decide to switch
+        back to getUpdates. Returns True on success.
         """
-        response = await self.api.request("deleteWebhook", self.get_params(locals()))
-        return response
+        response = await self.api.request("deleteWebhook", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def get_webhook_info(self, **kwargs) -> WebhookInfo:
         """
-        Use this method to get current webhook status. Requires no parameters. On success,
-        returns a WebhookInfo object. If the bot is using getUpdates, will return an object
-        with the url field empty.
+        Use this method to get current webhook status. Requires no parameters.
+        On success, returns a WebhookInfo object. If the bot is using
+        getUpdates, will return an object with the url field empty.
         """
-        response = await self.api.request("getWebhookInfo", self.get_params(locals()))
-        return WebhookInfo(**response)
+        response = await self.api.request("getWebhookInfo", get_params(locals()))
+        return json.decode(response, type=WebhookInfo)
 
     async def get_me(self, **kwargs) -> User:
         """
-        A simple method for testing your bot's authentication token. Requires no parameters.
-        Returns basic information about the bot in form of a User object.
+        A simple method for testing your bot's authentication token. Requires
+        no parameters. Returns basic information about the bot in form of a
+        User object.
         """
-        response = await self.api.request("getMe", self.get_params(locals()))
-        return User(**response)
+        response = await self.api.request("getMe", get_params(locals()))
+        return json.decode(response, type=User)
 
     async def log_out(self, **kwargs) -> bool:
         """
-        Use this method to log out from the cloud Bot API server before launching the bot
-        locally. You must log out the bot before running it locally, otherwise there is no
-        guarantee that the bot will receive updates. After a successful call, you can
-        immediately log in on a local server, but will not be able to log in back to the
-        cloud Bot API server for 10 minutes. Returns True on success. Requires no
+        Use this method to log out from the cloud Bot API server before
+        launching the bot locally. You must log out the bot before running it
+        locally, otherwise there is no guarantee that the bot will receive
+        updates. After a successful call, you can immediately log in on a
+        local server, but will not be able to log in back to the cloud Bot API
+        server for 10 minutes. Returns True on success. Requires no
         parameters.
         """
-        response = await self.api.request("logOut", self.get_params(locals()))
-        return response
+        response = await self.api.request("logOut", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def close(self, **kwargs) -> bool:
         """
-        Use this method to close the bot instance before moving it from one local server to
-        another. You need to delete the webhook before calling this method to ensure that
-        the bot isn't launched again after server restart. The method will return error 429
-        in the first 10 minutes after the bot is launched. Returns True on success. Requires
-        no parameters.
+        Use this method to close the bot instance before moving it from one
+        local server to another. You need to delete the webhook before calling
+        this method to ensure that the bot isn't launched again after server
+        restart. The method will return error 429 in the first 10 minutes
+        after the bot is launched. Returns True on success. Requires no
+        parameters.
         """
-        response = await self.api.request("close", self.get_params(locals()))
-        return response
+        response = await self.api.request("close", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def send_message(
         self,
         text: str,
-        chat_id: Union[int, str],
-        reply_to_message_id: Optional[int] = None,
-        reply_markup: Optional[
-            Union[
-                InlineKeyboardMarkup,
-                ReplyKeyboardMarkup,
-                ReplyKeyboardRemove,
-                ForceReply,
-            ]
-        ] = None,
-        protect_content: Optional[bool] = None,
-        parse_mode: Optional[str] = None,
-        message_thread_id: Optional[int] = None,
-        entities: Optional[List[MessageEntity]] = None,
-        disable_web_page_preview: Optional[bool] = None,
-        disable_notification: Optional[bool] = None,
-        allow_sending_without_reply: Optional[bool] = None,
+        chat_id: int | str,
+        reply_to_message_id: int | None = None,
+        reply_markup: InlineKeyboardMarkup
+        | ReplyKeyboardMarkup
+        | ReplyKeyboardRemove
+        | ForceReply
+        | None = None,
+        protect_content: bool | None = None,
+        parse_mode: str | None = None,
+        message_thread_id: int | None = None,
+        entities: list[MessageEntity] | None = None,
+        disable_web_page_preview: bool | None = None,
+        disable_notification: bool | None = None,
+        allow_sending_without_reply: bool | None = None,
         **kwargs
     ) -> Message:
         """
-        Use this method to send text messages. On success, the sent Message is returned.
+        Use this method to send text messages. On success, the sent Message is
+        returned.
         """
-        response = await self.api.request("sendMessage", self.get_params(locals()))
-        return Message(**response)
+        response = await self.api.request("sendMessage", get_params(locals()))
+        return json.decode(response, type=Message)
 
     async def forward_message(
         self,
         message_id: int,
-        from_chat_id: Union[int, str],
-        chat_id: Union[int, str],
-        protect_content: Optional[bool] = None,
-        message_thread_id: Optional[int] = None,
-        disable_notification: Optional[bool] = None,
+        from_chat_id: int | str,
+        chat_id: int | str,
+        protect_content: bool | None = None,
+        message_thread_id: int | None = None,
+        disable_notification: bool | None = None,
         **kwargs
     ) -> Message:
         """
-        Use this method to forward messages of any kind. Service messages can't be
-        forwarded. On success, the sent Message is returned.
+        Use this method to forward messages of any kind. Service messages
+        can't be forwarded. On success, the sent Message is returned.
         """
-        response = await self.api.request("forwardMessage", self.get_params(locals()))
-        return Message(**response)
+        response = await self.api.request("forwardMessage", get_params(locals()))
+        return json.decode(response, type=Message)
 
     async def copy_message(
         self,
         message_id: int,
-        from_chat_id: Union[int, str],
-        chat_id: Union[int, str],
-        reply_to_message_id: Optional[int] = None,
-        reply_markup: Optional[
-            Union[
-                InlineKeyboardMarkup,
-                ReplyKeyboardMarkup,
-                ReplyKeyboardRemove,
-                ForceReply,
-            ]
-        ] = None,
-        protect_content: Optional[bool] = None,
-        parse_mode: Optional[str] = None,
-        message_thread_id: Optional[int] = None,
-        disable_notification: Optional[bool] = None,
-        caption_entities: Optional[List[MessageEntity]] = None,
-        caption: Optional[str] = None,
-        allow_sending_without_reply: Optional[bool] = None,
+        from_chat_id: int | str,
+        chat_id: int | str,
+        reply_to_message_id: int | None = None,
+        reply_markup: InlineKeyboardMarkup
+        | ReplyKeyboardMarkup
+        | ReplyKeyboardRemove
+        | ForceReply
+        | None = None,
+        protect_content: bool | None = None,
+        parse_mode: str | None = None,
+        message_thread_id: int | None = None,
+        disable_notification: bool | None = None,
+        caption_entities: list[MessageEntity] | None = None,
+        caption: str | None = None,
+        allow_sending_without_reply: bool | None = None,
         **kwargs
     ) -> MessageId:
         """
-        Use this method to copy messages of any kind. Service messages and invoice messages
-        can't be copied. A quiz poll can be copied only if the value of the field
-        correct_option_id is known to the bot. The method is analogous to the method
-        forwardMessage, but the copied message doesn't have a link to the original message.
-        Returns the MessageId of the sent message on success.
+        Use this method to copy messages of any kind. Service messages and
+        invoice messages can't be copied. A quiz poll can be copied only if
+        the value of the field correct_option_id is known to the bot. The
+        method is analogous to the method forwardMessage, but the copied
+        message doesn't have a link to the original message. Returns the
+        MessageId of the sent message on success.
         """
-        response = await self.api.request("copyMessage", self.get_params(locals()))
-        return MessageId(**response)
+        response = await self.api.request("copyMessage", get_params(locals()))
+        return json.decode(response, type=MessageId)
 
     async def send_photo(
         self,
-        photo: Union[InputFile, str],
-        chat_id: Union[int, str],
-        reply_to_message_id: Optional[int] = None,
-        reply_markup: Optional[
-            Union[
-                InlineKeyboardMarkup,
-                ReplyKeyboardMarkup,
-                ReplyKeyboardRemove,
-                ForceReply,
-            ]
-        ] = None,
-        protect_content: Optional[bool] = None,
-        parse_mode: Optional[str] = None,
-        message_thread_id: Optional[int] = None,
-        has_spoiler: Optional[bool] = None,
-        disable_notification: Optional[bool] = None,
-        caption_entities: Optional[List[MessageEntity]] = None,
-        caption: Optional[str] = None,
-        allow_sending_without_reply: Optional[bool] = None,
+        photo: InputFile | str,
+        chat_id: int | str,
+        reply_to_message_id: int | None = None,
+        reply_markup: InlineKeyboardMarkup
+        | ReplyKeyboardMarkup
+        | ReplyKeyboardRemove
+        | ForceReply
+        | None = None,
+        protect_content: bool | None = None,
+        parse_mode: str | None = None,
+        message_thread_id: int | None = None,
+        has_spoiler: bool | None = None,
+        disable_notification: bool | None = None,
+        caption_entities: list[MessageEntity] | None = None,
+        caption: str | None = None,
+        allow_sending_without_reply: bool | None = None,
         **kwargs
     ) -> Message:
         """
-        Use this method to send photos. On success, the sent Message is returned.
+        Use this method to send photos. On success, the sent Message is
+        returned.
         """
-        response = await self.api.request("sendPhoto", self.get_params(locals()))
-        return Message(**response)
+        response = await self.api.request("sendPhoto", get_params(locals()))
+        return json.decode(response, type=Message)
 
     async def send_audio(
         self,
-        chat_id: Union[int, str],
-        audio: Union[InputFile, str],
-        title: Optional[str] = None,
-        thumbnail: Optional[Union[InputFile, str]] = None,
-        reply_to_message_id: Optional[int] = None,
-        reply_markup: Optional[
-            Union[
-                InlineKeyboardMarkup,
-                ReplyKeyboardMarkup,
-                ReplyKeyboardRemove,
-                ForceReply,
-            ]
-        ] = None,
-        protect_content: Optional[bool] = None,
-        performer: Optional[str] = None,
-        parse_mode: Optional[str] = None,
-        message_thread_id: Optional[int] = None,
-        duration: Optional[int] = None,
-        disable_notification: Optional[bool] = None,
-        caption_entities: Optional[List[MessageEntity]] = None,
-        caption: Optional[str] = None,
-        allow_sending_without_reply: Optional[bool] = None,
+        chat_id: int | str,
+        audio: InputFile | str,
+        title: str | None = None,
+        thumbnail: InputFile | str | None = None,
+        reply_to_message_id: int | None = None,
+        reply_markup: InlineKeyboardMarkup
+        | ReplyKeyboardMarkup
+        | ReplyKeyboardRemove
+        | ForceReply
+        | None = None,
+        protect_content: bool | None = None,
+        performer: str | None = None,
+        parse_mode: str | None = None,
+        message_thread_id: int | None = None,
+        duration: int | None = None,
+        disable_notification: bool | None = None,
+        caption_entities: list[MessageEntity] | None = None,
+        caption: str | None = None,
+        allow_sending_without_reply: bool | None = None,
         **kwargs
     ) -> Message:
         """
-        Use this method to send audio files, if you want Telegram clients to display them in
-        the music player. Your audio must be in the .MP3 or .M4A format. On success, the
-        sent Message is returned. Bots can currently send audio files of up to 50 MB in
-        size, this limit may be changed in the future. For sending voice messages, use the
-        sendVoice method instead.
+        Use this method to send audio files, if you want Telegram clients to
+        display them in the music player. Your audio must be in the .MP3 or
+        .M4A format. On success, the sent Message is returned. Bots can
+        currently send audio files of up to 50 MB in size, this limit may be
+        changed in the future. For sending voice messages, use the sendVoice
+        method instead.
         """
-        response = await self.api.request("sendAudio", self.get_params(locals()))
-        return Message(**response)
+        response = await self.api.request("sendAudio", get_params(locals()))
+        return json.decode(response, type=Message)
 
     async def send_document(
         self,
-        document: Union[InputFile, str],
-        chat_id: Union[int, str],
-        thumbnail: Optional[Union[InputFile, str]] = None,
-        reply_to_message_id: Optional[int] = None,
-        reply_markup: Optional[
-            Union[
-                InlineKeyboardMarkup,
-                ReplyKeyboardMarkup,
-                ReplyKeyboardRemove,
-                ForceReply,
-            ]
-        ] = None,
-        protect_content: Optional[bool] = None,
-        parse_mode: Optional[str] = None,
-        message_thread_id: Optional[int] = None,
-        disable_notification: Optional[bool] = None,
-        disable_content_type_detection: Optional[bool] = None,
-        caption_entities: Optional[List[MessageEntity]] = None,
-        caption: Optional[str] = None,
-        allow_sending_without_reply: Optional[bool] = None,
+        document: InputFile | str,
+        chat_id: int | str,
+        thumbnail: InputFile | str | None = None,
+        reply_to_message_id: int | None = None,
+        reply_markup: InlineKeyboardMarkup
+        | ReplyKeyboardMarkup
+        | ReplyKeyboardRemove
+        | ForceReply
+        | None = None,
+        protect_content: bool | None = None,
+        parse_mode: str | None = None,
+        message_thread_id: int | None = None,
+        disable_notification: bool | None = None,
+        disable_content_type_detection: bool | None = None,
+        caption_entities: list[MessageEntity] | None = None,
+        caption: str | None = None,
+        allow_sending_without_reply: bool | None = None,
         **kwargs
     ) -> Message:
         """
-        Use this method to send general files. On success, the sent Message is returned.
-        Bots can currently send files of any type of up to 50 MB in size, this limit may be
-        changed in the future.
+        Use this method to send general files. On success, the sent Message is
+        returned. Bots can currently send files of any type of up to 50 MB in
+        size, this limit may be changed in the future.
         """
-        response = await self.api.request("sendDocument", self.get_params(locals()))
-        return Message(**response)
+        response = await self.api.request("sendDocument", get_params(locals()))
+        return json.decode(response, type=Message)
 
     async def send_video(
         self,
-        video: Union[InputFile, str],
-        chat_id: Union[int, str],
-        width: Optional[int] = None,
-        thumbnail: Optional[Union[InputFile, str]] = None,
-        supports_streaming: Optional[bool] = None,
-        reply_to_message_id: Optional[int] = None,
-        reply_markup: Optional[
-            Union[
-                InlineKeyboardMarkup,
-                ReplyKeyboardMarkup,
-                ReplyKeyboardRemove,
-                ForceReply,
-            ]
-        ] = None,
-        protect_content: Optional[bool] = None,
-        parse_mode: Optional[str] = None,
-        message_thread_id: Optional[int] = None,
-        height: Optional[int] = None,
-        has_spoiler: Optional[bool] = None,
-        duration: Optional[int] = None,
-        disable_notification: Optional[bool] = None,
-        caption_entities: Optional[List[MessageEntity]] = None,
-        caption: Optional[str] = None,
-        allow_sending_without_reply: Optional[bool] = None,
+        video: InputFile | str,
+        chat_id: int | str,
+        width: int | None = None,
+        thumbnail: InputFile | str | None = None,
+        supports_streaming: bool | None = None,
+        reply_to_message_id: int | None = None,
+        reply_markup: InlineKeyboardMarkup
+        | ReplyKeyboardMarkup
+        | ReplyKeyboardRemove
+        | ForceReply
+        | None = None,
+        protect_content: bool | None = None,
+        parse_mode: str | None = None,
+        message_thread_id: int | None = None,
+        height: int | None = None,
+        has_spoiler: bool | None = None,
+        duration: int | None = None,
+        disable_notification: bool | None = None,
+        caption_entities: list[MessageEntity] | None = None,
+        caption: str | None = None,
+        allow_sending_without_reply: bool | None = None,
         **kwargs
     ) -> Message:
         """
-        Use this method to send video files, Telegram clients support MPEG4 videos (other
-        formats may be sent as Document). On success, the sent Message is returned. Bots can
-        currently send video files of up to 50 MB in size, this limit may be changed in the
-        future.
+        Use this method to send video files, Telegram clients support MPEG4
+        videos (other formats may be sent as Document). On success, the sent
+        Message is returned. Bots can currently send video files of up to 50
+        MB in size, this limit may be changed in the future.
         """
-        response = await self.api.request("sendVideo", self.get_params(locals()))
-        return Message(**response)
+        response = await self.api.request("sendVideo", get_params(locals()))
+        return json.decode(response, type=Message)
 
     async def send_animation(
         self,
-        chat_id: Union[int, str],
-        animation: Union[InputFile, str],
-        width: Optional[int] = None,
-        thumbnail: Optional[Union[InputFile, str]] = None,
-        reply_to_message_id: Optional[int] = None,
-        reply_markup: Optional[
-            Union[
-                InlineKeyboardMarkup,
-                ReplyKeyboardMarkup,
-                ReplyKeyboardRemove,
-                ForceReply,
-            ]
-        ] = None,
-        protect_content: Optional[bool] = None,
-        parse_mode: Optional[str] = None,
-        message_thread_id: Optional[int] = None,
-        height: Optional[int] = None,
-        has_spoiler: Optional[bool] = None,
-        duration: Optional[int] = None,
-        disable_notification: Optional[bool] = None,
-        caption_entities: Optional[List[MessageEntity]] = None,
-        caption: Optional[str] = None,
-        allow_sending_without_reply: Optional[bool] = None,
+        chat_id: int | str,
+        animation: InputFile | str,
+        width: int | None = None,
+        thumbnail: InputFile | str | None = None,
+        reply_to_message_id: int | None = None,
+        reply_markup: InlineKeyboardMarkup
+        | ReplyKeyboardMarkup
+        | ReplyKeyboardRemove
+        | ForceReply
+        | None = None,
+        protect_content: bool | None = None,
+        parse_mode: str | None = None,
+        message_thread_id: int | None = None,
+        height: int | None = None,
+        has_spoiler: bool | None = None,
+        duration: int | None = None,
+        disable_notification: bool | None = None,
+        caption_entities: list[MessageEntity] | None = None,
+        caption: str | None = None,
+        allow_sending_without_reply: bool | None = None,
         **kwargs
     ) -> Message:
         """
-        Use this method to send animation files (GIF or H.264/MPEG-4 AVC video without
-        sound). On success, the sent Message is returned. Bots can currently send animation
-        files of up to 50 MB in size, this limit may be changed in the future.
+        Use this method to send animation files (GIF or H.264/MPEG-4 AVC video
+        without sound). On success, the sent Message is returned. Bots can
+        currently send animation files of up to 50 MB in size, this limit may
+        be changed in the future.
         """
-        response = await self.api.request("sendAnimation", self.get_params(locals()))
-        return Message(**response)
+        response = await self.api.request("sendAnimation", get_params(locals()))
+        return json.decode(response, type=Message)
 
     async def send_voice(
         self,
-        voice: Union[InputFile, str],
-        chat_id: Union[int, str],
-        reply_to_message_id: Optional[int] = None,
-        reply_markup: Optional[
-            Union[
-                InlineKeyboardMarkup,
-                ReplyKeyboardMarkup,
-                ReplyKeyboardRemove,
-                ForceReply,
-            ]
-        ] = None,
-        protect_content: Optional[bool] = None,
-        parse_mode: Optional[str] = None,
-        message_thread_id: Optional[int] = None,
-        duration: Optional[int] = None,
-        disable_notification: Optional[bool] = None,
-        caption_entities: Optional[List[MessageEntity]] = None,
-        caption: Optional[str] = None,
-        allow_sending_without_reply: Optional[bool] = None,
+        voice: InputFile | str,
+        chat_id: int | str,
+        reply_to_message_id: int | None = None,
+        reply_markup: InlineKeyboardMarkup
+        | ReplyKeyboardMarkup
+        | ReplyKeyboardRemove
+        | ForceReply
+        | None = None,
+        protect_content: bool | None = None,
+        parse_mode: str | None = None,
+        message_thread_id: int | None = None,
+        duration: int | None = None,
+        disable_notification: bool | None = None,
+        caption_entities: list[MessageEntity] | None = None,
+        caption: str | None = None,
+        allow_sending_without_reply: bool | None = None,
         **kwargs
     ) -> Message:
         """
-        Use this method to send audio files, if you want Telegram clients to display the
-        file as a playable voice message. For this to work, your audio must be in an .OGG
-        file encoded with OPUS (other formats may be sent as Audio or Document). On success,
-        the sent Message is returned. Bots can currently send voice messages of up to 50 MB
-        in size, this limit may be changed in the future.
+        Use this method to send audio files, if you want Telegram clients to
+        display the file as a playable voice message. For this to work, your
+        audio must be in an .OGG file encoded with OPUS (other formats may be
+        sent as Audio or Document). On success, the sent Message is returned.
+        Bots can currently send voice messages of up to 50 MB in size, this
+        limit may be changed in the future.
         """
-        response = await self.api.request("sendVoice", self.get_params(locals()))
-        return Message(**response)
+        response = await self.api.request("sendVoice", get_params(locals()))
+        return json.decode(response, type=Message)
 
     async def send_video_note(
         self,
-        video_note: Union[InputFile, str],
-        chat_id: Union[int, str],
-        thumbnail: Optional[Union[InputFile, str]] = None,
-        reply_to_message_id: Optional[int] = None,
-        reply_markup: Optional[
-            Union[
-                InlineKeyboardMarkup,
-                ReplyKeyboardMarkup,
-                ReplyKeyboardRemove,
-                ForceReply,
-            ]
-        ] = None,
-        protect_content: Optional[bool] = None,
-        message_thread_id: Optional[int] = None,
-        length: Optional[int] = None,
-        duration: Optional[int] = None,
-        disable_notification: Optional[bool] = None,
-        allow_sending_without_reply: Optional[bool] = None,
+        video_note: InputFile | str,
+        chat_id: int | str,
+        thumbnail: InputFile | str | None = None,
+        reply_to_message_id: int | None = None,
+        reply_markup: InlineKeyboardMarkup
+        | ReplyKeyboardMarkup
+        | ReplyKeyboardRemove
+        | ForceReply
+        | None = None,
+        protect_content: bool | None = None,
+        message_thread_id: int | None = None,
+        length: int | None = None,
+        duration: int | None = None,
+        disable_notification: bool | None = None,
+        allow_sending_without_reply: bool | None = None,
         **kwargs
     ) -> Message:
         """
-        As of v.4.0, Telegram clients support rounded square MPEG4 videos of up to 1 minute
-        long. Use this method to send video messages. On success, the sent Message is
-        returned.
+        As of v.4.0, Telegram clients support rounded square MPEG4 videos of
+        up to 1 minute long. Use this method to send video messages. On
+        success, the sent Message is returned.
         """
-        response = await self.api.request("sendVideoNote", self.get_params(locals()))
-        return Message(**response)
+        response = await self.api.request("sendVideoNote", get_params(locals()))
+        return json.decode(response, type=Message)
 
     async def send_media_group(
         self,
-        media: List[
-            Union[InputMediaAudio, InputMediaDocument, InputMediaPhoto, InputMediaVideo]
+        media: list[
+            InputMediaAudio | InputMediaDocument | InputMediaPhoto | InputMediaVideo
         ],
-        chat_id: Union[int, str],
-        reply_to_message_id: Optional[int] = None,
-        protect_content: Optional[bool] = None,
-        message_thread_id: Optional[int] = None,
-        disable_notification: Optional[bool] = None,
-        allow_sending_without_reply: Optional[bool] = None,
-        **kwargs
-    ) -> List[Message]:
-        """
-        Use this method to send a group of photos, videos, documents or audios as an album.
-        Documents and audio files can be only grouped in an album with messages of the same
-        type. On success, an array of Messages that were sent is returned.
+        chat_id: int | str,
+        reply_to_message_id: int | None = None,
+        protect_content: bool | None = None,
+        message_thread_id: int | None = None,
+        disable_notification: bool | None = None,
+        allow_sending_without_reply: bool | None = None,
+        **kwargs
+    ) -> list[Message]:
+        """
+        Use this method to send a group of photos, videos, documents or audios
+        as an album. Documents and audio files can be only grouped in an album
+        with messages of the same type. On success, an array of Messages that
+        were sent is returned.
         """
-        response = await self.api.request("sendMediaGroup", self.get_params(locals()))
-        return parse_obj_as(List[Message], response)
+        response = await self.api.request("sendMediaGroup", get_params(locals()))
+        return json.decode(response, type=list[Message])
 
     async def send_location(
         self,
         longitude: float,
         latitude: float,
-        chat_id: Union[int, str],
-        reply_to_message_id: Optional[int] = None,
-        reply_markup: Optional[
-            Union[
-                InlineKeyboardMarkup,
-                ReplyKeyboardMarkup,
-                ReplyKeyboardRemove,
-                ForceReply,
-            ]
-        ] = None,
-        proximity_alert_radius: Optional[int] = None,
-        protect_content: Optional[bool] = None,
-        message_thread_id: Optional[int] = None,
-        live_period: Optional[int] = None,
-        horizontal_accuracy: Optional[float] = None,
-        heading: Optional[int] = None,
-        disable_notification: Optional[bool] = None,
-        allow_sending_without_reply: Optional[bool] = None,
+        chat_id: int | str,
+        reply_to_message_id: int | None = None,
+        reply_markup: InlineKeyboardMarkup
+        | ReplyKeyboardMarkup
+        | ReplyKeyboardRemove
+        | ForceReply
+        | None = None,
+        proximity_alert_radius: int | None = None,
+        protect_content: bool | None = None,
+        message_thread_id: int | None = None,
+        live_period: int | None = None,
+        horizontal_accuracy: float | None = None,
+        heading: int | None = None,
+        disable_notification: bool | None = None,
+        allow_sending_without_reply: bool | None = None,
         **kwargs
     ) -> Message:
         """
-        Use this method to send point on the map. On success, the sent Message is returned.
+        Use this method to send point on the map. On success, the sent Message
+        is returned.
         """
-        response = await self.api.request("sendLocation", self.get_params(locals()))
-        return Message(**response)
+        response = await self.api.request("sendLocation", get_params(locals()))
+        return json.decode(response, type=Message)
 
     async def send_venue(
         self,
         title: str,
         longitude: float,
         latitude: float,
-        chat_id: Union[int, str],
+        chat_id: int | str,
         address: str,
-        reply_to_message_id: Optional[int] = None,
-        reply_markup: Optional[
-            Union[
-                InlineKeyboardMarkup,
-                ReplyKeyboardMarkup,
-                ReplyKeyboardRemove,
-                ForceReply,
-            ]
-        ] = None,
-        protect_content: Optional[bool] = None,
-        message_thread_id: Optional[int] = None,
-        google_place_type: Optional[str] = None,
-        google_place_id: Optional[str] = None,
-        foursquare_type: Optional[str] = None,
-        foursquare_id: Optional[str] = None,
-        disable_notification: Optional[bool] = None,
-        allow_sending_without_reply: Optional[bool] = None,
+        reply_to_message_id: int | None = None,
+        reply_markup: InlineKeyboardMarkup
+        | ReplyKeyboardMarkup
+        | ReplyKeyboardRemove
+        | ForceReply
+        | None = None,
+        protect_content: bool | None = None,
+        message_thread_id: int | None = None,
+        google_place_type: str | None = None,
+        google_place_id: str | None = None,
+        foursquare_type: str | None = None,
+        foursquare_id: str | None = None,
+        disable_notification: bool | None = None,
+        allow_sending_without_reply: bool | None = None,
         **kwargs
     ) -> Message:
         """
-        Use this method to send information about a venue. On success, the sent Message is
-        returned.
+        Use this method to send information about a venue. On success, the
+        sent Message is returned.
         """
-        response = await self.api.request("sendVenue", self.get_params(locals()))
-        return Message(**response)
+        response = await self.api.request("sendVenue", get_params(locals()))
+        return json.decode(response, type=Message)
 
     async def send_contact(
         self,
         phone_number: str,
         first_name: str,
-        chat_id: Union[int, str],
-        vcard: Optional[str] = None,
-        reply_to_message_id: Optional[int] = None,
-        reply_markup: Optional[
-            Union[
-                InlineKeyboardMarkup,
-                ReplyKeyboardMarkup,
-                ReplyKeyboardRemove,
-                ForceReply,
-            ]
-        ] = None,
-        protect_content: Optional[bool] = None,
-        message_thread_id: Optional[int] = None,
-        last_name: Optional[str] = None,
-        disable_notification: Optional[bool] = None,
-        allow_sending_without_reply: Optional[bool] = None,
+        chat_id: int | str,
+        vcard: str | None = None,
+        reply_to_message_id: int | None = None,
+        reply_markup: InlineKeyboardMarkup
+        | ReplyKeyboardMarkup
+        | ReplyKeyboardRemove
+        | ForceReply
+        | None = None,
+        protect_content: bool | None = None,
+        message_thread_id: int | None = None,
+        last_name: str | None = None,
+        disable_notification: bool | None = None,
+        allow_sending_without_reply: bool | None = None,
         **kwargs
     ) -> Message:
         """
-        Use this method to send phone contacts. On success, the sent Message is returned.
+        Use this method to send phone contacts. On success, the sent Message
+        is returned.
         """
-        response = await self.api.request("sendContact", self.get_params(locals()))
-        return Message(**response)
+        response = await self.api.request("sendContact", get_params(locals()))
+        return json.decode(response, type=Message)
 
     async def send_poll(
         self,
         question: str,
-        options: List[str],
-        chat_id: Union[int, str],
-        type: Optional[str] = None,
-        reply_to_message_id: Optional[int] = None,
-        reply_markup: Optional[
-            Union[
-                InlineKeyboardMarkup,
-                ReplyKeyboardMarkup,
-                ReplyKeyboardRemove,
-                ForceReply,
-            ]
-        ] = None,
-        protect_content: Optional[bool] = None,
-        open_period: Optional[int] = None,
-        message_thread_id: Optional[int] = None,
-        is_closed: Optional[bool] = None,
-        is_anonymous: Optional[bool] = None,
-        explanation_parse_mode: Optional[str] = None,
-        explanation_entities: Optional[List[MessageEntity]] = None,
-        explanation: Optional[str] = None,
-        disable_notification: Optional[bool] = None,
-        correct_option_id: Optional[int] = None,
-        close_date: Optional[int] = None,
-        allows_multiple_answers: Optional[bool] = None,
-        allow_sending_without_reply: Optional[bool] = None,
+        options: list[str],
+        chat_id: int | str,
+        type: str | None = None,
+        reply_to_message_id: int | None = None,
+        reply_markup: InlineKeyboardMarkup
+        | ReplyKeyboardMarkup
+        | ReplyKeyboardRemove
+        | ForceReply
+        | None = None,
+        protect_content: bool | None = None,
+        open_period: int | None = None,
+        message_thread_id: int | None = None,
+        is_closed: bool | None = None,
+        is_anonymous: bool | None = None,
+        explanation_parse_mode: str | None = None,
+        explanation_entities: list[MessageEntity] | None = None,
+        explanation: str | None = None,
+        disable_notification: bool | None = None,
+        correct_option_id: int | None = None,
+        close_date: int | None = None,
+        allows_multiple_answers: bool | None = None,
+        allow_sending_without_reply: bool | None = None,
         **kwargs
     ) -> Message:
         """
-        Use this method to send a native poll. On success, the sent Message is returned.
+        Use this method to send a native poll. On success, the sent Message is
+        returned.
         """
-        response = await self.api.request("sendPoll", self.get_params(locals()))
-        return Message(**response)
+        response = await self.api.request("sendPoll", get_params(locals()))
+        return json.decode(response, type=Message)
 
     async def send_dice(
         self,
-        chat_id: Union[int, str],
-        reply_to_message_id: Optional[int] = None,
-        reply_markup: Optional[
-            Union[
-                InlineKeyboardMarkup,
-                ReplyKeyboardMarkup,
-                ReplyKeyboardRemove,
-                ForceReply,
-            ]
-        ] = None,
-        protect_content: Optional[bool] = None,
-        message_thread_id: Optional[int] = None,
-        emoji: Optional[str] = None,
-        disable_notification: Optional[bool] = None,
-        allow_sending_without_reply: Optional[bool] = None,
+        chat_id: int | str,
+        reply_to_message_id: int | None = None,
+        reply_markup: InlineKeyboardMarkup
+        | ReplyKeyboardMarkup
+        | ReplyKeyboardRemove
+        | ForceReply
+        | None = None,
+        protect_content: bool | None = None,
+        message_thread_id: int | None = None,
+        emoji: str | None = None,
+        disable_notification: bool | None = None,
+        allow_sending_without_reply: bool | None = None,
         **kwargs
     ) -> Message:
         """
-        Use this method to send an animated emoji that will display a random value. On
-        success, the sent Message is returned.
+        Use this method to send an animated emoji that will display a random
+        value. On success, the sent Message is returned.
         """
-        response = await self.api.request("sendDice", self.get_params(locals()))
-        return Message(**response)
+        response = await self.api.request("sendDice", get_params(locals()))
+        return json.decode(response, type=Message)
 
     async def send_chat_action(
         self,
-        chat_id: Union[int, str],
+        chat_id: int | str,
         action: str,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: int | None = None,
         **kwargs
     ) -> bool:
         """
-        Use this method when you need to tell the user that something is happening on the
-        bot's side. The status is set for 5 seconds or less (when a message arrives from
-        your bot, Telegram clients clear its typing status). Returns True on success.
-        Example: The ImageBot needs some time to process a request and upload the image.
-        Instead of sending a text message along the lines of “Retrieving image, please
-        wait…”, the bot may use sendChatAction with action = upload_photo. The user will see
-        a “sending photo” status for the bot. We only recommend using this method when a
-        response from the bot will take a noticeable amount of time to arrive.
+        Use this method when you need to tell the user that something is
+        happening on the bot's side. The status is set for 5 seconds or less
+        (when a message arrives from your bot, Telegram clients clear its
+        typing status). Returns True on success. Example: The ImageBot needs
+        some time to process a request and upload the image. Instead of
+        sending a text message along the lines of “Retrieving image, please
+        wait…”, the bot may use sendChatAction with action = upload_photo. The
+        user will see a “sending photo” status for the bot. We only recommend
+        using this method when a response from the bot will take a noticeable
+        amount of time to arrive.
         """
-        response = await self.api.request("sendChatAction", self.get_params(locals()))
-        return response
+        response = await self.api.request("sendChatAction", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def get_user_profile_photos(
         self,
         user_id: int,
-        offset: Optional[int] = None,
-        limit: Optional[int] = None,
+        offset: int | None = None,
+        limit: int | None = None,
         **kwargs
     ) -> UserProfilePhotos:
         """
-        Use this method to get a list of profile pictures for a user. Returns a
-        UserProfilePhotos object.
+        Use this method to get a list of profile pictures for a user. Returns
+        a UserProfilePhotos object.
         """
-        response = await self.api.request(
-            "getUserProfilePhotos", self.get_params(locals())
-        )
-        return UserProfilePhotos(**response)
+        response = await self.api.request("getUserProfilePhotos", get_params(locals()))
+        return json.decode(response, type=UserProfilePhotos)
 
     async def get_file(self, file_id: str, **kwargs) -> File:
         """
-        Use this method to get basic information about a file and prepare it for
-        downloading. For the moment, bots can download files of up to 20MB in size. On
-        success, a File object is returned. The file can then be downloaded via the link
-        https://api.telegram.org/file/bot<token>/<file_path>, where <file_path> is taken
-        from the response. It is guaranteed that the link will be valid for at least 1 hour.
-        When the link expires, a new one can be requested by calling getFile again.
+        Use this method to get basic information about a file and prepare it
+        for downloading. For the moment, bots can download files of up to 20MB
+        in size. On success, a File object is returned. The file can then be
+        downloaded via the link
+        https://api.telegram.org/file/bot<token>/<file_path>, where
+        <file_path> is taken from the response. It is guaranteed that the link
+        will be valid for at least 1 hour. When the link expires, a new one
+        can be requested by calling getFile again.
         """
-        response = await self.api.request("getFile", self.get_params(locals()))
-        return File(**response)
+        response = await self.api.request("getFile", get_params(locals()))
+        return json.decode(response, type=File)
 
     async def ban_chat_member(
         self,
         user_id: int,
-        chat_id: Union[int, str],
-        until_date: Optional[int] = None,
-        revoke_messages: Optional[bool] = None,
+        chat_id: int | str,
+        until_date: int | None = None,
+        revoke_messages: bool | None = None,
         **kwargs
     ) -> bool:
         """
-        Use this method to ban a user in a group, a supergroup or a channel. In the case of
-        supergroups and channels, the user will not be able to return to the chat on their
-        own using invite links, etc., unless unbanned first. The bot must be an
-        administrator in the chat for this to work and must have the appropriate
-        administrator rights. Returns True on success.
+        Use this method to ban a user in a group, a supergroup or a channel.
+        In the case of supergroups and channels, the user will not be able to
+        return to the chat on their own using invite links, etc., unless
+        unbanned first. The bot must be an administrator in the chat for this
+        to work and must have the appropriate administrator rights. Returns
+        True on success.
         """
-        response = await self.api.request("banChatMember", self.get_params(locals()))
-        return response
+        response = await self.api.request("banChatMember", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def unban_chat_member(
         self,
         user_id: int,
-        chat_id: Union[int, str],
-        only_if_banned: Optional[bool] = None,
+        chat_id: int | str,
+        only_if_banned: bool | None = None,
         **kwargs
     ) -> bool:
         """
-        Use this method to unban a previously banned user in a supergroup or channel. The
-        user will not return to the group or channel automatically, but will be able to join
-        via link, etc. The bot must be an administrator for this to work. By default, this
-        method guarantees that after the call the user is not a member of the chat, but will
-        be able to join it. So if the user is a member of the chat they will also be removed
-        from the chat. If you don't want this, use the parameter only_if_banned. Returns
-        True on success.
+        Use this method to unban a previously banned user in a supergroup or
+        channel. The user will not return to the group or channel
+        automatically, but will be able to join via link, etc. The bot must be
+        an administrator for this to work. By default, this method guarantees
+        that after the call the user is not a member of the chat, but will be
+        able to join it. So if the user is a member of the chat they will also
+        be removed from the chat. If you don't want this, use the parameter
+        only_if_banned. Returns True on success.
         """
-        response = await self.api.request("unbanChatMember", self.get_params(locals()))
-        return response
+        response = await self.api.request("unbanChatMember", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def restrict_chat_member(
         self,
         user_id: int,
         permissions: ChatPermissions,
-        chat_id: Union[int, str],
-        use_independent_chat_permissions: Optional[bool] = None,
-        until_date: Optional[int] = None,
+        chat_id: int | str,
+        use_independent_chat_permissions: bool | None = None,
+        until_date: int | None = None,
         **kwargs
     ) -> bool:
         """
-        Use this method to restrict a user in a supergroup. The bot must be an administrator
-        in the supergroup for this to work and must have the appropriate administrator
-        rights. Pass True for all permissions to lift restrictions from a user. Returns True
-        on success.
+        Use this method to restrict a user in a supergroup. The bot must be an
+        administrator in the supergroup for this to work and must have the
+        appropriate administrator rights. Pass True for all permissions to
+        lift restrictions from a user. Returns True on success.
         """
-        response = await self.api.request(
-            "restrictChatMember", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("restrictChatMember", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def promote_chat_member(
         self,
         user_id: int,
-        chat_id: Union[int, str],
-        is_anonymous: Optional[bool] = None,
-        can_restrict_members: Optional[bool] = None,
-        can_promote_members: Optional[bool] = None,
-        can_post_messages: Optional[bool] = None,
-        can_pin_messages: Optional[bool] = None,
-        can_manage_video_chats: Optional[bool] = None,
-        can_manage_topics: Optional[bool] = None,
-        can_manage_chat: Optional[bool] = None,
-        can_invite_users: Optional[bool] = None,
-        can_edit_messages: Optional[bool] = None,
-        can_delete_messages: Optional[bool] = None,
-        can_change_info: Optional[bool] = None,
+        chat_id: int | str,
+        is_anonymous: bool | None = None,
+        can_restrict_members: bool | None = None,
+        can_promote_members: bool | None = None,
+        can_post_messages: bool | None = None,
+        can_pin_messages: bool | None = None,
+        can_manage_video_chats: bool | None = None,
+        can_manage_topics: bool | None = None,
+        can_manage_chat: bool | None = None,
+        can_invite_users: bool | None = None,
+        can_edit_messages: bool | None = None,
+        can_delete_messages: bool | None = None,
+        can_change_info: bool | None = None,
         **kwargs
     ) -> bool:
         """
-        Use this method to promote or demote a user in a supergroup or a channel. The bot
-        must be an administrator in the chat for this to work and must have the appropriate
-        administrator rights. Pass False for all boolean parameters to demote a user.
-        Returns True on success.
+        Use this method to promote or demote a user in a supergroup or a
+        channel. The bot must be an administrator in the chat for this to work
+        and must have the appropriate administrator rights. Pass False for all
+        boolean parameters to demote a user. Returns True on success.
         """
-        response = await self.api.request(
-            "promoteChatMember", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("promoteChatMember", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def set_chat_administrator_custom_title(
-        self, user_id: int, custom_title: str, chat_id: Union[int, str], **kwargs
+        self, user_id: int, custom_title: str, chat_id: int | str, **kwargs
     ) -> bool:
         """
-        Use this method to set a custom title for an administrator in a supergroup promoted
-        by the bot. Returns True on success.
+        Use this method to set a custom title for an administrator in a
+        supergroup promoted by the bot. Returns True on success.
         """
         response = await self.api.request(
-            "setChatAdministratorCustomTitle", self.get_params(locals())
+            "setChatAdministratorCustomTitle", get_params(locals())
         )
-        return response
+        return json.decode(response, type=bool)
 
     async def ban_chat_sender_chat(
-        self, sender_chat_id: int, chat_id: Union[int, str], **kwargs
+        self, sender_chat_id: int, chat_id: int | str, **kwargs
     ) -> bool:
         """
-        Use this method to ban a channel chat in a supergroup or a channel. Until the chat
-        is unbanned, the owner of the banned chat won't be able to send messages on behalf
-        of any of their channels. The bot must be an administrator in the supergroup or
-        channel for this to work and must have the appropriate administrator rights. Returns
-        True on success.
+        Use this method to ban a channel chat in a supergroup or a channel.
+        Until the chat is unbanned, the owner of the banned chat won't be able
+        to send messages on behalf of any of their channels. The bot must be
+        an administrator in the supergroup or channel for this to work and
+        must have the appropriate administrator rights. Returns True on
+        success.
         """
-        response = await self.api.request(
-            "banChatSenderChat", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("banChatSenderChat", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def unban_chat_sender_chat(
-        self, sender_chat_id: int, chat_id: Union[int, str], **kwargs
+        self, sender_chat_id: int, chat_id: int | str, **kwargs
     ) -> bool:
         """
-        Use this method to unban a previously banned channel chat in a supergroup or
-        channel. The bot must be an administrator for this to work and must have the
-        appropriate administrator rights. Returns True on success.
+        Use this method to unban a previously banned channel chat in a
+        supergroup or channel. The bot must be an administrator for this to
+        work and must have the appropriate administrator rights. Returns True
+        on success.
         """
-        response = await self.api.request(
-            "unbanChatSenderChat", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("unbanChatSenderChat", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def set_chat_permissions(
         self,
         permissions: ChatPermissions,
-        chat_id: Union[int, str],
-        use_independent_chat_permissions: Optional[bool] = None,
+        chat_id: int | str,
+        use_independent_chat_permissions: bool | None = None,
         **kwargs
     ) -> bool:
         """
-        Use this method to set default chat permissions for all members. The bot must be an
-        administrator in the group or a supergroup for this to work and must have the
-        can_restrict_members administrator rights. Returns True on success.
+        Use this method to set default chat permissions for all members. The
+        bot must be an administrator in the group or a supergroup for this to
+        work and must have the can_restrict_members administrator rights.
+        Returns True on success.
         """
-        response = await self.api.request(
-            "setChatPermissions", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("setChatPermissions", get_params(locals()))
+        return json.decode(response, type=bool)
 
-    async def export_chat_invite_link(self, chat_id: Union[int, str], **kwargs) -> str:
+    async def export_chat_invite_link(self, chat_id: int | str, **kwargs) -> str:
         """
-        Use this method to generate a new primary invite link for a chat; any previously
-        generated primary link is revoked. The bot must be an administrator in the chat for
-        this to work and must have the appropriate administrator rights. Returns the new
-        invite link as String on success.
+        Use this method to generate a new primary invite link for a chat; any
+        previously generated primary link is revoked. The bot must be an
+        administrator in the chat for this to work and must have the
+        appropriate administrator rights. Returns the new invite link as
+        String on success.
         """
-        response = await self.api.request(
-            "exportChatInviteLink", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("exportChatInviteLink", get_params(locals()))
+        return json.decode(response, type=str)
 
     async def create_chat_invite_link(
         self,
-        chat_id: Union[int, str],
-        name: Optional[str] = None,
-        member_limit: Optional[int] = None,
-        expire_date: Optional[int] = None,
-        creates_join_request: Optional[bool] = None,
+        chat_id: int | str,
+        name: str | None = None,
+        member_limit: int | None = None,
+        expire_date: int | None = None,
+        creates_join_request: bool | None = None,
         **kwargs
     ) -> ChatInviteLink:
         """
-        Use this method to create an additional invite link for a chat. The bot must be an
-        administrator in the chat for this to work and must have the appropriate
-        administrator rights. The link can be revoked using the method revokeChatInviteLink.
-        Returns the new invite link as ChatInviteLink object.
+        Use this method to create an additional invite link for a chat. The
+        bot must be an administrator in the chat for this to work and must
+        have the appropriate administrator rights. The link can be revoked
+        using the method revokeChatInviteLink. Returns the new invite link as
+        ChatInviteLink object.
         """
-        response = await self.api.request(
-            "createChatInviteLink", self.get_params(locals())
-        )
-        return ChatInviteLink(**response)
+        response = await self.api.request("createChatInviteLink", get_params(locals()))
+        return json.decode(response, type=ChatInviteLink)
 
     async def edit_chat_invite_link(
         self,
         invite_link: str,
-        chat_id: Union[int, str],
-        name: Optional[str] = None,
-        member_limit: Optional[int] = None,
-        expire_date: Optional[int] = None,
-        creates_join_request: Optional[bool] = None,
+        chat_id: int | str,
+        name: str | None = None,
+        member_limit: int | None = None,
+        expire_date: int | None = None,
+        creates_join_request: bool | None = None,
         **kwargs
     ) -> ChatInviteLink:
         """
-        Use this method to edit a non-primary invite link created by the bot. The bot must
-        be an administrator in the chat for this to work and must have the appropriate
-        administrator rights. Returns the edited invite link as a ChatInviteLink object.
+        Use this method to edit a non-primary invite link created by the bot.
+        The bot must be an administrator in the chat for this to work and must
+        have the appropriate administrator rights. Returns the edited invite
+        link as a ChatInviteLink object.
         """
-        response = await self.api.request(
-            "editChatInviteLink", self.get_params(locals())
-        )
-        return ChatInviteLink(**response)
+        response = await self.api.request("editChatInviteLink", get_params(locals()))
+        return json.decode(response, type=ChatInviteLink)
 
     async def revoke_chat_invite_link(
-        self, invite_link: str, chat_id: Union[int, str], **kwargs
+        self, invite_link: str, chat_id: int | str, **kwargs
     ) -> ChatInviteLink:
         """
-        Use this method to revoke an invite link created by the bot. If the primary link is
-        revoked, a new link is automatically generated. The bot must be an administrator in
-        the chat for this to work and must have the appropriate administrator rights.
-        Returns the revoked invite link as ChatInviteLink object.
+        Use this method to revoke an invite link created by the bot. If the
+        primary link is revoked, a new link is automatically generated. The
+        bot must be an administrator in the chat for this to work and must
+        have the appropriate administrator rights. Returns the revoked invite
+        link as ChatInviteLink object.
         """
-        response = await self.api.request(
-            "revokeChatInviteLink", self.get_params(locals())
-        )
-        return ChatInviteLink(**response)
+        response = await self.api.request("revokeChatInviteLink", get_params(locals()))
+        return json.decode(response, type=ChatInviteLink)
 
     async def approve_chat_join_request(
-        self, user_id: int, chat_id: Union[int, str], **kwargs
+        self, user_id: int, chat_id: int | str, **kwargs
     ) -> bool:
         """
-        Use this method to approve a chat join request. The bot must be an administrator in
-        the chat for this to work and must have the can_invite_users administrator right.
-        Returns True on success.
+        Use this method to approve a chat join request. The bot must be an
+        administrator in the chat for this to work and must have the
+        can_invite_users administrator right. Returns True on success.
         """
         response = await self.api.request(
-            "approveChatJoinRequest", self.get_params(locals())
+            "approveChatJoinRequest", get_params(locals())
         )
-        return response
+        return json.decode(response, type=bool)
 
     async def decline_chat_join_request(
-        self, user_id: int, chat_id: Union[int, str], **kwargs
+        self, user_id: int, chat_id: int | str, **kwargs
     ) -> bool:
         """
-        Use this method to decline a chat join request. The bot must be an administrator in
-        the chat for this to work and must have the can_invite_users administrator right.
-        Returns True on success.
+        Use this method to decline a chat join request. The bot must be an
+        administrator in the chat for this to work and must have the
+        can_invite_users administrator right. Returns True on success.
         """
         response = await self.api.request(
-            "declineChatJoinRequest", self.get_params(locals())
+            "declineChatJoinRequest", get_params(locals())
         )
-        return response
+        return json.decode(response, type=bool)
 
     async def set_chat_photo(
-        self, photo: InputFile, chat_id: Union[int, str], **kwargs
+        self, photo: InputFile, chat_id: int | str, **kwargs
     ) -> bool:
         """
-        Use this method to set a new profile photo for the chat. Photos can't be changed for
-        private chats. The bot must be an administrator in the chat for this to work and
-        must have the appropriate administrator rights. Returns True on success.
+        Use this method to set a new profile photo for the chat. Photos can't
+        be changed for private chats. The bot must be an administrator in the
+        chat for this to work and must have the appropriate administrator
+        rights. Returns True on success.
         """
-        response = await self.api.request("setChatPhoto", self.get_params(locals()))
-        return response
+        response = await self.api.request("setChatPhoto", get_params(locals()))
+        return json.decode(response, type=bool)
 
-    async def delete_chat_photo(self, chat_id: Union[int, str], **kwargs) -> bool:
+    async def delete_chat_photo(self, chat_id: int | str, **kwargs) -> bool:
         """
-        Use this method to delete a chat photo. Photos can't be changed for private chats.
-        The bot must be an administrator in the chat for this to work and must have the
-        appropriate administrator rights. Returns True on success.
+        Use this method to delete a chat photo. Photos can't be changed for
+        private chats. The bot must be an administrator in the chat for this
+        to work and must have the appropriate administrator rights. Returns
+        True on success.
         """
-        response = await self.api.request("deleteChatPhoto", self.get_params(locals()))
-        return response
+        response = await self.api.request("deleteChatPhoto", get_params(locals()))
+        return json.decode(response, type=bool)
 
-    async def set_chat_title(
-        self, title: str, chat_id: Union[int, str], **kwargs
-    ) -> bool:
+    async def set_chat_title(self, title: str, chat_id: int | str, **kwargs) -> bool:
         """
-        Use this method to change the title of a chat. Titles can't be changed for private
-        chats. The bot must be an administrator in the chat for this to work and must have
-        the appropriate administrator rights. Returns True on success.
+        Use this method to change the title of a chat. Titles can't be changed
+        for private chats. The bot must be an administrator in the chat for
+        this to work and must have the appropriate administrator rights.
+        Returns True on success.
         """
-        response = await self.api.request("setChatTitle", self.get_params(locals()))
-        return response
+        response = await self.api.request("setChatTitle", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def set_chat_description(
-        self, chat_id: Union[int, str], description: Optional[str] = None, **kwargs
+        self, chat_id: int | str, description: str | None = None, **kwargs
     ) -> bool:
         """
-        Use this method to change the description of a group, a supergroup or a channel. The
-        bot must be an administrator in the chat for this to work and must have the
-        appropriate administrator rights. Returns True on success.
+        Use this method to change the description of a group, a supergroup or
+        a channel. The bot must be an administrator in the chat for this to
+        work and must have the appropriate administrator rights. Returns True
+        on success.
         """
-        response = await self.api.request(
-            "setChatDescription", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("setChatDescription", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def pin_chat_message(
         self,
         message_id: int,
-        chat_id: Union[int, str],
-        disable_notification: Optional[bool] = None,
+        chat_id: int | str,
+        disable_notification: bool | None = None,
         **kwargs
     ) -> bool:
         """
-        Use this method to add a message to the list of pinned messages in a chat. If the
-        chat is not a private chat, the bot must be an administrator in the chat for this to
-        work and must have the 'can_pin_messages' administrator right in a supergroup or
-        'can_edit_messages' administrator right in a channel. Returns True on success.
+        Use this method to add a message to the list of pinned messages in a
+        chat. If the chat is not a private chat, the bot must be an
+        administrator in the chat for this to work and must have the
+        'can_pin_messages' administrator right in a supergroup or
+        'can_edit_messages' administrator right in a channel. Returns True on
+        success.
         """
-        response = await self.api.request("pinChatMessage", self.get_params(locals()))
-        return response
+        response = await self.api.request("pinChatMessage", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def unpin_chat_message(
-        self, chat_id: Union[int, str], message_id: Optional[int] = None, **kwargs
+        self, chat_id: int | str, message_id: int | None = None, **kwargs
     ) -> bool:
         """
-        Use this method to remove a message from the list of pinned messages in a chat. If
-        the chat is not a private chat, the bot must be an administrator in the chat for
-        this to work and must have the 'can_pin_messages' administrator right in a
-        supergroup or 'can_edit_messages' administrator right in a channel. Returns True on
+        Use this method to remove a message from the list of pinned messages
+        in a chat. If the chat is not a private chat, the bot must be an
+        administrator in the chat for this to work and must have the
+        'can_pin_messages' administrator right in a supergroup or
+        'can_edit_messages' administrator right in a channel. Returns True on
         success.
         """
-        response = await self.api.request("unpinChatMessage", self.get_params(locals()))
-        return response
+        response = await self.api.request("unpinChatMessage", get_params(locals()))
+        return json.decode(response, type=bool)
 
-    async def unpin_all_chat_messages(self, chat_id: Union[int, str], **kwargs) -> bool:
+    async def unpin_all_chat_messages(self, chat_id: int | str, **kwargs) -> bool:
         """
-        Use this method to clear the list of pinned messages in a chat. If the chat is not a
-        private chat, the bot must be an administrator in the chat for this to work and must
-        have the 'can_pin_messages' administrator right in a supergroup or
-        'can_edit_messages' administrator right in a channel. Returns True on success.
+        Use this method to clear the list of pinned messages in a chat. If the
+        chat is not a private chat, the bot must be an administrator in the
+        chat for this to work and must have the 'can_pin_messages'
+        administrator right in a supergroup or 'can_edit_messages'
+        administrator right in a channel. Returns True on success.
         """
-        response = await self.api.request(
-            "unpinAllChatMessages", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("unpinAllChatMessages", get_params(locals()))
+        return json.decode(response, type=bool)
 
-    async def leave_chat(self, chat_id: Union[int, str], **kwargs) -> bool:
+    async def leave_chat(self, chat_id: int | str, **kwargs) -> bool:
         """
-        Use this method for your bot to leave a group, supergroup or channel. Returns True
-        on success.
+        Use this method for your bot to leave a group, supergroup or channel.
+        Returns True on success.
         """
-        response = await self.api.request("leaveChat", self.get_params(locals()))
-        return response
+        response = await self.api.request("leaveChat", get_params(locals()))
+        return json.decode(response, type=bool)
 
-    async def get_chat(self, chat_id: Union[int, str], **kwargs) -> Chat:
+    async def get_chat(self, chat_id: int | str, **kwargs) -> Chat:
         """
-        Use this method to get up to date information about the chat (current name of the
-        user for one-on-one conversations, current username of a user, group or channel,
-        etc.). Returns a Chat object on success.
+        Use this method to get up to date information about the chat (current
+        name of the user for one-on-one conversations, current username of a
+        user, group or channel, etc.). Returns a Chat object on success.
         """
-        response = await self.api.request("getChat", self.get_params(locals()))
-        return Chat(**response)
+        response = await self.api.request("getChat", get_params(locals()))
+        return json.decode(response, type=Chat)
 
     async def get_chat_administrators(
-        self, chat_id: Union[int, str], **kwargs
-    ) -> List[ChatMember]:
+        self, chat_id: int | str, **kwargs
+    ) -> list[ChatMember]:
         """
-        Use this method to get a list of administrators in a chat, which aren't bots.
-        Returns an Array of ChatMember objects.
+        Use this method to get a list of administrators in a chat, which
+        aren't bots. Returns an Array of ChatMember objects.
         """
-        response = await self.api.request(
-            "getChatAdministrators", self.get_params(locals())
-        )
-        return parse_obj_as(List[ChatMember], response)
+        response = await self.api.request("getChatAdministrators", get_params(locals()))
+        return json.decode(response, type=list[ChatMember])
 
-    async def get_chat_member_count(self, chat_id: Union[int, str], **kwargs) -> int:
+    async def get_chat_member_count(self, chat_id: int | str, **kwargs) -> int:
         """
-        Use this method to get the number of members in a chat. Returns Int on success.
+        Use this method to get the number of members in a chat. Returns Int on
+        success.
         """
-        response = await self.api.request(
-            "getChatMemberCount", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("getChatMemberCount", get_params(locals()))
+        return json.decode(response, type=int)
 
     async def get_chat_member(
-        self, user_id: int, chat_id: Union[int, str], **kwargs
+        self, user_id: int, chat_id: int | str, **kwargs
     ) -> ChatMember:
         """
-        Use this method to get information about a member of a chat. The method is only
-        guaranteed to work for other users if the bot is an administrator in the chat.
-        Returns a ChatMember object on success.
-        """
-        response = await self.api.request("getChatMember", self.get_params(locals()))
-        return parse_obj_as(ChatMember, response)
+        Use this method to get information about a member of a chat. The
+        method is only guaranteed to work for other users if the bot is an
+        administrator in the chat. Returns a ChatMember object on success.
+        """
+        response = await self.api.request("getChatMember", get_params(locals()))
+        return json.decode(
+            response,
+            type=ChatMemberOwner
+            | ChatMemberAdministrator
+            | ChatMemberMember
+            | ChatMemberRestricted
+            | ChatMemberLeft
+            | ChatMemberBanned,
+        )
 
     async def set_chat_sticker_set(
-        self, sticker_set_name: str, chat_id: Union[int, str], **kwargs
+        self, sticker_set_name: str, chat_id: int | str, **kwargs
     ) -> bool:
         """
-        Use this method to set a new group sticker set for a supergroup. The bot must be an
-        administrator in the chat for this to work and must have the appropriate
-        administrator rights. Use the field can_set_sticker_set optionally returned in
-        getChat requests to check if the bot can use this method. Returns True on success.
+        Use this method to set a new group sticker set for a supergroup. The
+        bot must be an administrator in the chat for this to work and must
+        have the appropriate administrator rights. Use the field
+        can_set_sticker_set optionally returned in getChat requests to check
+        if the bot can use this method. Returns True on success.
         """
-        response = await self.api.request(
-            "setChatStickerSet", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("setChatStickerSet", get_params(locals()))
+        return json.decode(response, type=bool)
 
-    async def delete_chat_sticker_set(self, chat_id: Union[int, str], **kwargs) -> bool:
+    async def delete_chat_sticker_set(self, chat_id: int | str, **kwargs) -> bool:
         """
-        Use this method to delete a group sticker set from a supergroup. The bot must be an
-        administrator in the chat for this to work and must have the appropriate
-        administrator rights. Use the field can_set_sticker_set optionally returned in
-        getChat requests to check if the bot can use this method. Returns True on success.
+        Use this method to delete a group sticker set from a supergroup. The
+        bot must be an administrator in the chat for this to work and must
+        have the appropriate administrator rights. Use the field
+        can_set_sticker_set optionally returned in getChat requests to check
+        if the bot can use this method. Returns True on success.
         """
-        response = await self.api.request(
-            "deleteChatStickerSet", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("deleteChatStickerSet", get_params(locals()))
+        return json.decode(response, type=bool)
 
-    async def get_forum_topic_icon_stickers(self, **kwargs) -> List[Sticker]:
+    async def get_forum_topic_icon_stickers(self, **kwargs) -> list[Sticker]:
         """
-        Use this method to get custom emoji stickers, which can be used as a forum topic
-        icon by any user. Requires no parameters. Returns an Array of Sticker objects.
+        Use this method to get custom emoji stickers, which can be used as a
+        forum topic icon by any user. Requires no parameters. Returns an Array
+        of Sticker objects.
         """
         response = await self.api.request(
-            "getForumTopicIconStickers", self.get_params(locals())
+            "getForumTopicIconStickers", get_params(locals())
         )
-        return parse_obj_as(List[Sticker], response)
+        return json.decode(response, type=list[Sticker])
 
     async def create_forum_topic(
         self,
         name: str,
-        chat_id: Union[int, str],
-        icon_custom_emoji_id: Optional[str] = None,
-        icon_color: Optional[int] = None,
+        chat_id: int | str,
+        icon_custom_emoji_id: str | None = None,
+        icon_color: int | None = None,
         **kwargs
     ) -> ForumTopic:
         """
-        Use this method to create a topic in a forum supergroup chat. The bot must be an
-        administrator in the chat for this to work and must have the can_manage_topics
-        administrator rights. Returns information about the created topic as a ForumTopic
-        object.
+        Use this method to create a topic in a forum supergroup chat. The bot
+        must be an administrator in the chat for this to work and must have
+        the can_manage_topics administrator rights. Returns information about
+        the created topic as a ForumTopic object.
         """
-        response = await self.api.request("createForumTopic", self.get_params(locals()))
-        return ForumTopic(**response)
+        response = await self.api.request("createForumTopic", get_params(locals()))
+        return json.decode(response, type=ForumTopic)
 
     async def edit_forum_topic(
         self,
         message_thread_id: int,
-        chat_id: Union[int, str],
-        name: Optional[str] = None,
-        icon_custom_emoji_id: Optional[str] = None,
+        chat_id: int | str,
+        name: str | None = None,
+        icon_custom_emoji_id: str | None = None,
         **kwargs
     ) -> bool:
         """
-        Use this method to edit name and icon of a topic in a forum supergroup chat. The bot
-        must be an administrator in the chat for this to work and must have
-        can_manage_topics administrator rights, unless it is the creator of the topic.
-        Returns True on success.
+        Use this method to edit name and icon of a topic in a forum supergroup
+        chat. The bot must be an administrator in the chat for this to work
+        and must have can_manage_topics administrator rights, unless it is the
+        creator of the topic. Returns True on success.
         """
-        response = await self.api.request("editForumTopic", self.get_params(locals()))
-        return response
+        response = await self.api.request("editForumTopic", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def close_forum_topic(
-        self, message_thread_id: int, chat_id: Union[int, str], **kwargs
+        self, message_thread_id: int, chat_id: int | str, **kwargs
     ) -> bool:
         """
-        Use this method to close an open topic in a forum supergroup chat. The bot must be
-        an administrator in the chat for this to work and must have the can_manage_topics
-        administrator rights, unless it is the creator of the topic. Returns True on
-        success.
+        Use this method to close an open topic in a forum supergroup chat. The
+        bot must be an administrator in the chat for this to work and must
+        have the can_manage_topics administrator rights, unless it is the
+        creator of the topic. Returns True on success.
         """
-        response = await self.api.request("closeForumTopic", self.get_params(locals()))
-        return response
+        response = await self.api.request("closeForumTopic", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def reopen_forum_topic(
-        self, message_thread_id: int, chat_id: Union[int, str], **kwargs
+        self, message_thread_id: int, chat_id: int | str, **kwargs
     ) -> bool:
         """
-        Use this method to reopen a closed topic in a forum supergroup chat. The bot must be
-        an administrator in the chat for this to work and must have the can_manage_topics
-        administrator rights, unless it is the creator of the topic. Returns True on
-        success.
+        Use this method to reopen a closed topic in a forum supergroup chat.
+        The bot must be an administrator in the chat for this to work and must
+        have the can_manage_topics administrator rights, unless it is the
+        creator of the topic. Returns True on success.
         """
-        response = await self.api.request("reopenForumTopic", self.get_params(locals()))
-        return response
+        response = await self.api.request("reopenForumTopic", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def delete_forum_topic(
-        self, message_thread_id: int, chat_id: Union[int, str], **kwargs
+        self, message_thread_id: int, chat_id: int | str, **kwargs
     ) -> bool:
         """
-        Use this method to delete a forum topic along with all its messages in a forum
-        supergroup chat. The bot must be an administrator in the chat for this to work and
-        must have the can_delete_messages administrator rights. Returns True on success.
+        Use this method to delete a forum topic along with all its messages in
+        a forum supergroup chat. The bot must be an administrator in the chat
+        for this to work and must have the can_delete_messages administrator
+        rights. Returns True on success.
         """
-        response = await self.api.request("deleteForumTopic", self.get_params(locals()))
-        return response
+        response = await self.api.request("deleteForumTopic", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def unpin_all_forum_topic_messages(
-        self, message_thread_id: int, chat_id: Union[int, str], **kwargs
+        self, message_thread_id: int, chat_id: int | str, **kwargs
     ) -> bool:
         """
-        Use this method to clear the list of pinned messages in a forum topic. The bot must
-        be an administrator in the chat for this to work and must have the can_pin_messages
-        administrator right in the supergroup. Returns True on success.
+        Use this method to clear the list of pinned messages in a forum topic.
+        The bot must be an administrator in the chat for this to work and must
+        have the can_pin_messages administrator right in the supergroup.
+        Returns True on success.
         """
         response = await self.api.request(
-            "unpinAllForumTopicMessages", self.get_params(locals())
+            "unpinAllForumTopicMessages", get_params(locals())
         )
-        return response
+        return json.decode(response, type=bool)
 
     async def edit_general_forum_topic(
-        self, name: str, chat_id: Union[int, str], **kwargs
+        self, name: str, chat_id: int | str, **kwargs
     ) -> bool:
         """
-        Use this method to edit the name of the 'General' topic in a forum supergroup chat.
-        The bot must be an administrator in the chat for this to work and must have
-        can_manage_topics administrator rights. Returns True on success.
+        Use this method to edit the name of the 'General' topic in a forum
+        supergroup chat. The bot must be an administrator in the chat for this
+        to work and must have can_manage_topics administrator rights. Returns
+        True on success.
         """
-        response = await self.api.request(
-            "editGeneralForumTopic", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("editGeneralForumTopic", get_params(locals()))
+        return json.decode(response, type=bool)
 
-    async def close_general_forum_topic(
-        self, chat_id: Union[int, str], **kwargs
-    ) -> bool:
+    async def close_general_forum_topic(self, chat_id: int | str, **kwargs) -> bool:
         """
-        Use this method to close an open 'General' topic in a forum supergroup chat. The bot
-        must be an administrator in the chat for this to work and must have the
-        can_manage_topics administrator rights. Returns True on success.
+        Use this method to close an open 'General' topic in a forum supergroup
+        chat. The bot must be an administrator in the chat for this to work
+        and must have the can_manage_topics administrator rights. Returns True
+        on success.
         """
         response = await self.api.request(
-            "closeGeneralForumTopic", self.get_params(locals())
+            "closeGeneralForumTopic", get_params(locals())
         )
-        return response
+        return json.decode(response, type=bool)
 
-    async def reopen_general_forum_topic(
-        self, chat_id: Union[int, str], **kwargs
-    ) -> bool:
+    async def reopen_general_forum_topic(self, chat_id: int | str, **kwargs) -> bool:
         """
-        Use this method to reopen a closed 'General' topic in a forum supergroup chat. The
-        bot must be an administrator in the chat for this to work and must have the
-        can_manage_topics administrator rights. The topic will be automatically unhidden if
-        it was hidden. Returns True on success.
+        Use this method to reopen a closed 'General' topic in a forum
+        supergroup chat. The bot must be an administrator in the chat for this
+        to work and must have the can_manage_topics administrator rights. The
+        topic will be automatically unhidden if it was hidden. Returns True on
+        success.
         """
         response = await self.api.request(
-            "reopenGeneralForumTopic", self.get_params(locals())
+            "reopenGeneralForumTopic", get_params(locals())
         )
-        return response
+        return json.decode(response, type=bool)
 
-    async def hide_general_forum_topic(
-        self, chat_id: Union[int, str], **kwargs
-    ) -> bool:
+    async def hide_general_forum_topic(self, chat_id: int | str, **kwargs) -> bool:
         """
-        Use this method to hide the 'General' topic in a forum supergroup chat. The bot must
-        be an administrator in the chat for this to work and must have the can_manage_topics
-        administrator rights. The topic will be automatically closed if it was open. Returns
-        True on success.
+        Use this method to hide the 'General' topic in a forum supergroup
+        chat. The bot must be an administrator in the chat for this to work
+        and must have the can_manage_topics administrator rights. The topic
+        will be automatically closed if it was open. Returns True on success.
         """
-        response = await self.api.request(
-            "hideGeneralForumTopic", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("hideGeneralForumTopic", get_params(locals()))
+        return json.decode(response, type=bool)
 
-    async def unhide_general_forum_topic(
-        self, chat_id: Union[int, str], **kwargs
-    ) -> bool:
+    async def unhide_general_forum_topic(self, chat_id: int | str, **kwargs) -> bool:
         """
-        Use this method to unhide the 'General' topic in a forum supergroup chat. The bot
-        must be an administrator in the chat for this to work and must have the
-        can_manage_topics administrator rights. Returns True on success.
+        Use this method to unhide the 'General' topic in a forum supergroup
+        chat. The bot must be an administrator in the chat for this to work
+        and must have the can_manage_topics administrator rights. Returns True
+        on success.
         """
         response = await self.api.request(
-            "unhideGeneralForumTopic", self.get_params(locals())
+            "unhideGeneralForumTopic", get_params(locals())
         )
-        return response
+        return json.decode(response, type=bool)
 
     async def answer_callback_query(
         self,
         callback_query_id: str,
-        url: Optional[str] = None,
-        text: Optional[str] = None,
-        show_alert: Optional[bool] = None,
-        cache_time: Optional[int] = None,
+        url: str | None = None,
+        text: str | None = None,
+        show_alert: bool | None = None,
+        cache_time: int | None = None,
         **kwargs
     ) -> bool:
         """
-        Use this method to send answers to callback queries sent from inline keyboards. The
-        answer will be displayed to the user as a notification at the top of the chat screen
-        or as an alert. On success, True is returned. Alternatively, the user can be
-        redirected to the specified Game URL. For this option to work, you must first create
-        a game for your bot via @BotFather and accept the terms. Otherwise, you may use
-        links like t.me/your_bot?start=XXXX that open your bot with a parameter.
+        Use this method to send answers to callback queries sent from inline
+        keyboards. The answer will be displayed to the user as a notification
+        at the top of the chat screen or as an alert. On success, True is
+        returned. Alternatively, the user can be redirected to the specified
+        Game URL. For this option to work, you must first create a game for
+        your bot via @BotFather and accept the terms. Otherwise, you may use
+        links like t.me/your_bot?start=XXXX that open your bot with a
+        parameter.
         """
-        response = await self.api.request(
-            "answerCallbackQuery", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("answerCallbackQuery", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def set_my_commands(
         self,
-        commands: List[BotCommand],
-        scope: Optional[BotCommandScope] = None,
-        language_code: Optional[str] = None,
+        commands: list[BotCommand],
+        scope: BotCommandScope | None = None,
+        language_code: str | None = None,
         **kwargs
     ) -> bool:
         """
-        Use this method to change the list of the bot's commands. See this manual for more
-        details about bot commands. Returns True on success.
+        Use this method to change the list of the bot's commands. See this
+        manual for more details about bot commands. Returns True on success.
         """
-        response = await self.api.request("setMyCommands", self.get_params(locals()))
-        return response
+        response = await self.api.request("setMyCommands", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def delete_my_commands(
         self,
-        scope: Optional[BotCommandScope] = None,
-        language_code: Optional[str] = None,
+        scope: BotCommandScope | None = None,
+        language_code: str | None = None,
         **kwargs
     ) -> bool:
         """
-        Use this method to delete the list of the bot's commands for the given scope and
-        user language. After deletion, higher level commands will be shown to affected
-        users. Returns True on success.
+        Use this method to delete the list of the bot's commands for the given
+        scope and user language. After deletion, higher level commands will be
+        shown to affected users. Returns True on success.
         """
-        response = await self.api.request("deleteMyCommands", self.get_params(locals()))
-        return response
+        response = await self.api.request("deleteMyCommands", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def get_my_commands(
         self,
-        scope: Optional[BotCommandScope] = None,
-        language_code: Optional[str] = None,
+        scope: BotCommandScope | None = None,
+        language_code: str | None = None,
         **kwargs
-    ) -> List[BotCommand]:
+    ) -> list[BotCommand]:
+        """
+        Use this method to get the current list of the bot's commands for the
+        given scope and user language. Returns an Array of BotCommand objects.
+        If commands aren't set, an empty list is returned.
+        """
+        response = await self.api.request("getMyCommands", get_params(locals()))
+        return json.decode(response, type=list[BotCommand])
+
+    async def set_my_name(
+        self, name: str | None = None, language_code: str | None = None, **kwargs
+    ) -> bool:
         """
-        Use this method to get the current list of the bot's commands for the given scope
-        and user language. Returns an Array of BotCommand objects. If commands aren't set,
-        an empty list is returned.
+        Use this method to change the bot's name. Returns True on success.
         """
-        response = await self.api.request("getMyCommands", self.get_params(locals()))
-        return parse_obj_as(List[BotCommand], response)
+        response = await self.api.request("setMyName", get_params(locals()))
+        return json.decode(response, type=bool)
+
+    async def get_my_name(self, language_code: str | None = None, **kwargs) -> BotName:
+        """
+        Use this method to get the current bot name for the given user
+        language. Returns BotName on success.
+        """
+        response = await self.api.request("getMyName", get_params(locals()))
+        return json.decode(response, type=BotName)
 
     async def set_my_description(
-        self,
-        language_code: Optional[str] = None,
-        description: Optional[str] = None,
-        **kwargs
+        self, language_code: str | None = None, description: str | None = None, **kwargs
     ) -> bool:
         """
-        Use this method to change the bot's description, which is shown in the chat with the
-        bot if the chat is empty. Returns True on success.
+        Use this method to change the bot's description, which is shown in the
+        chat with the bot if the chat is empty. Returns True on success.
         """
-        response = await self.api.request("setMyDescription", self.get_params(locals()))
-        return response
+        response = await self.api.request("setMyDescription", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def get_my_description(
-        self, language_code: Optional[str] = None, **kwargs
+        self, language_code: str | None = None, **kwargs
     ) -> BotDescription:
         """
-        Use this method to get the current bot description for the given user language.
-        Returns BotDescription on success.
+        Use this method to get the current bot description for the given user
+        language. Returns BotDescription on success.
         """
-        response = await self.api.request("getMyDescription", self.get_params(locals()))
-        return BotDescription(**response)
+        response = await self.api.request("getMyDescription", get_params(locals()))
+        return json.decode(response, type=BotDescription)
 
     async def set_my_short_description(
         self,
-        short_description: Optional[str] = None,
-        language_code: Optional[str] = None,
+        short_description: str | None = None,
+        language_code: str | None = None,
         **kwargs
     ) -> bool:
         """
-        Use this method to change the bot's short description, which is shown on the bot's
-        profile page and is sent together with the link when users share the bot. Returns
-        True on success.
+        Use this method to change the bot's short description, which is shown
+        on the bot's profile page and is sent together with the link when
+        users share the bot. Returns True on success.
         """
-        response = await self.api.request(
-            "setMyShortDescription", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("setMyShortDescription", get_params(locals()))
+        return json.decode(response, type=bool)
+
+    async def get_my_short_description(
+        self, language_code: str | None = None, **kwargs
+    ) -> BotShortDescription:
+        """
+        Use this method to get the current bot short description for the given
+        user language. Returns BotShortDescription on success.
+        """
+        response = await self.api.request("getMyShortDescription", get_params(locals()))
+        return json.decode(response, type=BotShortDescription)
+
+    async def set_chat_menu_button(
+        self,
+        menu_button: MenuButton | None = None,
+        chat_id: int | None = None,
+        **kwargs
+    ) -> bool:
+        """
+        Use this method to change the bot's menu button in a private chat, or
+        the default menu button. Returns True on success.
+        """
+        response = await self.api.request("setChatMenuButton", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def get_my_short_description(
-        self, language_code: Optional[str] = None, **kwargs
+        self, language_code: str | None = None, **kwargs
     ) -> BotShortDescription:
         """
         Use this method to get the current bot short description for the given user
         language. Returns BotShortDescription on success.
         """
         response = await self.api.request(
             "getMyShortDescription", self.get_params(locals())
         )
-        return BotShortDescription(**response)
+        return json.decode(response, type=BotShortDescription)
 
     async def set_chat_menu_button(
         self,
-        menu_button: Optional[MenuButton] = None,
-        chat_id: Optional[int] = None,
+        menu_button: MenuButton | None = None,
+        chat_id: int | None = None,
         **kwargs
     ) -> bool:
         """
-        Use this method to change the bot's menu button in a private chat, or the default
-        menu button. Returns True on success.
+        Use this method to change the bot's menu button in a private chat, or
+        the default menu button. Returns True on success.
         """
-        response = await self.api.request(
-            "setChatMenuButton", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("setChatMenuButton", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def get_chat_menu_button(
-        self, chat_id: Optional[int] = None, **kwargs
+        self, chat_id: int | None = None, **kwargs
     ) -> MenuButton:
         """
-        Use this method to get the current value of the bot's menu button in a private chat,
-        or the default menu button. Returns MenuButton on success.
+        Use this method to get the current value of the bot's menu button in a
+        private chat, or the default menu button. Returns MenuButton on
+        success.
         """
-        response = await self.api.request(
-            "getChatMenuButton", self.get_params(locals())
+        response = await self.api.request("getChatMenuButton", get_params(locals()))
+        return json.decode(
+            response, type=MenuButtonCommands | MenuButtonWebApp | MenuButtonDefault
         )
-        return parse_obj_as(MenuButton, response)
 
     async def set_my_default_administrator_rights(
         self,
-        rights: Optional[ChatAdministratorRights] = None,
-        for_channels: Optional[bool] = None,
+        rights: ChatAdministratorRights | None = None,
+        for_channels: bool | None = None,
         **kwargs
     ) -> bool:
         """
-        Use this method to change the default administrator rights requested by the bot when
-        it's added as an administrator to groups or channels. These rights will be suggested
-        to users, but they are free to modify the list before adding the bot. Returns True
-        on success.
+        Use this method to change the default administrator rights requested
+        by the bot when it's added as an administrator to groups or channels.
+        These rights will be suggested to users, but they are free to modify
+        the list before adding the bot. Returns True on success.
         """
         response = await self.api.request(
-            "setMyDefaultAdministratorRights", self.get_params(locals())
+            "setMyDefaultAdministratorRights", get_params(locals())
         )
-        return response
+        return json.decode(response, type=bool)
 
     async def get_my_default_administrator_rights(
-        self, for_channels: Optional[bool] = None, **kwargs
+        self, for_channels: bool | None = None, **kwargs
     ) -> ChatAdministratorRights:
         """
-        Use this method to get the current default administrator rights of the bot. Returns
-        ChatAdministratorRights on success.
+        Use this method to get the current default administrator rights of the
+        bot. Returns ChatAdministratorRights on success.
         """
         response = await self.api.request(
-            "getMyDefaultAdministratorRights", self.get_params(locals())
+            "getMyDefaultAdministratorRights", get_params(locals())
         )
-        return ChatAdministratorRights(**response)
+        return json.decode(response, type=ChatAdministratorRights)
 
     async def edit_message_text(
         self,
         text: str,
-        reply_markup: Optional[InlineKeyboardMarkup] = None,
-        parse_mode: Optional[str] = None,
-        message_id: Optional[int] = None,
-        inline_message_id: Optional[str] = None,
-        entities: Optional[List[MessageEntity]] = None,
-        disable_web_page_preview: Optional[bool] = None,
-        chat_id: Optional[Union[int, str]] = None,
-        **kwargs
-    ) -> Union[Message, bool]:
-        """
-        Use this method to edit text and game messages. On success, if the edited message is
-        not an inline message, the edited Message is returned, otherwise True is returned.
+        reply_markup: InlineKeyboardMarkup | None = None,
+        parse_mode: str | None = None,
+        message_id: int | None = None,
+        inline_message_id: str | None = None,
+        entities: list[MessageEntity] | None = None,
+        disable_web_page_preview: bool | None = None,
+        chat_id: int | str | None = None,
+        **kwargs
+    ) -> Message | bool:
+        """
+        Use this method to edit text and game messages. On success, if the
+        edited message is not an inline message, the edited Message is
+        returned, otherwise True is returned.
         """
-        response = await self.api.request("editMessageText", self.get_params(locals()))
-        return parse_obj_as(Union[Message, bool], response)
+        response = await self.api.request("editMessageText", get_params(locals()))
+        return json.decode(response, type=Message | bool)
 
     async def edit_message_caption(
         self,
-        reply_markup: Optional[InlineKeyboardMarkup] = None,
-        parse_mode: Optional[str] = None,
-        message_id: Optional[int] = None,
-        inline_message_id: Optional[str] = None,
-        chat_id: Optional[Union[int, str]] = None,
-        caption_entities: Optional[List[MessageEntity]] = None,
-        caption: Optional[str] = None,
-        **kwargs
-    ) -> Union[Message, bool]:
-        """
-        Use this method to edit captions of messages. On success, if the edited message is
-        not an inline message, the edited Message is returned, otherwise True is returned.
+        reply_markup: InlineKeyboardMarkup | None = None,
+        parse_mode: str | None = None,
+        message_id: int | None = None,
+        inline_message_id: str | None = None,
+        chat_id: int | str | None = None,
+        caption_entities: list[MessageEntity] | None = None,
+        caption: str | None = None,
+        **kwargs
+    ) -> Message | bool:
+        """
+        Use this method to edit captions of messages. On success, if the
+        edited message is not an inline message, the edited Message is
+        returned, otherwise True is returned.
         """
-        response = await self.api.request(
-            "editMessageCaption", self.get_params(locals())
-        )
-        return parse_obj_as(Union[Message, bool], response)
+        response = await self.api.request("editMessageCaption", get_params(locals()))
+        return json.decode(response, type=Message | bool)
 
-    async def edit_message_media(
+    async def stop_message_live_location(
         self,
         media: InputMedia,
-        reply_markup: Optional[InlineKeyboardMarkup] = None,
-        message_id: Optional[int] = None,
-        inline_message_id: Optional[str] = None,
-        chat_id: Optional[Union[int, str]] = None,
-        **kwargs
-    ) -> Union[Message, bool]:
-        """
-        Use this method to edit animation, audio, document, photo, or video messages. If a
-        message is part of a message album, then it can be edited only to an audio for audio
-        albums, only to a document for document albums and to a photo or a video otherwise.
-        When an inline message is edited, a new file can't be uploaded; use a previously
-        uploaded file via its file_id or specify a URL. On success, if the edited message is
-        not an inline message, the edited Message is returned, otherwise True is returned.
+        reply_markup: InlineKeyboardMarkup | None = None,
+        message_id: int | None = None,
+        inline_message_id: str | None = None,
+        chat_id: int | str | None = None,
+        **kwargs
+    ) -> Message | bool:
+        """
+        Use this method to edit animation, audio, document, photo, or video
+        messages. If a message is part of a message album, then it can be
+        edited only to an audio for audio albums, only to a document for
+        document albums and to a photo or a video otherwise. When an inline
+        message is edited, a new file can't be uploaded; use a previously
+        uploaded file via its file_id or specify a URL. On success, if the
+        edited message is not an inline message, the edited Message is
+        returned, otherwise True is returned.
         """
-        response = await self.api.request("editMessageMedia", self.get_params(locals()))
-        return parse_obj_as(Union[Message, bool], response)
+        response = await self.api.request("editMessageMedia", get_params(locals()))
+        return json.decode(response, type=Message | bool)
 
     async def edit_message_live_location(
         self,
         longitude: float,
         latitude: float,
-        reply_markup: Optional[InlineKeyboardMarkup] = None,
-        proximity_alert_radius: Optional[int] = None,
-        message_id: Optional[int] = None,
-        inline_message_id: Optional[str] = None,
-        horizontal_accuracy: Optional[float] = None,
-        heading: Optional[int] = None,
-        chat_id: Optional[Union[int, str]] = None,
-        **kwargs
-    ) -> Union[Message, bool]:
-        """
-        Use this method to edit live location messages. A location can be edited until its
-        live_period expires or editing is explicitly disabled by a call to
-        stopMessageLiveLocation. On success, if the edited message is not an inline message,
-        the edited Message is returned, otherwise True is returned.
+        reply_markup: InlineKeyboardMarkup | None = None,
+        proximity_alert_radius: int | None = None,
+        message_id: int | None = None,
+        inline_message_id: str | None = None,
+        horizontal_accuracy: float | None = None,
+        heading: int | None = None,
+        chat_id: int | str | None = None,
+        **kwargs
+    ) -> Message | bool:
+        """
+        Use this method to edit live location messages. A location can be
+        edited until its live_period expires or editing is explicitly disabled
+        by a call to stopMessageLiveLocation. On success, if the edited
+        message is not an inline message, the edited Message is returned,
+        otherwise True is returned.
         """
         response = await self.api.request(
-            "editMessageLiveLocation", self.get_params(locals())
+            "editMessageLiveLocation", get_params(locals())
         )
-        return parse_obj_as(Union[Message, bool], response)
+        return json.decode(response, type=Message | bool)
 
     async def stop_message_live_location(
         self,
-        reply_markup: Optional[InlineKeyboardMarkup] = None,
-        message_id: Optional[int] = None,
-        inline_message_id: Optional[str] = None,
-        chat_id: Optional[Union[int, str]] = None,
+        reply_markup: InlineKeyboardMarkup | None = None,
+        message_id: int | None = None,
+        inline_message_id: str | None = None,
+        chat_id: int | str | None = None,
         **kwargs
-    ) -> Union[Message, bool]:
+    ) -> Message | bool:
         """
-        Use this method to stop updating a live location message before live_period expires.
-        On success, if the message is not an inline message, the edited Message is returned,
-        otherwise True is returned.
+        Use this method to stop updating a live location message before
+        live_period expires. On success, if the message is not an inline
+        message, the edited Message is returned, otherwise True is returned.
         """
         response = await self.api.request(
-            "stopMessageLiveLocation", self.get_params(locals())
+            "stopMessageLiveLocation", get_params(locals())
         )
-        return parse_obj_as(Union[Message, bool], response)
+        return json.decode(response, type=Message | bool)
 
     async def edit_message_reply_markup(
         self,
-        reply_markup: Optional[InlineKeyboardMarkup] = None,
-        message_id: Optional[int] = None,
-        inline_message_id: Optional[str] = None,
-        chat_id: Optional[Union[int, str]] = None,
+        reply_markup: InlineKeyboardMarkup | None = None,
+        message_id: int | None = None,
+        inline_message_id: str | None = None,
+        chat_id: int | str | None = None,
         **kwargs
-    ) -> Union[Message, bool]:
+    ) -> Message | bool:
         """
-        Use this method to edit only the reply markup of messages. On success, if the edited
-        message is not an inline message, the edited Message is returned, otherwise True is
-        returned.
+        Use this method to edit only the reply markup of messages. On success,
+        if the edited message is not an inline message, the edited Message is
+        returned, otherwise True is returned.
         """
         response = await self.api.request(
-            "editMessageReplyMarkup", self.get_params(locals())
+            "editMessageReplyMarkup", get_params(locals())
         )
-        return parse_obj_as(Union[Message, bool], response)
+        return json.decode(response, type=Message | bool)
 
     async def stop_poll(
         self,
         message_id: int,
-        chat_id: Union[int, str],
-        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        chat_id: int | str,
+        reply_markup: InlineKeyboardMarkup | None = None,
         **kwargs
     ) -> Poll:
         """
-        Use this method to stop a poll which was sent by the bot. On success, the stopped
-        Poll is returned.
+        Use this method to stop a poll which was sent by the bot. On success,
+        the stopped Poll is returned.
         """
-        response = await self.api.request("stopPoll", self.get_params(locals()))
-        return Poll(**response)
+        response = await self.api.request("stopPoll", get_params(locals()))
+        return json.decode(response, type=Poll)
 
     async def delete_message(
-        self, message_id: int, chat_id: Union[int, str], **kwargs
+        self, message_id: int, chat_id: int | str, **kwargs
     ) -> bool:
         """
-        Use this method to delete a message, including service messages, with the following
-        limitations: - A message can only be deleted if it was sent less than 48 hours ago.
-        - Service messages about a supergroup, channel, or forum topic creation can't be
-        deleted. - A dice message in a private chat can only be deleted if it was sent more
-        than 24 hours ago. - Bots can delete outgoing messages in private chats, groups, and
-        supergroups. - Bots can delete incoming messages in private chats. - Bots granted
-        can_post_messages permissions can delete outgoing messages in channels. - If the bot
-        is an administrator of a group, it can delete any message there. - If the bot has
-        can_delete_messages permission in a supergroup or a channel, it can delete any
-        message there. Returns True on success.
+        Use this method to delete a message, including service messages, with
+        the following limitations: - A message can only be deleted if it was
+        sent less than 48 hours ago. - Service messages about a supergroup,
+        channel, or forum topic creation can't be deleted. - A dice message in
+        a private chat can only be deleted if it was sent more than 24 hours
+        ago. - Bots can delete outgoing messages in private chats, groups, and
+        supergroups. - Bots can delete incoming messages in private chats. -
+        Bots granted can_post_messages permissions can delete outgoing
+        messages in channels. - If the bot is an administrator of a group, it
+        can delete any message there. - If the bot has can_delete_messages
+        permission in a supergroup or a channel, it can delete any message
+        there. Returns True on success.
         """
-        response = await self.api.request("deleteMessage", self.get_params(locals()))
-        return response
+        response = await self.api.request("deleteMessage", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def send_sticker(
         self,
-        sticker: Union[InputFile, str],
-        chat_id: Union[int, str],
-        reply_to_message_id: Optional[int] = None,
-        reply_markup: Optional[
-            Union[
-                InlineKeyboardMarkup,
-                ReplyKeyboardMarkup,
-                ReplyKeyboardRemove,
-                ForceReply,
-            ]
-        ] = None,
-        protect_content: Optional[bool] = None,
-        message_thread_id: Optional[int] = None,
-        emoji: Optional[str] = None,
-        disable_notification: Optional[bool] = None,
-        allow_sending_without_reply: Optional[bool] = None,
+        sticker: InputFile | str,
+        chat_id: int | str,
+        reply_to_message_id: int | None = None,
+        reply_markup: InlineKeyboardMarkup
+        | ReplyKeyboardMarkup
+        | ReplyKeyboardRemove
+        | ForceReply
+        | None = None,
+        protect_content: bool | None = None,
+        message_thread_id: int | None = None,
+        emoji: str | None = None,
+        disable_notification: bool | None = None,
+        allow_sending_without_reply: bool | None = None,
         **kwargs
     ) -> Message:
         """
-        Use this method to send static .WEBP, animated .TGS, or video .WEBM stickers. On
-        success, the sent Message is returned.
+        Use this method to send static .WEBP, animated .TGS, or video .WEBM
+        stickers. On success, the sent Message is returned.
         """
-        response = await self.api.request("sendSticker", self.get_params(locals()))
-        return Message(**response)
+        response = await self.api.request("sendSticker", get_params(locals()))
+        return json.decode(response, type=Message)
 
     async def get_sticker_set(self, name: str, **kwargs) -> StickerSet:
         """
-        Use this method to get a sticker set. On success, a StickerSet object is returned.
+        Use this method to get a sticker set. On success, a StickerSet object
+        is returned.
         """
-        response = await self.api.request("getStickerSet", self.get_params(locals()))
-        return StickerSet(**response)
+        response = await self.api.request("getStickerSet", get_params(locals()))
+        return json.decode(response, type=StickerSet)
 
     async def get_custom_emoji_stickers(
-        self, custom_emoji_ids: List[str], **kwargs
-    ) -> List[Sticker]:
+        self, custom_emoji_ids: list[str], **kwargs
+    ) -> list[Sticker]:
         """
-        Use this method to get information about custom emoji stickers by their identifiers.
-        Returns an Array of Sticker objects.
+        Use this method to get information about custom emoji stickers by
+        their identifiers. Returns an Array of Sticker objects.
         """
         response = await self.api.request(
-            "getCustomEmojiStickers", self.get_params(locals())
+            "getCustomEmojiStickers", get_params(locals())
         )
-        return parse_obj_as(List[Sticker], response)
+        return json.decode(response, type=list[Sticker])
 
     async def upload_sticker_file(
         self, user_id: int, sticker_format: str, sticker: InputFile, **kwargs
     ) -> File:
         """
         Use this method to upload a file with a sticker for later use in the
-        createNewStickerSet and addStickerToSet methods (the file can be used multiple
-        times). Returns the uploaded File on success.
+        createNewStickerSet and addStickerToSet methods (the file can be used
+        multiple times). Returns the uploaded File on success.
         """
-        response = await self.api.request(
-            "uploadStickerFile", self.get_params(locals())
-        )
-        return File(**response)
+        response = await self.api.request("uploadStickerFile", get_params(locals()))
+        return json.decode(response, type=File)
 
     async def create_new_sticker_set(
         self,
         user_id: int,
         title: str,
-        stickers: List[InputSticker],
+        stickers: list[InputSticker],
         sticker_format: str,
         name: str,
-        sticker_type: Optional[str] = None,
-        needs_repainting: Optional[bool] = None,
+        sticker_type: str | None = None,
+        needs_repainting: bool | None = None,
         **kwargs
     ) -> bool:
         """
-        Use this method to create a new sticker set owned by a user. The bot will be able to
-        edit the sticker set thus created. Returns True on success.
+        Use this method to create a new sticker set owned by a user. The bot
+        will be able to edit the sticker set thus created. Returns True on
+        success.
         """
-        response = await self.api.request(
-            "createNewStickerSet", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("createNewStickerSet", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def add_sticker_to_set(
         self, user_id: int, sticker: InputSticker, name: str, **kwargs
     ) -> bool:
         """
-        Use this method to add a new sticker to a set created by the bot. The format of the
-        added sticker must match the format of the other stickers in the set. Emoji sticker
-        sets can have up to 200 stickers. Animated and video sticker sets can have up to 50
-        stickers. Static sticker sets can have up to 120 stickers. Returns True on success.
+        Use this method to add a new sticker to a set created by the bot. The
+        format of the added sticker must match the format of the other
+        stickers in the set. Emoji sticker sets can have up to 200 stickers.
+        Animated and video sticker sets can have up to 50 stickers. Static
+        sticker sets can have up to 120 stickers. Returns True on success.
         """
-        response = await self.api.request("addStickerToSet", self.get_params(locals()))
-        return response
+        response = await self.api.request("addStickerToSet", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def set_sticker_position_in_set(
         self, sticker: str, position: int, **kwargs
     ) -> bool:
         """
-        Use this method to move a sticker in a set created by the bot to a specific
-        position. Returns True on success.
+        Use this method to move a sticker in a set created by the bot to a
+        specific position. Returns True on success.
         """
         response = await self.api.request(
-            "setStickerPositionInSet", self.get_params(locals())
+            "setStickerPositionInSet", get_params(locals())
         )
-        return response
+        return json.decode(response, type=bool)
 
     async def delete_sticker_from_set(self, sticker: str, **kwargs) -> bool:
         """
-        Use this method to delete a sticker from a set created by the bot. Returns True on
-        success.
+        Use this method to delete a sticker from a set created by the bot.
+        Returns True on success.
         """
-        response = await self.api.request(
-            "deleteStickerFromSet", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("deleteStickerFromSet", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def set_sticker_emoji_list(
-        self, sticker: str, emoji_list: List[str], **kwargs
+        self, sticker: str, emoji_list: list[str], **kwargs
     ) -> bool:
         """
-        Use this method to change the list of emoji assigned to a regular or custom emoji
-        sticker. The sticker must belong to a sticker set created by the bot. Returns True
-        on success.
+        Use this method to change the list of emoji assigned to a regular or
+        custom emoji sticker. The sticker must belong to a sticker set created
+        by the bot. Returns True on success.
         """
-        response = await self.api.request(
-            "setStickerEmojiList", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("setStickerEmojiList", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def set_sticker_keywords(
-        self, sticker: str, keywords: Optional[List[str]] = None, **kwargs
+        self, sticker: str, keywords: list[str] | None = None, **kwargs
     ) -> bool:
         """
-        Use this method to change search keywords assigned to a regular or custom emoji
-        sticker. The sticker must belong to a sticker set created by the bot. Returns True
-        on success.
+        Use this method to change search keywords assigned to a regular or
+        custom emoji sticker. The sticker must belong to a sticker set created
+        by the bot. Returns True on success.
         """
-        response = await self.api.request(
-            "setStickerKeywords", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("setStickerKeywords", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def set_sticker_mask_position(
-        self, sticker: str, mask_position: Optional[MaskPosition] = None, **kwargs
+        self, sticker: str, mask_position: MaskPosition | None = None, **kwargs
     ) -> bool:
         """
-        Use this method to change the mask position of a mask sticker. The sticker must
-        belong to a sticker set that was created by the bot. Returns True on success.
+        Use this method to change the mask position of a mask sticker. The
+        sticker must belong to a sticker set that was created by the bot.
+        Returns True on success.
         """
         response = await self.api.request(
-            "setStickerMaskPosition", self.get_params(locals())
+            "setStickerMaskPosition", get_params(locals())
         )
-        return response
+        return json.decode(response, type=bool)
 
     async def set_sticker_set_title(self, title: str, name: str, **kwargs) -> bool:
         """
-        Use this method to set the title of a created sticker set. Returns True on success.
+        Use this method to set the title of a created sticker set. Returns
+        True on success.
         """
-        response = await self.api.request(
-            "setStickerSetTitle", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("setStickerSetTitle", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def set_sticker_set_thumbnail(
         self,
         user_id: int,
         name: str,
-        thumbnail: Optional[Union[InputFile, str]] = None,
+        thumbnail: InputFile | str | None = None,
         **kwargs
     ) -> bool:
         """
-        Use this method to set the thumbnail of a regular or mask sticker set. The format of
-        the thumbnail file must match the format of the stickers in the set. Returns True on
-        success.
+        Use this method to set the thumbnail of a regular or mask sticker set.
+        The format of the thumbnail file must match the format of the stickers
+        in the set. Returns True on success.
         """
         response = await self.api.request(
-            "setStickerSetThumbnail", self.get_params(locals())
+            "setStickerSetThumbnail", get_params(locals())
         )
-        return response
+        return json.decode(response, type=bool)
 
     async def set_custom_emoji_sticker_set_thumbnail(
-        self, name: str, custom_emoji_id: Optional[str] = None, **kwargs
+        self, name: str, custom_emoji_id: str | None = None, **kwargs
     ) -> bool:
         """
-        Use this method to set the thumbnail of a custom emoji sticker set. Returns True on
-        success.
+        Use this method to set the thumbnail of a custom emoji sticker set.
+        Returns True on success.
         """
         response = await self.api.request(
-            "setCustomEmojiStickerSetThumbnail", self.get_params(locals())
+            "setCustomEmojiStickerSetThumbnail", get_params(locals())
         )
-        return response
+        return json.decode(response, type=bool)
 
     async def delete_sticker_set(self, name: str, **kwargs) -> bool:
         """
-        Use this method to delete a sticker set that was created by the bot. Returns True on
-        success.
+        Use this method to delete a sticker set that was created by the bot.
+        Returns True on success.
         """
-        response = await self.api.request("deleteStickerSet", self.get_params(locals()))
-        return response
+        response = await self.api.request("deleteStickerSet", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def answer_inline_query(
         self,
-        results: List[InlineQueryResult],
+        results: list[InlineQueryResult],
         inline_query_id: str,
-        switch_pm_text: Optional[str] = None,
-        switch_pm_parameter: Optional[str] = None,
-        next_offset: Optional[str] = None,
-        is_personal: Optional[bool] = None,
-        cache_time: Optional[int] = None,
+        next_offset: str | None = None,
+        is_personal: bool | None = None,
+        cache_time: int | None = None,
+        button: InlineQueryResultsButton | None = None,
         **kwargs
     ) -> bool:
         """
-        Use this method to send answers to an inline query. On success, True is returned. No
-        more than 50 results per query are allowed.
+        Use this method to send answers to an inline query. On success, True
+        is returned. No more than 50 results per query are allowed.
         """
-        response = await self.api.request(
-            "answerInlineQuery", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("answerInlineQuery", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def answer_web_app_query(
         self, web_app_query_id: str, result: InlineQueryResult, **kwargs
     ) -> SentWebAppMessage:
         """
-        Use this method to set the result of an interaction with a Web App and send a
-        corresponding message on behalf of the user to the chat from which the query
-        originated. On success, a SentWebAppMessage object is returned.
+        Use this method to set the result of an interaction with a Web App and
+        send a corresponding message on behalf of the user to the chat from
+        which the query originated. On success, a SentWebAppMessage object is
+        returned.
         """
-        response = await self.api.request(
-            "answerWebAppQuery", self.get_params(locals())
-        )
-        return SentWebAppMessage(**response)
+        response = await self.api.request("answerWebAppQuery", get_params(locals()))
+        return json.decode(response, type=SentWebAppMessage)
 
     async def send_invoice(
         self,
         title: str,
         provider_token: str,
-        prices: List[LabeledPrice],
+        prices: list[LabeledPrice],
         payload: str,
         description: str,
         currency: str,
-        chat_id: Union[int, str],
-        suggested_tip_amounts: Optional[List[int]] = None,
-        start_parameter: Optional[str] = None,
-        send_phone_number_to_provider: Optional[bool] = None,
-        send_email_to_provider: Optional[bool] = None,
-        reply_to_message_id: Optional[int] = None,
-        reply_markup: Optional[InlineKeyboardMarkup] = None,
-        provider_data: Optional[str] = None,
-        protect_content: Optional[bool] = None,
-        photo_width: Optional[int] = None,
-        photo_url: Optional[str] = None,
-        photo_size: Optional[int] = None,
-        photo_height: Optional[int] = None,
-        need_shipping_address: Optional[bool] = None,
-        need_phone_number: Optional[bool] = None,
-        need_name: Optional[bool] = None,
-        need_email: Optional[bool] = None,
-        message_thread_id: Optional[int] = None,
-        max_tip_amount: Optional[int] = None,
-        is_flexible: Optional[bool] = None,
-        disable_notification: Optional[bool] = None,
-        allow_sending_without_reply: Optional[bool] = None,
+        chat_id: int | str,
+        suggested_tip_amounts: list[int] | None = None,
+        start_parameter: str | None = None,
+        send_phone_number_to_provider: bool | None = None,
+        send_email_to_provider: bool | None = None,
+        reply_to_message_id: int | None = None,
+        reply_markup: InlineKeyboardMarkup | None = None,
+        provider_data: str | None = None,
+        protect_content: bool | None = None,
+        photo_width: int | None = None,
+        photo_url: str | None = None,
+        photo_size: int | None = None,
+        photo_height: int | None = None,
+        need_shipping_address: bool | None = None,
+        need_phone_number: bool | None = None,
+        need_name: bool | None = None,
+        need_email: bool | None = None,
+        message_thread_id: int | None = None,
+        max_tip_amount: int | None = None,
+        is_flexible: bool | None = None,
+        disable_notification: bool | None = None,
+        allow_sending_without_reply: bool | None = None,
         **kwargs
     ) -> Message:
         """
-        Use this method to send invoices. On success, the sent Message is returned.
+        Use this method to send invoices. On success, the sent Message is
+        returned.
         """
-        response = await self.api.request("sendInvoice", self.get_params(locals()))
-        return Message(**response)
+        response = await self.api.request("sendInvoice", get_params(locals()))
+        return json.decode(response, type=Message)
 
     async def create_invoice_link(
         self,
         title: str,
         provider_token: str,
-        prices: List[LabeledPrice],
+        prices: list[LabeledPrice],
         payload: str,
         description: str,
         currency: str,
-        suggested_tip_amounts: Optional[List[int]] = None,
-        send_phone_number_to_provider: Optional[bool] = None,
-        send_email_to_provider: Optional[bool] = None,
-        provider_data: Optional[str] = None,
-        photo_width: Optional[int] = None,
-        photo_url: Optional[str] = None,
-        photo_size: Optional[int] = None,
-        photo_height: Optional[int] = None,
-        need_shipping_address: Optional[bool] = None,
-        need_phone_number: Optional[bool] = None,
-        need_name: Optional[bool] = None,
-        need_email: Optional[bool] = None,
-        max_tip_amount: Optional[int] = None,
-        is_flexible: Optional[bool] = None,
+        suggested_tip_amounts: list[int] | None = None,
+        send_phone_number_to_provider: bool | None = None,
+        send_email_to_provider: bool | None = None,
+        provider_data: str | None = None,
+        photo_width: int | None = None,
+        photo_url: str | None = None,
+        photo_size: int | None = None,
+        photo_height: int | None = None,
+        need_shipping_address: bool | None = None,
+        need_phone_number: bool | None = None,
+        need_name: bool | None = None,
+        need_email: bool | None = None,
+        max_tip_amount: int | None = None,
+        is_flexible: bool | None = None,
         **kwargs
     ) -> str:
         """
-        Use this method to create a link for an invoice. Returns the created invoice link as
-        String on success.
+        Use this method to create a link for an invoice. Returns the created
+        invoice link as String on success.
         """
-        response = await self.api.request(
-            "createInvoiceLink", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("createInvoiceLink", get_params(locals()))
+        return json.decode(response, type=str)
 
     async def answer_shipping_query(
         self,
         shipping_query_id: str,
         ok: bool,
-        shipping_options: Optional[List[ShippingOption]] = None,
-        error_message: Optional[str] = None,
+        shipping_options: list[ShippingOption] | None = None,
+        error_message: str | None = None,
         **kwargs
     ) -> bool:
         """
-        If you sent an invoice requesting a shipping address and the parameter is_flexible
-        was specified, the Bot API will send an Update with a shipping_query field to the
-        bot. Use this method to reply to shipping queries. On success, True is returned.
+        If you sent an invoice requesting a shipping address and the parameter
+        is_flexible was specified, the Bot API will send an Update with a
+        shipping_query field to the bot. Use this method to reply to shipping
+        queries. On success, True is returned.
         """
-        response = await self.api.request(
-            "answerShippingQuery", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("answerShippingQuery", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def answer_pre_checkout_query(
         self,
         pre_checkout_query_id: str,
         ok: bool,
-        error_message: Optional[str] = None,
+        error_message: str | None = None,
         **kwargs
     ) -> bool:
         """
-        Once the user has confirmed their payment and shipping details, the Bot API sends
-        the final confirmation in the form of an Update with the field pre_checkout_query.
-        Use this method to respond to such pre-checkout queries. On success, True is
-        returned. Note: The Bot API must receive an answer within 10 seconds after the pre-
-        checkout query was sent.
+        Once the user has confirmed their payment and shipping details, the
+        Bot API sends the final confirmation in the form of an Update with the
+        field pre_checkout_query. Use this method to respond to such pre-
+        checkout queries. On success, True is returned. Note: The Bot API must
+        receive an answer within 10 seconds after the pre-checkout query was
+        sent.
         """
         response = await self.api.request(
-            "answerPreCheckoutQuery", self.get_params(locals())
+            "answerPreCheckoutQuery", get_params(locals())
         )
-        return response
+        return json.decode(response, type=bool)
 
     async def set_passport_data_errors(
-        self, user_id: int, errors: List[PassportElementError], **kwargs
+        self, user_id: int, errors: list[PassportElementError], **kwargs
     ) -> bool:
         """
-        Informs a user that some of the Telegram Passport elements they provided contains
-        errors. The user will not be able to re-submit their Passport to you until the
-        errors are fixed (the contents of the field for which you returned the error must
-        change). Returns True on success. Use this if the data submitted by the user doesn't
-        satisfy the standards your service requires for any reason. For example, if a
-        birthday date seems invalid, a submitted document is blurry, a scan shows evidence
-        of tampering, etc. Supply some details in the error message to make sure the user
-        knows how to correct the issues.
+        Informs a user that some of the Telegram Passport elements they
+        provided contains errors. The user will not be able to re-submit their
+        Passport to you until the errors are fixed (the contents of the field
+        for which you returned the error must change). Returns True on
+        success. Use this if the data submitted by the user doesn't satisfy
+        the standards your service requires for any reason. For example, if a
+        birthday date seems invalid, a submitted document is blurry, a scan
+        shows evidence of tampering, etc. Supply some details in the error
+        message to make sure the user knows how to correct the issues.
         """
-        response = await self.api.request(
-            "setPassportDataErrors", self.get_params(locals())
-        )
-        return response
+        response = await self.api.request("setPassportDataErrors", get_params(locals()))
+        return json.decode(response, type=bool)
 
     async def send_game(
         self,
         game_short_name: str,
         chat_id: int,
-        reply_to_message_id: Optional[int] = None,
-        reply_markup: Optional[InlineKeyboardMarkup] = None,
-        protect_content: Optional[bool] = None,
-        message_thread_id: Optional[int] = None,
-        disable_notification: Optional[bool] = None,
-        allow_sending_without_reply: Optional[bool] = None,
+        reply_to_message_id: int | None = None,
+        reply_markup: InlineKeyboardMarkup | None = None,
+        protect_content: bool | None = None,
+        message_thread_id: int | None = None,
+        disable_notification: bool | None = None,
+        allow_sending_without_reply: bool | None = None,
         **kwargs
     ) -> Message:
         """
-        Use this method to send a game. On success, the sent Message is returned.
+        Use this method to send a game. On success, the sent Message is
+        returned.
         """
-        response = await self.api.request("sendGame", self.get_params(locals()))
-        return Message(**response)
+        response = await self.api.request("sendGame", get_params(locals()))
+        return json.decode(response, type=Message)
 
     async def set_game_score(
         self,
         user_id: int,
         score: int,
-        message_id: Optional[int] = None,
-        inline_message_id: Optional[str] = None,
-        force: Optional[bool] = None,
-        disable_edit_message: Optional[bool] = None,
-        chat_id: Optional[int] = None,
-        **kwargs
-    ) -> Union[Message, bool]:
-        """
-        Use this method to set the score of the specified user in a game message. On
-        success, if the message is not an inline message, the Message is returned, otherwise
-        True is returned. Returns an error, if the new score is not greater than the user's
-        current score in the chat and force is False.
+        message_id: int | None = None,
+        inline_message_id: str | None = None,
+        force: bool | None = None,
+        disable_edit_message: bool | None = None,
+        chat_id: int | None = None,
+        **kwargs
+    ) -> Message | bool:
+        """
+        Use this method to set the score of the specified user in a game
+        message. On success, if the message is not an inline message, the
+        Message is returned, otherwise True is returned. Returns an error, if
+        the new score is not greater than the user's current score in the chat
+        and force is False.
         """
-        response = await self.api.request("setGameScore", self.get_params(locals()))
-        return parse_obj_as(Union[Message, bool], response)
+        response = await self.api.request("setGameScore", get_params(locals()))
+        return json.decode(response, type=Message | bool)
 
     async def get_game_high_scores(
         self,
         user_id: int,
-        message_id: Optional[int] = None,
-        inline_message_id: Optional[str] = None,
-        chat_id: Optional[int] = None,
-        **kwargs
-    ) -> List[GameHighScore]:
-        """
-        Use this method to get data for high score tables. Will return the score of the
-        specified user and several of their neighbors in a game. Returns an Array of
-        GameHighScore objects. This method will currently return scores for the target user,
-        plus two of their closest neighbors on each side. Will also return the top three
-        users if the user and their neighbors are not among them. Please note that this
-        behavior is subject to change.
+        message_id: int | None = None,
+        inline_message_id: str | None = None,
+        chat_id: int | None = None,
+        **kwargs
+    ) -> list[GameHighScore]:
+        """
+        Use this method to get data for high score tables. Will return the
+        score of the specified user and several of their neighbors in a game.
+        Returns an Array of GameHighScore objects. This method will currently
+        return scores for the target user, plus two of their closest neighbors
+        on each side. Will also return the top three users if the user and
+        their neighbors are not among them. Please note that this behavior is
+        subject to change.
         """
-        response = await self.api.request(
-            "getGameHighScores", self.get_params(locals())
-        )
-        return parse_obj_as(List[GameHighScore], response)
+        response = await self.api.request("getGameHighScores", get_params(locals()))
+        return json.decode(response, type=list[GameHighScore])
```

### Comparing `wonda-0.5.7/PKG-INFO` & `wonda-0.6.0a1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,96 +1,86 @@
 Metadata-Version: 2.1
 Name: wonda
-Version: 0.5.7
-Summary: Asynchronous feature-rich Telegram bot framework for building great bots
+Version: 0.6.0a1
+Summary: Asynchronous feature-rich framework for building Telegram bots
 Home-page: https://github.com/wondergram-org/wonda/
 License: MIT
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Provides-Extra: auto-reload
-Provides-Extra: power-ups
-Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
-Requires-Dist: certifi (>=2022.6.15,<2023.0.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
+Requires-Dist: certifi (>=2023.7.22,<2024.0.0)
 Requires-Dist: choicelib (>=0.1.5,<0.2.0)
-Requires-Dist: orjson (>=3.8.5,<4.0.0); extra == "power-ups"
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
-Requires-Dist: typing-extensions (>=4.3.0,<5.0.0)
-Requires-Dist: uvloop (>=0.16.0,<0.17.0); extra == "power-ups"
-Requires-Dist: watchfiles (>=0.16.0,<0.17.0); extra == "auto-reload"
+Requires-Dist: msgspec (>=0.17.0,<0.18.0)
+Requires-Dist: structlog (>=23.1.0,<24.0.0)
 Description-Content-Type: text/markdown
 
-# Wonda ✨
+# Wonda 🫧
 
-[//]: # (Examples)
+[//]: # (Features)
 [examples]: examples/high_level
-[text formatting]: examples/high_level/formatting_example.py
-[middleware]: examples/high_level/setup_middleware.py
-[file uploading]: examples/high_level/file_upload_example.py
-[blueprints]: examples/high_level/load_blueprints.py
-[FSM]: examples/high_level/use_state_dispenser.py
+[format text]: examples/high_level/formatting_example.py
+[upload files]: examples/high_level/file_upload_example.py
+[an advanced state system]: examples/high_level/use_state_dispenser.py
 
 [//]: # (Badges)
 ![Version](https://img.shields.io/pypi/v/wonda?label=version&style=flat-square)
 ![Package downloads](https://img.shields.io/pypi/dw/wonda?label=downloads&style=flat-square)
 ![Supported Python versions](https://img.shields.io/pypi/pyversions/wonda?label=supported%20python%20versions&style=flat-square)
 
-## Why
+Wonda is a Telegram bot framework. It supports latest versions and features of the API. Incredibly fast and extraordinarily customizable, it gives you power to build the bot you always wanted.
 
-Wonda can help you build bots using simple tools with exceptional performance. All batteries are included: there are [text formatting], [file uploading], [blueprints], [middleware] and [FSM].
+## Features
 
-## Flavors
+Ever wanted to build a bot? You can do that in only 6 lines of code.
 
-### Regular
-
-To install regular version of Wonda, enter this command in your terminal:
-
-```shell script
-pip install -U wonda
-```
+```python
+from wonda import Bot, Message
 
-If you decide to go beta, use the same command with `--pre` option or update from dev branch .zip [archive](https://github.com/wondergram-org/wonda/archive/refs/heads/dev.zip).
+bot = Bot("your-token")
 
-### Performance
 
-Wonda is built with customizations in mind, so you can squeeze out the most speed from it. To do so, install it with some extras:
+@bot.on.message()
+async def handler(m: Message) -> None:
+    await m.answer("Hello world!")
 
-```shell script
-pip install --force wonda[power-ups]
+bot.run_forever()
 ```
 
-To see the full list of extra packages, refer to our [project file](pyproject.toml).
+You can already [format text], [upload files], and make use of [an advanced state system] to craft complex interactions. And more features are expected to come! Check out the [examples].
 
-## Guide
+## Customization
 
-It's easy to build a bot with Wonda — it's ready in *six* lines of code. Extending it is no problem too.
+### Speed up event loop
 
-```python
-from wonda import Bot
-
-bot = Bot("your-token")
+```bash
+pip install uvloop
+```
 
+Wonda supports uvloop, an event loop implementation which makes I/O [2-4x quicker](https://github.com/magicstack/uvloop#performance).
 
-@bot.on.message()
-async def handler(_) -> str:
-    return "Hello world!"
+### Replace default JSON module
 
-bot.run_forever()
+``` bash
+pip install orjson
 ```
 
-With Wonda, it's possible to achieve this much with so little code. To get started, check out our [examples].
+Swap out the module that is used under the hood to manipulate JSON and increase speed up to [5 times](https://github.com/ijl/orjson#performance).
+
+## Install
 
-## Contributing
+```bash
+pip install wonda
+```
 
-Wonda is a work in progress and a lot of stuff is expected to change! It's the right time for your input.
+A stable version of Wonda can be installed using this command. Add `--pre` to the command to install a pre-release version.
 
-If you want to report a bug or suggest a feature, [create an issue](https://github.com/wondergram-org/wonda/issues/new/choose). To ask a question, please use [discussions](https://github.com/wondergram-org/wonda/discussions). Big thanks!
+## Contrubuting
 
-## License
+The framework is not yet ready for production. If you like what you see, help us develop this amazing project! [Create an issue](https://github.com/wondergram-org/wonda/issues/new/choose) or [make a pull request](https://github.com/wondergram-org/wonda/compare).
 
-This project is MIT licensed. Based upon hard work of maintainers and contributors of [VKBottle](https://github.com/vkbottle/vkbottle).
+## Copyright
 
-Copyright © timoniq (2019-2021), feeeek (2022), geo-madness (2022-2023)
+(c) timoniq (2019-2021), feeeek (2022-2023), geo-madness (2022-2023)
```

