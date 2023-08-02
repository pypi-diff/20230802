# Comparing `tmp/nonebot_plugin_talk_with_poe_ai-0.1.3.tar.gz` & `tmp/nonebot_plugin_talk_with_poe_ai-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_talk_with_poe_ai-0.1.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_talk_with_poe_ai-0.1.4.tar", max compression
```

## Comparing `nonebot_plugin_talk_with_poe_ai-0.1.3.tar` & `nonebot_plugin_talk_with_poe_ai-0.1.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    12104 2023-08-01 13:22:09.154390 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/__init__.py
--rw-r--r--   0        0        0       32 2023-08-01 03:19:51.510068 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/__init__.py
--rw-r--r--   0        0        0    49240 2023-08-01 13:31:07.632194 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/client.py
--rw-r--r--   0        0        0     1145 2023-08-01 03:19:51.511055 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql
--rw-r--r--   0        0        0      536 2023-08-01 03:19:51.512054 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql
--rw-r--r--   0        0        0      187 2023-08-01 03:19:51.512054 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AutoSubscriptionMutation.graphql
--rw-r--r--   0        0        0      701 2023-08-01 03:19:51.513055 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql
--rw-r--r--   0        0        0      105 2023-08-01 03:19:51.513055 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/BioFragment.graphql
--rw-r--r--   0        0        0      169 2023-08-01 03:19:51.514055 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/BotDeletionButton_poeBotDelete_Mutation.graphql
--rw-r--r--   0        0        0       78 2023-08-01 03:19:51.514055 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatAddedSubscription.graphql
--rw-r--r--   0        0        0      106 2023-08-01 03:19:51.515056 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatFragment.graphql
--rw-r--r--   0        0        0    12084 2023-08-01 03:19:51.515056 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql
--rw-r--r--   0        0        0      712 2023-08-01 03:19:51.516054 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatPaginationQuery.graphql
--rw-r--r--   0        0        0      162 2023-08-01 03:19:51.516054 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatViewQuery.graphql
--rw-r--r--   0        0        0      167 2023-08-01 03:19:51.517055 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteHumanMessagesMutation.graphql
--rw-r--r--   0        0        0      129 2023-08-01 03:19:51.517055 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteMessageMutation.graphql
--rw-r--r--   0        0        0      154 2023-08-01 03:19:51.517993 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteUserMessagesMutation.graphql
--rw-r--r--   0        0        0     1148 2023-08-01 03:19:51.517993 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql
--rw-r--r--   0        0        0      111 2023-08-01 03:19:51.518986 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/HandleFragment.graphql
--rw-r--r--   0        0        0      319 2023-08-01 03:19:51.518986 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/LoginWithVerificationCodeMutation.graphql
--rw-r--r--   0        0        0     1985 2023-08-01 03:19:51.519987 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageAddedSubscription.graphql
--rw-r--r--   0        0        0      141 2023-08-01 03:19:51.520991 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageDeletedSubscription.graphql
--rw-r--r--   0        0        0      207 2023-08-01 03:19:51.520991 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageFragment.graphql
--rw-r--r--   0        0        0      152 2023-08-01 03:19:51.521987 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageRemoveVoteMutation.graphql
--rw-r--r--   0        0        0      223 2023-08-01 03:19:51.522987 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageSetVoteMutation.graphql
--rw-r--r--   0        0        0     1832 2023-08-01 03:19:51.522987 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql
--rw-r--r--   0        0        0      968 2023-08-01 03:19:51.523987 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotEditMutation.graphql
--rw-r--r--   0        0        0      963 2023-08-01 03:19:51.524986 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendMessageMutation.graphql
--rw-r--r--   0        0        0      275 2023-08-01 03:19:51.524986 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendVerificationCodeForLoginMutation.graphql
--rw-r--r--   0        0        0      222 2023-08-01 03:19:51.525986 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ShareMessagesMutation.graphql
--rw-r--r--   0        0        0      321 2023-08-01 03:19:51.525986 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SignupWithVerificationCodeMutation.graphql
--rw-r--r--   0        0        0      166 2023-08-01 03:19:51.526987 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/StaleChatUpdateMutation.graphql
--rw-r--r--   0        0        0      170 2023-08-01 03:19:51.526987 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SubscriptionsMutation.graphql
--rw-r--r--   0        0        0       98 2023-08-01 03:19:51.527990 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizePlainPostQuery.graphql
--rw-r--r--   0        0        0      150 2023-08-01 03:19:51.528991 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizeQuotePostQuery.graphql
--rw-r--r--   0        0        0      183 2023-08-01 03:19:51.528991 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizeSharePostQuery.graphql
--rw-r--r--   0        0        0      382 2023-08-01 03:19:51.529994 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/UserSnippetFragment.graphql
--rw-r--r--   0        0        0      421 2023-08-01 03:19:51.529994 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerInfoQuery.graphql
--rw-r--r--   0        0        0     1068 2023-08-01 03:19:51.530986 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateFragment.graphql
--rw-r--r--   0        0        0      700 2023-08-01 03:19:51.530986 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql
--rw-r--r--   0        0        0       53 2023-08-01 03:19:51.531986 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/requirements.txt
--rw-r--r--   0        0        0     1648 2023-08-01 13:29:20.242168 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/util.py
--rw-r--r--   0        0        0    10484 2023-08-01 13:11:08.666579 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/config.py
--rw-r--r--   0        0        0     4826 2023-08-01 08:04:47.152640 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/data_handle.py
--rw-r--r--   0        0        0  7232220 2023-01-06 09:31:31.000000 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/HYWenHei-85W.ttf
--rw-r--r--   0        0        0     1009 2023-08-01 13:31:16.850270 nonebot_plugin_talk_with_poe_ai-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5466 2023-08-01 13:31:11.755619 nonebot_plugin_talk_with_poe_ai-0.1.3/README.md
--rw-r--r--   0        0        0     6451 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_poe_ai-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    12104 2023-08-02 02:10:29.423123 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/__init__.py
+-rw-r--r--   0        0        0       32 2023-08-01 03:19:51.510068 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/__init__.py
+-rw-r--r--   0        0        0    49240 2023-08-01 13:31:07.632194 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/client.py
+-rw-r--r--   0        0        0     1145 2023-08-01 03:19:51.511055 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql
+-rw-r--r--   0        0        0      536 2023-08-01 03:19:51.512054 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql
+-rw-r--r--   0        0        0      187 2023-08-01 03:19:51.512054 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AutoSubscriptionMutation.graphql
+-rw-r--r--   0        0        0      701 2023-08-01 03:19:51.513055 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql
+-rw-r--r--   0        0        0      105 2023-08-01 03:19:51.513055 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/BioFragment.graphql
+-rw-r--r--   0        0        0      169 2023-08-01 03:19:51.514055 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/BotDeletionButton_poeBotDelete_Mutation.graphql
+-rw-r--r--   0        0        0       78 2023-08-01 03:19:51.514055 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatAddedSubscription.graphql
+-rw-r--r--   0        0        0      106 2023-08-01 03:19:51.515056 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatFragment.graphql
+-rw-r--r--   0        0        0    12084 2023-08-01 03:19:51.515056 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql
+-rw-r--r--   0        0        0      712 2023-08-01 03:19:51.516054 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatPaginationQuery.graphql
+-rw-r--r--   0        0        0      162 2023-08-01 03:19:51.516054 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatViewQuery.graphql
+-rw-r--r--   0        0        0      167 2023-08-01 03:19:51.517055 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteHumanMessagesMutation.graphql
+-rw-r--r--   0        0        0      129 2023-08-01 03:19:51.517055 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteMessageMutation.graphql
+-rw-r--r--   0        0        0      154 2023-08-01 03:19:51.517993 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteUserMessagesMutation.graphql
+-rw-r--r--   0        0        0     1148 2023-08-01 03:19:51.517993 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql
+-rw-r--r--   0        0        0      111 2023-08-01 03:19:51.518986 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/HandleFragment.graphql
+-rw-r--r--   0        0        0      319 2023-08-01 03:19:51.518986 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/LoginWithVerificationCodeMutation.graphql
+-rw-r--r--   0        0        0     1985 2023-08-01 03:19:51.519987 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageAddedSubscription.graphql
+-rw-r--r--   0        0        0      141 2023-08-01 03:19:51.520991 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageDeletedSubscription.graphql
+-rw-r--r--   0        0        0      207 2023-08-01 03:19:51.520991 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageFragment.graphql
+-rw-r--r--   0        0        0      152 2023-08-01 03:19:51.521987 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageRemoveVoteMutation.graphql
+-rw-r--r--   0        0        0      223 2023-08-01 03:19:51.522987 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageSetVoteMutation.graphql
+-rw-r--r--   0        0        0     1832 2023-08-01 03:19:51.522987 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql
+-rw-r--r--   0        0        0      968 2023-08-01 03:19:51.523987 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotEditMutation.graphql
+-rw-r--r--   0        0        0      963 2023-08-01 03:19:51.524986 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendMessageMutation.graphql
+-rw-r--r--   0        0        0      275 2023-08-01 03:19:51.524986 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendVerificationCodeForLoginMutation.graphql
+-rw-r--r--   0        0        0      222 2023-08-01 03:19:51.525986 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ShareMessagesMutation.graphql
+-rw-r--r--   0        0        0      321 2023-08-01 03:19:51.525986 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SignupWithVerificationCodeMutation.graphql
+-rw-r--r--   0        0        0      166 2023-08-01 03:19:51.526987 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/StaleChatUpdateMutation.graphql
+-rw-r--r--   0        0        0      170 2023-08-01 03:19:51.526987 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SubscriptionsMutation.graphql
+-rw-r--r--   0        0        0       98 2023-08-01 03:19:51.527990 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizePlainPostQuery.graphql
+-rw-r--r--   0        0        0      150 2023-08-01 03:19:51.528991 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizeQuotePostQuery.graphql
+-rw-r--r--   0        0        0      183 2023-08-01 03:19:51.528991 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizeSharePostQuery.graphql
+-rw-r--r--   0        0        0      382 2023-08-01 03:19:51.529994 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/UserSnippetFragment.graphql
+-rw-r--r--   0        0        0      421 2023-08-01 03:19:51.529994 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerInfoQuery.graphql
+-rw-r--r--   0        0        0     1068 2023-08-01 03:19:51.530986 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateFragment.graphql
+-rw-r--r--   0        0        0      700 2023-08-01 03:19:51.530986 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql
+-rw-r--r--   0        0        0       53 2023-08-01 03:19:51.531986 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/requirements.txt
+-rw-r--r--   0        0        0     1648 2023-08-01 13:29:20.242168 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/util.py
+-rw-r--r--   0        0        0    10484 2023-08-01 13:11:08.666579 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/config.py
+-rw-r--r--   0        0        0     4916 2023-08-02 02:05:16.072584 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/data_handle.py
+-rw-r--r--   0        0        0  7232220 2023-01-06 09:31:31.000000 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/HYWenHei-85W.ttf
+-rw-r--r--   0        0        0     1009 2023-08-02 02:10:19.202014 nonebot_plugin_talk_with_poe_ai-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5571 2023-08-02 02:10:52.567117 nonebot_plugin_talk_with_poe_ai-0.1.4/README.md
+-rw-r--r--   0        0        0     6552 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_poe_ai-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/__init__.py` & `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/client.py` & `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatPaginationQuery.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageAddedSubscription.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageAddedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotEditMutation.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotEditMutation.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendMessageMutation.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateFragment.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateFragment.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/util.py` & `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/util.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/config.py` & `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/data_handle.py` & `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/data_handle.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,15 @@
     except Exception as e:
         err_msg = str(e)
         logger.error(err_msg)
         # 如果不存在则创建
         if (
             "The bot doesn't exist or isn't accessible" in err_msg
             or "Failed to create a bot with error: handle_already_taken" in err_msg
+            or "Failed to get bot chat_data from https://poe.com/_next/data/" in err_msg
         ):
             # 重置handle，重新请求
             var.session_data[id][0] = ""
             return await handle_req(id, req_text, op)
 
         elif (
             "Failed to extract 'viewer' or 'user_id' from 'next_data'." in err_msg
```

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/HYWenHei-85W.ttf` & `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/HYWenHei-85W.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.3/pyproject.toml` & `nonebot_plugin_talk_with_poe_ai-0.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_talk_with_poe_ai"
-version = "0.1.3"
+version = "0.1.4"
 description = "Nonebot2 基于poe cookie登录AI聊天插件"
 authors = ["nikissXI <1299577815@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_talk_with_poe_ai"}]
 homepage = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_poe_ai"
 repository = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_poe_ai"
```

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.3/README.md` & `nonebot_plugin_talk_with_poe_ai-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 **p_b值** 浏览器登陆[poe官网](https://poe.com/)，打开开发者工具（一般是按F12），依次点击应用程序、存储、Cookie，就可以看到p_b的值了  
 <img width="100%" src="https://raw.githubusercontent.com/nikissXI/nonebot_plugins/main/nonebot_plugin_talk_with_poe_ai/readme_img/2.jpg"/>  
 
 **formkey值** 浏览器登陆[poe官网](https://poe.com/)，打开开发者工具（一般是按F12），然后随便跟一个ai发一句话，点网络，选Fetch/XHR，随便一个请求，在标头那，往下找到请求标头那类，里面有一个Poe-Formkey字段，后面就是值了  
 <img width="100%" src="https://raw.githubusercontent.com/nikissXI/nonebot_plugins/main/nonebot_plugin_talk_with_poe_ai/readme_img/3.jpg"/>  
 
-注意：不同浏览器可能会有点不同，自己变通一下啦！两个值在安装好插件后，使用命令“/poeai auth”进行登录  
+注意：需要先手动create bot试试能不能创建。不同浏览器可能会有点不同，自己变通一下啦！两个值在安装好插件后，使用命令“/poeai auth”进行登录  
 
 
 #### 国内必填
 ```bash
 # 代理地址，支持http和socks代理，国内的话不用代理无法连接poe
 talk_with_poe_ai_proxy = http://127.0.0.1:7890
 ```
@@ -117,10 +117,14 @@
 | /reset | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
 | /poeai | 如果talk_with_poe_ai_all_group_enable为false，则用该命令启用 |
 | /poeai re | poe ai 重连，有时候可能各种因素导致登陆失败 |
 | /poeai auth | 修改登录凭证并重新登录 |
 
 ## 更新日志
+### 2023/8/2 \[v0.1.4]
+
+* 增加一个异常捕获
+
 ### 2023/8/1 \[v0.1.3]
 
 * 发布插件
```

#### html2text {}

```diff
@@ -21,15 +21,16 @@
 [https://raw.githubusercontent.com/nikissXI/nonebot_plugins/main/
 nonebot_plugin_talk_with_poe_ai/readme_img/2.jpg] **formkeyå¼**
 æµè§å¨ç»é[poeå®ç½](https://poe.com/
 )ï¼æå¼å¼åèå·¥å·ï¼ä¸è¬æ¯æF12ï¼ï¼ç¶åéä¾¿è·ä¸ä¸ªaiåä¸å¥è¯ï¼ç¹ç½ç»ï¼éFetch/
 XHRï¼éä¾¿ä¸ä¸ªè¯·æ±ï¼å¨æ å¤´é£ï¼å¾ä¸æ¾å°è¯·æ±æ å¤´é£ç±»ï¼éé¢æä¸ä¸ªPoe-
 Formkeyå­æ®µï¼åé¢å°±æ¯å¼äº [https://raw.githubusercontent.com/nikissXI/
 nonebot_plugins/main/nonebot_plugin_talk_with_poe_ai/readme_img/3.jpg]
-æ³¨æï¼ä¸åæµè§å¨å¯è½ä¼æç¹ä¸åï¼èªå·±åéä¸ä¸å¦ï¼ä¸¤ä¸ªå¼å¨å®è£å¥½æä»¶åï¼ä½¿ç¨å½ä»¤â/
+æ³¨æï¼éè¦åæå¨create
+botè¯è¯è½ä¸è½åå»ºãä¸åæµè§å¨å¯è½ä¼æç¹ä¸åï¼èªå·±åéä¸ä¸å¦ï¼ä¸¤ä¸ªå¼å¨å®è£å¥½æä»¶åï¼ä½¿ç¨å½ä»¤â/
 poeai authâè¿è¡ç»å½ #### å½åå¿å¡« ```bash #
 ä»£çå°åï¼æ¯æhttpåsocksä»£çï¼å½åçè¯ä¸ç¨ä»£çæ æ³è¿æ¥poe
 talk_with_poe_ai_proxy = http://127.0.0.1:7890 ``` ####
 å¤§æ¦çç¨å¾ä¸çéå¡«é¡¹ ```bash # å¤çæ¶æ¯æ¶æ¯å¦æç¤º
 talk_with_poe_ai_reply_notice = true # ç¾¤èæ¯å¦å±äº«ä¼è¯
 talk_with_poe_ai_group_share = false # åªåè®¸è¶çº§ç®¡çåä¿®æ¹é¢è®¾
 talk_with_poe_ai_prompt_admin_only = true #
@@ -62,9 +63,9 @@
 æä»¶å½ä»¤ï¼åå¯ä¿®æ¹ï¼ï¼ | æä»¤ | è¯´æ | |:-----:|:----:| | /talk
 | å¼å§å¯¹è¯ï¼é»è®¤ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /hi |
 æ²æµ¸å¼å¯¹è¯ï¼ä»éç§èï¼ | | /reset |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | | /poeai |
 å¦ætalk_with_poe_ai_all_group_enableä¸ºfalseï¼åç¨è¯¥å½ä»¤å¯ç¨ | | /
 poeai re | poe ai éè¿ï¼ææ¶åå¯è½åç§å ç´ å¯¼è´ç»éå¤±è´¥ | | /
-poeai auth | ä¿®æ¹ç»å½å­è¯å¹¶éæ°ç»å½ | ## æ´æ°æ¥å¿ ### 2023/8/1 \
-[v0.1.3] * åå¸æä»¶
+poeai auth | ä¿®æ¹ç»å½å­è¯å¹¶éæ°ç»å½ | ## æ´æ°æ¥å¿ ### 2023/8/2 \
+[v0.1.4] * å¢å ä¸ä¸ªå¼å¸¸æè· ### 2023/8/1 \[v0.1.3] * åå¸æä»¶
```

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.3/PKG-INFO` & `nonebot_plugin_talk_with_poe_ai-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-talk-with-poe-ai
-Version: 0.1.3
+Version: 0.1.4
 Summary: Nonebot2 基于poe cookie登录AI聊天插件
 Home-page: https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_poe_ai
 License: MIT
 Author: nikissXI
 Author-email: 1299577815@qq.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -70,15 +70,15 @@
 
 **p_b值** 浏览器登陆[poe官网](https://poe.com/)，打开开发者工具（一般是按F12），依次点击应用程序、存储、Cookie，就可以看到p_b的值了  
 <img width="100%" src="https://raw.githubusercontent.com/nikissXI/nonebot_plugins/main/nonebot_plugin_talk_with_poe_ai/readme_img/2.jpg"/>  
 
 **formkey值** 浏览器登陆[poe官网](https://poe.com/)，打开开发者工具（一般是按F12），然后随便跟一个ai发一句话，点网络，选Fetch/XHR，随便一个请求，在标头那，往下找到请求标头那类，里面有一个Poe-Formkey字段，后面就是值了  
 <img width="100%" src="https://raw.githubusercontent.com/nikissXI/nonebot_plugins/main/nonebot_plugin_talk_with_poe_ai/readme_img/3.jpg"/>  
 
-注意：不同浏览器可能会有点不同，自己变通一下啦！两个值在安装好插件后，使用命令“/poeai auth”进行登录  
+注意：需要先手动create bot试试能不能创建。不同浏览器可能会有点不同，自己变通一下啦！两个值在安装好插件后，使用命令“/poeai auth”进行登录  
 
 
 #### 国内必填
 ```bash
 # 代理地址，支持http和socks代理，国内的话不用代理无法连接poe
 talk_with_poe_ai_proxy = http://127.0.0.1:7890
 ```
@@ -142,11 +142,15 @@
 | /reset | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
 | /poeai | 如果talk_with_poe_ai_all_group_enable为false，则用该命令启用 |
 | /poeai re | poe ai 重连，有时候可能各种因素导致登陆失败 |
 | /poeai auth | 修改登录凭证并重新登录 |
 
 ## 更新日志
+### 2023/8/2 \[v0.1.4]
+
+* 增加一个异常捕获
+
 ### 2023/8/1 \[v0.1.3]
 
 * 发布插件
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-poe-ai Version: 0.1.3
+Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-poe-ai Version: 0.1.4
 Summary: Nonebot2 åºäºpoe cookieç»å½AIèå¤©æä»¶ Home-page: https://
 github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_poe_ai
 License: MIT Author: nikissXI Author-email: 1299577815@qq.com Requires-Python:
 >=3.8 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -36,15 +36,16 @@
 [https://raw.githubusercontent.com/nikissXI/nonebot_plugins/main/
 nonebot_plugin_talk_with_poe_ai/readme_img/2.jpg] **formkeyå¼**
 æµè§å¨ç»é[poeå®ç½](https://poe.com/
 )ï¼æå¼å¼åèå·¥å·ï¼ä¸è¬æ¯æF12ï¼ï¼ç¶åéä¾¿è·ä¸ä¸ªaiåä¸å¥è¯ï¼ç¹ç½ç»ï¼éFetch/
 XHRï¼éä¾¿ä¸ä¸ªè¯·æ±ï¼å¨æ å¤´é£ï¼å¾ä¸æ¾å°è¯·æ±æ å¤´é£ç±»ï¼éé¢æä¸ä¸ªPoe-
 Formkeyå­æ®µï¼åé¢å°±æ¯å¼äº [https://raw.githubusercontent.com/nikissXI/
 nonebot_plugins/main/nonebot_plugin_talk_with_poe_ai/readme_img/3.jpg]
-æ³¨æï¼ä¸åæµè§å¨å¯è½ä¼æç¹ä¸åï¼èªå·±åéä¸ä¸å¦ï¼ä¸¤ä¸ªå¼å¨å®è£å¥½æä»¶åï¼ä½¿ç¨å½ä»¤â/
+æ³¨æï¼éè¦åæå¨create
+botè¯è¯è½ä¸è½åå»ºãä¸åæµè§å¨å¯è½ä¼æç¹ä¸åï¼èªå·±åéä¸ä¸å¦ï¼ä¸¤ä¸ªå¼å¨å®è£å¥½æä»¶åï¼ä½¿ç¨å½ä»¤â/
 poeai authâè¿è¡ç»å½ #### å½åå¿å¡« ```bash #
 ä»£çå°åï¼æ¯æhttpåsocksä»£çï¼å½åçè¯ä¸ç¨ä»£çæ æ³è¿æ¥poe
 talk_with_poe_ai_proxy = http://127.0.0.1:7890 ``` ####
 å¤§æ¦çç¨å¾ä¸çéå¡«é¡¹ ```bash # å¤çæ¶æ¯æ¶æ¯å¦æç¤º
 talk_with_poe_ai_reply_notice = true # ç¾¤èæ¯å¦å±äº«ä¼è¯
 talk_with_poe_ai_group_share = false # åªåè®¸è¶çº§ç®¡çåä¿®æ¹é¢è®¾
 talk_with_poe_ai_prompt_admin_only = true #
@@ -77,9 +78,9 @@
 æä»¶å½ä»¤ï¼åå¯ä¿®æ¹ï¼ï¼ | æä»¤ | è¯´æ | |:-----:|:----:| | /talk
 | å¼å§å¯¹è¯ï¼é»è®¤ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /hi |
 æ²æµ¸å¼å¯¹è¯ï¼ä»éç§èï¼ | | /reset |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | | /poeai |
 å¦ætalk_with_poe_ai_all_group_enableä¸ºfalseï¼åç¨è¯¥å½ä»¤å¯ç¨ | | /
 poeai re | poe ai éè¿ï¼ææ¶åå¯è½åç§å ç´ å¯¼è´ç»éå¤±è´¥ | | /
-poeai auth | ä¿®æ¹ç»å½å­è¯å¹¶éæ°ç»å½ | ## æ´æ°æ¥å¿ ### 2023/8/1 \
-[v0.1.3] * åå¸æä»¶
+poeai auth | ä¿®æ¹ç»å½å­è¯å¹¶éæ°ç»å½ | ## æ´æ°æ¥å¿ ### 2023/8/2 \
+[v0.1.4] * å¢å ä¸ä¸ªå¼å¸¸æè· ### 2023/8/1 \[v0.1.3] * åå¸æä»¶
```

