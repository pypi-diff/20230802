# Comparing `tmp/nonebot_plugin_talk_with_poe_ai-0.1.5.tar.gz` & `tmp/nonebot_plugin_talk_with_poe_ai-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_talk_with_poe_ai-0.1.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_talk_with_poe_ai-0.1.6.tar", max compression
```

## Comparing `nonebot_plugin_talk_with_poe_ai-0.1.5.tar` & `nonebot_plugin_talk_with_poe_ai-0.1.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    12104 2023-08-02 06:59:54.535689 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/__init__.py
--rw-r--r--   0        0        0       32 2023-08-01 03:19:51.510068 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/__init__.py
--rw-r--r--   0        0        0    49240 2023-08-01 13:31:07.632194 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/client.py
--rw-r--r--   0        0        0     1145 2023-08-01 03:19:51.511055 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql
--rw-r--r--   0        0        0      536 2023-08-01 03:19:51.512054 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql
--rw-r--r--   0        0        0      187 2023-08-01 03:19:51.512054 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AutoSubscriptionMutation.graphql
--rw-r--r--   0        0        0      701 2023-08-01 03:19:51.513055 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql
--rw-r--r--   0        0        0      105 2023-08-01 03:19:51.513055 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/BioFragment.graphql
--rw-r--r--   0        0        0      169 2023-08-01 03:19:51.514055 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/BotDeletionButton_poeBotDelete_Mutation.graphql
--rw-r--r--   0        0        0       78 2023-08-01 03:19:51.514055 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatAddedSubscription.graphql
--rw-r--r--   0        0        0      106 2023-08-01 03:19:51.515056 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatFragment.graphql
--rw-r--r--   0        0        0    12084 2023-08-01 03:19:51.515056 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql
--rw-r--r--   0        0        0      712 2023-08-01 03:19:51.516054 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatPaginationQuery.graphql
--rw-r--r--   0        0        0      162 2023-08-01 03:19:51.516054 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatViewQuery.graphql
--rw-r--r--   0        0        0      167 2023-08-01 03:19:51.517055 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteHumanMessagesMutation.graphql
--rw-r--r--   0        0        0      129 2023-08-01 03:19:51.517055 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteMessageMutation.graphql
--rw-r--r--   0        0        0      154 2023-08-01 03:19:51.517993 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteUserMessagesMutation.graphql
--rw-r--r--   0        0        0     1148 2023-08-01 03:19:51.517993 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql
--rw-r--r--   0        0        0      111 2023-08-01 03:19:51.518986 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/HandleFragment.graphql
--rw-r--r--   0        0        0      319 2023-08-01 03:19:51.518986 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/LoginWithVerificationCodeMutation.graphql
--rw-r--r--   0        0        0     1985 2023-08-01 03:19:51.519987 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageAddedSubscription.graphql
--rw-r--r--   0        0        0      141 2023-08-01 03:19:51.520991 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageDeletedSubscription.graphql
--rw-r--r--   0        0        0      207 2023-08-01 03:19:51.520991 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageFragment.graphql
--rw-r--r--   0        0        0      152 2023-08-01 03:19:51.521987 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageRemoveVoteMutation.graphql
--rw-r--r--   0        0        0      223 2023-08-01 03:19:51.522987 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageSetVoteMutation.graphql
--rw-r--r--   0        0        0     1832 2023-08-01 03:19:51.522987 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql
--rw-r--r--   0        0        0      968 2023-08-01 03:19:51.523987 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotEditMutation.graphql
--rw-r--r--   0        0        0      963 2023-08-01 03:19:51.524986 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendMessageMutation.graphql
--rw-r--r--   0        0        0      275 2023-08-01 03:19:51.524986 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendVerificationCodeForLoginMutation.graphql
--rw-r--r--   0        0        0      222 2023-08-01 03:19:51.525986 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ShareMessagesMutation.graphql
--rw-r--r--   0        0        0      321 2023-08-01 03:19:51.525986 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SignupWithVerificationCodeMutation.graphql
--rw-r--r--   0        0        0      166 2023-08-01 03:19:51.526987 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/StaleChatUpdateMutation.graphql
--rw-r--r--   0        0        0      170 2023-08-01 03:19:51.526987 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SubscriptionsMutation.graphql
--rw-r--r--   0        0        0       98 2023-08-01 03:19:51.527990 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizePlainPostQuery.graphql
--rw-r--r--   0        0        0      150 2023-08-01 03:19:51.528991 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizeQuotePostQuery.graphql
--rw-r--r--   0        0        0      183 2023-08-01 03:19:51.528991 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizeSharePostQuery.graphql
--rw-r--r--   0        0        0      382 2023-08-01 03:19:51.529994 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/UserSnippetFragment.graphql
--rw-r--r--   0        0        0      421 2023-08-01 03:19:51.529994 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerInfoQuery.graphql
--rw-r--r--   0        0        0     1068 2023-08-01 03:19:51.530986 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateFragment.graphql
--rw-r--r--   0        0        0      700 2023-08-01 03:19:51.530986 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql
--rw-r--r--   0        0        0       53 2023-08-01 03:19:51.531986 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/requirements.txt
--rw-r--r--   0        0        0     1648 2023-08-01 13:29:20.242168 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/util.py
--rw-r--r--   0        0        0    10484 2023-08-01 13:11:08.666579 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/config.py
--rw-r--r--   0        0        0     4906 2023-08-02 08:17:38.173640 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/data_handle.py
--rw-r--r--   0        0        0  7232220 2023-01-06 09:31:31.000000 nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/HYWenHei-85W.ttf
--rw-r--r--   0        0        0     1009 2023-08-02 08:27:30.818986 nonebot_plugin_talk_with_poe_ai-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     5620 2023-08-02 08:27:25.129835 nonebot_plugin_talk_with_poe_ai-0.1.5/README.md
--rw-r--r--   0        0        0     6597 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_poe_ai-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    12145 2023-08-02 11:43:54.171847 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/__init__.py
+-rw-r--r--   0        0        0       32 2023-08-01 03:19:51.510068 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/__init__.py
+-rw-r--r--   0        0        0    49240 2023-08-01 13:31:07.632194 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/client.py
+-rw-r--r--   0        0        0     1145 2023-08-01 03:19:51.511055 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql
+-rw-r--r--   0        0        0      536 2023-08-01 03:19:51.512054 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql
+-rw-r--r--   0        0        0      187 2023-08-01 03:19:51.512054 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AutoSubscriptionMutation.graphql
+-rw-r--r--   0        0        0      701 2023-08-01 03:19:51.513055 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql
+-rw-r--r--   0        0        0      105 2023-08-01 03:19:51.513055 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/BioFragment.graphql
+-rw-r--r--   0        0        0      169 2023-08-01 03:19:51.514055 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/BotDeletionButton_poeBotDelete_Mutation.graphql
+-rw-r--r--   0        0        0       78 2023-08-01 03:19:51.514055 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatAddedSubscription.graphql
+-rw-r--r--   0        0        0      106 2023-08-01 03:19:51.515056 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatFragment.graphql
+-rw-r--r--   0        0        0    12084 2023-08-01 03:19:51.515056 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql
+-rw-r--r--   0        0        0      712 2023-08-01 03:19:51.516054 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatPaginationQuery.graphql
+-rw-r--r--   0        0        0      162 2023-08-01 03:19:51.516054 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatViewQuery.graphql
+-rw-r--r--   0        0        0      167 2023-08-01 03:19:51.517055 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteHumanMessagesMutation.graphql
+-rw-r--r--   0        0        0      129 2023-08-01 03:19:51.517055 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteMessageMutation.graphql
+-rw-r--r--   0        0        0      154 2023-08-01 03:19:51.517993 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteUserMessagesMutation.graphql
+-rw-r--r--   0        0        0     1148 2023-08-01 03:19:51.517993 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql
+-rw-r--r--   0        0        0      111 2023-08-01 03:19:51.518986 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/HandleFragment.graphql
+-rw-r--r--   0        0        0      319 2023-08-01 03:19:51.518986 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/LoginWithVerificationCodeMutation.graphql
+-rw-r--r--   0        0        0     1985 2023-08-01 03:19:51.519987 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageAddedSubscription.graphql
+-rw-r--r--   0        0        0      141 2023-08-01 03:19:51.520991 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageDeletedSubscription.graphql
+-rw-r--r--   0        0        0      207 2023-08-01 03:19:51.520991 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageFragment.graphql
+-rw-r--r--   0        0        0      152 2023-08-01 03:19:51.521987 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageRemoveVoteMutation.graphql
+-rw-r--r--   0        0        0      223 2023-08-01 03:19:51.522987 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageSetVoteMutation.graphql
+-rw-r--r--   0        0        0     1832 2023-08-01 03:19:51.522987 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql
+-rw-r--r--   0        0        0      968 2023-08-01 03:19:51.523987 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotEditMutation.graphql
+-rw-r--r--   0        0        0      963 2023-08-01 03:19:51.524986 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendMessageMutation.graphql
+-rw-r--r--   0        0        0      275 2023-08-01 03:19:51.524986 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendVerificationCodeForLoginMutation.graphql
+-rw-r--r--   0        0        0      222 2023-08-01 03:19:51.525986 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ShareMessagesMutation.graphql
+-rw-r--r--   0        0        0      321 2023-08-01 03:19:51.525986 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SignupWithVerificationCodeMutation.graphql
+-rw-r--r--   0        0        0      166 2023-08-01 03:19:51.526987 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/StaleChatUpdateMutation.graphql
+-rw-r--r--   0        0        0      170 2023-08-01 03:19:51.526987 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SubscriptionsMutation.graphql
+-rw-r--r--   0        0        0       98 2023-08-01 03:19:51.527990 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizePlainPostQuery.graphql
+-rw-r--r--   0        0        0      150 2023-08-01 03:19:51.528991 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizeQuotePostQuery.graphql
+-rw-r--r--   0        0        0      183 2023-08-01 03:19:51.528991 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizeSharePostQuery.graphql
+-rw-r--r--   0        0        0      382 2023-08-01 03:19:51.529994 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/UserSnippetFragment.graphql
+-rw-r--r--   0        0        0      421 2023-08-01 03:19:51.529994 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerInfoQuery.graphql
+-rw-r--r--   0        0        0     1068 2023-08-01 03:19:51.530986 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateFragment.graphql
+-rw-r--r--   0        0        0      700 2023-08-01 03:19:51.530986 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql
+-rw-r--r--   0        0        0       53 2023-08-01 03:19:51.531986 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/requirements.txt
+-rw-r--r--   0        0        0     1648 2023-08-01 13:29:20.242168 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/util.py
+-rw-r--r--   0        0        0    10484 2023-08-01 13:11:08.666579 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/config.py
+-rw-r--r--   0        0        0     4906 2023-08-02 08:17:38.173640 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/data_handle.py
+-rw-r--r--   0        0        0  7232220 2023-01-06 09:31:31.000000 nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/HYWenHei-85W.ttf
+-rw-r--r--   0        0        0     1009 2023-08-02 11:43:43.606388 nonebot_plugin_talk_with_poe_ai-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     5726 2023-08-02 11:44:54.552980 nonebot_plugin_talk_with_poe_ai-0.1.6/README.md
+-rw-r--r--   0        0        0     6702 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_poe_ai-0.1.6/PKG-INFO
```

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/__init__.py` & `nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 re_cmd = pc.talk_with_poe_ai_reconnect_cmd
 auth_cmd = pc.talk_with_poe_ai_auth_cmd
 __plugin_meta__ = PluginMetadata(
     name="talk with poe ai",
     description="Nonebot2 基于poe cookie登录AI聊天插件",
     type="application",
     homepage="https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_poe_ai",
+    supported_adapters={"~onebot.v11"},
     usage=f"""插件命令如下
 {talk_cmd}   # 开始对话，默认群里@机器人也可以
 {talk_p_cmd}   # 沉浸式对话（仅限私聊）
 {reset_cmd}   # 重置对话（不会重置预设）
 {prompt_cmd}   # 设置预设（人格），设置后会重置对话
 {enable_cmd}   # 如果关闭所有群启用，则用这个命令启用
 {re_cmd}   # poe ai 重连
```

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/client.py` & `nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatPaginationQuery.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageAddedSubscription.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageAddedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotEditMutation.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotEditMutation.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendMessageMutation.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateFragment.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateFragment.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/async_poe_client/util.py` & `nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/async_poe_client/util.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/config.py` & `nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/data_handle.py` & `nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/data_handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.5/nonebot_plugin_talk_with_poe_ai/HYWenHei-85W.ttf` & `nonebot_plugin_talk_with_poe_ai-0.1.6/nonebot_plugin_talk_with_poe_ai/HYWenHei-85W.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.5/pyproject.toml` & `nonebot_plugin_talk_with_poe_ai-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_talk_with_poe_ai"
-version = "0.1.5"
+version = "0.1.6"
 description = "Nonebot2 基于poe cookie登录AI聊天插件"
 authors = ["nikissXI <1299577815@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_talk_with_poe_ai"}]
 homepage = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_poe_ai"
 repository = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_poe_ai"
```

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.5/README.md` & `nonebot_plugin_talk_with_poe_ai-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
   <a href="https://v2.nonebot.dev/">
     <img src="https://img.shields.io/static/v1?label=nonebot&message=v2rc1%2B&color=green" alt="nonebot2">
   </a>
   <img src="https://img.shields.io/static/v1?label=python+&message=3.8%2B&color=blue" alt="python">
 </p>
 
 # 注意！
-使用本插件需要配置代理，要么把nb配置在大陆外的网络环境。
+使用本插件需要配置代理，要么把nb配置在大陆外的网络环境。  
+插件由于刚写好还没做好长期的稳定性测试，所以可能会出现比较多的问题~  
 
 ## 简介
 大家都在搓chatgpt的插件，来试试poe哇，不会因为各种问题连不上或封号，能跟官网一样调用chatgpt，甚至能用其他模型的ai，[poe官网](https://poe.com/)。  
 本插件是基于[talk_with_chatgpt](https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt)插件修改过来的，使用了[Spark-GPT](https://github.com/canxin121/Spark-GPT)这个插件的poe请求库。  
 <img width="100%" src="https://raw.githubusercontent.com/nikissXI/nonebot_plugins/main/nonebot_plugin_talk_with_poe_ai/readme_img/1.jpg"/>  
 
 
@@ -117,15 +118,15 @@
 | /reset | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
 | /poeai | 如果talk_with_poe_ai_all_group_enable为false，则用该命令启用 |
 | /poeai re | poe ai 重连，有时候可能各种因素导致登陆失败 |
 | /poeai auth | 修改登录凭证并重新登录 |
 
 ## 更新日志
-### 2023/8/2 \[v0.1.5]
+### 2023/8/2 \[v0.1.6]
 
 * 优化reset逻辑
 
 ### 2023/8/2 \[v0.1.4]
 
 * 增加一个异常捕获
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
                               [NoneBotPluginLogo]
    # nonebot_plugin_talk_with_poe_ai _â¨ Nonebot2 ä¸ä¸ªç®åæç¨çpoe
                                  aiæä»¶ â¨_
                          [license] [nonebot2] [python]
 # æ³¨æï¼
 ä½¿ç¨æ¬æä»¶éè¦éç½®ä»£çï¼è¦ä¹ænbéç½®å¨å¤§éå¤çç½ç»ç¯å¢ã
+æä»¶ç±äºååå¥½è¿æ²¡åå¥½é¿æçç¨³å®æ§æµè¯ï¼æä»¥å¯è½ä¼åºç°æ¯è¾å¤çé®é¢~
 ## ç®ä»
 å¤§å®¶é½å¨æchatgptçæä»¶ï¼æ¥è¯è¯poeåï¼ä¸ä¼å ä¸ºåç§é®é¢è¿ä¸ä¸æå°å·ï¼è½è·å®ç½ä¸æ ·è°ç¨chatgptï¼çè³è½ç¨å¶ä»æ¨¡åçaiï¼
 [poeå®ç½](https://poe.com/)ã æ¬æä»¶æ¯åºäº[talk_with_chatgpt](https://
 github.com/nikissXI/nonebot_plugins/tree/main/
 nonebot_plugin_talk_with_chatgpt)æä»¶ä¿®æ¹è¿æ¥çï¼ä½¿ç¨äº[Spark-GPT]
 (https://github.com/canxin121/Spark-GPT)è¿ä¸ªæä»¶çpoeè¯·æ±åºã [https:/
 /raw.githubusercontent.com/nikissXI/nonebot_plugins/main/
@@ -64,9 +65,9 @@
 | å¼å§å¯¹è¯ï¼é»è®¤ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /hi |
 æ²æµ¸å¼å¯¹è¯ï¼ä»éç§èï¼ | | /reset |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | | /poeai |
 å¦ætalk_with_poe_ai_all_group_enableä¸ºfalseï¼åç¨è¯¥å½ä»¤å¯ç¨ | | /
 poeai re | poe ai éè¿ï¼ææ¶åå¯è½åç§å ç´ å¯¼è´ç»éå¤±è´¥ | | /
 poeai auth | ä¿®æ¹ç»å½å­è¯å¹¶éæ°ç»å½ | ## æ´æ°æ¥å¿ ### 2023/8/2 \
-[v0.1.5] * ä¼åreseté»è¾ ### 2023/8/2 \[v0.1.4] * å¢å ä¸ä¸ªå¼å¸¸æè·
+[v0.1.6] * ä¼åreseté»è¾ ### 2023/8/2 \[v0.1.4] * å¢å ä¸ä¸ªå¼å¸¸æè·
 ### 2023/8/1 \[v0.1.3] * åå¸æä»¶
```

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.5/PKG-INFO` & `nonebot_plugin_talk_with_poe_ai-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-talk-with-poe-ai
-Version: 0.1.5
+Version: 0.1.6
 Summary: Nonebot2 基于poe cookie登录AI聊天插件
 Home-page: https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_poe_ai
 License: MIT
 Author: nikissXI
 Author-email: 1299577815@qq.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -42,15 +42,16 @@
   <a href="https://v2.nonebot.dev/">
     <img src="https://img.shields.io/static/v1?label=nonebot&message=v2rc1%2B&color=green" alt="nonebot2">
   </a>
   <img src="https://img.shields.io/static/v1?label=python+&message=3.8%2B&color=blue" alt="python">
 </p>
 
 # 注意！
-使用本插件需要配置代理，要么把nb配置在大陆外的网络环境。
+使用本插件需要配置代理，要么把nb配置在大陆外的网络环境。  
+插件由于刚写好还没做好长期的稳定性测试，所以可能会出现比较多的问题~  
 
 ## 简介
 大家都在搓chatgpt的插件，来试试poe哇，不会因为各种问题连不上或封号，能跟官网一样调用chatgpt，甚至能用其他模型的ai，[poe官网](https://poe.com/)。  
 本插件是基于[talk_with_chatgpt](https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt)插件修改过来的，使用了[Spark-GPT](https://github.com/canxin121/Spark-GPT)这个插件的poe请求库。  
 <img width="100%" src="https://raw.githubusercontent.com/nikissXI/nonebot_plugins/main/nonebot_plugin_talk_with_poe_ai/readme_img/1.jpg"/>  
 
 
@@ -142,15 +143,15 @@
 | /reset | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
 | /poeai | 如果talk_with_poe_ai_all_group_enable为false，则用该命令启用 |
 | /poeai re | poe ai 重连，有时候可能各种因素导致登陆失败 |
 | /poeai auth | 修改登录凭证并重新登录 |
 
 ## 更新日志
-### 2023/8/2 \[v0.1.5]
+### 2023/8/2 \[v0.1.6]
 
 * 优化reset逻辑
 
 ### 2023/8/2 \[v0.1.4]
 
 * 增加一个异常捕获
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-poe-ai Version: 0.1.5
+Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-poe-ai Version: 0.1.6
 Summary: Nonebot2 åºäºpoe cookieç»å½AIèå¤©æä»¶ Home-page: https://
 github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_poe_ai
 License: MIT Author: nikissXI Author-email: 1299577815@qq.com Requires-Python:
 >=3.8 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -15,14 +15,15 @@
 nonebot_plugin_talk_with_poe_ai Description-Content-Type: text/markdown
                               [NoneBotPluginLogo]
    # nonebot_plugin_talk_with_poe_ai _â¨ Nonebot2 ä¸ä¸ªç®åæç¨çpoe
                                  aiæä»¶ â¨_
                          [license] [nonebot2] [python]
 # æ³¨æï¼
 ä½¿ç¨æ¬æä»¶éè¦éç½®ä»£çï¼è¦ä¹ænbéç½®å¨å¤§éå¤çç½ç»ç¯å¢ã
+æä»¶ç±äºååå¥½è¿æ²¡åå¥½é¿æçç¨³å®æ§æµè¯ï¼æä»¥å¯è½ä¼åºç°æ¯è¾å¤çé®é¢~
 ## ç®ä»
 å¤§å®¶é½å¨æchatgptçæä»¶ï¼æ¥è¯è¯poeåï¼ä¸ä¼å ä¸ºåç§é®é¢è¿ä¸ä¸æå°å·ï¼è½è·å®ç½ä¸æ ·è°ç¨chatgptï¼çè³è½ç¨å¶ä»æ¨¡åçaiï¼
 [poeå®ç½](https://poe.com/)ã æ¬æä»¶æ¯åºäº[talk_with_chatgpt](https://
 github.com/nikissXI/nonebot_plugins/tree/main/
 nonebot_plugin_talk_with_chatgpt)æä»¶ä¿®æ¹è¿æ¥çï¼ä½¿ç¨äº[Spark-GPT]
 (https://github.com/canxin121/Spark-GPT)è¿ä¸ªæä»¶çpoeè¯·æ±åºã [https:/
 /raw.githubusercontent.com/nikissXI/nonebot_plugins/main/
@@ -79,9 +80,9 @@
 | å¼å§å¯¹è¯ï¼é»è®¤ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /hi |
 æ²æµ¸å¼å¯¹è¯ï¼ä»éç§èï¼ | | /reset |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | | /poeai |
 å¦ætalk_with_poe_ai_all_group_enableä¸ºfalseï¼åç¨è¯¥å½ä»¤å¯ç¨ | | /
 poeai re | poe ai éè¿ï¼ææ¶åå¯è½åç§å ç´ å¯¼è´ç»éå¤±è´¥ | | /
 poeai auth | ä¿®æ¹ç»å½å­è¯å¹¶éæ°ç»å½ | ## æ´æ°æ¥å¿ ### 2023/8/2 \
-[v0.1.5] * ä¼åreseté»è¾ ### 2023/8/2 \[v0.1.4] * å¢å ä¸ä¸ªå¼å¸¸æè·
+[v0.1.6] * ä¼åreseté»è¾ ### 2023/8/2 \[v0.1.4] * å¢å ä¸ä¸ªå¼å¸¸æè·
 ### 2023/8/1 \[v0.1.3] * åå¸æä»¶
```

