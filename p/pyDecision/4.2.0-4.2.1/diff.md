# Comparing `tmp/pyDecision-4.2.0.tar.gz` & `tmp/pyDecision-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyDecision-4.2.0.tar", last modified: Tue Aug  1 01:10:56 2023, max compression
+gzip compressed data, was "dist\pyDecision-4.2.1.tar", last modified: Wed Aug  2 19:41:50 2023, max compression
```

## Comparing `pyDecision-4.2.0.tar` & `pyDecision-4.2.1.tar`

### file list

```diff
@@ -1,85 +1,84 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 01:10:56.000000 pyDecision-4.2.0/
--rw-rw-rw-   0        0        0      659 2022-03-01 20:02:45.000000 pyDecision-4.2.0/LICENSE
--rw-rw-rw-   0        0        0    17106 2023-08-01 01:10:56.000000 pyDecision-4.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    16625 2023-08-01 01:04:49.000000 pyDecision-4.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 01:10:55.000000 pyDecision-4.2.0/pyDecision/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-4.2.0/pyDecision/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:10:56.000000 pyDecision-4.2.0/pyDecision/algorithm/
--rw-rw-rw-   0        0        0     2503 2023-07-29 23:13:09.000000 pyDecision-4.2.0/pyDecision/algorithm/__init__.py
--rw-rw-rw-   0        0        0     1079 2023-07-21 17:12:59.000000 pyDecision-4.2.0/pyDecision/algorithm/ahp.py
--rw-rw-rw-   0        0        0     2591 2023-07-21 17:32:54.000000 pyDecision-4.2.0/pyDecision/algorithm/aras.py
--rw-rw-rw-   0        0        0     2147 2023-07-21 20:21:53.000000 pyDecision-4.2.0/pyDecision/algorithm/borda.py
--rw-rw-rw-   0        0        0     1548 2023-07-21 17:33:22.000000 pyDecision-4.2.0/pyDecision/algorithm/bwm.py
--rw-rw-rw-   0        0        0      862 2023-07-18 00:52:46.000000 pyDecision-4.2.0/pyDecision/algorithm/cilos.py
--rw-rw-rw-   0        0        0     2762 2023-07-22 02:44:56.000000 pyDecision-4.2.0/pyDecision/algorithm/cocoso.py
--rw-rw-rw-   0        0        0     2754 2023-07-21 17:33:49.000000 pyDecision-4.2.0/pyDecision/algorithm/codas.py
--rw-rw-rw-   0        0        0     2870 2023-07-23 17:00:58.000000 pyDecision-4.2.0/pyDecision/algorithm/copeland.py
--rw-rw-rw-   0        0        0     2471 2023-07-21 17:34:03.000000 pyDecision-4.2.0/pyDecision/algorithm/copras.py
--rw-rw-rw-   0        0        0     2347 2023-07-23 16:38:01.000000 pyDecision-4.2.0/pyDecision/algorithm/cradis.py
--rw-rw-rw-   0        0        0     1121 2021-04-26 20:45:47.000000 pyDecision-4.2.0/pyDecision/algorithm/critic.py
--rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-4.2.0/pyDecision/algorithm/dematel.py
--rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-4.2.0/pyDecision/algorithm/e_i.py
--rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-4.2.0/pyDecision/algorithm/e_i_s.py
--rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-4.2.0/pyDecision/algorithm/e_i_v.py
--rw-rw-rw-   0        0        0    16907 2023-07-21 20:38:15.000000 pyDecision-4.2.0/pyDecision/algorithm/e_ii.py
--rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-4.2.0/pyDecision/algorithm/e_iii.py
--rw-rw-rw-   0        0        0    14298 2023-07-21 19:41:40.000000 pyDecision-4.2.0/pyDecision/algorithm/e_iv.py
--rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-4.2.0/pyDecision/algorithm/e_tri_b.py
--rw-rw-rw-   0        0        0     2711 2023-07-21 20:33:16.000000 pyDecision-4.2.0/pyDecision/algorithm/edas.py
--rw-rw-rw-   0        0        0      925 2023-07-19 01:09:53.000000 pyDecision-4.2.0/pyDecision/algorithm/entropy.py
--rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-4.2.0/pyDecision/algorithm/fuzzy_ahp.py
--rw-rw-rw-   0        0        0     3321 2023-07-25 15:17:23.000000 pyDecision-4.2.0/pyDecision/algorithm/fuzzy_aras.py
--rw-rw-rw-   0        0        0     4545 2023-07-21 17:31:44.000000 pyDecision-4.2.0/pyDecision/algorithm/fuzzy_copras.py
--rw-rw-rw-   0        0        0     4100 2023-08-01 01:06:41.000000 pyDecision-4.2.0/pyDecision/algorithm/fuzzy_dematel.py
--rw-rw-rw-   0        0        0     5042 2023-07-21 18:03:22.000000 pyDecision-4.2.0/pyDecision/algorithm/fuzzy_edas.py
--rw-rw-rw-   0        0        0     3706 2023-07-21 18:11:21.000000 pyDecision-4.2.0/pyDecision/algorithm/fuzzy_moora.py
--rw-rw-rw-   0        0        0     4098 2023-07-21 18:13:14.000000 pyDecision-4.2.0/pyDecision/algorithm/fuzzy_ocra.py
--rw-rw-rw-   0        0        0     4086 2023-07-21 18:17:14.000000 pyDecision-4.2.0/pyDecision/algorithm/fuzzy_topsis.py
--rw-rw-rw-   0        0        0     5994 2023-07-21 18:18:25.000000 pyDecision-4.2.0/pyDecision/algorithm/fuzzy_vikor.py
--rw-rw-rw-   0        0        0     2553 2023-07-22 02:46:58.000000 pyDecision-4.2.0/pyDecision/algorithm/gra.py
--rw-rw-rw-   0        0        0     2617 2023-07-25 20:31:22.000000 pyDecision-4.2.0/pyDecision/algorithm/idocriw.py
--rw-rw-rw-   0        0        0     2585 2023-07-21 18:06:06.000000 pyDecision-4.2.0/pyDecision/algorithm/mabac.py
--rw-rw-rw-   0        0        0     2388 2023-07-28 22:31:36.000000 pyDecision-4.2.0/pyDecision/algorithm/macbeth.py
--rw-rw-rw-   0        0        0     2575 2023-07-23 16:39:11.000000 pyDecision-4.2.0/pyDecision/algorithm/mairca.py
--rw-rw-rw-   0        0        0     3048 2023-07-21 18:09:18.000000 pyDecision-4.2.0/pyDecision/algorithm/marcos.py
--rw-rw-rw-   0        0        0     3766 2023-07-22 02:46:58.000000 pyDecision-4.2.0/pyDecision/algorithm/maut.py
--rw-rw-rw-   0        0        0      965 2023-07-21 18:10:23.000000 pyDecision-4.2.0/pyDecision/algorithm/merec.py
--rw-rw-rw-   0        0        0     2541 2023-07-21 18:10:51.000000 pyDecision-4.2.0/pyDecision/algorithm/moora.py
--rw-rw-rw-   0        0        0     2549 2023-07-21 18:12:07.000000 pyDecision-4.2.0/pyDecision/algorithm/moosra.py
--rw-rw-rw-   0        0        0     4968 2023-07-22 01:50:19.000000 pyDecision-4.2.0/pyDecision/algorithm/multimoora.py
--rw-rw-rw-   0        0        0     2477 2023-07-21 23:26:24.000000 pyDecision-4.2.0/pyDecision/algorithm/ocra.py
--rw-rw-rw-   0        0        0     2553 2023-07-28 23:58:56.000000 pyDecision-4.2.0/pyDecision/algorithm/oreste.py
--rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-4.2.0/pyDecision/algorithm/p_i.py
--rw-rw-rw-   0        0        0     5891 2023-07-21 19:40:41.000000 pyDecision-4.2.0/pyDecision/algorithm/p_ii.py
--rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-4.2.0/pyDecision/algorithm/p_iii.py
--rw-rw-rw-   0        0        0     8547 2023-07-21 19:39:42.000000 pyDecision-4.2.0/pyDecision/algorithm/p_iv.py
--rw-rw-rw-   0        0        0     6472 2023-07-21 19:39:01.000000 pyDecision-4.2.0/pyDecision/algorithm/p_v.py
--rw-rw-rw-   0        0        0     9380 2023-07-21 19:37:53.000000 pyDecision-4.2.0/pyDecision/algorithm/p_vi.py
--rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-4.2.0/pyDecision/algorithm/p_xgaia.py
--rw-rw-rw-   0        0        0     2139 2023-07-23 16:40:26.000000 pyDecision-4.2.0/pyDecision/algorithm/piv.py
--rw-rw-rw-   0        0        0     2184 2023-07-21 18:14:04.000000 pyDecision-4.2.0/pyDecision/algorithm/psi.py
--rw-rw-rw-   0        0        0     5228 2023-07-29 11:05:11.000000 pyDecision-4.2.0/pyDecision/algorithm/regime.py
--rw-rw-rw-   0        0        0     2434 2023-07-22 02:08:59.000000 pyDecision-4.2.0/pyDecision/algorithm/rov.py
--rw-rw-rw-   0        0        0     2130 2023-07-21 18:14:55.000000 pyDecision-4.2.0/pyDecision/algorithm/saw.py
--rw-rw-rw-   0        0        0     2344 2023-07-21 18:15:17.000000 pyDecision-4.2.0/pyDecision/algorithm/smart.py
--rw-rw-rw-   0        0        0     2867 2023-07-21 18:15:39.000000 pyDecision-4.2.0/pyDecision/algorithm/todim.py
--rw-rw-rw-   0        0        0     2600 2023-07-21 18:16:04.000000 pyDecision-4.2.0/pyDecision/algorithm/topsis.py
--rw-rw-rw-   0        0        0     3703 2023-07-22 03:11:26.000000 pyDecision-4.2.0/pyDecision/algorithm/vikor.py
--rw-rw-rw-   0        0        0     4242 2023-07-25 13:24:23.000000 pyDecision-4.2.0/pyDecision/algorithm/waspas.py
--rw-rw-rw-   0        0        0     2643 2023-07-21 18:23:36.000000 pyDecision-4.2.0/pyDecision/algorithm/wings.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:10:56.000000 pyDecision-4.2.0/pyDecision/compare/
--rw-rw-rw-   0        0        0       94 2023-07-25 21:52:02.000000 pyDecision-4.2.0/pyDecision/compare/__init__.py
--rw-rw-rw-   0        0        0    18822 2023-07-29 22:20:55.000000 pyDecision-4.2.0/pyDecision/compare/compare.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:10:56.000000 pyDecision-4.2.0/pyDecision/util/
--rw-rw-rw-   0        0        0     4211 2023-07-30 00:44:26.000000 pyDecision-4.2.0/pyDecision/util/LLM.py
--rw-rw-rw-   0        0        0      138 2023-07-25 21:52:24.000000 pyDecision-4.2.0/pyDecision/util/__init__.py
--rw-rw-rw-   0        0        0     6266 2023-07-21 21:06:34.000000 pyDecision-4.2.0/pyDecision/util/ga.py
--rw-rw-rw-   0        0        0     6113 2023-07-25 20:17:38.000000 pyDecision-4.2.0/pyDecision/util/gwo.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:10:55.000000 pyDecision-4.2.0/pyDecision.egg-info/
--rw-rw-rw-   0        0        0    17106 2023-08-01 01:10:53.000000 pyDecision-4.2.0/pyDecision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2293 2023-08-01 01:10:54.000000 pyDecision-4.2.0/pyDecision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 01:10:53.000000 pyDecision-4.2.0/pyDecision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-08-01 01:10:53.000000 pyDecision-4.2.0/pyDecision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-01 01:10:53.000000 pyDecision-4.2.0/pyDecision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 01:10:56.000000 pyDecision-4.2.0/setup.cfg
--rw-rw-rw-   0        0        0      727 2023-08-01 01:05:20.000000 pyDecision-4.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:41:50.000000 pyDecision-4.2.1/
+-rw-rw-rw-   0        0        0      659 2022-03-01 20:02:45.000000 pyDecision-4.2.1/LICENSE
+-rw-rw-rw-   0        0        0    17333 2023-08-02 19:41:50.000000 pyDecision-4.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    16851 2023-08-02 01:05:09.000000 pyDecision-4.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 19:41:49.000000 pyDecision-4.2.1/pyDecision/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-4.2.1/pyDecision/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:41:50.000000 pyDecision-4.2.1/pyDecision/algorithm/
+-rw-rw-rw-   0        0        0     2544 2023-08-02 00:36:24.000000 pyDecision-4.2.1/pyDecision/algorithm/__init__.py
+-rw-rw-rw-   0        0        0     1079 2023-07-21 17:12:59.000000 pyDecision-4.2.1/pyDecision/algorithm/ahp.py
+-rw-rw-rw-   0        0        0     2591 2023-07-21 17:32:54.000000 pyDecision-4.2.1/pyDecision/algorithm/aras.py
+-rw-rw-rw-   0        0        0     2147 2023-07-21 20:21:53.000000 pyDecision-4.2.1/pyDecision/algorithm/borda.py
+-rw-rw-rw-   0        0        0     1649 2023-08-01 23:39:36.000000 pyDecision-4.2.1/pyDecision/algorithm/bwm.py
+-rw-rw-rw-   0        0        0      862 2023-07-18 00:52:46.000000 pyDecision-4.2.1/pyDecision/algorithm/cilos.py
+-rw-rw-rw-   0        0        0     2762 2023-07-22 02:44:56.000000 pyDecision-4.2.1/pyDecision/algorithm/cocoso.py
+-rw-rw-rw-   0        0        0     2754 2023-07-21 17:33:49.000000 pyDecision-4.2.1/pyDecision/algorithm/codas.py
+-rw-rw-rw-   0        0        0     2870 2023-07-23 17:00:58.000000 pyDecision-4.2.1/pyDecision/algorithm/copeland.py
+-rw-rw-rw-   0        0        0     2471 2023-07-21 17:34:03.000000 pyDecision-4.2.1/pyDecision/algorithm/copras.py
+-rw-rw-rw-   0        0        0     2347 2023-07-23 16:38:01.000000 pyDecision-4.2.1/pyDecision/algorithm/cradis.py
+-rw-rw-rw-   0        0        0     1121 2021-04-26 20:45:47.000000 pyDecision-4.2.1/pyDecision/algorithm/critic.py
+-rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-4.2.1/pyDecision/algorithm/dematel.py
+-rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-4.2.1/pyDecision/algorithm/e_i.py
+-rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-4.2.1/pyDecision/algorithm/e_i_s.py
+-rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-4.2.1/pyDecision/algorithm/e_i_v.py
+-rw-rw-rw-   0        0        0    16907 2023-07-21 20:38:15.000000 pyDecision-4.2.1/pyDecision/algorithm/e_ii.py
+-rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-4.2.1/pyDecision/algorithm/e_iii.py
+-rw-rw-rw-   0        0        0    14298 2023-07-21 19:41:40.000000 pyDecision-4.2.1/pyDecision/algorithm/e_iv.py
+-rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-4.2.1/pyDecision/algorithm/e_tri_b.py
+-rw-rw-rw-   0        0        0     2711 2023-07-21 20:33:16.000000 pyDecision-4.2.1/pyDecision/algorithm/edas.py
+-rw-rw-rw-   0        0        0      925 2023-07-19 01:09:53.000000 pyDecision-4.2.1/pyDecision/algorithm/entropy.py
+-rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-4.2.1/pyDecision/algorithm/fuzzy_ahp.py
+-rw-rw-rw-   0        0        0     3321 2023-07-25 15:17:23.000000 pyDecision-4.2.1/pyDecision/algorithm/fuzzy_aras.py
+-rw-rw-rw-   0        0        0     4545 2023-07-21 17:31:44.000000 pyDecision-4.2.1/pyDecision/algorithm/fuzzy_copras.py
+-rw-rw-rw-   0        0        0     4100 2023-08-01 01:06:41.000000 pyDecision-4.2.1/pyDecision/algorithm/fuzzy_dematel.py
+-rw-rw-rw-   0        0        0     5042 2023-07-21 18:03:22.000000 pyDecision-4.2.1/pyDecision/algorithm/fuzzy_edas.py
+-rw-rw-rw-   0        0        0     3706 2023-07-21 18:11:21.000000 pyDecision-4.2.1/pyDecision/algorithm/fuzzy_moora.py
+-rw-rw-rw-   0        0        0     4098 2023-07-21 18:13:14.000000 pyDecision-4.2.1/pyDecision/algorithm/fuzzy_ocra.py
+-rw-rw-rw-   0        0        0     4086 2023-07-21 18:17:14.000000 pyDecision-4.2.1/pyDecision/algorithm/fuzzy_topsis.py
+-rw-rw-rw-   0        0        0     5994 2023-07-21 18:18:25.000000 pyDecision-4.2.1/pyDecision/algorithm/fuzzy_vikor.py
+-rw-rw-rw-   0        0        0     2553 2023-07-22 02:46:58.000000 pyDecision-4.2.1/pyDecision/algorithm/gra.py
+-rw-rw-rw-   0        0        0     2216 2023-08-01 23:41:39.000000 pyDecision-4.2.1/pyDecision/algorithm/idocriw.py
+-rw-rw-rw-   0        0        0     2585 2023-07-21 18:06:06.000000 pyDecision-4.2.1/pyDecision/algorithm/mabac.py
+-rw-rw-rw-   0        0        0     2388 2023-07-28 22:31:36.000000 pyDecision-4.2.1/pyDecision/algorithm/macbeth.py
+-rw-rw-rw-   0        0        0     2575 2023-07-23 16:39:11.000000 pyDecision-4.2.1/pyDecision/algorithm/mairca.py
+-rw-rw-rw-   0        0        0     3048 2023-07-21 18:09:18.000000 pyDecision-4.2.1/pyDecision/algorithm/marcos.py
+-rw-rw-rw-   0        0        0     3766 2023-07-22 02:46:58.000000 pyDecision-4.2.1/pyDecision/algorithm/maut.py
+-rw-rw-rw-   0        0        0      965 2023-07-21 18:10:23.000000 pyDecision-4.2.1/pyDecision/algorithm/merec.py
+-rw-rw-rw-   0        0        0     2541 2023-07-21 18:10:51.000000 pyDecision-4.2.1/pyDecision/algorithm/moora.py
+-rw-rw-rw-   0        0        0     2549 2023-07-21 18:12:07.000000 pyDecision-4.2.1/pyDecision/algorithm/moosra.py
+-rw-rw-rw-   0        0        0     4968 2023-07-22 01:50:19.000000 pyDecision-4.2.1/pyDecision/algorithm/multimoora.py
+-rw-rw-rw-   0        0        0     2477 2023-07-21 23:26:24.000000 pyDecision-4.2.1/pyDecision/algorithm/ocra.py
+-rw-rw-rw-   0        0        0     2553 2023-07-28 23:58:56.000000 pyDecision-4.2.1/pyDecision/algorithm/oreste.py
+-rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-4.2.1/pyDecision/algorithm/p_i.py
+-rw-rw-rw-   0        0        0     5891 2023-07-21 19:40:41.000000 pyDecision-4.2.1/pyDecision/algorithm/p_ii.py
+-rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-4.2.1/pyDecision/algorithm/p_iii.py
+-rw-rw-rw-   0        0        0     8547 2023-07-21 19:39:42.000000 pyDecision-4.2.1/pyDecision/algorithm/p_iv.py
+-rw-rw-rw-   0        0        0     6472 2023-07-21 19:39:01.000000 pyDecision-4.2.1/pyDecision/algorithm/p_v.py
+-rw-rw-rw-   0        0        0     9380 2023-07-21 19:37:53.000000 pyDecision-4.2.1/pyDecision/algorithm/p_vi.py
+-rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-4.2.1/pyDecision/algorithm/p_xgaia.py
+-rw-rw-rw-   0        0        0     2139 2023-07-23 16:40:26.000000 pyDecision-4.2.1/pyDecision/algorithm/piv.py
+-rw-rw-rw-   0        0        0     2184 2023-07-21 18:14:04.000000 pyDecision-4.2.1/pyDecision/algorithm/psi.py
+-rw-rw-rw-   0        0        0     5228 2023-07-29 11:05:11.000000 pyDecision-4.2.1/pyDecision/algorithm/regime.py
+-rw-rw-rw-   0        0        0     2434 2023-07-22 02:08:59.000000 pyDecision-4.2.1/pyDecision/algorithm/rov.py
+-rw-rw-rw-   0        0        0     2130 2023-07-21 18:14:55.000000 pyDecision-4.2.1/pyDecision/algorithm/saw.py
+-rw-rw-rw-   0        0        0     2344 2023-07-21 18:15:17.000000 pyDecision-4.2.1/pyDecision/algorithm/smart.py
+-rw-rw-rw-   0        0        0     2185 2023-08-02 00:35:27.000000 pyDecision-4.2.1/pyDecision/algorithm/spotis.py
+-rw-rw-rw-   0        0        0     2867 2023-07-21 18:15:39.000000 pyDecision-4.2.1/pyDecision/algorithm/todim.py
+-rw-rw-rw-   0        0        0     2600 2023-07-21 18:16:04.000000 pyDecision-4.2.1/pyDecision/algorithm/topsis.py
+-rw-rw-rw-   0        0        0     3703 2023-07-22 03:11:26.000000 pyDecision-4.2.1/pyDecision/algorithm/vikor.py
+-rw-rw-rw-   0        0        0     4242 2023-07-25 13:24:23.000000 pyDecision-4.2.1/pyDecision/algorithm/waspas.py
+-rw-rw-rw-   0        0        0     2643 2023-07-21 18:23:36.000000 pyDecision-4.2.1/pyDecision/algorithm/wings.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:41:50.000000 pyDecision-4.2.1/pyDecision/compare/
+-rw-rw-rw-   0        0        0      104 2023-08-02 19:39:50.000000 pyDecision-4.2.1/pyDecision/compare/__init__.py
+-rw-rw-rw-   0        0        0    20313 2023-08-02 19:36:09.000000 pyDecision-4.2.1/pyDecision/compare/compare.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:41:50.000000 pyDecision-4.2.1/pyDecision/util/
+-rw-rw-rw-   0        0        0     6036 2023-08-02 01:02:08.000000 pyDecision-4.2.1/pyDecision/util/LLM.py
+-rw-rw-rw-   0        0        0       73 2023-08-02 19:38:54.000000 pyDecision-4.2.1/pyDecision/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:41:49.000000 pyDecision-4.2.1/pyDecision.egg-info/
+-rw-rw-rw-   0        0        0    17333 2023-08-02 19:41:48.000000 pyDecision-4.2.1/pyDecision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2279 2023-08-02 19:41:48.000000 pyDecision-4.2.1/pyDecision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 19:41:48.000000 pyDecision-4.2.1/pyDecision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-08-02 19:41:48.000000 pyDecision-4.2.1/pyDecision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-02 19:41:48.000000 pyDecision-4.2.1/pyDecision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 19:41:50.000000 pyDecision-4.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      727 2023-08-02 00:39:52.000000 pyDecision-4.2.1/setup.py
```

### Comparing `pyDecision-4.2.0/LICENSE` & `pyDecision-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/PKG-INFO` & `pyDecision-4.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 4.2.0
+Version: 4.2.1
 Summary: A MCDA Library Incorporating Large Language Models to Enhance Decision Analysis
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **PSI** (Preference Selection Index); **Regime**; **ROV** (Range Of Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **Regime**; **ROV** (Range Of Value); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution), **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **PSI** (Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment). 
 
 pyDecision offers an array of features including the **comparison of ranking alternatives** and **comparison of criterion weights** from various methods. The library is also fully integrated with **chatGPT**, elevating result interpretation through AI. Additionally, pyDecision provides the flexibility to import results from custom methods or those not yet implemented in the library for swift comparison.
 
 ## Usage
 
 1. Install
 ```bash
@@ -115,14 +115,15 @@
 - PROMETHEE Gaia ([ Colab Demo ](https://colab.research.google.com/drive/1lj7IRKXcuRjrpoBp_KmQn_3sI3P_Qxju?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PIV ([ Colab Demo ](https://colab.research.google.com/drive/1PwJoBqYn1O2s22MqC9euP89Uyv4sedS0?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835218301360))
 - PSI ([ Colab Demo ](https://colab.research.google.com/drive/1u9tN8cYl2mx6KK6yLW2oz6fuVoy8xcCI?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0261306909006396))
 - Regime ([ Colab Demo ](https://colab.research.google.com/drive/1jcAcjAS92rxvE2urhc6HPixvzJ60HqEg?usp=sharing)) ( [ Paper ](https://link.springer.com/chapter/10.1007/978-3-030-15009-9_2))
 - ROV ([ Colab Demo ](https://colab.research.google.com/drive/1sQAPCem0pcS29uf6-n4TpncXMXNx9JDh?usp=sharing)) ( [ Paper ](https://doi.org/10.5267/j.dsl.2015.12.001))
 - SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
 - SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
+- SPOTIS ([ Colab Demo ](https://colab.research.google.com/drive/1TyjDn-xwut3w6Rf0zMiugdwytwmGY_NE?usp=sharing)) ( [ Paper ](https://doi.org/10.1002/mcda.1525))
 - TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0377221707010740))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
 - Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
 - VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_8))
 - Fuzzy VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1anfCnU2TSrW-Z5vMkS_qXFrYZ0ciQE53?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2011.04.097))
 - WINGS ([ Colab Demo ](https://colab.research.google.com/drive/1li1_cPxwEM3NOZ4hbI8RROXyOmXeoWew?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2013.02.007))
 - WSM, WPM, WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1HbLwXI4HkrmI-lsNzDtBOlCiwxfJltHi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_15))
```

### Comparing `pyDecision-4.2.0/README.md` & `pyDecision-4.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **PSI** (Preference Selection Index); **Regime**; **ROV** (Range Of Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **Regime**; **ROV** (Range Of Value); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution), **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **PSI** (Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment). 
 
 pyDecision offers an array of features including the **comparison of ranking alternatives** and **comparison of criterion weights** from various methods. The library is also fully integrated with **chatGPT**, elevating result interpretation through AI. Additionally, pyDecision provides the flexibility to import results from custom methods or those not yet implemented in the library for swift comparison.
 
 ## Usage
 
 1. Install
 ```bash
@@ -104,14 +104,15 @@
 - PROMETHEE Gaia ([ Colab Demo ](https://colab.research.google.com/drive/1lj7IRKXcuRjrpoBp_KmQn_3sI3P_Qxju?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PIV ([ Colab Demo ](https://colab.research.google.com/drive/1PwJoBqYn1O2s22MqC9euP89Uyv4sedS0?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835218301360))
 - PSI ([ Colab Demo ](https://colab.research.google.com/drive/1u9tN8cYl2mx6KK6yLW2oz6fuVoy8xcCI?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0261306909006396))
 - Regime ([ Colab Demo ](https://colab.research.google.com/drive/1jcAcjAS92rxvE2urhc6HPixvzJ60HqEg?usp=sharing)) ( [ Paper ](https://link.springer.com/chapter/10.1007/978-3-030-15009-9_2))
 - ROV ([ Colab Demo ](https://colab.research.google.com/drive/1sQAPCem0pcS29uf6-n4TpncXMXNx9JDh?usp=sharing)) ( [ Paper ](https://doi.org/10.5267/j.dsl.2015.12.001))
 - SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
 - SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
+- SPOTIS ([ Colab Demo ](https://colab.research.google.com/drive/1TyjDn-xwut3w6Rf0zMiugdwytwmGY_NE?usp=sharing)) ( [ Paper ](https://doi.org/10.1002/mcda.1525))
 - TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0377221707010740))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
 - Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
 - VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_8))
 - Fuzzy VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1anfCnU2TSrW-Z5vMkS_qXFrYZ0ciQE53?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2011.04.097))
 - WINGS ([ Colab Demo ](https://colab.research.google.com/drive/1li1_cPxwEM3NOZ4hbI8RROXyOmXeoWew?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2013.02.007))
 - WSM, WPM, WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1HbLwXI4HkrmI-lsNzDtBOlCiwxfJltHi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_15))
```

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/__init__.py` & `pyDecision-4.2.1/pyDecision/algorithm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,12 +50,13 @@
 from .p_xgaia       import promethee_gaia
 from .piv           import piv_method
 from .psi           import psi_method
 from .regime        import regime_method
 from .rov           import rov_method
 from .saw           import saw_method
 from .smart         import smart_method
+from .spotis        import spotis_method
 from .todim         import todim_method
 from .topsis        import topsis_method
 from .vikor         import vikor_method, ranking
 from .waspas        import waspas_method
 from .wings         import wings_method
```

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/ahp.py` & `pyDecision-4.2.1/pyDecision/algorithm/ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/aras.py` & `pyDecision-4.2.1/pyDecision/algorithm/aras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/borda.py` & `pyDecision-4.2.1/pyDecision/algorithm/borda.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/bwm.py` & `pyDecision-4.2.1/pyDecision/algorithm/critic.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,29 @@
 ###############################################################################
 
 # Required Libraries
 import numpy as np
 
-from pyDecision.util.gwo import grey_wolf_optimizer
-
 ###############################################################################
 
-# Function: BWM
-def bw_method(dataset, mic, lic, size = 50, iterations = 150, verbose = True):
-    X         = np.copy(dataset)/1.0
-    best      = np.where(mic == 1)[0][0]
-    worst     = np.where(lic == 1)[0][0]
-    pairs_b   = [(best, i)  for i in range(0, mic.shape[0])]
-    pairs_w   = [(i, worst) for i in range(0, mic.shape[0]) if (i, worst) not in pairs_b]
-    def target_function(variables):
-        eps       = [float('+inf')]
-        for pair in pairs_b:
-            i, j = pair
-            diff = abs(variables[i] - variables[j]*mic[j])
-            if ( i != j):
-                eps.append(diff)
-        for pair in pairs_w:
-            i, j = pair
-            diff = abs(variables[i] - variables[j]*lic[j])
-            if ( i != j):
-                eps.append(diff)
-        if ( np.sum(variables) == 0):
-            eps = float('+inf')
+# Function: CRITIC (CRiteria Importance Through Intercriteria Correlation)
+def critic_method(dataset, criterion_type):
+    X = np.copy(dataset)/1.0
+    best  = np.zeros(X.shape[1])
+    worst = np.zeros(X.shape[1])
+    for i in range(0, dataset.shape[1]):
+        if (criterion_type[i] == 'max'):
+            best[i]  = np.max(X[:, i])
+            worst[i] = np.min(X[:, i])
         else:
-            eps = max(eps[1:])
-        return eps
-    weights = grey_wolf_optimizer(pack_size = size, min_values = [0.01]*X.shape[1], max_values = [1]*X.shape[1], iterations = iterations, target_function = target_function, verbose = verbose)
-    weights = weights[0][:-1]/sum(weights[0][:-1])
+            best[i]  = np.min(X[:, i])
+            worst[i] = np.max(X[:, i])        
+    for j in range(0, X.shape[1]):
+        X[:,j] = ( X[:,j] - worst[j] ) / ( best[j] - worst[j] ) 
+    std      = (np.sum((X - X.mean())**2, axis = 0)/(X.shape[0] - 1))**(1/2)
+    sim_mat  = np.corrcoef(X.T)
+    conflict = np.sum(1 - sim_mat, axis = 1)
+    infor    = std*conflict
+    weights  = infor/np.sum(infor)
     return weights
 
 ###############################################################################
```

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/cilos.py` & `pyDecision-4.2.1/pyDecision/algorithm/cilos.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/cocoso.py` & `pyDecision-4.2.1/pyDecision/algorithm/cocoso.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/codas.py` & `pyDecision-4.2.1/pyDecision/algorithm/codas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/copeland.py` & `pyDecision-4.2.1/pyDecision/algorithm/copeland.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/copras.py` & `pyDecision-4.2.1/pyDecision/algorithm/copras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/cradis.py` & `pyDecision-4.2.1/pyDecision/algorithm/cradis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/dematel.py` & `pyDecision-4.2.1/pyDecision/algorithm/dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/e_i.py` & `pyDecision-4.2.1/pyDecision/algorithm/e_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/e_i_s.py` & `pyDecision-4.2.1/pyDecision/algorithm/e_i_s.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/e_i_v.py` & `pyDecision-4.2.1/pyDecision/algorithm/e_i_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/e_ii.py` & `pyDecision-4.2.1/pyDecision/algorithm/e_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/e_iii.py` & `pyDecision-4.2.1/pyDecision/algorithm/e_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/e_iv.py` & `pyDecision-4.2.1/pyDecision/algorithm/e_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/e_tri_b.py` & `pyDecision-4.2.1/pyDecision/algorithm/e_tri_b.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/edas.py` & `pyDecision-4.2.1/pyDecision/algorithm/edas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/entropy.py` & `pyDecision-4.2.1/pyDecision/algorithm/entropy.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/fuzzy_ahp.py` & `pyDecision-4.2.1/pyDecision/algorithm/fuzzy_ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/fuzzy_aras.py` & `pyDecision-4.2.1/pyDecision/algorithm/fuzzy_aras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/fuzzy_copras.py` & `pyDecision-4.2.1/pyDecision/algorithm/fuzzy_copras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/fuzzy_dematel.py` & `pyDecision-4.2.1/pyDecision/algorithm/fuzzy_dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/fuzzy_edas.py` & `pyDecision-4.2.1/pyDecision/algorithm/fuzzy_edas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/fuzzy_moora.py` & `pyDecision-4.2.1/pyDecision/algorithm/fuzzy_moora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/fuzzy_ocra.py` & `pyDecision-4.2.1/pyDecision/algorithm/fuzzy_ocra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/fuzzy_topsis.py` & `pyDecision-4.2.1/pyDecision/algorithm/fuzzy_topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/fuzzy_vikor.py` & `pyDecision-4.2.1/pyDecision/algorithm/fuzzy_vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/gra.py` & `pyDecision-4.2.1/pyDecision/algorithm/gra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/idocriw.py` & `pyDecision-4.2.1/pyDecision/algorithm/idocriw.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 ###############################################################################
 
 # Required Libraries
 import numpy as np
 
-from pyDecision.util.ga import genetic_algorithm
+from scipy.optimize import minimize, Bounds
 
 ###############################################################################
 
 # Function: IDOCRIW (Integrated Determination of Objective CRIteria Weights)
-def idocriw_method(dataset, criterion_type, size = 20, gen = 12000, verbose = False):
-    X    = np.copy(dataset)
+def idocriw_method(dataset, criterion_type, verbose = False):
+    X    = np.copy(dataset)/1.0
     X    = X/X.sum(axis = 0)
-    X_ln = np.copy(dataset)
-    X_r  = np.copy(dataset)
-    for i in range(0, X.shape[0]):
-        for j in range(0, X.shape[1]):
-            X_ln[i,j] = X[i,j]*np.log(X[i,j])
-    d = np.zeros((1, X.shape[1]))
-    w = np.zeros((1, X.shape[1]))
-    for i in range(0, d.shape[1]):
-        d[0,i] = 1-( -1/(np.log(d.shape[1]))*sum(X_ln[:,i])) 
-    for i in range(0, w.shape[1]):
-        w[0,i] = d[0,i]/d.sum(axis = 1)
+    X_ln = np.zeros(X.shape[1])
+    X_r  = np.copy(dataset)/1.0
+    for j in range(0, X.shape[1]):
+        X_ln[j] = np.sum(X[:,j]*np.log(X[:,j]))
+        X_ln[j] = X_ln[j]*(-1/np.log(X.shape[1]))
+    d = 1 - X_ln
+    w = d/np.sum(d)
     for i in range(0, len(criterion_type)):
         if (criterion_type[i] == 'min'):
            X_r[:,i] = dataset[:,i].min() / X_r[:,i]
     X_r   = X_r/X_r.sum(axis = 0)   
     a_max = X_r.max(axis = 0) 
     A     = np.zeros(dataset.shape)
     np.fill_diagonal(A, a_max)
@@ -38,28 +34,26 @@
     P      = np.copy(A)    
     for i in range(0, P.shape[1]):
         P[:,i] = (-P[:,i] + a_max_[i])/a_max[i]
     WP     = np.copy(P)
     np.fill_diagonal(WP, -P.sum(axis = 0))
     
     ################################################
-    def target_function(variable = [0]*WP.shape[1]):
-        variable = [variable[i]/sum(variable) for i in range(0, len(variable))]
-        WP_s     = np.copy(WP)
+    def target_function(variables):
+        WP_s = np.copy(WP)
         for i in range(0, WP.shape[0]):
             for j in range(0, WP.shape[1]):
-                WP_s[i, j] = WP_s[i, j]*variable[j]
-        total = abs(WP_s.sum(axis = 1)) 
-        total = sum(total) 
+                if (WP_s[i, j] != 0):
+                    WP_s[i, j] = WP_s[i, j]*variables[j]
+        total = np.sum((WP_s.sum(axis = 1)))
         return total
     ################################################
     
-    solution = genetic_algorithm(population_size = size, mutation_rate = 0.1, elite = 1, min_values = [0]*WP.shape[1], max_values = [1]*WP.shape[1], eta = 1, mu = 1, generations = gen, target_function = target_function, verbose = verbose)
-    solution = solution[:-1]
-    solution = solution/sum(solution)
-    w_       = np.copy(w)
-    w_       = w_*solution
-    w_       = w_/w_.sum()
-    w_       = w_.T
-    return w_
+    variables = np.ones(WP.shape[1])
+    bounds    = Bounds([0.0000001]*len(variables), [1]*len(variables))
+    results   = minimize(target_function, variables, method = 'L-BFGS-B', bounds = bounds)
+    weights   = results.x
+    weights   = weights * w
+    weights   = weights / np.sum(weights)
+    return weights
 
 ###############################################################################
```

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/mabac.py` & `pyDecision-4.2.1/pyDecision/algorithm/mabac.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/macbeth.py` & `pyDecision-4.2.1/pyDecision/algorithm/macbeth.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/mairca.py` & `pyDecision-4.2.1/pyDecision/algorithm/mairca.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/marcos.py` & `pyDecision-4.2.1/pyDecision/algorithm/marcos.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/maut.py` & `pyDecision-4.2.1/pyDecision/algorithm/maut.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/merec.py` & `pyDecision-4.2.1/pyDecision/algorithm/merec.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/moora.py` & `pyDecision-4.2.1/pyDecision/algorithm/moora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/moosra.py` & `pyDecision-4.2.1/pyDecision/algorithm/moosra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/multimoora.py` & `pyDecision-4.2.1/pyDecision/algorithm/multimoora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/ocra.py` & `pyDecision-4.2.1/pyDecision/algorithm/ocra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/oreste.py` & `pyDecision-4.2.1/pyDecision/algorithm/oreste.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/p_i.py` & `pyDecision-4.2.1/pyDecision/algorithm/p_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/p_ii.py` & `pyDecision-4.2.1/pyDecision/algorithm/p_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/p_iii.py` & `pyDecision-4.2.1/pyDecision/algorithm/p_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/p_iv.py` & `pyDecision-4.2.1/pyDecision/algorithm/p_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/p_v.py` & `pyDecision-4.2.1/pyDecision/algorithm/p_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/p_vi.py` & `pyDecision-4.2.1/pyDecision/algorithm/p_vi.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/p_xgaia.py` & `pyDecision-4.2.1/pyDecision/algorithm/p_xgaia.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/piv.py` & `pyDecision-4.2.1/pyDecision/algorithm/piv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/psi.py` & `pyDecision-4.2.1/pyDecision/algorithm/psi.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/regime.py` & `pyDecision-4.2.1/pyDecision/algorithm/regime.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/rov.py` & `pyDecision-4.2.1/pyDecision/algorithm/rov.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/saw.py` & `pyDecision-4.2.1/pyDecision/algorithm/saw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/smart.py` & `pyDecision-4.2.1/pyDecision/algorithm/smart.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/todim.py` & `pyDecision-4.2.1/pyDecision/algorithm/todim.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/topsis.py` & `pyDecision-4.2.1/pyDecision/algorithm/topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/vikor.py` & `pyDecision-4.2.1/pyDecision/algorithm/vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/waspas.py` & `pyDecision-4.2.1/pyDecision/algorithm/waspas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/algorithm/wings.py` & `pyDecision-4.2.1/pyDecision/algorithm/wings.py`

 * *Files identical despite different names*

### Comparing `pyDecision-4.2.0/pyDecision/compare/compare.py` & `pyDecision-4.2.1/pyDecision/compare/compare.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from pyDecision.algorithm.oreste       import oreste_method
 from pyDecision.algorithm.piv          import piv_method
 from pyDecision.algorithm.p_ii         import promethee_ii
 from pyDecision.algorithm.p_iv         import promethee_iv
 from pyDecision.algorithm.psi          import psi_method
 from pyDecision.algorithm.rov          import rov_method
 from pyDecision.algorithm.saw          import saw_method
+from pyDecision.algorithm.spotis       import spotis_method
 from pyDecision.algorithm.todim        import todim_method
 from pyDecision.algorithm.topsis       import topsis_method
 from pyDecision.algorithm.vikor        import vikor_method
 from pyDecision.algorithm.waspas       import waspas_method
 
 from pyDecision.algorithm.fuzzy_aras   import fuzzy_aras_method
 from pyDecision.algorithm.fuzzy_copras import fuzzy_copras_method
@@ -88,31 +89,47 @@
     ax.xaxis.set_major_locator(MaxNLocator(integer = True))
     ax.set_xlabel('Frequency')
     ax.set_ylabel('Alternative')
     ax.set_title('Rank Frequency per Alternative')
     plt.show()
     return
 
+# Function: Calc & Plot Correlation. correlation_method = 'kendall', correlation_method = 'spearman', correlation_method = 'pearson'
+def corr_viz(df, correlation_method = 'kendall', size = 10, font_size = 10, graph = True):
+    corr_df = df.corr(method = correlation_method)
+    if (graph == True):
+        plt.figure(figsize = (size, size))
+        cax = plt.matshow(corr_df, cmap = 'YlGnBu', fignum = 1)
+        plt.colorbar(cax)
+        plt.xticks(np.arange(len(corr_df.columns)), corr_df.columns, rotation = 90)
+        plt.yticks(np.arange(len(corr_df.columns)), corr_df.columns)
+        for i in range(len(corr_df.columns)):
+                    for j in range(len(corr_df.columns)):
+                        plt.gca().add_patch(plt.Rectangle((i-0.5, j-0.5), 1, 1, fill = False, edgecolor = 'black', lw = 0.2))
+        for (i, j), z in np.ndenumerate(corr_df):
+            plt.text(j, i, '{:0.2f}'.format(z), ha = 'center', va = 'center', fontsize = font_size, bbox = dict(boxstyle = 'round', facecolor = 'white', edgecolor = '0.1'))
+    return corr_df
+
 ###############################################################################
 
 # Function: Compare Weights
-def compare_weigths(dataset, criterion_type, custom_methods = [], custom_weigths = [], methods_list = [], mic = [], lic = [], size_bw = 50, iterations_bw = 150, size_ido = 20, iterations_ido = 1200):
+def compare_weigths(dataset, criterion_type, custom_methods = [], custom_weigths = [], methods_list = [], mic = [], lic = []):
     if ('all' in methods_list):
         methods_list = ['bwm', 'cilos', 'critic', 'idocriw', 'entropy',  'merec']
     if (len(custom_methods) > 0):
         methods_list = custom_methods + methods_list 
     X       = np.zeros((dataset.shape[1], len(methods_list)))
     j       = 0
     for i in range(0, len(custom_weigths)):
         X[:,j] = custom_weigths[i]
         j      = j + 1 
         print(custom_methods[i], ': Done!')
     for method in methods_list:
         if (method == 'bwm' or method == 'all'):
-            w      = bw_method(dataset, mic, lic, size_bw, iterations_bw, False)
+            w      = bw_method(dataset, mic, lic, False)
             X[:,j] = w
             j      = j + 1
             print('BWM: Done!')
         if (method == 'cilos' or method == 'all'):
             w      = cilos_method(dataset, criterion_type)
             X[:,j] = w
             j      = j + 1
@@ -124,30 +141,30 @@
             print('CRITIC: Done!')
         if (method == 'entropy' or method == 'all'):
             w      = entropy_method(dataset, criterion_type)
             X[:,j] = w
             j      = j + 1
             print('Entropy: Done!')
         if (method == 'idocriw' or method == 'all'):
-            w      = idocriw_method(dataset, criterion_type, size_ido, iterations_ido, False)
-            X[:,j] = w[:,0]
+            w      = idocriw_method(dataset, criterion_type, False)
+            X[:,j] = w
             j      = j + 1
             print('IDOCRIW: Done!')
         if (method == 'merec' or method == 'all'):
             w      = merec_method(dataset, criterion_type)
             X[:,j] = w
             j      = j + 1
             print('MEREC: Done!')
     X = pd.DataFrame(X, index = ['g'+str(i+1) for i in range(0, X.shape[0])], columns = methods_list)    
     return X
 
 # Function: Compare Ranks Crisp
-def compare_ranks_crisp(dataset, weights, criterion_type, utility_functions = [], custom_methods = [], custom_ranks = [], methods_list = [], L = 0.5, lmbd = 0.02, epsilon = 0.5, step_size = 1, teta = 1, strategy_coefficient = 0.5, Q = [], S = [], P = [], F = [], lambda_value = 0.5, alpha = 0.4):
+def compare_ranks_crisp(dataset, weights, criterion_type, utility_functions = [], custom_methods = [], custom_ranks = [], methods_list = [], L = 0.5, lmbd = 0.02, epsilon = 0.5, step_size = 1, teta = 1, strategy_coefficient = 0.5, Q = [], S = [], P = [], F = [], lambda_value = 0.5, alpha = 0.4, s_min = [], s_max = []):
     if ('all' in methods_list):
-        methods_list = ['aras', 'borda', 'cocoso', 'codas', 'copras', 'cradis', 'edas', 'gra', 'mabac', 'macbeth', 'mairca', 'marcos', 'maut', 'moora', 'moosra', 'multimoora', 'ocra', 'oreste', 'piv', 'promethee_ii', 'promethee_iv', 'psi', 'rov', 'saw', 'todim', 'topsis', 'vikor', 'wsm', 'wpm', 'waspas']
+        methods_list = ['aras', 'borda', 'cocoso', 'codas', 'copeland', 'copras', 'cradis', 'edas', 'gra', 'mabac', 'macbeth', 'mairca', 'marcos', 'maut', 'moora', 'moosra', 'multimoora', 'ocra', 'oreste', 'piv', 'promethee_ii', 'promethee_iv', 'psi', 'rov', 'saw', 'spotis', 'todim', 'topsis', 'vikor', 'wsm', 'wpm', 'waspas']
     if (len(custom_methods) > 0):
         methods_list = custom_methods + methods_list 
     graph   = False
     verbose = False
     X       = np.zeros((dataset.shape[0], len(methods_list)))
     j       = 0
     for i in range(0, len(custom_ranks)):
@@ -158,15 +175,15 @@
         if (method == 'aras' or method == 'all'):
             rank   = aras_method(dataset, weights, criterion_type, graph, verbose)
             X[:,j] = rank[:,1]
             j      = j + 1
             print('ARAS: Done!')
         if (method == 'borda' or method == 'all'):
             rank   = borda_method(dataset, criterion_type, graph, verbose)
-            X[:,j] = -rank
+            X[:,j] = rank
             j      = j + 1
             print('Borda: Done!')
         if (method == 'cocoso' or method == 'all'):
             rank   = cocoso_method(dataset, criterion_type, weights, L, graph, verbose)
             X[:,j] = rank
             j      = j + 1
             print('CoCoSo: Done!')
@@ -243,15 +260,15 @@
         if (method == 'ocra' or method == 'all'):
             rank   = ocra_method(dataset, weights, criterion_type, graph, verbose)
             X[:,j] = rank
             j      = j + 1
             print('OCRA: Done!')
         if (method == 'oreste' or method == 'all'):
             rank   = oreste_method(dataset, weights, criterion_type, alpha, graph, verbose)
-            X[:,j] = -rank
+            X[:,j] = rank
             j      = j + 1
             print('ORESTE: Done!')
         if (method == 'piv' or method == 'all'):
             rank   = piv_method(dataset, weights, criterion_type, graph, verbose)
             X[:,j] = rank
             j      = j + 1
             print('PIV: Done!')
@@ -284,14 +301,19 @@
             j      = j + 1
             print('ROV: Done!')
         if (method == 'saw' or method == 'all'):
             rank   = saw_method(dataset, criterion_type, weights, graph, verbose)
             X[:,j] = rank[:,1]
             j      = j + 1
             print('SAW: Done!')
+        if (method == 'spotis' or method == 'all'):
+            rank   = spotis_method(dataset, criterion_type, weights, s_min,s_max, graph, verbose)
+            X[:,j] = rank
+            j      = j + 1
+            print('SPOTIS: Done!')
         if (method == 'todim' or method == 'all'):
             rank   = todim_method(dataset, criterion_type, weights, teta, graph, verbose)
             X[:,j] = rank
             j      = j + 1
             print('TODIM: Done!')
         if (method == 'topsis' or method == 'all'):
             rank   = topsis_method(dataset, weights, criterion_type, graph, verbose)
@@ -315,16 +337,19 @@
             print('WPM: Done!')
         if (method == 'waspas' or method == 'all'):
             _, _, w = waspas_method(dataset, criterion_type, weights, lambda_value, graph)
             X[:,j] = w
             j      = j + 1
             print('WASPAS: Done!')
     ranked = np.zeros_like(X)
-    for i in range(0, X.shape[1]):
-        ranked[:, i] = X.shape[0] + 1 - rankdata(X[:, i], method = 'max')
+    for i in range(0, len(methods_list)):
+        if (methods_list[i] in ['borda', 'cradis', 'mairca', 'oreste', 'piv', 'spotis']):
+            ranked[:, i] = X.shape[0] + 1 - rankdata(-X[:, i], method = 'max')
+        else:
+            ranked[:, i] = X.shape[0] + 1 - rankdata(X[:, i], method = 'max')
     X      = pd.DataFrame(X, index = ['a'+str(i+1) for i in range(0, X.shape[0])], columns = methods_list)    
     ranked = pd.DataFrame(ranked, index = ['a'+str(i+1) for i in range(0, X.shape[0])], columns = methods_list)
     return X, ranked
 
 # Function: Compare Ranks Fuzzy
 def compare_ranks_fuzzy(dataset, weights, criterion_type, custom_methods = [], custom_ranks = [], methods_list = [], strategy_coefficient = 0.5):
     if ('all' in methods_list):
```

### Comparing `pyDecision-4.2.0/pyDecision/util/LLM.py` & `pyDecision-4.2.1/pyDecision/util/LLM.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,44 @@
 
 # Required Libraries
 import openai  
 
 ###############################################################################
 
 # Function: Ask GPT Rank
+def ask_chatgpt_corr(ranks, char_limit = 4097, api_key = 'your_api_key_here', query = 'which methods are more similar?', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
+    def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
+        try: 
+            response = openai.ChatCompletion.create(
+                                                    model      = model,
+                                                    messages   = [{'role': 'user', 'content': prompt}],
+                                                    max_tokens = max_tokens
+                                                    )
+            response = response['choices'][0]['message']['content']
+        except:
+            response = openai.Completion.create(
+                                                engine      = model,
+                                                prompt      = prompt,
+                                                max_tokens  = max_tokens,
+                                                n           = n,
+                                                stop        = None,
+                                                temperature = temperature
+                                                )
+            response = response.choices[0].text.strip()
+        return response
+    corpus         = ranks.to_string(index = False)
+    openai.api_key = api_key
+    context        = ' knowing that for the given table, it shows the correlation values between MCDA methods'
+    prompt         = query + context + ':\n\n' + f'{corpus}\n'
+    prompt         = prompt[:char_limit]
+    analyze        = query_chatgpt(prompt)
+    print('Number of Characters: ' + str(len(prompt)))
+    return analyze
+
+# Function: Ask GPT Rank
 def ask_chatgpt_rank(ranks, char_limit = 4097, api_key = 'your_api_key_here', query = 'which methods are more similar?', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
     def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
         try: 
             response = openai.ChatCompletion.create(
                                                     model      = model,
                                                     messages   = [{'role': 'user', 'content': prompt}],
                                                     max_tokens = max_tokens
```

### Comparing `pyDecision-4.2.0/pyDecision.egg-info/PKG-INFO` & `pyDecision-4.2.1/pyDecision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 4.2.0
+Version: 4.2.1
 Summary: A MCDA Library Incorporating Large Language Models to Enhance Decision Analysis
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **PSI** (Preference Selection Index); **Regime**; **ROV** (Range Of Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Fuzzy ARAS**; **Borda**; **BWM** (Best-Worst Method); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **CODAS** (Combinative Distance-based Assessment); **Copeland**; **COPRAS** (Complex PRoportional Assessment); **Fuzzy COPRAS**; **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **Entropy**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MACBETH** (Measuring Attractiveness by a Categorical Based Evaluation TecHnique); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **Fuzzy MOORA**; **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **Fuzzy OCRA** ; **ORESTE** (Organisation Rangement Et SynThesE de donnees relationnelles); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **Regime**; **ROV** (Range Of Value); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **SPOTIS** (Stable Preference Ordering Towards Ideal Solution), **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **PSI** (Preference Selection Index); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment). 
 
 pyDecision offers an array of features including the **comparison of ranking alternatives** and **comparison of criterion weights** from various methods. The library is also fully integrated with **chatGPT**, elevating result interpretation through AI. Additionally, pyDecision provides the flexibility to import results from custom methods or those not yet implemented in the library for swift comparison.
 
 ## Usage
 
 1. Install
 ```bash
@@ -115,14 +115,15 @@
 - PROMETHEE Gaia ([ Colab Demo ](https://colab.research.google.com/drive/1lj7IRKXcuRjrpoBp_KmQn_3sI3P_Qxju?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PIV ([ Colab Demo ](https://colab.research.google.com/drive/1PwJoBqYn1O2s22MqC9euP89Uyv4sedS0?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835218301360))
 - PSI ([ Colab Demo ](https://colab.research.google.com/drive/1u9tN8cYl2mx6KK6yLW2oz6fuVoy8xcCI?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0261306909006396))
 - Regime ([ Colab Demo ](https://colab.research.google.com/drive/1jcAcjAS92rxvE2urhc6HPixvzJ60HqEg?usp=sharing)) ( [ Paper ](https://link.springer.com/chapter/10.1007/978-3-030-15009-9_2))
 - ROV ([ Colab Demo ](https://colab.research.google.com/drive/1sQAPCem0pcS29uf6-n4TpncXMXNx9JDh?usp=sharing)) ( [ Paper ](https://doi.org/10.5267/j.dsl.2015.12.001))
 - SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
 - SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
+- SPOTIS ([ Colab Demo ](https://colab.research.google.com/drive/1TyjDn-xwut3w6Rf0zMiugdwytwmGY_NE?usp=sharing)) ( [ Paper ](https://doi.org/10.1002/mcda.1525))
 - TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0377221707010740))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
 - Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
 - VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_8))
 - Fuzzy VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1anfCnU2TSrW-Z5vMkS_qXFrYZ0ciQE53?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2011.04.097))
 - WINGS ([ Colab Demo ](https://colab.research.google.com/drive/1li1_cPxwEM3NOZ4hbI8RROXyOmXeoWew?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2013.02.007))
 - WSM, WPM, WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1HbLwXI4HkrmI-lsNzDtBOlCiwxfJltHi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_15))
```

### Comparing `pyDecision-4.2.0/pyDecision.egg-info/SOURCES.txt` & `pyDecision-4.2.1/pyDecision.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -60,18 +60,17 @@
 pyDecision/algorithm/p_xgaia.py
 pyDecision/algorithm/piv.py
 pyDecision/algorithm/psi.py
 pyDecision/algorithm/regime.py
 pyDecision/algorithm/rov.py
 pyDecision/algorithm/saw.py
 pyDecision/algorithm/smart.py
+pyDecision/algorithm/spotis.py
 pyDecision/algorithm/todim.py
 pyDecision/algorithm/topsis.py
 pyDecision/algorithm/vikor.py
 pyDecision/algorithm/waspas.py
 pyDecision/algorithm/wings.py
 pyDecision/compare/__init__.py
 pyDecision/compare/compare.py
 pyDecision/util/LLM.py
-pyDecision/util/__init__.py
-pyDecision/util/ga.py
-pyDecision/util/gwo.py
+pyDecision/util/__init__.py
```

### Comparing `pyDecision-4.2.0/setup.py` & `pyDecision-4.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyDecision',
-    version='4.2.0',
+    version='4.2.1',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyDecisions',
     packages=find_packages(),
     install_requires=[
         'matplotlib',
```

