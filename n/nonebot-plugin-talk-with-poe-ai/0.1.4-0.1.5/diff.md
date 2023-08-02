# Comparing `tmp/nonebot_plugin_talk_with_poe_ai-0.1.4.tar.gz` & `tmp/nonebot_plugin_talk_with_poe_ai-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_talk_with_poe_ai-0.1.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_talk_with_poe_ai-0.1.5.tar", max compression
```

## Comparing `nonebot_plugin_talk_with_poe_ai-0.1.4.tar` & `nonebot_plugin_talk_with_poe_ai-0.1.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    12104 2023-08-02 02:10:29.423123 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/__init__.py
--rw-r--r--   0        0        0       32 2023-08-01 03:19:51.510068 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/__init__.py
--rw-r--r--   0        0        0    49240 2023-08-01 13:31:07.632194 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/client.py
--rw-r--r--   0        0        0     1145 2023-08-01 03:19:51.511055 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql
--rw-r--r--   0        0        0      536 2023-08-01 03:19:51.512054 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql
--rw-r--r--   0        0        0      187 2023-08-01 03:19:51.512054 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AutoSubscriptionMutation.graphql
--rw-r--r--   0        0        0      701 2023-08-01 03:19:51.513055 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql
--rw-r--r--   0        0        0      105 2023-08-01 03:19:51.513055 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/BioFragment.graphql
--rw-r--r--   0        0        0      169 2023-08-01 03:19:51.514055 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/BotDeletionButton_poeBotDelete_Mutation.graphql
--rw-r--r--   0        0        0       78 2023-08-01 03:19:51.514055 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatAddedSubscription.graphql
--rw-r--r--   0        0        0      106 2023-08-01 03:19:51.515056 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatFragment.graphql
--rw-r--r--   0        0        0    12084 2023-08-01 03:19:51.515056 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql
--rw-r--r--   0        0        0      712 2023-08-01 03:19:51.516054 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatPaginationQuery.graphql
--rw-r--r--   0        0        0      162 2023-08-01 03:19:51.516054 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatViewQuery.graphql
--rw-r--r--   0        0        0      167 2023-08-01 03:19:51.517055 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteHumanMessagesMutation.graphql
--rw-r--r--   0        0        0      129 2023-08-01 03:19:51.517055 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteMessageMutation.graphql
--rw-r--r--   0        0        0      154 2023-08-01 03:19:51.517993 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteUserMessagesMutation.graphql
--rw-r--r--   0        0        0     1148 2023-08-01 03:19:51.517993 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql
--rw-r--r--   0        0        0      111 2023-08-01 03:19:51.518986 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/HandleFragment.graphql
--rw-r--r--   0        0        0      319 2023-08-01 03:19:51.518986 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/LoginWithVerificationCodeMutation.graphql
--rw-r--r--   0        0        0     1985 2023-08-01 03:19:51.519987 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageAddedSubscription.graphql
--rw-r--r--   0        0        0      141 2023-08-01 03:19:51.520991 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageDeletedSubscription.graphql
--rw-r--r--   0        0        0      207 2023-08-01 03:19:51.520991 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageFragment.graphql
--rw-r--r--   0        0        0      152 2023-08-01 03:19:51.521987 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageRemoveVoteMutation.graphql
--rw-r--r--   0        0        0      223 2023-08-01 03:19:51.522987 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageSetVoteMutation.graphql
--rw-r--r--   0        0        0     1832 2023-08-01 03:19:51.522987 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql
--rw-r--r--   0        0        0      968 2023-08-01 03:19:51.523987 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotEditMutation.graphql
--rw-r--r--   0        0        0      963 2023-08-01 03:19:51.524986 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendMessageMutation.graphql
--rw-r--r--   0        0        0      275 2023-08-01 03:19:51.524986 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendVerificationCodeForLoginMutation.graphql
--rw-r--r--   0        0        0      222 2023-08-01 03:19:51.525986 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ShareMessagesMutation.graphql
--rw-r--r--   0        0        0      321 2023-08-01 03:19:51.525986 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SignupWithVerificationCodeMutation.graphql
--rw-r--r--   0        0        0      166 2023-08-01 03:19:51.526987 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/StaleChatUpdateMutation.graphql
--rw-r--r--   0        0        0      170 2023-08-01 03:19:51.526987 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SubscriptionsMutation.graphql
--rw-r--r--   0        0        0       98 2023-08-01 03:19:51.527990 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizePlainPostQuery.graphql
--rw-r--r--   0        0        0      150 2023-08-01 03:19:51.528991 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizeQuotePostQuery.graphql
--rw-r--r--   0        0        0      183 2023-08-01 03:19:51.528991 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizeSharePostQuery.graphql
--rw-r--r--   0        0        0      382 2023-08-01 03:19:51.529994 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/UserSnippetFragment.graphql
--rw-r--r--   0        0        0      421 2023-08-01 03:19:51.529994 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerInfoQuery.graphql
--rw-r--r--   0        0        0     1068 2023-08-01 03:19:51.530986 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateFragment.graphql
--rw-r--r--   0        0        0      700 2023-08-01 03:19:51.530986 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql
--rw-r--r--   0        0        0       53 2023-08-01 03:19:51.531986 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/requirements.txt
--rw-r--r--   0        0        0     1648 2023-08-01 13:29:20.242168 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/util.py
--rw-r--r--   0        0        0    10484 2023-08-01 13:11:08.666579 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/config.py
--rw-r--r--   0        0        0     4916 2023-08-02 02:05:16.072584 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/data_handle.py
--rw-r--r--   0        0        0  7232220 2023-01-06 09:31:31.000000 nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/HYWenHei-85W.ttf
--rw-r--r--   0        0        0     1009 2023-08-02 02:10:19.202014 nonebot_plugin_talk_with_poe_ai-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5571 2023-08-02 02:10:52.567117 nonebot_plugin_talk_with_poe_ai-0.1.4/README.md
--rw-r--r--   0        0        0     6552 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_poe_ai-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    12104 2023-08-02 06:59:54.535689 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/__init__.py
+-rw-r--r--   0        0        0       32 2023-08-01 03:19:51.510068 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/__init__.py
+-rw-r--r--   0        0        0    49240 2023-08-01 13:31:07.632194 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/client.py
+-rw-r--r--   0        0        0     1145 2023-08-01 03:19:51.511055 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql
+-rw-r--r--   0        0        0      536 2023-08-01 03:19:51.512054 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql
+-rw-r--r--   0        0        0      187 2023-08-01 03:19:51.512054 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AutoSubscriptionMutation.graphql
+-rw-r--r--   0        0        0      701 2023-08-01 03:19:51.513055 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql
+-rw-r--r--   0        0        0      105 2023-08-01 03:19:51.513055 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/BioFragment.graphql
+-rw-r--r--   0        0        0      169 2023-08-01 03:19:51.514055 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/BotDeletionButton_poeBotDelete_Mutation.graphql
+-rw-r--r--   0        0        0       78 2023-08-01 03:19:51.514055 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatAddedSubscription.graphql
+-rw-r--r--   0        0        0      106 2023-08-01 03:19:51.515056 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatFragment.graphql
+-rw-r--r--   0        0        0    12084 2023-08-01 03:19:51.515056 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql
+-rw-r--r--   0        0        0      712 2023-08-01 03:19:51.516054 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatPaginationQuery.graphql
+-rw-r--r--   0        0        0      162 2023-08-01 03:19:51.516054 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatViewQuery.graphql
+-rw-r--r--   0        0        0      167 2023-08-01 03:19:51.517055 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteHumanMessagesMutation.graphql
+-rw-r--r--   0        0        0      129 2023-08-01 03:19:51.517055 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteMessageMutation.graphql
+-rw-r--r--   0        0        0      154 2023-08-01 03:19:51.517993 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteUserMessagesMutation.graphql
+-rw-r--r--   0        0        0     1148 2023-08-01 03:19:51.517993 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql
+-rw-r--r--   0        0        0      111 2023-08-01 03:19:51.518986 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/HandleFragment.graphql
+-rw-r--r--   0        0        0      319 2023-08-01 03:19:51.518986 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/LoginWithVerificationCodeMutation.graphql
+-rw-r--r--   0        0        0     1985 2023-08-01 03:19:51.519987 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageAddedSubscription.graphql
+-rw-r--r--   0        0        0      141 2023-08-01 03:19:51.520991 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageDeletedSubscription.graphql
+-rw-r--r--   0        0        0      207 2023-08-01 03:19:51.520991 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageFragment.graphql
+-rw-r--r--   0        0        0      152 2023-08-01 03:19:51.521987 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageRemoveVoteMutation.graphql
+-rw-r--r--   0        0        0      223 2023-08-01 03:19:51.522987 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageSetVoteMutation.graphql
+-rw-r--r--   0        0        0     1832 2023-08-01 03:19:51.522987 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql
+-rw-r--r--   0        0        0      968 2023-08-01 03:19:51.523987 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotEditMutation.graphql
+-rw-r--r--   0        0        0      963 2023-08-01 03:19:51.524986 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendMessageMutation.graphql
+-rw-r--r--   0        0        0      275 2023-08-01 03:19:51.524986 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendVerificationCodeForLoginMutation.graphql
+-rw-r--r--   0        0        0      222 2023-08-01 03:19:51.525986 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ShareMessagesMutation.graphql
+-rw-r--r--   0        0        0      321 2023-08-01 03:19:51.525986 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SignupWithVerificationCodeMutation.graphql
+-rw-r--r--   0        0        0      166 2023-08-01 03:19:51.526987 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/StaleChatUpdateMutation.graphql
+-rw-r--r--   0        0        0      170 2023-08-01 03:19:51.526987 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SubscriptionsMutation.graphql
+-rw-r--r--   0        0        0       98 2023-08-01 03:19:51.527990 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizePlainPostQuery.graphql
+-rw-r--r--   0        0        0      150 2023-08-01 03:19:51.528991 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizeQuotePostQuery.graphql
+-rw-r--r--   0        0        0      183 2023-08-01 03:19:51.528991 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizeSharePostQuery.graphql
+-rw-r--r--   0        0        0      382 2023-08-01 03:19:51.529994 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/UserSnippetFragment.graphql
+-rw-r--r--   0        0        0      421 2023-08-01 03:19:51.529994 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerInfoQuery.graphql
+-rw-r--r--   0        0        0     1068 2023-08-01 03:19:51.530986 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateFragment.graphql
+-rw-r--r--   0        0        0      700 2023-08-01 03:19:51.530986 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql
+-rw-r--r--   0        0        0       53 2023-08-01 03:19:51.531986 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/requirements.txt
+-rw-r--r--   0        0        0     1648 2023-08-01 13:29:20.242168 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/util.py
+-rw-r--r--   0        0        0    10484 2023-08-01 13:11:08.666579 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/config.py
+-rw-r--r--   0        0        0     4906 2023-08-02 08:17:38.173640 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/data_handle.py
+-rw-r--r--   0        0        0  7232220 2023-01-06 09:31:31.000000 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/HYWenHei-85W.ttf
+-rw-r--r--   0        0        0     1009 2023-08-02 08:27:30.818986 nonebot_plugin_talk_with_poe_ai-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5620 2023-08-02 08:27:25.129835 nonebot_plugin_talk_with_poe_ai-0.1.5/README.md
+-rw-r--r--   0        0        0     6597 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_poe_ai-0.1.5/PKG-INFO
```

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/__init__.py` & `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -291,21 +291,21 @@
         # 修改预设
         var.session_data[id][1] = prompt_name
 
         await prompt_set.send(f"设置中，请稍后。。。", at_sender=True)
 
         # 检查之前是否进行过对话
         if id in var.session_data and var.session_data[id][0]:
-            # 修改预设
-            result = await put_in_req_queue(id, "", "prompt")
+            # 清空聊天记录
+            result = await put_in_req_queue(id, "", "reset")
             if result:
                 await prompt_set.send(result)
 
-            # 清空聊天记录
-            result = await put_in_req_queue(id, "", "reset")
+            # 修改预设
+            result = await put_in_req_queue(id, "", "prompt")
             if result:
                 await prompt_set.send(result)
 
         await prompt_set.reject(f"已设置预设为“{prompt_name}”并清空聊天记录", at_sender=True)
 
     # 增加预设
     if text == "增加":
```

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/client.py` & `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatPaginationQuery.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageAddedSubscription.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageAddedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotEditMutation.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotEditMutation.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendMessageMutation.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateFragment.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateFragment.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/async_poe_client/util.py` & `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/util.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/config.py` & `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/data_handle.py` & `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/data_handle.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,14 +60,15 @@
                 suggested_replies=False,
             )
 
         if op == "reset":
             await var.poe.delete_bot_conversation(
                 url_botname=var.session_data[id][0], del_all=True
             )
+            await var.poe.send_chat_break(url_botname=var.session_data[id][0])
             result = ""
 
         elif op == "prompt":
             await var.poe.edit_bot(
                 url_botname=var.session_data[id][0],
                 prompt=var.prompt_list[var.session_data[id][1]],
             )
@@ -87,15 +88,14 @@
     except Exception as e:
         err_msg = str(e)
         logger.error(err_msg)
         # 如果不存在则创建
         if (
             "The bot doesn't exist or isn't accessible" in err_msg
             or "Failed to create a bot with error: handle_already_taken" in err_msg
-            or "Failed to get bot chat_data from https://poe.com/_next/data/" in err_msg
         ):
             # 重置handle，重新请求
             var.session_data[id][0] = ""
             return await handle_req(id, req_text, op)
 
         elif (
             "Failed to extract 'viewer' or 'user_id' from 'next_data'." in err_msg
```

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.4/nonebot_plugin_talk_with_poe_ai/HYWenHei-85W.ttf` & `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/HYWenHei-85W.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.4/pyproject.toml` & `nonebot_plugin_talk_with_poe_ai-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_talk_with_poe_ai"
-version = "0.1.4"
+version = "0.1.5"
 description = "Nonebot2 基于poe cookie登录AI聊天插件"
 authors = ["nikissXI <1299577815@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_talk_with_poe_ai"}]
 homepage = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_poe_ai"
 repository = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_poe_ai"
```

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.4/README.md` & `nonebot_plugin_talk_with_poe_ai-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,18 @@
 | /reset | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
 | /poeai | 如果talk_with_poe_ai_all_group_enable为false，则用该命令启用 |
 | /poeai re | poe ai 重连，有时候可能各种因素导致登陆失败 |
 | /poeai auth | 修改登录凭证并重新登录 |
 
 ## 更新日志
+### 2023/8/2 \[v0.1.5]
+
+* 优化reset逻辑
+
 ### 2023/8/2 \[v0.1.4]
 
 * 增加一个异常捕获
 
 ### 2023/8/1 \[v0.1.3]
 
 * 发布插件
```

#### html2text {}

```diff
@@ -64,8 +64,9 @@
 | å¼å§å¯¹è¯ï¼é»è®¤ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /hi |
 æ²æµ¸å¼å¯¹è¯ï¼ä»éç§èï¼ | | /reset |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | | /poeai |
 å¦ætalk_with_poe_ai_all_group_enableä¸ºfalseï¼åç¨è¯¥å½ä»¤å¯ç¨ | | /
 poeai re | poe ai éè¿ï¼ææ¶åå¯è½åç§å ç´ å¯¼è´ç»éå¤±è´¥ | | /
 poeai auth | ä¿®æ¹ç»å½å­è¯å¹¶éæ°ç»å½ | ## æ´æ°æ¥å¿ ### 2023/8/2 \
-[v0.1.4] * å¢å ä¸ä¸ªå¼å¸¸æè· ### 2023/8/1 \[v0.1.3] * åå¸æä»¶
+[v0.1.5] * ä¼åreseté»è¾ ### 2023/8/2 \[v0.1.4] * å¢å ä¸ä¸ªå¼å¸¸æè·
+### 2023/8/1 \[v0.1.3] * åå¸æä»¶
```

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.4/PKG-INFO` & `nonebot_plugin_talk_with_poe_ai-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-talk-with-poe-ai
-Version: 0.1.4
+Version: 0.1.5
 Summary: Nonebot2 基于poe cookie登录AI聊天插件
 Home-page: https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_poe_ai
 License: MIT
 Author: nikissXI
 Author-email: 1299577815@qq.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -142,14 +142,18 @@
 | /reset | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
 | /poeai | 如果talk_with_poe_ai_all_group_enable为false，则用该命令启用 |
 | /poeai re | poe ai 重连，有时候可能各种因素导致登陆失败 |
 | /poeai auth | 修改登录凭证并重新登录 |
 
 ## 更新日志
+### 2023/8/2 \[v0.1.5]
+
+* 优化reset逻辑
+
 ### 2023/8/2 \[v0.1.4]
 
 * 增加一个异常捕获
 
 ### 2023/8/1 \[v0.1.3]
 
 * 发布插件
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-poe-ai Version: 0.1.4
+Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-poe-ai Version: 0.1.5
 Summary: Nonebot2 åºäºpoe cookieç»å½AIèå¤©æä»¶ Home-page: https://
 github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_poe_ai
 License: MIT Author: nikissXI Author-email: 1299577815@qq.com Requires-Python:
 >=3.8 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -79,8 +79,9 @@
 | å¼å§å¯¹è¯ï¼é»è®¤ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /hi |
 æ²æµ¸å¼å¯¹è¯ï¼ä»éç§èï¼ | | /reset |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | | /poeai |
 å¦ætalk_with_poe_ai_all_group_enableä¸ºfalseï¼åç¨è¯¥å½ä»¤å¯ç¨ | | /
 poeai re | poe ai éè¿ï¼ææ¶åå¯è½åç§å ç´ å¯¼è´ç»éå¤±è´¥ | | /
 poeai auth | ä¿®æ¹ç»å½å­è¯å¹¶éæ°ç»å½ | ## æ´æ°æ¥å¿ ### 2023/8/2 \
-[v0.1.4] * å¢å ä¸ä¸ªå¼å¸¸æè· ### 2023/8/1 \[v0.1.3] * åå¸æä»¶
+[v0.1.5] * ä¼åreseté»è¾ ### 2023/8/2 \[v0.1.4] * å¢å ä¸ä¸ªå¼å¸¸æè·
+### 2023/8/1 \[v0.1.3] * åå¸æä»¶
```

