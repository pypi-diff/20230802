# Comparing `tmp/joatmon-2.1.2.tar.gz` & `tmp/joatmon-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joatmon-2.1.2.tar", last modified: Wed Aug  2 21:41:53 2023, max compression
+gzip compressed data, was "joatmon-2.1.3.tar", last modified: Wed Aug  2 21:58:03 2023, max compression
```

## Comparing `joatmon-2.1.2.tar` & `joatmon-2.1.3.tar`

### file list

```diff
@@ -1,350 +1,350 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.244483 joatmon-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-02 21:41:42.000000 joatmon-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-08-02 21:41:53.244483 joatmon-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-08-02 21:41:42.000000 joatmon-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.208482 joatmon-2.1.2/joatmon/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.208482 joatmon-2.1.2/joatmon/ai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.208482 joatmon-2.1.2/joatmon/ai/models/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/models/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.208482 joatmon-2.1.2/joatmon/ai/models/reinforcement/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/models/reinforcement/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.208482 joatmon-2.1.2/joatmon/ai/models/reinforcement/hybrid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/models/reinforcement/hybrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/models/reinforcement/hybrid/ddpg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/models/reinforcement/hybrid/td3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.212482 joatmon-2.1.2/joatmon/ai/models/reinforcement/policy_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/models/reinforcement/policy_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/models/reinforcement/policy_optimization/ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.212482 joatmon-2.1.2/joatmon/ai/models/reinforcement/q_learning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/models/reinforcement/q_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/models/reinforcement/q_learning/dqn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.212482 joatmon-2.1.2/joatmon/ai/models/semisupervised/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/models/semisupervised/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.212482 joatmon-2.1.2/joatmon/ai/models/supervised/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/models/supervised/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.212482 joatmon-2.1.2/joatmon/ai/models/supervised/classification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/models/supervised/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/models/supervised/classification/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.212482 joatmon-2.1.2/joatmon/ai/models/supervised/regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/models/supervised/regression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.212482 joatmon-2.1.2/joatmon/ai/models/unsupervised/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/models/unsupervised/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.212482 joatmon-2.1.2/joatmon/ai/models/unsupervised/clustering/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/models/unsupervised/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.212482 joatmon-2.1.2/joatmon/ai/models/unsupervised/dimension_reduction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/models/unsupervised/dimension_reduction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.212482 joatmon-2.1.2/joatmon/ai/network/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/network/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.212482 joatmon-2.1.2/joatmon/ai/network/reinforcement/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/network/reinforcement/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.212482 joatmon-2.1.2/joatmon/ai/network/reinforcement/hybrid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/network/reinforcement/hybrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/network/reinforcement/hybrid/ddpg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/network/reinforcement/hybrid/td3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.212482 joatmon-2.1.2/joatmon/ai/network/reinforcement/policy_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/network/reinforcement/policy_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/network/reinforcement/policy_optimization/ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.212482 joatmon-2.1.2/joatmon/ai/network/reinforcement/q_learning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/network/reinforcement/q_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/network/reinforcement/q_learning/dqn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.212482 joatmon-2.1.2/joatmon/ai/network/semisupervised/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/network/semisupervised/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.212482 joatmon-2.1.2/joatmon/ai/network/supervised/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/network/supervised/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.212482 joatmon-2.1.2/joatmon/ai/network/supervised/classification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/network/supervised/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/network/supervised/classification/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.212482 joatmon-2.1.2/joatmon/ai/network/supervised/regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/network/supervised/regression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.212482 joatmon-2.1.2/joatmon/ai/network/unsupervised/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/network/unsupervised/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.212482 joatmon-2.1.2/joatmon/ai/network/unsupervised/clustering/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/network/unsupervised/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.212482 joatmon-2.1.2/joatmon/ai/network/unsupervised/dimension_reduction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/network/unsupervised/dimension_reduction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    21835 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/ai/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.212482 joatmon-2.1.2/joatmon/algoritm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/algoritm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.216482 joatmon-2.1.2/joatmon/algoritm/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/algoritm/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/algoritm/search/bfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/algoritm/search/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/algoritm/search/dfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/algoritm/search/linear.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.216482 joatmon-2.1.2/joatmon/algoritm/sort/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/algoritm/sort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.216482 joatmon-2.1.2/joatmon/algoritm/traverse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/algoritm/traverse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/algoritm/traverse/inorder.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/algoritm/traverse/postorder.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/algoritm/traverse/preorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.216482 joatmon-2.1.2/joatmon/array/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/array/array.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/array/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    23501 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/array/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/array/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.216482 joatmon-2.1.2/joatmon/assistant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13596 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.220482 joatmon-2.1.2/joatmon/assistant/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/agenda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/cd.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/contact.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/cwd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/greeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/help.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/mkdir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/move.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/note.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/rm.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/save.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/say.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/todo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/core/weather.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/stt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/assistant/tts.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.224482 joatmon-2.1.2/joatmon/decorator/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/decorator/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/decorator/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/decorator/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/decorator/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/decorator/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/decorator/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/decorator/otp.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/decorator/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/decorator/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/decorator/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.224482 joatmon-2.1.2/joatmon/game/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.204482 joatmon-2.1.2/joatmon/game/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.224482 joatmon-2.1.2/joatmon/game/assets/chess/
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/assets/chess/black-bishop.png
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/assets/chess/black-king.png
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/assets/chess/black-knight.png
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/assets/chess/black-pawn.png
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/assets/chess/black-queen.png
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/assets/chess/black-rook.png
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/assets/chess/white-bishop.png
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/assets/chess/white-king.png
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/assets/chess/white-knight.png
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/assets/chess/white-pawn.png
--rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/assets/chess/white-queen.png
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/assets/chess/white-rook.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.204482 joatmon-2.1.2/joatmon/game/assets/sokoban/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.228483 joatmon-2.1.2/joatmon/game/assets/sokoban/sprites/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/assets/sokoban/sprites/block.png
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/assets/sokoban/sprites/goal.png
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/assets/sokoban/sprites/obstacle.png
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/assets/sokoban/sprites/player.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.228483 joatmon-2.1.2/joatmon/game/assets/sokoban/xmls/
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/assets/sokoban/xmls/default.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/assets/sokoban/xmls/medium.xml
--rw-r--r--   0 runner    (1001) docker     (123)    15196 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/puzzle.py
--rw-r--r--   0 runner    (1001) docker     (123)    30825 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/sokoban.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/game/tiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.228483 joatmon-2.1.2/joatmon/message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/message/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)    27913 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/message/broker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/message/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/message/codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/message/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/message/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.228483 joatmon-2.1.2/joatmon/message/mqtt/
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/message/mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/message/mqtt/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    33394 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/message/mqtt/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    36033 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/message/mqtt/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/message/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/message/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.228483 joatmon-2.1.2/joatmon/nn/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30581 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    57625 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.228483 joatmon-2.1.2/joatmon/nn/layer/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/layer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.232483 joatmon-2.1.2/joatmon/nn/layer/activation/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/layer/activation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/layer/activation/relu.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/layer/activation/sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/layer/activation/softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/layer/activation/tanh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/layer/batchnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/layer/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/layer/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/layer/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/layer/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/layer/lstm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.232483 joatmon-2.1.2/joatmon/nn/layer/pool/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/layer/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/layer/pool/avgpool.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/layer/pool/maxpool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.232483 joatmon-2.1.2/joatmon/nn/loss/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/loss/cce.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/loss/ce.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/loss/mae.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/loss/mse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.232483 joatmon-2.1.2/joatmon/nn/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/optimizer/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/optimizer/rmsprop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.232483 joatmon-2.1.2/joatmon/nn/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/scheduler/exponential.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/nn/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/noise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.232483 joatmon-2.1.2/joatmon/orm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/orm/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/orm/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/orm/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/orm/field.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/orm/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/orm/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    17862 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/orm/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/orm/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.236483 joatmon-2.1.2/joatmon/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.236483 joatmon-2.1.2/joatmon/plugin/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/auth/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/auth/jwt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.236483 joatmon-2.1.2/joatmon/plugin/cache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/cache/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/cache/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.236483 joatmon-2.1.2/joatmon/plugin/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/database/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/database/couchbase.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/database/elastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/database/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/database/postgresql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.236483 joatmon-2.1.2/joatmon/plugin/localizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/localizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/localizer/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/localizer/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.236483 joatmon-2.1.2/joatmon/plugin/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/logger/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/logger/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/logger/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/logger/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.236483 joatmon-2.1.2/joatmon/plugin/message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/message/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/message/kafka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.236483 joatmon-2.1.2/joatmon/plugin/otp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/otp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/otp/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/otp/otp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/plugin/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.240483 joatmon-2.1.2/joatmon/rdp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/rdp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/rdp/client.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/rdp/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    45504 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/rdp/rfb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/serializable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.240483 joatmon-2.1.2/joatmon/structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/structure/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/structure/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.240483 joatmon-2.1.2/joatmon/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.240483 joatmon-2.1.2/joatmon/system/fs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/fs/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/fs/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.240483 joatmon-2.1.2/joatmon/system/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.240483 joatmon-2.1.2/joatmon/system/gui/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/gui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/gui/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/gui/widgets/dropdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/gui/widgets/label.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/gui/widgets/lineedit.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/gui/widgets/list_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/gui/widgets/option.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/gui/widgets/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/gui/widgets/scroll_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/gui/widgets/tab_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/gui/widgets/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.244483 joatmon-2.1.2/joatmon/system/hid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/hid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/hid/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/hid/console.py
--rw-r--r--   0 runner    (1001) docker     (123)    42766 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/hid/desktop.py
--rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/hid/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/hid/microphone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/hid/mouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/hid/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/hid/speaker.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/lock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.244483 joatmon-2.1.2/joatmon/system/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/memory/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/memory/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/memory/locator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/memory/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/system/memory/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14369 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-02 21:41:42.000000 joatmon-2.1.2/joatmon/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.208482 joatmon-2.1.2/joatmon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-08-02 21:41:53.000000 joatmon-2.1.2/joatmon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-08-02 21:41:53.000000 joatmon-2.1.2/joatmon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:41:53.000000 joatmon-2.1.2/joatmon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-02 21:41:53.000000 joatmon-2.1.2/joatmon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-02 21:41:53.000000 joatmon-2.1.2/joatmon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-02 21:41:53.000000 joatmon-2.1.2/joatmon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 21:41:53.244483 joatmon-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-08-02 21:41:42.000000 joatmon-2.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:53.244483 joatmon-2.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:41:42.000000 joatmon-2.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-02 21:41:42.000000 joatmon-2.1.2/tests/test_.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-08-02 21:41:42.000000 joatmon-2.1.2/tests/test_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-02 21:41:42.000000 joatmon-2.1.2/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.464582 joatmon-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-02 21:57:51.000000 joatmon-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-08-02 21:58:03.464582 joatmon-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-08-02 21:57:51.000000 joatmon-2.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.420582 joatmon-2.1.3/joatmon/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.420582 joatmon-2.1.3/joatmon/ai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.420582 joatmon-2.1.3/joatmon/ai/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/models/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.420582 joatmon-2.1.3/joatmon/ai/models/reinforcement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/models/reinforcement/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.420582 joatmon-2.1.3/joatmon/ai/models/reinforcement/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/models/reinforcement/hybrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/models/reinforcement/hybrid/ddpg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/models/reinforcement/hybrid/td3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.420582 joatmon-2.1.3/joatmon/ai/models/reinforcement/policy_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/models/reinforcement/policy_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/models/reinforcement/policy_optimization/ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.420582 joatmon-2.1.3/joatmon/ai/models/reinforcement/q_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/models/reinforcement/q_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/models/reinforcement/q_learning/dqn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.420582 joatmon-2.1.3/joatmon/ai/models/semisupervised/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/models/semisupervised/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.420582 joatmon-2.1.3/joatmon/ai/models/supervised/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/models/supervised/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.424582 joatmon-2.1.3/joatmon/ai/models/supervised/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/models/supervised/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/models/supervised/classification/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.424582 joatmon-2.1.3/joatmon/ai/models/supervised/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/models/supervised/regression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.424582 joatmon-2.1.3/joatmon/ai/models/unsupervised/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/models/unsupervised/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.424582 joatmon-2.1.3/joatmon/ai/models/unsupervised/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/models/unsupervised/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.424582 joatmon-2.1.3/joatmon/ai/models/unsupervised/dimension_reduction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/models/unsupervised/dimension_reduction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.424582 joatmon-2.1.3/joatmon/ai/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/network/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.424582 joatmon-2.1.3/joatmon/ai/network/reinforcement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/network/reinforcement/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.424582 joatmon-2.1.3/joatmon/ai/network/reinforcement/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/network/reinforcement/hybrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/network/reinforcement/hybrid/ddpg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/network/reinforcement/hybrid/td3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.424582 joatmon-2.1.3/joatmon/ai/network/reinforcement/policy_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/network/reinforcement/policy_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/network/reinforcement/policy_optimization/ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.424582 joatmon-2.1.3/joatmon/ai/network/reinforcement/q_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/network/reinforcement/q_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/network/reinforcement/q_learning/dqn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.424582 joatmon-2.1.3/joatmon/ai/network/semisupervised/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/network/semisupervised/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.424582 joatmon-2.1.3/joatmon/ai/network/supervised/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/network/supervised/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.424582 joatmon-2.1.3/joatmon/ai/network/supervised/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/network/supervised/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/network/supervised/classification/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.424582 joatmon-2.1.3/joatmon/ai/network/supervised/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/network/supervised/regression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.424582 joatmon-2.1.3/joatmon/ai/network/unsupervised/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/network/unsupervised/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.424582 joatmon-2.1.3/joatmon/ai/network/unsupervised/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/network/unsupervised/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.424582 joatmon-2.1.3/joatmon/ai/network/unsupervised/dimension_reduction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/network/unsupervised/dimension_reduction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21835 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/ai/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.424582 joatmon-2.1.3/joatmon/algoritm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/algoritm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.428582 joatmon-2.1.3/joatmon/algoritm/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/algoritm/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/algoritm/search/bfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/algoritm/search/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/algoritm/search/dfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/algoritm/search/linear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.428582 joatmon-2.1.3/joatmon/algoritm/sort/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/algoritm/sort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.428582 joatmon-2.1.3/joatmon/algoritm/traverse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/algoritm/traverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/algoritm/traverse/inorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/algoritm/traverse/postorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/algoritm/traverse/preorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.428582 joatmon-2.1.3/joatmon/array/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/array/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/array/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23501 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/array/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/array/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.428582 joatmon-2.1.3/joatmon/assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13596 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.432582 joatmon-2.1.3/joatmon/assistant/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/agenda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/cd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/cwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/greeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/mkdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/move.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/say.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/todo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/core/weather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/stt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/assistant/tts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.436582 joatmon-2.1.3/joatmon/decorator/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/decorator/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/decorator/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/decorator/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/decorator/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/decorator/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/decorator/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/decorator/otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/decorator/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/decorator/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/decorator/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.436582 joatmon-2.1.3/joatmon/game/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.416582 joatmon-2.1.3/joatmon/game/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.436582 joatmon-2.1.3/joatmon/game/assets/chess/
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/assets/chess/black-bishop.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/assets/chess/black-king.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/assets/chess/black-knight.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/assets/chess/black-pawn.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/assets/chess/black-queen.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/assets/chess/black-rook.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/assets/chess/white-bishop.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/assets/chess/white-king.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/assets/chess/white-knight.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/assets/chess/white-pawn.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/assets/chess/white-queen.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/assets/chess/white-rook.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.416582 joatmon-2.1.3/joatmon/game/assets/sokoban/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.440582 joatmon-2.1.3/joatmon/game/assets/sokoban/sprites/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/assets/sokoban/sprites/block.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/assets/sokoban/sprites/goal.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/assets/sokoban/sprites/obstacle.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/assets/sokoban/sprites/player.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.440582 joatmon-2.1.3/joatmon/game/assets/sokoban/xmls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/assets/sokoban/xmls/default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/assets/sokoban/xmls/medium.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    15196 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/puzzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30825 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/sokoban.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/game/tiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.440582 joatmon-2.1.3/joatmon/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/message/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27913 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/message/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/message/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/message/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/message/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/message/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.440582 joatmon-2.1.3/joatmon/message/mqtt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/message/mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/message/mqtt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33394 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/message/mqtt/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36033 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/message/mqtt/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/message/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/message/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.440582 joatmon-2.1.3/joatmon/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30581 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57625 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.444582 joatmon-2.1.3/joatmon/nn/layer/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/layer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.444582 joatmon-2.1.3/joatmon/nn/layer/activation/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/layer/activation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/layer/activation/relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/layer/activation/sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/layer/activation/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/layer/activation/tanh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/layer/batchnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/layer/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/layer/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/layer/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/layer/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/layer/lstm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.444582 joatmon-2.1.3/joatmon/nn/layer/pool/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/layer/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/layer/pool/avgpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/layer/pool/maxpool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.444582 joatmon-2.1.3/joatmon/nn/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/loss/cce.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/loss/ce.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/loss/mae.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/loss/mse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.444582 joatmon-2.1.3/joatmon/nn/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/optimizer/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/optimizer/rmsprop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.444582 joatmon-2.1.3/joatmon/nn/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/scheduler/exponential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/nn/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/noise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.448582 joatmon-2.1.3/joatmon/orm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/orm/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/orm/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/orm/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/orm/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/orm/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/orm/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17862 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/orm/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/orm/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.448582 joatmon-2.1.3/joatmon/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.448582 joatmon-2.1.3/joatmon/plugin/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/auth/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/auth/jwt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.448582 joatmon-2.1.3/joatmon/plugin/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/cache/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/cache/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.448582 joatmon-2.1.3/joatmon/plugin/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/database/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/database/couchbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/database/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/database/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/database/postgresql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.448582 joatmon-2.1.3/joatmon/plugin/localizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/localizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/localizer/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/localizer/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.456582 joatmon-2.1.3/joatmon/plugin/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/logger/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/logger/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/logger/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/logger/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.456582 joatmon-2.1.3/joatmon/plugin/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/message/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/message/kafka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.456582 joatmon-2.1.3/joatmon/plugin/otp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/otp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/otp/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/otp/otp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/plugin/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.456582 joatmon-2.1.3/joatmon/rdp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/rdp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/rdp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/rdp/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45504 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/rdp/rfb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/serializable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.456582 joatmon-2.1.3/joatmon/structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/structure/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/structure/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.456582 joatmon-2.1.3/joatmon/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.456582 joatmon-2.1.3/joatmon/system/fs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/fs/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/fs/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.464582 joatmon-2.1.3/joatmon/system/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.464582 joatmon-2.1.3/joatmon/system/gui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/gui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/gui/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/gui/widgets/dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/gui/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/gui/widgets/lineedit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/gui/widgets/list_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/gui/widgets/option.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/gui/widgets/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/gui/widgets/scroll_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/gui/widgets/tab_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/gui/widgets/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.464582 joatmon-2.1.3/joatmon/system/hid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/hid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/hid/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/hid/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42766 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/hid/desktop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/hid/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/hid/microphone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/hid/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/hid/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/hid/speaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.464582 joatmon-2.1.3/joatmon/system/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/memory/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/memory/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/memory/locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/memory/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/system/memory/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14369 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-02 21:57:51.000000 joatmon-2.1.3/joatmon/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.420582 joatmon-2.1.3/joatmon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-08-02 21:58:03.000000 joatmon-2.1.3/joatmon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-08-02 21:58:03.000000 joatmon-2.1.3/joatmon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:58:03.000000 joatmon-2.1.3/joatmon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-02 21:58:03.000000 joatmon-2.1.3/joatmon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-02 21:58:03.000000 joatmon-2.1.3/joatmon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-02 21:58:03.000000 joatmon-2.1.3/joatmon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 21:58:03.464582 joatmon-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-08-02 21:57:51.000000 joatmon-2.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:58:03.464582 joatmon-2.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:57:51.000000 joatmon-2.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-02 21:57:51.000000 joatmon-2.1.3/tests/test_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-08-02 21:57:51.000000 joatmon-2.1.3/tests/test_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-02 21:57:51.000000 joatmon-2.1.3/tests/test_version.py
```

### Comparing `joatmon-2.1.2/LICENSE` & `joatmon-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/PKG-INFO` & `joatmon-2.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: joatmon
-Version: 2.1.2
+Version: 2.1.3
 Summary: General Purpose Python Library
 Home-page: https://github.com/malkoch/joatmon
 Download-URL: https://github.com/malkoch/joatmon/tags
 Author: Hamitcan Malkoç
 Author-email: hamitcanmalkoc@gmail.com
 License: MIT
 Keywords: joatmon ml idm automation iva
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.10.1
+Requires-Python: >=3.9.1
 Description-Content-Type: text/markdown
 Provides-Extra: ai
 Provides-Extra: algorithm
 Provides-Extra: assistant
 Provides-Extra: content
 Provides-Extra: core
 Provides-Extra: decorator
```

### Comparing `joatmon-2.1.2/README.md` & `joatmon-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/ai/models/core.py` & `joatmon-2.1.3/joatmon/ai/models/core.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/ai/models/reinforcement/hybrid/ddpg.py` & `joatmon-2.1.3/joatmon/ai/models/reinforcement/hybrid/ddpg.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/ai/models/reinforcement/hybrid/td3.py` & `joatmon-2.1.3/joatmon/ai/models/reinforcement/hybrid/td3.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/ai/models/reinforcement/policy_optimization/ppo.py` & `joatmon-2.1.3/joatmon/ai/models/reinforcement/policy_optimization/ppo.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/ai/models/reinforcement/q_learning/dqn.py` & `joatmon-2.1.3/joatmon/ai/models/reinforcement/q_learning/dqn.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/ai/models/supervised/classification/unet.py` & `joatmon-2.1.3/joatmon/ai/models/supervised/classification/unet.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/ai/network/core.py` & `joatmon-2.1.3/joatmon/ai/network/core.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/ai/network/reinforcement/hybrid/ddpg.py` & `joatmon-2.1.3/joatmon/ai/network/reinforcement/hybrid/ddpg.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/ai/network/reinforcement/hybrid/td3.py` & `joatmon-2.1.3/joatmon/ai/network/reinforcement/hybrid/td3.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/ai/network/reinforcement/policy_optimization/ppo.py` & `joatmon-2.1.3/joatmon/ai/network/reinforcement/policy_optimization/ppo.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/ai/network/reinforcement/q_learning/dqn.py` & `joatmon-2.1.3/joatmon/ai/network/reinforcement/q_learning/dqn.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/ai/network/supervised/classification/unet.py` & `joatmon-2.1.3/joatmon/ai/network/supervised/classification/unet.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/ai/processor.py` & `joatmon-2.1.3/joatmon/ai/processor.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/ai/trainer.py` & `joatmon-2.1.3/joatmon/ai/trainer.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/ai/utility.py` & `joatmon-2.1.3/joatmon/ai/utility.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/algoritm/search/bfs.py` & `joatmon-2.1.3/joatmon/algoritm/search/bfs.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/algoritm/search/binary.py` & `joatmon-2.1.3/joatmon/algoritm/search/binary.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/algoritm/search/dfs.py` & `joatmon-2.1.3/joatmon/algoritm/search/dfs.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/algoritm/traverse/postorder.py` & `joatmon-2.1.3/joatmon/algoritm/traverse/postorder.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/array/__init__.py` & `joatmon-2.1.3/joatmon/array/__init__.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/array/array.py` & `joatmon-2.1.3/joatmon/array/array.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/array/functional.py` & `joatmon-2.1.3/joatmon/array/functional.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/api.py` & `joatmon-2.1.3/joatmon/assistant/api.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/agenda.py` & `joatmon-2.1.3/joatmon/assistant/core/agenda.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/browser.py` & `joatmon-2.1.3/joatmon/assistant/core/browser.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/camera.py` & `joatmon-2.1.3/joatmon/assistant/core/camera.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/cd.py` & `joatmon-2.1.3/joatmon/assistant/core/cd.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/clock.py` & `joatmon-2.1.3/joatmon/assistant/core/clock.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/config.py` & `joatmon-2.1.3/joatmon/assistant/core/config.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/contact.py` & `joatmon-2.1.3/joatmon/assistant/core/contact.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/create.py` & `joatmon-2.1.3/joatmon/assistant/core/create.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/cwd.py` & `joatmon-2.1.3/joatmon/assistant/core/cwd.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/download.py` & `joatmon-2.1.3/joatmon/assistant/core/download.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/exchange.py` & `joatmon-2.1.3/joatmon/assistant/core/exchange.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/greeter.py` & `joatmon-2.1.3/joatmon/assistant/core/greeter.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/help.py` & `joatmon-2.1.3/joatmon/assistant/core/help.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/ls.py` & `joatmon-2.1.3/joatmon/assistant/core/ls.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/mail.py` & `joatmon-2.1.3/joatmon/assistant/core/mail.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/mkdir.py` & `joatmon-2.1.3/joatmon/assistant/core/mkdir.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/move.py` & `joatmon-2.1.3/joatmon/assistant/core/move.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/note.py` & `joatmon-2.1.3/joatmon/assistant/core/note.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/notification.py` & `joatmon-2.1.3/joatmon/assistant/core/notification.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/rm.py` & `joatmon-2.1.3/joatmon/assistant/core/rm.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/run.py` & `joatmon-2.1.3/joatmon/assistant/core/run.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/save.py` & `joatmon-2.1.3/joatmon/assistant/core/save.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/say.py` & `joatmon-2.1.3/joatmon/assistant/core/say.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/search.py` & `joatmon-2.1.3/joatmon/assistant/core/search.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/system.py` & `joatmon-2.1.3/joatmon/assistant/core/system.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/todo.py` & `joatmon-2.1.3/joatmon/assistant/core/todo.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/translate.py` & `joatmon-2.1.3/joatmon/assistant/core/translate.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/viewer.py` & `joatmon-2.1.3/joatmon/assistant/core/viewer.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/core/weather.py` & `joatmon-2.1.3/joatmon/assistant/core/weather.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/intent.py` & `joatmon-2.1.3/joatmon/assistant/intent.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/service.py` & `joatmon-2.1.3/joatmon/assistant/service.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/stt.py` & `joatmon-2.1.3/joatmon/assistant/stt.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/task.py` & `joatmon-2.1.3/joatmon/assistant/task.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/assistant/tts.py` & `joatmon-2.1.3/joatmon/assistant/tts.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/callback.py` & `joatmon-2.1.3/joatmon/callback.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/decorator/auth.py` & `joatmon-2.1.3/joatmon/decorator/auth.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/decorator/cache.py` & `joatmon-2.1.3/joatmon/decorator/cache.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/decorator/database.py` & `joatmon-2.1.3/joatmon/decorator/database.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/decorator/logger.py` & `joatmon-2.1.3/joatmon/decorator/logger.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/decorator/message.py` & `joatmon-2.1.3/joatmon/decorator/message.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/decorator/otp.py` & `joatmon-2.1.3/joatmon/decorator/otp.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/decorator/version.py` & `joatmon-2.1.3/joatmon/decorator/version.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/decorator/web.py` & `joatmon-2.1.3/joatmon/decorator/web.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/download.py` & `joatmon-2.1.3/joatmon/download.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/event.py` & `joatmon-2.1.3/joatmon/event.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/assets/chess/black-bishop.png` & `joatmon-2.1.3/joatmon/game/assets/chess/black-bishop.png`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/assets/chess/black-king.png` & `joatmon-2.1.3/joatmon/game/assets/chess/black-king.png`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/assets/chess/black-knight.png` & `joatmon-2.1.3/joatmon/game/assets/chess/black-knight.png`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/assets/chess/black-pawn.png` & `joatmon-2.1.3/joatmon/game/assets/chess/black-pawn.png`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/assets/chess/black-queen.png` & `joatmon-2.1.3/joatmon/game/assets/chess/black-queen.png`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/assets/chess/black-rook.png` & `joatmon-2.1.3/joatmon/game/assets/chess/black-rook.png`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/assets/chess/white-bishop.png` & `joatmon-2.1.3/joatmon/game/assets/chess/white-bishop.png`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/assets/chess/white-king.png` & `joatmon-2.1.3/joatmon/game/assets/chess/white-king.png`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/assets/chess/white-knight.png` & `joatmon-2.1.3/joatmon/game/assets/chess/white-knight.png`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/assets/chess/white-pawn.png` & `joatmon-2.1.3/joatmon/game/assets/chess/white-pawn.png`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/assets/chess/white-queen.png` & `joatmon-2.1.3/joatmon/game/assets/chess/white-queen.png`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/assets/chess/white-rook.png` & `joatmon-2.1.3/joatmon/game/assets/chess/white-rook.png`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/assets/sokoban/sprites/block.png` & `joatmon-2.1.3/joatmon/game/assets/sokoban/sprites/block.png`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/assets/sokoban/sprites/goal.png` & `joatmon-2.1.3/joatmon/game/assets/sokoban/sprites/goal.png`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/assets/sokoban/sprites/obstacle.png` & `joatmon-2.1.3/joatmon/game/assets/sokoban/sprites/obstacle.png`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/assets/sokoban/sprites/player.png` & `joatmon-2.1.3/joatmon/game/assets/sokoban/sprites/player.png`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/assets/sokoban/xmls/default.xml` & `joatmon-2.1.3/joatmon/game/assets/sokoban/xmls/default.xml`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/assets/sokoban/xmls/medium.xml` & `joatmon-2.1.3/joatmon/game/assets/sokoban/xmls/medium.xml`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/chess.py` & `joatmon-2.1.3/joatmon/game/chess.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/core.py` & `joatmon-2.1.3/joatmon/game/core.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/cube.py` & `joatmon-2.1.3/joatmon/game/cube.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/puzzle.py` & `joatmon-2.1.3/joatmon/game/puzzle.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/sokoban.py` & `joatmon-2.1.3/joatmon/game/sokoban.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/game/tiles.py` & `joatmon-2.1.3/joatmon/game/tiles.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/image.py` & `joatmon-2.1.3/joatmon/image.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/memory.py` & `joatmon-2.1.3/joatmon/memory.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/message/adapters.py` & `joatmon-2.1.3/joatmon/message/adapters.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/message/broker.py` & `joatmon-2.1.3/joatmon/message/broker.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/message/client.py` & `joatmon-2.1.3/joatmon/message/client.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/message/codecs.py` & `joatmon-2.1.3/joatmon/message/codecs.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/message/mqtt/__init__.py` & `joatmon-2.1.3/joatmon/message/mqtt/__init__.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/message/mqtt/handler.py` & `joatmon-2.1.3/joatmon/message/mqtt/handler.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/message/mqtt/packet.py` & `joatmon-2.1.3/joatmon/message/mqtt/packet.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/message/session.py` & `joatmon-2.1.3/joatmon/message/session.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/message/utils.py` & `joatmon-2.1.3/joatmon/message/utils.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/nn/__init__.py` & `joatmon-2.1.3/joatmon/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/nn/core.py` & `joatmon-2.1.3/joatmon/nn/core.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/nn/functional.py` & `joatmon-2.1.3/joatmon/nn/functional.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/nn/layer/batchnorm.py` & `joatmon-2.1.3/joatmon/nn/layer/batchnorm.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/nn/layer/conv.py` & `joatmon-2.1.3/joatmon/nn/layer/conv.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/nn/layer/linear.py` & `joatmon-2.1.3/joatmon/nn/layer/linear.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/nn/layer/lstm.py` & `joatmon-2.1.3/joatmon/nn/layer/lstm.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/nn/optimizer/adam.py` & `joatmon-2.1.3/joatmon/nn/optimizer/adam.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/nn/optimizer/rmsprop.py` & `joatmon-2.1.3/joatmon/nn/optimizer/rmsprop.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/nn/scheduler/exponential.py` & `joatmon-2.1.3/joatmon/nn/scheduler/exponential.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/nn/utility.py` & `joatmon-2.1.3/joatmon/nn/utility.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/noise.py` & `joatmon-2.1.3/joatmon/noise.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/orm/constraint.py` & `joatmon-2.1.3/joatmon/orm/constraint.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/orm/document.py` & `joatmon-2.1.3/joatmon/orm/document.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/orm/enum.py` & `joatmon-2.1.3/joatmon/orm/enum.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/orm/field.py` & `joatmon-2.1.3/joatmon/orm/field.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/orm/meta.py` & `joatmon-2.1.3/joatmon/orm/meta.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/orm/query.py` & `joatmon-2.1.3/joatmon/orm/query.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/orm/relation.py` & `joatmon-2.1.3/joatmon/orm/relation.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/plugin/auth/jwt.py` & `joatmon-2.1.3/joatmon/plugin/auth/jwt.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/plugin/cache/redis.py` & `joatmon-2.1.3/joatmon/plugin/cache/redis.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/plugin/core.py` & `joatmon-2.1.3/joatmon/plugin/core.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/plugin/database/core.py` & `joatmon-2.1.3/joatmon/plugin/database/core.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/plugin/database/couchbase.py` & `joatmon-2.1.3/joatmon/plugin/database/couchbase.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/plugin/database/elastic.py` & `joatmon-2.1.3/joatmon/plugin/database/elastic.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/plugin/database/mongo.py` & `joatmon-2.1.3/joatmon/plugin/database/mongo.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/plugin/database/postgresql.py` & `joatmon-2.1.3/joatmon/plugin/database/postgresql.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/plugin/localizer/database.py` & `joatmon-2.1.3/joatmon/plugin/localizer/database.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/plugin/logger/core.py` & `joatmon-2.1.3/joatmon/plugin/logger/core.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/plugin/logger/file.py` & `joatmon-2.1.3/joatmon/plugin/logger/file.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/plugin/message/kafka.py` & `joatmon-2.1.3/joatmon/plugin/message/kafka.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/plugin/web.py` & `joatmon-2.1.3/joatmon/plugin/web.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/policy.py` & `joatmon-2.1.3/joatmon/policy.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/random.py` & `joatmon-2.1.3/joatmon/random.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/rdp/client.py` & `joatmon-2.1.3/joatmon/rdp/client.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/rdp/rfb.py` & `joatmon-2.1.3/joatmon/rdp/rfb.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/search.py` & `joatmon-2.1.3/joatmon/search.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/serializable.py` & `joatmon-2.1.3/joatmon/serializable.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/system/fs/path.py` & `joatmon-2.1.3/joatmon/system/fs/path.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/system/gui/widgets/button.py` & `joatmon-2.1.3/joatmon/system/gui/widgets/button.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/system/gui/widgets/dropdown.py` & `joatmon-2.1.3/joatmon/system/gui/widgets/dropdown.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/system/gui/widgets/label.py` & `joatmon-2.1.3/joatmon/system/gui/widgets/label.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/system/gui/widgets/lineedit.py` & `joatmon-2.1.3/joatmon/system/gui/widgets/lineedit.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/system/gui/widgets/list_view.py` & `joatmon-2.1.3/joatmon/system/gui/widgets/list_view.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/system/gui/widgets/option.py` & `joatmon-2.1.3/joatmon/system/gui/widgets/option.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/system/gui/widgets/scroll_view.py` & `joatmon-2.1.3/joatmon/system/gui/widgets/scroll_view.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/system/gui/widgets/tab_view.py` & `joatmon-2.1.3/joatmon/system/gui/widgets/tab_view.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/system/gui/widgets/widget.py` & `joatmon-2.1.3/joatmon/system/gui/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/system/hid/camera.py` & `joatmon-2.1.3/joatmon/system/hid/camera.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/system/hid/desktop.py` & `joatmon-2.1.3/joatmon/system/hid/desktop.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/system/hid/keyboard.py` & `joatmon-2.1.3/joatmon/system/hid/keyboard.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/system/hid/microphone.py` & `joatmon-2.1.3/joatmon/system/hid/microphone.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/system/hid/mouse.py` & `joatmon-2.1.3/joatmon/system/hid/mouse.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/system/hid/screen.py` & `joatmon-2.1.3/joatmon/system/hid/screen.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/system/lock.py` & `joatmon-2.1.3/joatmon/system/lock.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/system/memory/address.py` & `joatmon-2.1.3/joatmon/system/memory/address.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/system/memory/core.py` & `joatmon-2.1.3/joatmon/system/memory/core.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/system/memory/locator.py` & `joatmon-2.1.3/joatmon/system/memory/locator.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/system/memory/process.py` & `joatmon-2.1.3/joatmon/system/memory/process.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/system/memory/worker.py` & `joatmon-2.1.3/joatmon/system/memory/worker.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/utility.py` & `joatmon-2.1.3/joatmon/utility.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon/version.py` & `joatmon-2.1.3/joatmon/version.py`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon.egg-info/PKG-INFO` & `joatmon-2.1.3/joatmon.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: joatmon
-Version: 2.1.2
+Version: 2.1.3
 Summary: General Purpose Python Library
 Home-page: https://github.com/malkoch/joatmon
 Download-URL: https://github.com/malkoch/joatmon/tags
 Author: Hamitcan Malkoç
 Author-email: hamitcanmalkoc@gmail.com
 License: MIT
 Keywords: joatmon ml idm automation iva
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.10.1
+Requires-Python: >=3.9.1
 Description-Content-Type: text/markdown
 Provides-Extra: ai
 Provides-Extra: algorithm
 Provides-Extra: assistant
 Provides-Extra: content
 Provides-Extra: core
 Provides-Extra: decorator
```

### Comparing `joatmon-2.1.2/joatmon.egg-info/SOURCES.txt` & `joatmon-2.1.3/joatmon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joatmon-2.1.2/joatmon.egg-info/requires.txt` & `joatmon-2.1.3/joatmon.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -5,45 +5,45 @@
 matplotlib
 six
 Pillow
 
 [algorithm]
 
 [all]
+matplotlib
+colorama
 pyotp
-psutil
-numpy
-opencv-contrib-python
-elevenlabs
+pymunk
+elasticsearch
+pykafka
 pymongo
-psycopg2
+elevenlabs
+Pillow
 gym
-colorama
-pykafka
-feedparser
-six
-pygame
-pyttsx3
-elasticsearch
-transitions
-nltk
-async_exit_stack
+psycopg2
+openai
 torch
 pyjwt
-pycurl
+couchbase
 schedule
+six
+pycurl
 whisper
-redis
-pymunk
-couchbase
+pyttsx3
+psutil
 requests
-matplotlib
-Pillow
-openai
+feedparser
+pygame
+numpy
+async_exit_stack
+redis
+nltk
 tensorflow
+transitions
+opencv-contrib-python
 
 [assistant]
 feedparser
 requests
 colorama
 schedule
 psutil
```

### Comparing `joatmon-2.1.2/setup.py` & `joatmon-2.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 if sys.version_info < (3,):
     print("Python 2 has reached end-of-life and is no longer supported by joatmon.")
     sys.exit(-1)
 if sys.platform == 'win32' and sys.maxsize.bit_length() == 31:
     print("32-bit Windows Python runtime is not supported. Please switch to 64-bit Python.")
     sys.exit(-1)
 
-python_min_version = (3, 10, 1)
+python_min_version = (3, 9, 1)
 python_min_version_str = '.'.join(map(str, python_min_version))
 if sys.version_info < python_min_version:
     print("You are using Python {}. Python >={} is required.".format(platform.python_version(), python_min_version_str))
     sys.exit(-1)
 
 if __name__ == '__main__':
     with open(os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"), encoding="utf-8") as f:
```

### Comparing `joatmon-2.1.2/tests/test_utility.py` & `joatmon-2.1.3/tests/test_utility.py`

 * *Files identical despite different names*

