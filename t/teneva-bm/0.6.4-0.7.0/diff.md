# Comparing `tmp/teneva_bm-0.6.4.tar.gz` & `tmp/teneva_bm-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teneva_bm-0.6.4.tar", last modified: Mon Jul 31 14:44:45 2023, max compression
+gzip compressed data, was "teneva_bm-0.7.0.tar", last modified: Wed Aug  2 12:48:14 2023, max compression
```

## Comparing `teneva_bm-0.6.4.tar` & `teneva_bm-0.7.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-31 14:44:45.556486 teneva_bm-0.6.4/
--rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:29:59.000000 teneva_bm-0.6.4/LICENSE.txt
--rw-r--r--   0 andrei     (501) staff       (20)       79 2023-07-27 07:17:23.000000 teneva_bm-0.6.4/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)    19920 2023-07-31 14:44:45.556671 teneva_bm-0.6.4/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)    18659 2023-07-31 14:43:15.000000 teneva_bm-0.6.4/README.md
--rw-r--r--   0 andrei     (501) staff       (20)      899 2023-07-29 14:29:03.000000 teneva_bm-0.6.4/demo.py
--rw-r--r--   0 andrei     (501) staff       (20)       33 2023-07-29 13:15:53.000000 teneva_bm-0.6.4/requirements.txt
--rw-r--r--   0 andrei     (501) staff       (20)      107 2023-07-31 14:44:45.557290 teneva_bm-0.6.4/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2518 2023-07-16 14:04:06.000000 teneva_bm-0.6.4/setup.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-31 14:44:45.519719 teneva_bm-0.6.4/teneva_bm/
--rw-r--r--   0 andrei     (501) staff       (20)      211 2023-07-31 14:43:21.000000 teneva_bm-0.6.4/teneva_bm/__init__.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-31 14:44:45.529361 teneva_bm-0.6.4/teneva_bm/agent/
--rw-r--r--   0 andrei     (501) staff       (20)      319 2023-07-30 16:47:21.000000 teneva_bm-0.6.4/teneva_bm/agent/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     7694 2023-07-31 14:37:55.000000 teneva_bm-0.6.4/teneva_bm/agent/agent.py
--rw-r--r--   0 andrei     (501) staff       (20)     2076 2023-07-30 16:06:42.000000 teneva_bm-0.6.4/teneva_bm/agent/bm_agent_ant.py
--rw-r--r--   0 andrei     (501) staff       (20)     2092 2023-07-30 15:54:04.000000 teneva_bm-0.6.4/teneva_bm/agent/bm_agent_human.py
--rw-r--r--   0 andrei     (501) staff       (20)     2139 2023-07-30 15:53:56.000000 teneva_bm-0.6.4/teneva_bm/agent/bm_agent_human_stand.py
--rw-r--r--   0 andrei     (501) staff       (20)     6926 2023-07-30 19:52:28.000000 teneva_bm-0.6.4/teneva_bm/agent/bm_agent_lake.py
--rw-r--r--   0 andrei     (501) staff       (20)     2136 2023-07-30 16:47:47.000000 teneva_bm-0.6.4/teneva_bm/agent/bm_agent_pend_inv.py
--rw-r--r--   0 andrei     (501) staff       (20)     2185 2023-07-30 16:47:42.000000 teneva_bm-0.6.4/teneva_bm/agent/bm_agent_pend_inv_double.py
--rw-r--r--   0 andrei     (501) staff       (20)     2288 2023-07-30 15:24:14.000000 teneva_bm-0.6.4/teneva_bm/agent/bm_agent_swimmer.py
--rw-r--r--   0 andrei     (501) staff       (20)     3323 2023-07-30 15:46:50.000000 teneva_bm-0.6.4/teneva_bm/agent/policy.py
--rw-r--r--   0 andrei     (501) staff       (20)    35278 2023-07-31 14:36:37.000000 teneva_bm-0.6.4/teneva_bm/bm.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-31 14:44:45.537690 teneva_bm-0.6.4/teneva_bm/func/
--rw-r--r--   0 andrei     (501) staff       (20)      516 2023-07-13 07:42:30.000000 teneva_bm-0.6.4/teneva_bm/func/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     3548 2023-07-30 10:47:49.000000 teneva_bm-0.6.4/teneva_bm/func/bm_func_ackley.py
--rw-r--r--   0 andrei     (501) staff       (20)     2301 2023-07-30 10:08:14.000000 teneva_bm-0.6.4/teneva_bm/func/bm_func_alpine.py
--rw-r--r--   0 andrei     (501) staff       (20)     2430 2023-07-30 10:52:13.000000 teneva_bm-0.6.4/teneva_bm/func/bm_func_dixon.py
--rw-r--r--   0 andrei     (501) staff       (20)     2295 2023-07-30 10:52:30.000000 teneva_bm-0.6.4/teneva_bm/func/bm_func_exp.py
--rw-r--r--   0 andrei     (501) staff       (20)     2746 2023-07-30 10:13:15.000000 teneva_bm-0.6.4/teneva_bm/func/bm_func_griewank.py
--rw-r--r--   0 andrei     (501) staff       (20)     3590 2023-07-30 10:53:24.000000 teneva_bm-0.6.4/teneva_bm/func/bm_func_michalewicz.py
--rw-r--r--   0 andrei     (501) staff       (20)     2421 2023-07-30 10:17:40.000000 teneva_bm-0.6.4/teneva_bm/func/bm_func_piston.py
--rw-r--r--   0 andrei     (501) staff       (20)     2478 2023-07-30 10:55:11.000000 teneva_bm-0.6.4/teneva_bm/func/bm_func_qing.py
--rw-r--r--   0 andrei     (501) staff       (20)     3091 2023-07-30 10:19:45.000000 teneva_bm-0.6.4/teneva_bm/func/bm_func_rastrigin.py
--rw-r--r--   0 andrei     (501) staff       (20)     3155 2023-07-30 10:56:44.000000 teneva_bm-0.6.4/teneva_bm/func/bm_func_rosenbrock.py
--rw-r--r--   0 andrei     (501) staff       (20)     2129 2023-07-30 10:56:51.000000 teneva_bm-0.6.4/teneva_bm/func/bm_func_schaffer.py
--rw-r--r--   0 andrei     (501) staff       (20)     3132 2023-07-30 10:22:30.000000 teneva_bm-0.6.4/teneva_bm/func/bm_func_schwefel.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-31 14:44:45.539760 teneva_bm-0.6.4/teneva_bm/hs/
--rw-r--r--   0 andrei     (501) staff       (20)       78 2023-07-17 21:02:17.000000 teneva_bm-0.6.4/teneva_bm/hs/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     1755 2023-07-30 11:13:53.000000 teneva_bm-0.6.4/teneva_bm/hs/bm_hs_func001.py
--rw-r--r--   0 andrei     (501) staff       (20)     2430 2023-07-30 11:26:02.000000 teneva_bm-0.6.4/teneva_bm/hs/bm_hs_func006.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-31 14:44:45.544368 teneva_bm-0.6.4/teneva_bm/hs/draft_constrained_functions/
--rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.6.4/teneva_bm/hs/draft_constrained_functions/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     2272 2023-07-17 20:25:36.000000 teneva_bm-0.6.4/teneva_bm/hs/draft_constrained_functions/bm_hs007.py
--rw-r--r--   0 andrei     (501) staff       (20)     2459 2023-07-17 20:25:36.000000 teneva_bm-0.6.4/teneva_bm/hs/draft_constrained_functions/bm_hs008.py
--rw-r--r--   0 andrei     (501) staff       (20)     2318 2023-07-17 20:25:36.000000 teneva_bm-0.6.4/teneva_bm/hs/draft_constrained_functions/bm_hs009.py
--rw-r--r--   0 andrei     (501) staff       (20)     2266 2023-07-17 20:25:36.000000 teneva_bm-0.6.4/teneva_bm/hs/draft_constrained_functions/bm_hs010.py
--rw-r--r--   0 andrei     (501) staff       (20)     2251 2023-07-17 20:25:36.000000 teneva_bm-0.6.4/teneva_bm/hs/draft_constrained_functions/bm_hs011.py
--rw-r--r--   0 andrei     (501) staff       (20)     2376 2023-07-17 20:25:36.000000 teneva_bm-0.6.4/teneva_bm/hs/draft_constrained_functions/bm_hs012.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-31 14:44:45.548661 teneva_bm-0.6.4/teneva_bm/hs/draft_unconstrained_functions/
--rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.6.4/teneva_bm/hs/draft_unconstrained_functions/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     1937 2023-07-17 20:25:36.000000 teneva_bm-0.6.4/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py
--rw-r--r--   0 andrei     (501) staff       (20)     1857 2023-07-17 20:25:36.000000 teneva_bm-0.6.4/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py
--rw-r--r--   0 andrei     (501) staff       (20)     1839 2023-07-17 20:25:36.000000 teneva_bm-0.6.4/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py
--rw-r--r--   0 andrei     (501) staff       (20)     2197 2023-07-17 20:25:36.000000 teneva_bm-0.6.4/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py
--rw-r--r--   0 andrei     (501) staff       (20)     2275 2023-07-17 20:25:36.000000 teneva_bm-0.6.4/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py
--rw-r--r--   0 andrei     (501) staff       (20)     1929 2023-07-17 20:25:36.000000 teneva_bm-0.6.4/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-31 14:44:45.550497 teneva_bm-0.6.4/teneva_bm/odeoc/
--rw-r--r--   0 andrei     (501) staff       (20)       99 2023-07-30 11:32:37.000000 teneva_bm-0.6.4/teneva_bm/odeoc/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     4237 2023-07-30 11:37:21.000000 teneva_bm-0.6.4/teneva_bm/odeoc/bm_odeoc_simple.py
--rw-r--r--   0 andrei     (501) staff       (20)     2292 2023-07-30 11:37:44.000000 teneva_bm-0.6.4/teneva_bm/odeoc/bm_odeoc_simple_constr.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-31 14:44:45.554396 teneva_bm-0.6.4/teneva_bm/qubo/
--rw-r--r--   0 andrei     (501) staff       (20)      166 2023-07-22 15:44:37.000000 teneva_bm-0.6.4/teneva_bm/qubo/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     7111 2023-07-30 11:04:30.000000 teneva_bm-0.6.4/teneva_bm/qubo/bm_qubo_knap_det.py
--rw-r--r--   0 andrei     (501) staff       (20)     1834 2023-07-30 11:06:13.000000 teneva_bm-0.6.4/teneva_bm/qubo/bm_qubo_knap_quad.py
--rw-r--r--   0 andrei     (501) staff       (20)     2967 2023-07-30 11:07:28.000000 teneva_bm-0.6.4/teneva_bm/qubo/bm_qubo_maxcut.py
--rw-r--r--   0 andrei     (501) staff       (20)     2973 2023-07-30 11:08:28.000000 teneva_bm-0.6.4/teneva_bm/qubo/bm_qubo_mvc.py
--rw-r--r--   0 andrei     (501) staff       (20)     3377 2023-07-29 14:31:04.000000 teneva_bm-0.6.4/teneva_bm/teneva_bm_demo.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-31 14:44:45.556186 teneva_bm-0.6.4/teneva_bm/various/
--rw-r--r--   0 andrei     (501) staff       (20)      105 2023-07-13 07:41:21.000000 teneva_bm-0.6.4/teneva_bm/various/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     7790 2023-07-30 11:28:44.000000 teneva_bm-0.6.4/teneva_bm/various/bm_matmul.py
--rw-r--r--   0 andrei     (501) staff       (20)    12705 2023-07-31 14:37:05.000000 teneva_bm-0.6.4/teneva_bm/various/bm_topopt.py
--rw-r--r--   0 andrei     (501) staff       (20)     1867 2023-07-30 11:18:40.000000 teneva_bm-0.6.4/teneva_bm/various/bm_wall_simple.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-31 14:44:45.522645 teneva_bm-0.6.4/teneva_bm.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)    19920 2023-07-31 14:44:45.000000 teneva_bm-0.6.4/teneva_bm.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     2312 2023-07-31 14:44:45.000000 teneva_bm-0.6.4/teneva_bm.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2023-07-31 14:44:45.000000 teneva_bm-0.6.4/teneva_bm.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)       33 2023-07-31 14:44:45.000000 teneva_bm-0.6.4/teneva_bm.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)       10 2023-07-31 14:44:45.000000 teneva_bm-0.6.4/teneva_bm.egg-info/top_level.txt
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 12:48:14.985127 teneva_bm-0.7.0/
+-rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:29:59.000000 teneva_bm-0.7.0/LICENSE.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       79 2023-07-27 07:17:23.000000 teneva_bm-0.7.0/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)    19920 2023-08-02 12:48:14.985303 teneva_bm-0.7.0/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)    18659 2023-08-02 12:47:38.000000 teneva_bm-0.7.0/README.md
+-rw-r--r--   0 andrei     (501) staff       (20)      899 2023-07-29 14:29:03.000000 teneva_bm-0.7.0/demo.py
+-rw-r--r--   0 andrei     (501) staff       (20)       33 2023-07-29 13:15:53.000000 teneva_bm-0.7.0/requirements.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      107 2023-08-02 12:48:14.986067 teneva_bm-0.7.0/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2518 2023-07-16 14:04:06.000000 teneva_bm-0.7.0/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 12:48:14.959105 teneva_bm-0.7.0/teneva_bm/
+-rw-r--r--   0 andrei     (501) staff       (20)      211 2023-08-02 12:47:31.000000 teneva_bm-0.7.0/teneva_bm/__init__.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 12:48:14.966175 teneva_bm-0.7.0/teneva_bm/agent/
+-rw-r--r--   0 andrei     (501) staff       (20)      319 2023-07-30 16:47:21.000000 teneva_bm-0.7.0/teneva_bm/agent/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7561 2023-08-02 11:35:35.000000 teneva_bm-0.7.0/teneva_bm/agent/agent.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2076 2023-07-30 16:06:42.000000 teneva_bm-0.7.0/teneva_bm/agent/bm_agent_ant.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2092 2023-07-30 15:54:04.000000 teneva_bm-0.7.0/teneva_bm/agent/bm_agent_human.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2139 2023-07-30 15:53:56.000000 teneva_bm-0.7.0/teneva_bm/agent/bm_agent_human_stand.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7432 2023-08-02 12:46:42.000000 teneva_bm-0.7.0/teneva_bm/agent/bm_agent_lake.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2136 2023-07-30 16:47:47.000000 teneva_bm-0.7.0/teneva_bm/agent/bm_agent_pend_inv.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2185 2023-07-30 16:47:42.000000 teneva_bm-0.7.0/teneva_bm/agent/bm_agent_pend_inv_double.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2288 2023-07-30 15:24:14.000000 teneva_bm-0.7.0/teneva_bm/agent/bm_agent_swimmer.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3323 2023-07-30 15:46:50.000000 teneva_bm-0.7.0/teneva_bm/agent/policy.py
+-rw-r--r--   0 andrei     (501) staff       (20)    35306 2023-08-02 12:05:32.000000 teneva_bm-0.7.0/teneva_bm/bm.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 12:48:14.971235 teneva_bm-0.7.0/teneva_bm/func/
+-rw-r--r--   0 andrei     (501) staff       (20)      516 2023-07-13 07:42:30.000000 teneva_bm-0.7.0/teneva_bm/func/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3641 2023-08-02 10:12:25.000000 teneva_bm-0.7.0/teneva_bm/func/bm_func_ackley.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2301 2023-07-30 10:08:14.000000 teneva_bm-0.7.0/teneva_bm/func/bm_func_alpine.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2430 2023-07-30 10:52:13.000000 teneva_bm-0.7.0/teneva_bm/func/bm_func_dixon.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2295 2023-07-30 10:52:30.000000 teneva_bm-0.7.0/teneva_bm/func/bm_func_exp.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2746 2023-07-30 10:13:15.000000 teneva_bm-0.7.0/teneva_bm/func/bm_func_griewank.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3623 2023-08-02 10:10:43.000000 teneva_bm-0.7.0/teneva_bm/func/bm_func_michalewicz.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2421 2023-07-30 10:17:40.000000 teneva_bm-0.7.0/teneva_bm/func/bm_func_piston.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2478 2023-07-30 10:55:11.000000 teneva_bm-0.7.0/teneva_bm/func/bm_func_qing.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3130 2023-08-02 10:10:09.000000 teneva_bm-0.7.0/teneva_bm/func/bm_func_rastrigin.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3155 2023-07-30 10:56:44.000000 teneva_bm-0.7.0/teneva_bm/func/bm_func_rosenbrock.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2129 2023-07-30 10:56:51.000000 teneva_bm-0.7.0/teneva_bm/func/bm_func_schaffer.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3165 2023-08-02 10:10:07.000000 teneva_bm-0.7.0/teneva_bm/func/bm_func_schwefel.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 12:48:14.972640 teneva_bm-0.7.0/teneva_bm/hs/
+-rw-r--r--   0 andrei     (501) staff       (20)       78 2023-07-17 21:02:17.000000 teneva_bm-0.7.0/teneva_bm/hs/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1755 2023-07-30 11:13:53.000000 teneva_bm-0.7.0/teneva_bm/hs/bm_hs_func001.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2430 2023-07-30 11:26:02.000000 teneva_bm-0.7.0/teneva_bm/hs/bm_hs_func006.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 12:48:14.976111 teneva_bm-0.7.0/teneva_bm/hs/draft_constrained_functions/
+-rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.7.0/teneva_bm/hs/draft_constrained_functions/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2272 2023-07-17 20:25:36.000000 teneva_bm-0.7.0/teneva_bm/hs/draft_constrained_functions/bm_hs007.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2459 2023-07-17 20:25:36.000000 teneva_bm-0.7.0/teneva_bm/hs/draft_constrained_functions/bm_hs008.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2318 2023-07-17 20:25:36.000000 teneva_bm-0.7.0/teneva_bm/hs/draft_constrained_functions/bm_hs009.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2266 2023-07-17 20:25:36.000000 teneva_bm-0.7.0/teneva_bm/hs/draft_constrained_functions/bm_hs010.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2251 2023-07-17 20:25:36.000000 teneva_bm-0.7.0/teneva_bm/hs/draft_constrained_functions/bm_hs011.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2376 2023-07-17 20:25:36.000000 teneva_bm-0.7.0/teneva_bm/hs/draft_constrained_functions/bm_hs012.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 12:48:14.979913 teneva_bm-0.7.0/teneva_bm/hs/draft_unconstrained_functions/
+-rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.7.0/teneva_bm/hs/draft_unconstrained_functions/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1937 2023-07-17 20:25:36.000000 teneva_bm-0.7.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1857 2023-07-17 20:25:36.000000 teneva_bm-0.7.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1839 2023-07-17 20:25:36.000000 teneva_bm-0.7.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2197 2023-07-17 20:25:36.000000 teneva_bm-0.7.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2275 2023-07-17 20:25:36.000000 teneva_bm-0.7.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1929 2023-07-17 20:25:36.000000 teneva_bm-0.7.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 12:48:14.981369 teneva_bm-0.7.0/teneva_bm/odeoc/
+-rw-r--r--   0 andrei     (501) staff       (20)       99 2023-07-30 11:32:37.000000 teneva_bm-0.7.0/teneva_bm/odeoc/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     4218 2023-08-02 10:06:50.000000 teneva_bm-0.7.0/teneva_bm/odeoc/bm_odeoc_simple.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2292 2023-07-30 11:37:44.000000 teneva_bm-0.7.0/teneva_bm/odeoc/bm_odeoc_simple_constr.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 12:48:14.983256 teneva_bm-0.7.0/teneva_bm/qubo/
+-rw-r--r--   0 andrei     (501) staff       (20)      166 2023-07-22 15:44:37.000000 teneva_bm-0.7.0/teneva_bm/qubo/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7111 2023-07-30 11:04:30.000000 teneva_bm-0.7.0/teneva_bm/qubo/bm_qubo_knap_det.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1834 2023-07-30 11:06:13.000000 teneva_bm-0.7.0/teneva_bm/qubo/bm_qubo_knap_quad.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2962 2023-08-02 10:05:08.000000 teneva_bm-0.7.0/teneva_bm/qubo/bm_qubo_maxcut.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2968 2023-08-02 10:04:56.000000 teneva_bm-0.7.0/teneva_bm/qubo/bm_qubo_mvc.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3377 2023-07-29 14:31:04.000000 teneva_bm-0.7.0/teneva_bm/teneva_bm_demo.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 12:48:14.984841 teneva_bm-0.7.0/teneva_bm/various/
+-rw-r--r--   0 andrei     (501) staff       (20)      105 2023-07-13 07:41:21.000000 teneva_bm-0.7.0/teneva_bm/various/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7774 2023-08-02 10:24:54.000000 teneva_bm-0.7.0/teneva_bm/various/bm_matmul.py
+-rw-r--r--   0 andrei     (501) staff       (20)    12683 2023-08-02 10:23:16.000000 teneva_bm-0.7.0/teneva_bm/various/bm_topopt.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1867 2023-07-30 11:18:40.000000 teneva_bm-0.7.0/teneva_bm/various/bm_wall_simple.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-02 12:48:14.961707 teneva_bm-0.7.0/teneva_bm.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)    19920 2023-08-02 12:48:14.000000 teneva_bm-0.7.0/teneva_bm.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     2312 2023-08-02 12:48:14.000000 teneva_bm-0.7.0/teneva_bm.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2023-08-02 12:48:14.000000 teneva_bm-0.7.0/teneva_bm.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       33 2023-08-02 12:48:14.000000 teneva_bm-0.7.0/teneva_bm.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       10 2023-08-02 12:48:14.000000 teneva_bm-0.7.0/teneva_bm.egg-info/top_level.txt
```

### Comparing `teneva_bm-0.6.4/LICENSE.txt` & `teneva_bm-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/PKG-INFO` & `teneva_bm-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva_bm
-Version: 0.6.4
+Version: 0.7.0
 Summary: Benchmarks library, based on the software product teneva, for testing multivariate approximation and optimization methods
 Home-page: https://github.com/AndreiChertkov/teneva_bm
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_bm
 Keywords: benchmarks approximation optimization multidimensional array multivariate function low-rank representation tensor train format TT-decomposition
@@ -30,15 +30,15 @@
 ## Description
 
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.6.4".
+> Current version "0.7.0".
 
 The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
 
 > Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.5+) will be automatically installed during the installation of the main software product.
 
 Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following commands:
```

### Comparing `teneva_bm-0.6.4/README.md` & `teneva_bm-0.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ## Description
 
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.6.4".
+> Current version "0.7.0".
 
 The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
 
 > Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.5+) will be automatically installed during the installation of the main software product.
 
 Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following commands:
```

### Comparing `teneva_bm-0.6.4/demo.py` & `teneva_bm-0.7.0/demo.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/setup.py` & `teneva_bm-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/agent/agent.py` & `teneva_bm-0.7.0/teneva_bm/agent/agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,20 +28,20 @@
 
 from teneva_bm import Bm
 from teneva_bm.agent.policy import Policy
 from teneva_bm.agent.policy import PolicyToeplitz
 
 
 class Agent(Bm):
+    frozen_lake = gym_frozen_lake if with_gym else None
+
     def make(name, **args):
         if with_gym:
             return gym.make(name, render_mode='rgb_array', **args)
 
-    frozen_lake = gym_frozen_lake if with_gym else None
-
     def __init__(self, d=None, n=3, name='Agent-abstract-class', desc='',
                  steps=1000, policy='toeplitz'):
         super().__init__(None, None, name, desc)
         self._n_raw = n # We'll set it later in "prep_bm" method
 
         if not with_cv2:
             msg = 'Need "cv2" module. For installation please see README.md'
@@ -51,36 +51,37 @@
             msg = 'Need "gym" module. For installation please see README.md'
             self.set_err(msg)
 
         if d is not None:
             msg = 'Dimension number (d) should not be set manually'
             self.set_err(msg)
 
-        self._steps = steps
+        self.steps = steps
 
         if isinstance(policy, str):
-            self._policy_name = policy
+            self.policy = policy
 
-            if self._policy_name == 'direct':
+            if self.policy == 'direct':
                 self._policy = Policy()
-            elif self._policy_name == 'toeplitz':
+            elif self.policy == 'toeplitz':
                 self._policy = PolicyToeplitz()
             else:
-                raise ValueError('Invalid policy name')
+                msg = f'Policy "{policy}" is not supported'
+                self.set_err(msg)
 
         else:
-            self._policy_name = policy.name
+            self.policy = policy.name
 
             self._policy = policy
 
         self._with_render = False
 
     @property
     def identity(self):
-        return ['_steps', '_policy_name', 'n']
+        return ['steps', 'policy', 'n']
 
     @property
     def is_func(self):
         return True
 
     @property
     def is_opti_max(self):
@@ -136,29 +137,29 @@
 
     @property
     def _state(self):
         return self._states[-1] if len(self._states) else self._state0
 
     def get_config(self):
         conf = super().get_config()
-        conf['_steps'] = self._steps
-        conf['_policy_name'] = self._policy_name
+        conf['steps'] = self.steps
+        conf['policy'] = self.policy
         conf['_d_st'] = self._d_st
         conf['_d_ac'] = self._d_ac
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'Number of agent steps                    : '
-        v = self._steps
+        v = self.steps
         text += f'{v}\n'
 
         text += 'Used policy                              : '
-        v = self._policy_name
+        v = self.policy
         text += f'{v}\n'
 
         text += 'Dimension of state space for agent       : '
         v = self._d_st
         text += f'{v}\n'
 
         text += 'Dimension of action space for agent      : '
@@ -168,29 +169,33 @@
         return super().info(text+footer)
 
     def prep_bm(self, env):
         if env is None:
             raise ValueError('Environment is not set')
         self._env = env
 
-        self._policy.prep(self._steps,
+        self._policy.prep(self.steps,
             self._d_st, self._n_st, self._a_st, self._b_st,
             self._d_ac, self._n_ac, self._a_ac, self._b_ac)
 
         self.set_dimension(self._policy.d)
         self.set_size(self._n_raw)
         if self.is_func:
             self.set_grid(self._policy.a, self._policy.b)
         self._reset()
 
     def render(self, fpath=None, i=None, best=True, fps=20.):
         self._with_render = True
         i, y = self.get_solution(i, best)
         self._with_render = False
 
+        if not len(self._frames):
+            msg = 'Can not save rendered video for agent (empty frames)'
+            self.wrn(msg)
+
         frames = self._frames
         frames = [cv2.cvtColor(frame, cv2.COLOR_RGB2BGR) for frame in frames]
         # frame = cv2.resize(frame,(512, 512))
 
         fpath = self.path_build(fpath, 'mp4')
         fourcc = cv2.VideoWriter_fourcc(*'mp4v')
         out = cv2.VideoWriter(fpath, fourcc, fps, (frames[0].shape[:2]))
@@ -249,44 +254,41 @@
         self._frames = []
         self._rewards = []
         self._states = []
 
     def _run(self):
         self._reset()
 
-        if self._with_render:
+        def _render():
             try:
                 self._frames.append(self._env.render())
             except Exception as e:
                 msg = 'Can not render agent for video generation'
                 msg += f' [Error: {e}]'
                 self.wrn(msg)
                 self._with_render = False
 
-        for step in range(self._steps):
+        if self._with_render:
+            _render()
+
+        for step in range(self.steps):
             self._step = step
 
             state = self._parse_state_policy(self._state)
             action = self._policy(state)
             action = self._parse_action(action)
             self._actions.append(action)
 
-            action_gym = self._parse_action_gym(action)
-            state, reward, self._done = self._env.step(action_gym)[:3]
+            action = self._parse_action_gym(action)
+            state, reward, self._done = self._env.step(action)[:3]
 
             state = self._parse_state(state)
             self._states.append(state)
 
             reward = self._parse_reward(reward)
             self._rewards.append(reward)
 
             if self._with_render:
-                try:
-                    self._frames.append(self._env.render())
-                except Exception as e:
-                    msg = 'Can not render agent for video generation'
-                    msg += f' [Error: {e}]'
-                    self.wrn(msg)
-                    self._with_render = False
+                _render()
 
             if self._done:
                 break
```

### Comparing `teneva_bm-0.6.4/teneva_bm/agent/bm_agent_ant.py` & `teneva_bm-0.7.0/teneva_bm/agent/bm_agent_ant.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/agent/bm_agent_human.py` & `teneva_bm-0.7.0/teneva_bm/agent/bm_agent_human.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/agent/bm_agent_human_stand.py` & `teneva_bm-0.7.0/teneva_bm/agent/bm_agent_human_stand.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/agent/bm_agent_lake.py` & `teneva_bm-0.7.0/teneva_bm/agent/bm_agent_lake.py`

 * *Files 24% similar despite different names*

```diff
@@ -28,43 +28,60 @@
         holes = []
         for i in range(size):
             for j in range(size):
                 if map[i][j] == BmAgentLake.HOLE:
                     holes.append(np.array([i, j], dtype=int))
         return holes
 
-    def map(size=5, prob_hole=0.4, seed=42, iters=1.E+9):
+    def map(size=10, holes=10, seed=42, iters=1.E+4, prob_hole=0.05):
         map = []
         rand = np.random.default_rng(seed) if isinstance(seed, int) else seed
         iter = 0
         while len(map) == 0 or not Agent.frozen_lake.is_valid(map, size):
             iter += 1
             if iter > iters:
-                msg = 'Can not build the map for selected probability'
-                raise ValueError(msg)
+                if prob_hole > 0.9:
+                    msg = 'Can not build the map for selected size / holes'
+                    raise ValueError(msg)
+                return BmAgentLake.map(size, holes, seed, iters, prob_hole+0.1)
 
             map = rand.choice([BmAgentLake.FROZ, BmAgentLake.HOLE],
                 (size, size), p=[1-prob_hole, prob_hole])
             map[0, 0] = BmAgentLake.INIT
             map[-1, -1] = BmAgentLake.GOAL
 
+            if len(BmAgentLake.holes(map)) != holes:
+                map = []
+
         return [''.join(x) for x in map]
 
     def __init__(self, d=None, n=4, name='AgentLake', desc=DESC,
-                 steps=100, policy='direct',
-                 size=5, prob_hole=0.4, with_state_ext=False):
-        super().__init__(d, n, name, desc, steps, policy)
-
-        self._size = size
-        self._prob_hole = prob_hole
-        self._with_state_ext = with_state_ext
+                 policy='direct', size=10, holes=10, with_state_ext=False):
+        super().__init__(d, n, name, desc, size*size, policy)
+
+        self.size = size
+        self.holes = holes
+        self.with_state_ext = with_state_ext
+
+        if isinstance(policy, str):
+            if policy == 'direct':
+                if n != 4:
+                    msg = f'Mode size should be 4 for "direct" policy'
+                    self.set_err(msg)
+            else:
+                msg = f'Policy "{policy}" is not supported'
+                self.set_err(msg)
+
+    @property
+    def identity(self):
+        return ['size', 'holes', 'policy', 'n', 'with_state_ext']
 
     @property
     def is_func(self):
-        return False
+        return False if self.policy == 'direct' else True
 
     @property
     def _a_ac(self):
         return None
 
     @property
     def _a_st(self):
@@ -80,15 +97,15 @@
 
     @property
     def _d_ac(self):
         return 1
 
     @property
     def _d_st(self):
-        if self._with_state_ext:
+        if self.with_state_ext:
             # State includes positions of the holes, goal and agent
             return len(self._holes) * 2 + 2 + 2
         else:
             # State includes only current position of the agent
             return 2
 
     @property
@@ -139,65 +156,61 @@
         elif len(self._states) == 1:
             return self._state0
         else:
             return self._states[-2]
 
     def get_config(self):
         conf = super().get_config()
-        conf['_size'] = self._size
-        conf['_prob_hole'] = self._prob_hole
-        conf['_with_state_ext'] = self._with_state_ext
+        conf['size'] = self.size
+        conf['holes'] = self.holes
+        conf['with_state_ext'] = self.with_state_ext
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'Size of the lake                         : '
-        v = self._size
+        v = self.size
         text += f'{v}x{v}\n'
 
-        text += 'Probability of the hole                  : '
-        v = self._prob_hole
-        text += f'{v}\n'
-
-        text += 'Number of holes                          : '
-        v = len(self._holes)
+        text += 'Number of the holes                      : '
+        v = self.holes
         text += f'{v}\n'
 
         text += 'State is extended                        : '
-        v = 'YES' if self._with_state_ext else 'no'
+        v = 'YES' if self.with_state_ext else 'no'
         text += f'{v}\n'
 
         return super().info(text+footer)
 
     def prep_bm(self, policy=None):
-        self._map = BmAgentLake.map(self._size, self._prob_hole, self.rand)
+        self._map = BmAgentLake.map(self.size, self.holes, self.rand)
         self._holes = BmAgentLake.holes(self._map)
 
         env = Agent.make('FrozenLake-v1', desc=self._map, is_slippery=False)
 
-        self._state_goal = self._discretize(self._size*self._size-1)
+        self._state_goal = self._discretize(self.size*self.size-1)
 
         return super().prep_bm(env)
 
     def render(self, fpath=None, i=None, best=True, fps=5.):
         return super().render(fpath, i, best, fps)
 
     def _discretize(self, state):
-        x, y = (state // self._size, state % self._size)
+        x, y = (state // self.size, state % self.size)
         return np.array([x, y], dtype=int)
 
     def _parse_action_gym(self, action):
         return action[0]
 
     def _parse_state(self, state):
         return self._discretize(state)
 
     def _parse_state_policy(self, state):
-        if not self._with_state_ext:
+        if not self.with_state_ext:
             return state
 
         state_ext = []
         for hole in self._holes:
             state_ext.extend(list(hole))
         state_ext.extend(list(self._state_goal))
         state_ext.extend(list(state))
@@ -225,15 +238,15 @@
     text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
     text = 'Render for "direct" policy               :  '
-    bm = BmAgentLake().prep()
+    bm = BmAgentLake(size=10, holes=50).prep()
     fpath = f'result/{bm.name}/render_direct'
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     bm.render(fpath)
     text += f' see {fpath}'
     print(text)
```

### Comparing `teneva_bm-0.6.4/teneva_bm/agent/bm_agent_pend_inv.py` & `teneva_bm-0.7.0/teneva_bm/agent/bm_agent_pend_inv.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/agent/bm_agent_pend_inv_double.py` & `teneva_bm-0.7.0/teneva_bm/agent/bm_agent_pend_inv_double.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/agent/bm_agent_swimmer.py` & `teneva_bm-0.7.0/teneva_bm/agent/bm_agent_swimmer.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/agent/policy.py` & `teneva_bm-0.7.0/teneva_bm/agent/policy.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/bm.py` & `teneva_bm-0.7.0/teneva_bm/bm.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         if not self.is_n_equal:
             raise ValueError('Mode size is not constant, can`t get n0')
         return self.n[0] if self.n is not None else None
 
     @property
     def time_full(self):
         """Full time of benchmark existence in seconds."""
-        return tpc() - self.time_stamp_start
+        return tpc() - self.timestamp_start
 
     @property
     def with_constr(self):
         """Return True if benchmark has a constraint."""
         return False
 
     @property
@@ -371,15 +371,15 @@
             'i_max': self.list_copy(self.i_max, 'int'),
             'x_max': self.list_copy(self.x_max, 'float'),
             'y_max': self.y_max,
             'i_min': self.list_copy(self.i_min, 'int'),
             'x_min': self.list_copy(self.x_min, 'float'),
             'y_min': self.y_min,
             'y_list': self.list_copy(self.y_list, 'float'),
-            'time': self.time,
+            'time_call': self.time_call,
             'time_full': self.time_full,
             'err': '; '.join(self.err) if len(self.err) else '',
         }
 
         return hist
 
     def get_solution(self, i=None, best=True):
@@ -612,18 +612,18 @@
         text += 'Number of requests                       : '
         text += f'{self.m:-10.3e}\n'
 
         text += 'Number of cache uses                     : '
         text += f'{self.m_cache:-10.3e}\n'
 
         text += 'Average time of one request (sec)        : '
-        text += f'{self.time/self.m:-10.3e}\n'
+        text += f'{self.time_call/self.m:-10.3e}\n'
 
         text += 'Total requests time (sec)                : '
-        text += f'{self.time:-10.3e}\n'
+        text += f'{self.time_call:-10.3e}\n'
 
         text += 'Total work time (sec)                    : '
         text += f'{self.time_full:-10.3e}\n'
 
         if self.y_min is not None and self.y_min_real is not None:
             text += 'Minimum (found / real)                   : '
             text += f'{self.y_min:-10.3e}   / {self.y_min_real:-10.3e}\n'
@@ -668,19 +668,19 @@
         self.x_min = None
         self.y_min = None
 
         self.y_list = []
 
         self.m = 0
         self.m_cache = 0
-        self.time = 0.
 
         self.log_m_last = 0
 
-        self.time_stamp_start = tpc()
+        self.time_call = 0.
+        self.timestamp_start = tpc()
 
         self.cache = {}
 
     def list_convert(self, x, kind='float', eps=1.E-16):
         """Convert list of equal values to one number and back."""
         if x is None:
             return None
@@ -798,15 +798,15 @@
             return y if is_batch else y[0]
 
         self.y_list.extend(list(y))
 
         self.m += y.shape[0] - dm_cache
         self.m_cache += dm_cache
 
-        self.time += tpc() - t
+        self.time_call += tpc() - t
 
         self.i = I[-1, :].copy() if I is not None else None
         self.x = X[-1, :].copy() if X is not None else None
         self.y = y[-1]
 
         ind = np.argmax(y)
         if self.y_max is None or self.y_max < y[ind]:
```

### Comparing `teneva_bm-0.6.4/teneva_bm/func/__init__.py` & `teneva_bm-0.7.0/teneva_bm/func/__init__.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/func/bm_func_ackley.py` & `teneva_bm-0.7.0/teneva_bm/func/bm_func_ackley.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,68 +29,68 @@
 
     @property
     def is_func(self):
         return True
 
     def get_config(self):
         conf = super().get_config()
-        conf['_a'] = self._a
-        conf['_b'] = self._b
-        conf['_c'] = self._c
+        conf['opt_a'] = self.opt_a
+        conf['opt_b'] = self.opt_b
+        conf['opt_c'] = self.opt_c
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'Param a for Ackley function              : '
-        v = self._a
+        v = self.opt_a
         text += f'{v:.6f}\n'
 
         text += 'Param b for Ackley function              : '
-        v = self._b
+        v = self.opt_b
         text += f'{v:.6f}\n'
 
         text += 'Param c for Ackley function              : '
-        v = self._c
+        v = self.opt_c
         text += f'{v:.6f}\n'
 
         return super().info(text+footer)
 
-    def set_opts(self, a=20., b=0.2, c=2.*np.pi):
+    def set_opts(self, opt_a=20., opt_b=0.2, opt_c=2.*np.pi):
         """Set options specific to this benchmark.
 
         There are no plans to manually change the default values.
 
         Args:
-            a (float): parameter of the function.
-            b (float): parameter of the function.
-            c (float): parameter of the function.
+            opt_a (float): parameter of the function.
+            opt_b (float): parameter of the function.
+            opt_c (float): parameter of the function.
 
         """
-        self._a = a
-        self._b = b
-        self._c = c
+        self.opt_a = opt_a
+        self.opt_b = opt_b
+        self.opt_c = opt_c
 
     def target_batch(self, X):
         y1 = np.sqrt(np.sum(X**2, axis=1) / self.d)
-        y1 = -self._a * np.exp(-self._b * y1)
+        y1 = -self.opt_a * np.exp(-self.opt_b * y1)
 
-        y2 = np.sum(np.cos(self._c * X), axis=1)
+        y2 = np.sum(np.cos(self.opt_c * X), axis=1)
         y2 = -np.exp(y2 / self.d)
 
-        y3 = self._a + np.exp(1.)
+        y3 = self.opt_a + np.exp(1.)
 
         return y1 + y2 + y3
 
     def _target_pt(self, x):
         """Draft."""
         d = torch.tensor(self.d)
-        par_a = torch.tensor(self._a)
-        par_b = torch.tensor(self._b)
-        par_c = torch.tensor(self._c)
+        par_a = torch.tensor(self.opt_a)
+        par_b = torch.tensor(self.opt_b)
+        par_c = torch.tensor(self.opt_c)
 
         y1 = torch.sqrt(torch.sum(x**2) / d)
         y1 = - par_a * torch.exp(-par_b * y1)
 
         y2 = torch.sum(torch.cos(par_c * x))
         y2 = - torch.exp(y2 / d)
```

### Comparing `teneva_bm-0.6.4/teneva_bm/func/bm_func_alpine.py` & `teneva_bm-0.7.0/teneva_bm/func/bm_func_alpine.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/func/bm_func_dixon.py` & `teneva_bm-0.7.0/teneva_bm/func/bm_func_dixon.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/func/bm_func_exp.py` & `teneva_bm-0.7.0/teneva_bm/func/bm_func_exp.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/func/bm_func_griewank.py` & `teneva_bm-0.7.0/teneva_bm/func/bm_func_griewank.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/func/bm_func_michalewicz.py` & `teneva_bm-0.7.0/teneva_bm/func/bm_func_michalewicz.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,53 +40,53 @@
 
     @property
     def with_cores(self):
         return True
 
     def get_config(self):
         conf = super().get_config()
-        conf['_m'] = self._m
+        conf['opt_m'] = self.opt_m
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'Param m for Michalewicz function         : '
-        v = self._m
+        v = self.opt_m
         text += f'{v:.6f}\n'
 
         return super().info(text+footer)
 
-    def set_opts(self, m=10.):
+    def set_opts(self, opt_m=10.):
         """Set options specific to this benchmark.
 
         There are no plans to manually change the default values.
 
         Args:
-            m (float): parameter of the function.
+            opt_m (float): parameter of the function.
 
         """
-        self._m = m
+        self.opt_m = opt_m
 
     def cores(self, X):
         Y = self.cores_add(
-            [np.sin(x) * np.sin(i*x**2/np.pi)**(2*self._m)
+            [np.sin(x) * np.sin(i*x**2/np.pi)**(2*self.opt_m)
                 for i, x in enumerate(X.T, 1)])
         Y[-1] *= -1.
         return Y
 
     def target_batch(self, X):
         y1 = np.sin(((np.arange(self.d) + 1) * X**2 / np.pi))
-        y = -np.sum(np.sin(X) * y1**(2 * self._m), axis=1)
+        y = -np.sum(np.sin(X) * y1**(2 * self.opt_m), axis=1)
         return y
 
     def _target_pt(self, x):
         """Draft."""
         d = torch.tensor(self.d)
-        par_m = torch.tensor(self._m)
+        par_m = torch.tensor(self.opt_m)
         pi = torch.tensor(np.pi)
         y1 = torch.sin(((torch.arange(d) + 1) * x**2 / pi))
         y = -torch.sum(torch.sin(x) * y1**(2 * par_m))
         return y
 
 
 if __name__ == '__main__':
```

### Comparing `teneva_bm-0.6.4/teneva_bm/func/bm_func_piston.py` & `teneva_bm-0.7.0/teneva_bm/func/bm_func_piston.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/func/bm_func_qing.py` & `teneva_bm-0.7.0/teneva_bm/func/bm_func_qing.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/func/bm_func_rastrigin.py` & `teneva_bm-0.7.0/teneva_bm/func/bm_func_rastrigin.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,51 +32,51 @@
 
     @property
     def with_cores(self):
         return True
 
     def get_config(self):
         conf = super().get_config()
-        conf['_A'] = self._A
+        conf['opt_A'] = self.opt_A
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'Param A for Rastrigin function           : '
-        v = self._A
+        v = self.opt_A
         text += f'{v:.6f}\n'
 
         return super().info(text+footer)
 
-    def set_opts(self, A=10.):
+    def set_opts(self, opt_A=10.):
         """Set options specific to this benchmark.
 
         There are no plans to manually change the default values.
 
         Args:
-            A (float): parameter of the function.
+            opt_A (float): parameter of the function.
 
         """
-        self._A = A
+        self.opt_A = opt_A
 
     def cores(self, X):
         return self.cores_add(
-            [x**2 - self._A * np.cos(2 * np.pi * x) for x in X.T],
-            a0=self._A*self.d)
+            [x**2 - self.opt_A * np.cos(2 * np.pi * x) for x in X.T],
+            a0=self.opt_A*self.d)
 
     def target_batch(self, X):
-        y1 = self._A * self.d
-        y2 = np.sum(X**2 - self._A * np.cos(2. * np.pi * X), axis=1)
+        y1 = self.opt_A * self.d
+        y2 = np.sum(X**2 - self.opt_A * np.cos(2. * np.pi * X), axis=1)
         return y1 + y2
 
     def _target_pt(self, x):
         """Draft."""
         d = torch.tensor(self.d)
-        par_A = torch.tensor(self._A)
+        par_A = torch.tensor(self.opt_A)
         pi = torch.tensor(np.pi)
 
         y1 = par_A * d
         y2 = torch.sum(x**2 - par_A * torch.cos(2. * pi * x))
 
         return y1 + y2
```

### Comparing `teneva_bm-0.6.4/teneva_bm/func/bm_func_rosenbrock.py` & `teneva_bm-0.7.0/teneva_bm/func/bm_func_rosenbrock.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/func/bm_func_schaffer.py` & `teneva_bm-0.7.0/teneva_bm/func/bm_func_schaffer.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/func/bm_func_schwefel.py` & `teneva_bm-0.7.0/teneva_bm/func/bm_func_schwefel.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,50 +34,50 @@
 
     @property
     def with_cores(self):
         return True
 
     def get_config(self):
         conf = super().get_config()
-        conf['_a'] = self._a
+        conf['opt_a'] = self.opt_a
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'Param a for Schwefel function            : '
-        v = self._a
+        v = self.opt_a
         text += f'{v:.6f}\n'
 
         return super().info(text+footer)
 
-    def set_opts(self, a=418.9829):
+    def set_opts(self, opt_a=418.9829):
         """Set options specific to this benchmark.
 
         There are no plans to manually change the default values.
 
         Args:
-            a (float): parameter of the function.
+            opt_a (float): parameter of the function.
 
         """
-        self._a = a
+        self.opt_a = opt_a
 
     def cores(self, X):
         return self.cores_add(
             [-x * np.sin(np.sqrt(np.abs(x))) for x in X.T],
-            a0=self._a*self.d)
+            a0=self.opt_a*self.d)
 
     def target_batch(self, X):
-        y0 = self._a * self.d
+        y0 = self.opt_a * self.d
         return y0 - np.sum(X * np.sin(np.sqrt(np.abs(X))), axis=1)
 
     def _target_pt(self, x):
         """Draft."""
         d = torch.tensor(self.d)
-        par_a = torch.tensor(self._a)
+        par_a = torch.tensor(self.opt_a)
         y0 = par_a * d
         return y0 - torch.sum(x * torch.sin(torch.sqrt(torch.abs(x))))
 
 
 if __name__ == '__main__':
     np.random.seed(42)
```

### Comparing `teneva_bm-0.6.4/teneva_bm/hs/bm_hs_func001.py` & `teneva_bm-0.7.0/teneva_bm/hs/bm_hs_func001.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/hs/bm_hs_func006.py` & `teneva_bm-0.7.0/teneva_bm/hs/bm_hs_func006.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/hs/draft_constrained_functions/bm_hs007.py` & `teneva_bm-0.7.0/teneva_bm/hs/draft_constrained_functions/bm_hs007.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/hs/draft_constrained_functions/bm_hs008.py` & `teneva_bm-0.7.0/teneva_bm/hs/draft_constrained_functions/bm_hs008.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/hs/draft_constrained_functions/bm_hs009.py` & `teneva_bm-0.7.0/teneva_bm/hs/draft_constrained_functions/bm_hs009.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/hs/draft_constrained_functions/bm_hs010.py` & `teneva_bm-0.7.0/teneva_bm/hs/draft_constrained_functions/bm_hs010.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/hs/draft_constrained_functions/bm_hs011.py` & `teneva_bm-0.7.0/teneva_bm/hs/draft_constrained_functions/bm_hs011.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/hs/draft_constrained_functions/bm_hs012.py` & `teneva_bm-0.7.0/teneva_bm/hs/draft_constrained_functions/bm_hs012.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py` & `teneva_bm-0.7.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py` & `teneva_bm-0.7.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py` & `teneva_bm-0.7.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py` & `teneva_bm-0.7.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py` & `teneva_bm-0.7.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py` & `teneva_bm-0.7.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/odeoc/bm_odeoc_simple.py` & `teneva_bm-0.7.0/teneva_bm/odeoc/bm_odeoc_simple.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,37 +43,37 @@
 
     @property
     def is_tens(self):
         return True
 
     def get_config(self):
         conf = super().get_config()
-        conf['_x_ini'] = self._x_ini
-        conf['_x_ref'] = self._x_ref
-        conf['_t_max'] = self._t_max
-        conf['_y_err'] = self._y_err
+        conf['x_ini'] = self.x_ini
+        conf['x_ref'] = self.x_ref
+        conf['t_max'] = self.t_max
+        conf['y_err'] = self.y_err
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'Param x_ini (initial condition)          : '
-        v = self._x_ini
+        v = self.x_ini
         text += f'{v:.6f}\n'
 
         text += 'Param x_ref (target value)               : '
-        v = self._x_ref
+        v = self.x_ref
         text += f'{v:.6f}\n'
 
         text += 'Param t_max (upper limit for time)       : '
-        v = self._t_max
+        v = self.t_max
         text += f'{v:.6f}\n'
 
         text += 'Param y_err (returned value if error)    : '
-        v = self._y_err
+        v = self.y_err
         text += f'{v:-7.1e}\n'
 
         return super().info(text+footer)
 
     def set_opts(self, x_ini=0.8, x_ref=0.7, t_max=1., y_err=1.E+50):
         """Set options specific to the benchmark.
 
@@ -82,48 +82,48 @@
         Args:
             x_ini (float): initial condition for the ODE.
             x_ref (float): target (reference) value for solution of the ODE.
             t_max (float): upper limit for time variable in the ODE.
             y_err (float): returned value if GEKKO solver ends with error.
 
         """
-        self._x_ini = x_ini
-        self._x_ref = x_ref
-        self._t_max = t_max
-        self._y_err = y_err
+        self.x_ini = x_ini
+        self.x_ref = x_ref
+        self.t_max = t_max
+        self.y_err = y_err
 
         self._times = np.linspace(0, t_max, self.d)
 
     def target(self, i):
         solver = GEKKO(remote=False)
         solver.options.IMODE = 4
         solver.time = self._times
 
-        x = solver.Var(value=self._x_ini, name='x')
+        x = solver.Var(value=self.x_ini, name='x')
         c = solver.Param(list(i), name='i')
         y = solver.Var(value=0.)
 
         solver.Equation(x.dt() == self._ode(x, c))
         solver.Equation(y == self._obj(x, c))
 
         try:
             solver.solve(disp=False)
             y = sum(y.VALUE)
         except Exception as e:
-            y = self._y_err
+            y = self.y_err
 
         return y
 
     def _ode(self, x, i):
         """Target ordinary differential equation (ODE)."""
         return x**3 - i
 
     def _obj(self, x, i):
         """Objective function for ODE solution."""
-        return 0.5 * (x - self._x_ref)**2
+        return 0.5 * (x - self.x_ref)**2
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
     bm = BmOdeocSimple().prep()
     print(bm.info())
```

### Comparing `teneva_bm-0.6.4/teneva_bm/odeoc/bm_odeoc_simple_constr.py` & `teneva_bm-0.7.0/teneva_bm/odeoc/bm_odeoc_simple_constr.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/qubo/bm_qubo_knap_det.py` & `teneva_bm-0.7.0/teneva_bm/qubo/bm_qubo_knap_det.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/qubo/bm_qubo_knap_quad.py` & `teneva_bm-0.7.0/teneva_bm/qubo/bm_qubo_knap_quad.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/qubo/bm_qubo_maxcut.py` & `teneva_bm-0.7.0/teneva_bm/qubo/bm_qubo_maxcut.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,29 +49,29 @@
 
     @property
     def is_tens(self):
         return True
 
     def get_config(self):
         conf = super().get_config()
-        conf['_prob_con'] = self._prob_con
+        conf['prob_con'] = self.prob_con
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'Param prob_con (connection probability)  : '
-        v = self._prob_con
+        v = self.prob_con
         text += f'{v:.6f}\n'
 
         return super().info(text+footer)
 
     def prep_bm(self):
         d = self.d
-        p = self._prob_con
+        p = self.prob_con
         graph = nx.fast_gnp_random_graph(n=d, p=p, seed=self.seed)
         edges = np.array(list([list(e) for e in graph.edges]))
         n_nodes = len(np.unique(np.array(edges).flatten()))
 
         g = qubogen.Graph(edges=edges, n_nodes=n_nodes)
         self._Q = qubogen.qubo_max_cut(g)
 
@@ -80,15 +80,15 @@
 
         There are no plans to manually change the default values.
 
         Args:
             prob_con (float): probability of the connection in the graph.
 
         """
-        self._prob_con = prob_con
+        self.prob_con = prob_con
 
     def target_batch(self, I):
         return ((I @ self._Q) * I).sum(axis=1)
 
 
 if __name__ == '__main__':
     np.random.seed(42)
```

### Comparing `teneva_bm-0.6.4/teneva_bm/qubo/bm_qubo_mvc.py` & `teneva_bm-0.7.0/teneva_bm/qubo/bm_qubo_mvc.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,29 +49,29 @@
 
     @property
     def is_tens(self):
         return True
 
     def get_config(self):
         conf = super().get_config()
-        conf['_prob_con'] = self._prob_con
+        conf['prob_con'] = self.prob_con
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'Param prob_con (connection probability)  : '
-        v = self._prob_con
+        v = self.prob_con
         text += f'{v:.6f}\n'
 
         return super().info(text+footer)
 
     def prep_bm(self):
         d = self.d
-        p = self._prob_con
+        p = self.prob_con
         graph = nx.fast_gnp_random_graph(n=d, p=p, seed=self.seed)
         edges = np.array(list([list(e) for e in graph.edges]))
         n_nodes = len(np.unique(np.array(edges).flatten()))
 
         g = qubogen.Graph(edges=edges, n_nodes=n_nodes)
         self._Q = qubogen.qubo_mvc(g)
 
@@ -80,15 +80,15 @@
 
         There are no plans to manually change the default values.
 
         Args:
             prob_con (float): probability of the connection in the graph.
 
         """
-        self._prob_con = prob_con
+        self.prob_con = prob_con
 
     def target_batch(self, I):
         return ((I @ self._Q) * I).sum(axis=1)
 
 
 if __name__ == '__main__':
     np.random.seed(42)
```

### Comparing `teneva_bm-0.6.4/teneva_bm/teneva_bm_demo.py` & `teneva_bm-0.7.0/teneva_bm/teneva_bm_demo.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm/various/bm_matmul.py` & `teneva_bm-0.7.0/teneva_bm/various/bm_matmul.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,62 +65,62 @@
                 1, 2, 1, 2, 1, 1, 1,
                 2, 0, 2, 1, 1, 2, 1]
             self.set_min(i=i, y=0.)
 
         self._T = T_real
         self._E = E
 
-        self._size = size
-        self._rank = rank
-        self._only2 = only2
+        self.size = size
+        self.rank = rank
+        self.only2 = only2
 
     @property
     def identity(self):
-        return ['_size', '_rank', '_only2']
+        return ['size', 'rank', 'n', 'only2']
 
     @property
     def is_tens(self):
         return True
 
     def get_config(self):
         conf = super().get_config()
-        conf['_size'] = self._size
-        conf['_rank'] = self._rank
-        conf['_only2'] = self._only2
+        conf['size'] = self.size
+        conf['rank'] = self.rank
+        conf['only2'] = self.only2
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'Param size (sizes of the matrices)       : '
-        v = self._size
+        v = self.size
         text += f'{v:.0f}\n'
 
         text += 'Param rank (search rank for CP-decomp.)  : '
-        v = self._rank
+        v = self.rank
         text += f'{v:.0f}\n'
 
         text += 'Param only2 (if True, use 2 CP-factors)  : '
-        v = 'YES' if self._only2 else 'no'
+        v = 'YES' if self.only2 else 'no'
         text += f'{v}\n'
 
         return super().info(text+footer)
 
     def prep_bm(self):
-        self.loss = _loss_build(self._T, self._E, self._rank, self._only2)
+        self.loss = _loss_build(self._T, self._E, self.rank, self.only2)
 
     def recover(self, i=None, best=True):
         i, y = self.get_solution(i, best)
         x = _ind_to_poi(i, self._E)
 
-        if self._only2:
-            U, V = _factor_from_poi(x, self._rank, True)
+        if self.only2:
+            U, V = _factor_from_poi(x, self.rank, True)
             W = _factor_recover(U, V, self._T)
         else:
-            U, V, W = _factor_from_poi(x, self._rank, False)
+            U, V, W = _factor_from_poi(x, self.rank, False)
 
         return U, V, W
 
     def target(self, i):
         return self.loss(i)
 
 
@@ -226,15 +226,15 @@
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
-    if bm._size == 2 and bm.n0 == 3:
+    if bm.size == 2 and bm.n0 == 3:
         text = 'Value at the minimum (real vs calc)      :  '
         y_real = bm.y_min_real
         y_calc = bm[bm.i_min_real]
         text += f'{y_real:-10.3e}       /      {y_calc:-10.3e}'
         print(text)
 
     text = 'Check "only2" case                       :  '
```

### Comparing `teneva_bm-0.6.4/teneva_bm/various/bm_topopt.py` & `teneva_bm-0.7.0/teneva_bm/various/bm_topopt.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,118 +12,118 @@
     The dimension is defined from "nx" and "ny" parameters and mode size
     should be 2.
 """
 
 
 class BmTopopt(Bm):
     def __init__(self, d=None, n=2, name='BmTopopt', desc=DESC, nx=128, ny=32):
-        super().__init__(nx*ny, n, name, desc)
+        super().__init__(int(nx*ny), n, name, desc)
 
         if d is not None:
             self.set_err('Dimension number (d) should not be set manually')
 
         if not self.is_n_equal or self.n0 != 2:
             self.set_err('Mode size (n) should be "2"')
 
-        self._nx = nx
-        self._ny = ny
+        self.nx = int(nx)
+        self.ny = int(ny)
 
     @property
     def identity(self):
-        return ['_nx', '_ny']
+        return ['nx', 'ny']
 
     @property
     def is_tens(self):
         return True
 
     @property
     def with_show(self):
         return True
 
     def get_config(self):
         conf = super().get_config()
-        conf['_nx'] = self._nx
-        conf['_ny'] = self._ny
-        conf['_k_frac'] = self._k_frac
-        conf['_penal'] = self._penal
-        conf['_rmin'] = self._rmin
+        conf['nx'] = self.nx
+        conf['ny'] = self.ny
+        conf['k_frac'] = self.k_frac
+        conf['penal'] = self.penal
+        conf['rmin'] = self.rmin
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'Param nx (grid x-size)                   : '
-        v = self._nx
+        v = self.nx
         text += f'{v:.0f}\n'
 
         text += 'Param ny (grid y-size)                   : '
-        v = self._ny
+        v = self.ny
         text += f'{v:.0f}\n'
 
         text += 'Param k_frac for Topopt                  : '
-        v = self._k_frac
+        v = self.k_frac
         text += f'{v:.6f}\n'
 
         text += 'Param penal for Topopt                   : '
-        v = self._penal
+        v = self.penal
         text += f'{v:.6f}\n'
 
         text += 'Param rmin for Topopt                    : '
-        v = self._rmin
+        v = self.rmin
         text += f'{v:.6f}\n'
 
         return super().info(text+footer)
 
     def prep_bm(self):
-        self._solver = _topopt_lite(self._nx, self._ny,
-            self._k_frac, self._penal, self._rmin)
+        self._solver = _topopt_lite(self.nx, self.ny,
+            self.k_frac, self.penal, self.rmin)
 
     def set_opts(self, k_frac=0.4, penal=3., rmin=5.4):
         """Setting options specific to this benchmark.
 
         There are no plans to manually change the default values.
 
         Args:
             k_frac (float): ?.
             penal (float): ?.
             rmin (float): ?.
 
         """
-        self._k_frac = k_frac
-        self._penal = penal
-        self._rmin = rmin
+        self.k_frac = k_frac
+        self.penal = penal
+        self.rmin = rmin
 
     def show(self, fpath=None, i=None, best=True):
         i, y = self.get_solution(i, best)
 
-        x = i.reshape(self._nx, self._ny).T
+        x = i.reshape(self.nx, self.ny).T
 
         fig, ax = plt.subplots(1, 1, figsize=(21, 7))
         ax.imshow(x, cmap='gray', interpolation='none')
 
         k_frac_real = np.sum(x) / np.size(x)
 
         title = ''
         title += f'Shape: {x.shape[0]} x {x.shape[1]}. '
-        title += f'Frac: {k_frac_real:.2f} ({self._k_frac:.2f}). '
+        title += f'Frac: {k_frac_real:.2f} ({self.k_frac:.2f}). '
         title += f'Value: {y:.2f}.'
         fig.suptitle(title, fontsize=18)
 
         fpath = self.path_build(fpath, 'png')
         plt.savefig(fpath, bbox_inches='tight') if fpath else plt.show()
 
     def target(self, i):
         return self._solver(i)
 
     def _optimize_baseline(self):
         """Draft!"""
-        solver = TopOptLite(self._nx, self._ny, self._penal, self._rmin)
+        solver = TopOptLite(self.nx, self.ny, self.penal, self.rmin)
         solver.init(Emin=1.E-9, Emax=1.0)
         solver.prep()
-        x_ini = self._k_frac * np.ones(self._nx * self._ny, dtype=float)
+        x_ini = self.k_frac * np.ones(self.nx * self.ny, dtype=float)
         x_opt = solver.solve(x_ini)
         return x_opt
 
 
 class TopOptLite:
     def __init__(self, nx, ny, penal, rmin):
         self.nx = nx
```

### Comparing `teneva_bm-0.6.4/teneva_bm/various/bm_wall_simple.py` & `teneva_bm-0.7.0/teneva_bm/various/bm_wall_simple.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.6.4/teneva_bm.egg-info/PKG-INFO` & `teneva_bm-0.7.0/teneva_bm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva-bm
-Version: 0.6.4
+Version: 0.7.0
 Summary: Benchmarks library, based on the software product teneva, for testing multivariate approximation and optimization methods
 Home-page: https://github.com/AndreiChertkov/teneva_bm
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_bm
 Keywords: benchmarks approximation optimization multidimensional array multivariate function low-rank representation tensor train format TT-decomposition
@@ -30,15 +30,15 @@
 ## Description
 
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.6.4".
+> Current version "0.7.0".
 
 The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
 
 > Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.5+) will be automatically installed during the installation of the main software product.
 
 Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following commands:
```

### Comparing `teneva_bm-0.6.4/teneva_bm.egg-info/SOURCES.txt` & `teneva_bm-0.7.0/teneva_bm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

