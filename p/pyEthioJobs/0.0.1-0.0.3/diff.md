# Comparing `tmp/pyEthioJobs-0.0.1.tar.gz` & `tmp/pyEthioJobs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyEthioJobs-0.0.1.tar", last modified: Wed Aug  2 16:04:47 2023, max compression
+gzip compressed data, was "pyEthioJobs-0.0.3.tar", last modified: Wed Aug  2 16:23:54 2023, max compression
```

## Comparing `pyEthioJobs-0.0.1.tar` & `pyEthioJobs-0.0.3.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 16:04:47.079290 pyEthioJobs-0.0.1/
--rw-rw-rw-   0        0        0     1083 2023-07-31 11:01:26.000000 pyEthioJobs-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      142 2023-08-02 16:04:47.078299 pyEthioJobs-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2856 2023-04-15 12:26:55.000000 pyEthioJobs-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 16:04:46.816846 pyEthioJobs-0.0.1/pyEthioJobs.egg-info/
--rw-rw-rw-   0        0        0      142 2023-08-02 16:04:46.000000 pyEthioJobs-0.0.1/pyEthioJobs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1589 2023-08-02 16:04:46.000000 pyEthioJobs-0.0.1/pyEthioJobs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 16:04:46.000000 pyEthioJobs-0.0.1/pyEthioJobs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-08-02 16:04:46.000000 pyEthioJobs-0.0.1/pyEthioJobs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-02 16:04:46.848311 pyEthioJobs-0.0.1/pyethiojobs/
--rw-rw-rw-   0        0        0       35 2022-08-23 12:36:17.000000 pyEthioJobs-0.0.1/pyethiojobs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:04:46.855311 pyEthioJobs-0.0.1/pyethiojobs/errors/
--rw-rw-rw-   0        0        0      153 2023-07-31 10:59:34.000000 pyEthioJobs-0.0.1/pyethiojobs/errors/__init__.py
--rw-rw-rw-   0        0        0     3693 2023-04-10 07:51:27.000000 pyEthioJobs-0.0.1/pyethiojobs/filters.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:04:46.870311 pyEthioJobs-0.0.1/pyethiojobs/handler/
--rw-rw-rw-   0        0        0       45 2022-08-13 17:02:28.000000 pyEthioJobs-0.0.1/pyethiojobs/handler/__init__.py
--rw-rw-rw-   0        0        0     1105 2023-04-15 08:15:09.000000 pyEthioJobs-0.0.1/pyethiojobs/handler/handlers_holder.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:04:46.877328 pyEthioJobs-0.0.1/pyethiojobs/methods/
--rw-rw-rw-   0        0        0      239 2023-04-15 08:47:35.000000 pyEthioJobs-0.0.1/pyethiojobs/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:04:46.898373 pyEthioJobs-0.0.1/pyethiojobs/methods/category/
--rw-rw-rw-   0        0        0      143 2022-08-23 13:33:07.000000 pyEthioJobs-0.0.1/pyethiojobs/methods/category/__init__.py
--rw-rw-rw-   0        0        0      799 2022-11-05 07:40:34.000000 pyEthioJobs-0.0.1/pyethiojobs/methods/category/get_categories.py
--rw-rw-rw-   0        0        0      582 2022-08-23 12:09:41.000000 pyEthioJobs-0.0.1/pyethiojobs/methods/category/get_category.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:04:46.911975 pyEthioJobs-0.0.1/pyethiojobs/methods/decorators/
--rw-rw-rw-   0        0        0       72 2023-04-15 08:39:30.000000 pyEthioJobs-0.0.1/pyethiojobs/methods/decorators/__init__.py
--rw-rw-rw-   0        0        0      881 2023-04-10 07:57:37.000000 pyEthioJobs-0.0.1/pyethiojobs/methods/decorators/on_new_job.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:04:46.933303 pyEthioJobs-0.0.1/pyethiojobs/methods/gov/
--rw-rw-rw-   0        0        0      161 2022-11-05 12:53:06.000000 pyEthioJobs-0.0.1/pyethiojobs/methods/gov/__init__.py
--rw-rw-rw-   0        0        0     1590 2022-11-05 16:45:01.000000 pyEthioJobs-0.0.1/pyethiojobs/methods/gov/get_gov_job_details.py
--rw-rw-rw-   0        0        0     1014 2022-11-05 12:51:10.000000 pyEthioJobs-0.0.1/pyethiojobs/methods/gov/get_gov_jobs.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:04:46.944127 pyEthioJobs-0.0.1/pyethiojobs/methods/job/
--rw-rw-rw-   0        0        0      117 2023-07-31 14:36:54.000000 pyEthioJobs-0.0.1/pyethiojobs/methods/job/__init__.py
--rw-rw-rw-   0        0        0      469 2023-07-31 10:54:54.000000 pyEthioJobs-0.0.1/pyethiojobs/methods/job/get_job.py
--rw-rw-rw-   0        0        0     2626 2023-07-31 18:09:49.000000 pyEthioJobs-0.0.1/pyethiojobs/methods/job/get_latest_jobs.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:04:46.957402 pyEthioJobs-0.0.1/pyethiojobs/methods/search/
--rw-rw-rw-   0        0        0       66 2022-08-23 13:33:40.000000 pyEthioJobs-0.0.1/pyethiojobs/methods/search/__init__.py
--rw-rw-rw-   0        0        0     1019 2023-04-15 12:02:43.000000 pyEthioJobs-0.0.1/pyethiojobs/methods/search/search.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:04:46.986708 pyEthioJobs-0.0.1/pyethiojobs/methods/utlis/
--rw-rw-rw-   0        0        0      155 2023-04-15 08:34:22.000000 pyEthioJobs-0.0.1/pyethiojobs/methods/utlis/__init__.py
--rw-rw-rw-   0        0        0     2605 2023-08-02 13:57:40.000000 pyEthioJobs-0.0.1/pyethiojobs/methods/utlis/get_job_detail.py
--rw-rw-rw-   0        0        0     2659 2023-07-31 18:56:17.000000 pyEthioJobs-0.0.1/pyethiojobs/methods/utlis/get_jobs.py
--rw-rw-rw-   0        0        0     1247 2023-04-15 09:20:19.000000 pyEthioJobs-0.0.1/pyethiojobs/methods/utlis/run.py
--rw-rw-rw-   0        0        0     1240 2023-07-31 11:00:30.000000 pyEthioJobs-0.0.1/pyethiojobs/pyethiojobs.py
--rw-rw-rw-   0        0        0     3329 2023-07-31 10:56:03.000000 pyEthioJobs-0.0.1/pyethiojobs/scaffold.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:04:46.994960 pyEthioJobs-0.0.1/pyethiojobs/types/
--rw-rw-rw-   0        0        0      316 2023-04-10 07:14:55.000000 pyEthioJobs-0.0.1/pyethiojobs/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:04:47.006973 pyEthioJobs-0.0.1/pyethiojobs/types/category/
--rw-rw-rw-   0        0        0       32 2022-08-21 18:57:29.000000 pyEthioJobs-0.0.1/pyethiojobs/types/category/__init__.py
--rw-rw-rw-   0        0        0      377 2022-11-04 18:31:26.000000 pyEthioJobs-0.0.1/pyethiojobs/types/category/category.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:04:47.020147 pyEthioJobs-0.0.1/pyethiojobs/types/employment/
--rw-rw-rw-   0        0        0       44 2023-04-10 07:14:02.000000 pyEthioJobs-0.0.1/pyethiojobs/types/employment/__init__.py
--rw-rw-rw-   0        0        0      136 2023-04-10 07:26:47.000000 pyEthioJobs-0.0.1/pyethiojobs/types/employment/employment_type.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:04:47.076297 pyEthioJobs-0.0.1/pyethiojobs/types/jobs/
--rw-rw-rw-   0        0        0      231 2022-11-05 11:45:09.000000 pyEthioJobs-0.0.1/pyethiojobs/types/jobs/__init__.py
--rw-rw-rw-   0        0        0      652 2023-04-10 05:37:48.000000 pyEthioJobs-0.0.1/pyethiojobs/types/jobs/gov_job.py
--rw-rw-rw-   0        0        0      526 2022-11-05 15:24:04.000000 pyEthioJobs-0.0.1/pyethiojobs/types/jobs/gov_job_details.py
--rw-rw-rw-   0        0        0      112 2022-08-21 18:58:28.000000 pyEthioJobs-0.0.1/pyethiojobs/types/jobs/identifier.py
--rw-rw-rw-   0        0        0     1450 2023-07-31 18:07:17.000000 pyEthioJobs-0.0.1/pyethiojobs/types/jobs/job.py
--rw-rw-rw-   0        0        0     1082 2022-11-05 16:29:18.000000 pyEthioJobs-0.0.1/pyethiojobs/types/jobs/job_details.py
--rw-rw-rw-   0        0        0      203 2022-11-05 12:24:40.000000 pyEthioJobs-0.0.1/pyethiojobs/types/jobs/job_type.py
--rw-rw-rw-   0        0        0      296 2022-08-21 19:07:53.000000 pyEthioJobs-0.0.1/pyethiojobs/types/jobs/location.py
--rw-rw-rw-   0        0        0       85 2022-08-23 16:09:19.000000 pyEthioJobs-0.0.1/pyethiojobs/utils.py
--rw-rw-rw-   0        0        0       42 2023-08-02 16:04:47.079290 pyEthioJobs-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      235 2022-08-23 13:29:45.000000 pyEthioJobs-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.714229 pyEthioJobs-0.0.3/
+-rw-rw-rw-   0        0        0     1083 2023-07-31 11:01:26.000000 pyEthioJobs-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3140 2023-08-02 16:23:54.713221 pyEthioJobs-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2856 2023-04-15 12:26:55.000000 pyEthioJobs-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.662981 pyEthioJobs-0.0.3/pyEthioJobs.egg-info/
+-rw-rw-rw-   0        0        0     3140 2023-08-02 16:23:54.000000 pyEthioJobs-0.0.3/pyEthioJobs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1623 2023-08-02 16:23:54.000000 pyEthioJobs-0.0.3/pyEthioJobs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 16:23:54.000000 pyEthioJobs-0.0.3/pyEthioJobs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-02 16:23:54.000000 pyEthioJobs-0.0.3/pyEthioJobs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-02 16:23:54.000000 pyEthioJobs-0.0.3/pyEthioJobs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.677224 pyEthioJobs-0.0.3/pyethiojobs/
+-rw-rw-rw-   0        0        0       35 2022-08-23 12:36:17.000000 pyEthioJobs-0.0.3/pyethiojobs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.677224 pyEthioJobs-0.0.3/pyethiojobs/errors/
+-rw-rw-rw-   0        0        0      153 2023-07-31 10:59:34.000000 pyEthioJobs-0.0.3/pyethiojobs/errors/__init__.py
+-rw-rw-rw-   0        0        0     3693 2023-04-10 07:51:27.000000 pyEthioJobs-0.0.3/pyethiojobs/filters.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.679231 pyEthioJobs-0.0.3/pyethiojobs/handler/
+-rw-rw-rw-   0        0        0       45 2022-08-13 17:02:28.000000 pyEthioJobs-0.0.3/pyethiojobs/handler/__init__.py
+-rw-rw-rw-   0        0        0     1105 2023-04-15 08:15:09.000000 pyEthioJobs-0.0.3/pyethiojobs/handler/handlers_holder.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.680218 pyEthioJobs-0.0.3/pyethiojobs/methods/
+-rw-rw-rw-   0        0        0      239 2023-04-15 08:47:35.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.682222 pyEthioJobs-0.0.3/pyethiojobs/methods/category/
+-rw-rw-rw-   0        0        0      143 2022-08-23 13:33:07.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/category/__init__.py
+-rw-rw-rw-   0        0        0      799 2022-11-05 07:40:34.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/category/get_categories.py
+-rw-rw-rw-   0        0        0      582 2022-08-23 12:09:41.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/category/get_category.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.684223 pyEthioJobs-0.0.3/pyethiojobs/methods/decorators/
+-rw-rw-rw-   0        0        0       72 2023-04-15 08:39:30.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/decorators/__init__.py
+-rw-rw-rw-   0        0        0      881 2023-04-10 07:57:37.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/decorators/on_new_job.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.686223 pyEthioJobs-0.0.3/pyethiojobs/methods/gov/
+-rw-rw-rw-   0        0        0      161 2022-11-05 12:53:06.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/gov/__init__.py
+-rw-rw-rw-   0        0        0     1590 2022-11-05 16:45:01.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/gov/get_gov_job_details.py
+-rw-rw-rw-   0        0        0     1014 2022-11-05 12:51:10.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/gov/get_gov_jobs.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.690225 pyEthioJobs-0.0.3/pyethiojobs/methods/job/
+-rw-rw-rw-   0        0        0      117 2023-07-31 14:36:54.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/job/__init__.py
+-rw-rw-rw-   0        0        0      469 2023-07-31 10:54:54.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/job/get_job.py
+-rw-rw-rw-   0        0        0     2626 2023-07-31 18:09:49.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/job/get_latest_jobs.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.693228 pyEthioJobs-0.0.3/pyethiojobs/methods/search/
+-rw-rw-rw-   0        0        0       66 2022-08-23 13:33:40.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/search/__init__.py
+-rw-rw-rw-   0        0        0     1019 2023-04-15 12:02:43.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/search/search.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.696233 pyEthioJobs-0.0.3/pyethiojobs/methods/utlis/
+-rw-rw-rw-   0        0        0      155 2023-04-15 08:34:22.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/utlis/__init__.py
+-rw-rw-rw-   0        0        0     2605 2023-08-02 13:57:40.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/utlis/get_job_detail.py
+-rw-rw-rw-   0        0        0     2659 2023-07-31 18:56:17.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/utlis/get_jobs.py
+-rw-rw-rw-   0        0        0     1247 2023-04-15 09:20:19.000000 pyEthioJobs-0.0.3/pyethiojobs/methods/utlis/run.py
+-rw-rw-rw-   0        0        0     1240 2023-07-31 11:00:30.000000 pyEthioJobs-0.0.3/pyethiojobs/pyethiojobs.py
+-rw-rw-rw-   0        0        0     3329 2023-07-31 10:56:03.000000 pyEthioJobs-0.0.3/pyethiojobs/scaffold.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.697219 pyEthioJobs-0.0.3/pyethiojobs/types/
+-rw-rw-rw-   0        0        0      316 2023-04-10 07:14:55.000000 pyEthioJobs-0.0.3/pyethiojobs/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.698223 pyEthioJobs-0.0.3/pyethiojobs/types/category/
+-rw-rw-rw-   0        0        0       32 2022-08-21 18:57:29.000000 pyEthioJobs-0.0.3/pyethiojobs/types/category/__init__.py
+-rw-rw-rw-   0        0        0      377 2022-11-04 18:31:26.000000 pyEthioJobs-0.0.3/pyethiojobs/types/category/category.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.700223 pyEthioJobs-0.0.3/pyethiojobs/types/employment/
+-rw-rw-rw-   0        0        0       44 2023-04-10 07:14:02.000000 pyEthioJobs-0.0.3/pyethiojobs/types/employment/__init__.py
+-rw-rw-rw-   0        0        0      136 2023-04-10 07:26:47.000000 pyEthioJobs-0.0.3/pyethiojobs/types/employment/employment_type.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:23:54.711221 pyEthioJobs-0.0.3/pyethiojobs/types/jobs/
+-rw-rw-rw-   0        0        0      231 2022-11-05 11:45:09.000000 pyEthioJobs-0.0.3/pyethiojobs/types/jobs/__init__.py
+-rw-rw-rw-   0        0        0      652 2023-04-10 05:37:48.000000 pyEthioJobs-0.0.3/pyethiojobs/types/jobs/gov_job.py
+-rw-rw-rw-   0        0        0      526 2022-11-05 15:24:04.000000 pyEthioJobs-0.0.3/pyethiojobs/types/jobs/gov_job_details.py
+-rw-rw-rw-   0        0        0      112 2022-08-21 18:58:28.000000 pyEthioJobs-0.0.3/pyethiojobs/types/jobs/identifier.py
+-rw-rw-rw-   0        0        0     1450 2023-07-31 18:07:17.000000 pyEthioJobs-0.0.3/pyethiojobs/types/jobs/job.py
+-rw-rw-rw-   0        0        0     1082 2022-11-05 16:29:18.000000 pyEthioJobs-0.0.3/pyethiojobs/types/jobs/job_details.py
+-rw-rw-rw-   0        0        0      203 2022-11-05 12:24:40.000000 pyEthioJobs-0.0.3/pyethiojobs/types/jobs/job_type.py
+-rw-rw-rw-   0        0        0      296 2022-08-21 19:07:53.000000 pyEthioJobs-0.0.3/pyethiojobs/types/jobs/location.py
+-rw-rw-rw-   0        0        0       85 2022-08-23 16:09:19.000000 pyEthioJobs-0.0.3/pyethiojobs/utils.py
+-rw-rw-rw-   0        0        0       42 2023-08-02 16:23:54.714229 pyEthioJobs-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      580 2023-08-02 16:23:37.000000 pyEthioJobs-0.0.3/setup.py
```

### Comparing `pyEthioJobs-0.0.1/LICENSE` & `pyEthioJobs-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.1/README.md` & `pyEthioJobs-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.1/pyEthioJobs.egg-info/SOURCES.txt` & `pyEthioJobs-0.0.3/pyEthioJobs.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.py
 pyEthioJobs.egg-info/PKG-INFO
 pyEthioJobs.egg-info/SOURCES.txt
 pyEthioJobs.egg-info/dependency_links.txt
+pyEthioJobs.egg-info/requires.txt
 pyEthioJobs.egg-info/top_level.txt
 pyethiojobs/__init__.py
 pyethiojobs/filters.py
 pyethiojobs/pyethiojobs.py
 pyethiojobs/scaffold.py
 pyethiojobs/utils.py
 pyethiojobs/errors/__init__.py
```

### Comparing `pyEthioJobs-0.0.1/pyethiojobs/filters.py` & `pyEthioJobs-0.0.3/pyethiojobs/filters.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.1/pyethiojobs/handler/handlers_holder.py` & `pyEthioJobs-0.0.3/pyethiojobs/handler/handlers_holder.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.1/pyethiojobs/methods/category/get_categories.py` & `pyEthioJobs-0.0.3/pyethiojobs/methods/category/get_categories.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.1/pyethiojobs/methods/category/get_category.py` & `pyEthioJobs-0.0.3/pyethiojobs/methods/category/get_category.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.1/pyethiojobs/methods/decorators/on_new_job.py` & `pyEthioJobs-0.0.3/pyethiojobs/methods/decorators/on_new_job.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.1/pyethiojobs/methods/gov/get_gov_job_details.py` & `pyEthioJobs-0.0.3/pyethiojobs/methods/gov/get_gov_job_details.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.1/pyethiojobs/methods/gov/get_gov_jobs.py` & `pyEthioJobs-0.0.3/pyethiojobs/methods/gov/get_gov_jobs.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.1/pyethiojobs/methods/job/get_latest_jobs.py` & `pyEthioJobs-0.0.3/pyethiojobs/methods/job/get_latest_jobs.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.1/pyethiojobs/methods/search/search.py` & `pyEthioJobs-0.0.3/pyethiojobs/methods/search/search.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.1/pyethiojobs/methods/utlis/get_job_detail.py` & `pyEthioJobs-0.0.3/pyethiojobs/methods/utlis/get_job_detail.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.1/pyethiojobs/methods/utlis/get_jobs.py` & `pyEthioJobs-0.0.3/pyethiojobs/methods/utlis/get_jobs.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.1/pyethiojobs/methods/utlis/run.py` & `pyEthioJobs-0.0.3/pyethiojobs/methods/utlis/run.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.1/pyethiojobs/pyethiojobs.py` & `pyEthioJobs-0.0.3/pyethiojobs/pyethiojobs.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.1/pyethiojobs/scaffold.py` & `pyEthioJobs-0.0.3/pyethiojobs/scaffold.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.1/pyethiojobs/types/jobs/gov_job.py` & `pyEthioJobs-0.0.3/pyethiojobs/types/jobs/gov_job.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.1/pyethiojobs/types/jobs/gov_job_details.py` & `pyEthioJobs-0.0.3/pyethiojobs/types/jobs/gov_job_details.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.1/pyethiojobs/types/jobs/job.py` & `pyEthioJobs-0.0.3/pyethiojobs/types/jobs/job.py`

 * *Files identical despite different names*

### Comparing `pyEthioJobs-0.0.1/pyethiojobs/types/jobs/job_details.py` & `pyEthioJobs-0.0.3/pyethiojobs/types/jobs/job_details.py`

 * *Files identical despite different names*

