# Comparing `tmp/pyapep-0.1.3.tar.gz` & `tmp/pyapep-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyapep-0.1.3.tar", last modified: Mon Jul 31 17:52:40 2023, max compression
+gzip compressed data, was "dist\pyapep-0.1.4.tar", last modified: Wed Aug  2 04:29:33 2023, max compression
```

## Comparing `pyapep-0.1.3.tar` & `pyapep-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 17:52:40.550582 pyapep-0.1.3/
--rw-rw-rw-   0        0        0      329 2023-07-31 17:52:40.548582 pyapep-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      367 2022-05-27 15:52:19.000000 pyapep-0.1.3/README
-drwxrwxrwx   0        0        0        0 2023-07-31 17:52:40.536204 pyapep-0.1.3/pyAPEP/
--rw-rw-rw-   0        0        0     2453 2023-07-31 17:47:14.000000 pyapep-0.1.3/pyAPEP/Test_run_ma_linvel_blowdown.py
--rw-rw-rw-   0        0        0     2460 2023-07-31 17:47:14.000000 pyapep-0.1.3/pyAPEP/Test_run_ma_linvel_blowdown_reverse.py
--rw-rw-rw-   0        0        0     2369 2023-07-31 17:47:14.000000 pyapep-0.1.3/pyAPEP/Test_run_ma_linvel_flowthrough.py
--rw-rw-rw-   0        0        0     2380 2023-07-31 17:47:14.000000 pyapep-0.1.3/pyAPEP/Test_run_ma_linvel_flowthrough_reverse.py
--rw-rw-rw-   0        0        0     2459 2023-07-31 17:47:14.000000 pyapep-0.1.3/pyAPEP/Test_run_ma_linvel_pressurization.py
--rw-rw-rw-   0        0        0     2460 2023-07-31 17:47:14.000000 pyapep-0.1.3/pyAPEP/Test_run_ma_linvel_pressurization_reverse.py
--rw-rw-rw-   0        0        0        0 2023-07-31 17:47:14.000000 pyapep-0.1.3/pyAPEP/__init__.py
--rw-rw-rw-   0        0        0    22187 2023-07-31 17:47:14.000000 pyapep-0.1.3/pyAPEP/isofit.py
--rw-rw-rw-   0        0        0     8353 2023-07-31 17:47:14.000000 pyapep-0.1.3/pyAPEP/simide.py
--rw-rw-rw-   0        0        0   140667 2023-07-31 17:47:14.000000 pyapep-0.1.3/pyAPEP/simsep.py
--rw-rw-rw-   0        0        0    87603 2023-07-31 17:47:14.000000 pyapep-0.1.3/pyAPEP/simsep_backup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 17:52:40.546581 pyapep-0.1.3/pyapep.egg-info/
--rw-rw-rw-   0        0        0      329 2023-07-31 17:52:39.000000 pyapep-0.1.3/pyapep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-07-31 17:52:40.000000 pyapep-0.1.3/pyapep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 17:52:39.000000 pyapep-0.1.3/pyapep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-31 17:52:39.000000 pyapep-0.1.3/pyapep.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-31 17:52:39.000000 pyapep-0.1.3/pyapep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 17:52:40.550582 pyapep-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      908 2023-07-31 17:51:55.000000 pyapep-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:29:33.025473 pyapep-0.1.4/
+-rw-rw-rw-   0        0        0      338 2023-08-02 04:29:33.024476 pyapep-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-08-01 01:00:30.000000 pyapep-0.1.4/README
+drwxrwxrwx   0        0        0        0 2023-08-02 04:29:32.989569 pyapep-0.1.4/pyAPEP/
+-rw-rw-rw-   0        0        0     2453 2023-08-01 01:00:30.000000 pyapep-0.1.4/pyAPEP/Test_run_ma_linvel_blowdown.py
+-rw-rw-rw-   0        0        0     2484 2023-08-02 04:25:21.000000 pyapep-0.1.4/pyAPEP/Test_run_ma_linvel_blowdown_reverse.py
+-rw-rw-rw-   0        0        0     2369 2023-08-01 01:00:30.000000 pyapep-0.1.4/pyAPEP/Test_run_ma_linvel_flowthrough.py
+-rw-rw-rw-   0        0        0     2378 2023-08-02 04:26:09.000000 pyapep-0.1.4/pyAPEP/Test_run_ma_linvel_flowthrough_reverse.py
+-rw-rw-rw-   0        0        0     2459 2023-08-01 01:00:30.000000 pyapep-0.1.4/pyAPEP/Test_run_ma_linvel_pressurization.py
+-rw-rw-rw-   0        0        0     2481 2023-08-02 04:27:11.000000 pyapep-0.1.4/pyAPEP/Test_run_ma_linvel_pressurization_reverse.py
+-rw-rw-rw-   0        0        0        0 2023-08-01 01:00:30.000000 pyapep-0.1.4/pyAPEP/__init__.py
+-rw-rw-rw-   0        0        0    22187 2023-08-01 01:00:30.000000 pyapep-0.1.4/pyAPEP/isofit.py
+-rw-rw-rw-   0        0        0     8353 2023-08-01 01:00:30.000000 pyapep-0.1.4/pyAPEP/simide.py
+-rw-rw-rw-   0        0        0   140865 2023-08-02 04:24:54.000000 pyapep-0.1.4/pyAPEP/simsep.py
+-rw-rw-rw-   0        0        0    87603 2023-08-01 01:00:30.000000 pyapep-0.1.4/pyAPEP/simsep_backup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:29:33.022483 pyapep-0.1.4/pyapep.egg-info/
+-rw-rw-rw-   0        0        0      338 2023-08-02 04:29:32.000000 pyapep-0.1.4/pyapep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-08-02 04:29:32.000000 pyapep-0.1.4/pyapep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 04:29:32.000000 pyapep-0.1.4/pyapep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-08-02 04:29:32.000000 pyapep-0.1.4/pyapep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-02 04:29:32.000000 pyapep-0.1.4/pyapep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 04:29:33.025473 pyapep-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      908 2023-08-02 04:28:19.000000 pyapep-0.1.4/setup.py
```

### Comparing `pyapep-0.1.3/pyAPEP/Test_run_ma_linvel_blowdown.py` & `pyapep-0.1.4/pyAPEP/Test_run_ma_linvel_blowdown.py`

 * *Files identical despite different names*

### Comparing `pyapep-0.1.3/pyAPEP/Test_run_ma_linvel_blowdown_reverse.py` & `pyapep-0.1.4/pyAPEP/Test_run_ma_linvel_blowdown_reverse.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,17 @@
 c1.Graph(20, 0)
 # %%
 c1.Graph(20, 1)
 # %%
 c1.Graph(20,2)
 # %%
 c1.Graph(10,5, )
+
+# %%
+c1.Graph_P(10)
 # %%
 plt.plot(c1._z, c1._y_fra[0][0,:N])
 plt.plot(c1._z, c1._y_fra[0][1,:N])
 plt.plot(c1._z, c1._y_fra[0][20,:N])
 plt.plot(c1._z, c1._y_fra[1][0, :N])
 plt.plot(c1._z, c1._y_fra[1][20, :N])
 # %%
```

### Comparing `pyapep-0.1.3/pyAPEP/Test_run_ma_linvel_flowthrough.py` & `pyapep-0.1.4/pyAPEP/Test_run_ma_linvel_flowthrough.py`

 * *Files identical despite different names*

### Comparing `pyapep-0.1.3/pyAPEP/Test_run_ma_linvel_flowthrough_reverse.py` & `pyapep-0.1.4/pyAPEP/Test_run_ma_linvel_flowthrough_reverse.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 y_res, z_res, t_res = c1.run_ma_linvel(100,10)
 c1.Graph(20, 0)
 # %%
 c1.Graph(20, 1)
 # %%
 c1.Graph(20,2)
 # %%
-c1.Graph(10,1, )
+c1.Graph_P(10)
 # %%
 '''
 plt.plot(c1._z, c1._y_fra[0][0,:N])
 plt.plot(c1._z, c1._y_fra[0][1,:N])
 plt.plot(c1._z, c1._y_fra[0][20,:N])
 plt.plot(c1._z, c1._y_fra[1][0, :N])
 plt.plot(c1._z, c1._y_fra[1][20, :N])
```

### Comparing `pyapep-0.1.3/pyAPEP/Test_run_ma_linvel_pressurization.py` & `pyapep-0.1.4/pyAPEP/Test_run_ma_linvel_pressurization.py`

 * *Files identical despite different names*

### Comparing `pyapep-0.1.3/pyAPEP/Test_run_ma_linvel_pressurization_reverse.py` & `pyapep-0.1.4/pyAPEP/Test_run_ma_linvel_pressurization_reverse.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,13 +93,15 @@
 # %%
 c1.Graph(20, 1)
 # %%
 c1.Graph(20,2)
 # %%
 c1.Graph(10,5, )
 # %%
+c1.Graph_P(2)
+# %%
 plt.plot(c1._z, c1._y_fra[0][0,:N])
 plt.plot(c1._z, c1._y_fra[0][1,:N])
 plt.plot(c1._z, c1._y_fra[0][20,:N])
 plt.plot(c1._z, c1._y_fra[1][0, :N])
 plt.plot(c1._z, c1._y_fra[1][20, :N])
 # %%
```

### Comparing `pyapep-0.1.3/pyAPEP/isofit.py` & `pyapep-0.1.4/pyAPEP/isofit.py`

 * *Files identical despite different names*

### Comparing `pyapep-0.1.3/pyAPEP/simide.py` & `pyapep-0.1.4/pyAPEP/simide.py`

 * *Files identical despite different names*

### Comparing `pyapep-0.1.3/pyAPEP/simsep.py` & `pyapep-0.1.4/pyAPEP/simsep.py`

 * *Files 0% similar despite different names*

```diff
@@ -1925,14 +1925,15 @@
             Ts_tmp = T_feed*np.ones([len(t_dom), N])
             y_result = np.concatenate(C_tmp + q_tmp + [Tg_tmp, Ts_tmp], axis=1)
             self._y = y_result
             self._t = t_dom
 
             toc = time.time()/60 - tic
             self._CPU_min = toc
+            self._Tg_res = y_result[:,n_comp*2*N : n_comp*2*N+N]
             if CPUtime_print:
                 print('Simulation of this step is completed.')
                 print('This took {0:9.3f} mins to run. \n'.format(toc))
             
             return y_result, self._z, t_dom
 
         # Pressurization (open inlet only)
@@ -2087,14 +2088,15 @@
             Ts_tmp = T_feed*np.ones([len(t_dom), N])
             y_result = np.concatenate(C_tmp + q_tmp + [Tg_tmp, Ts_tmp], axis=1)
             self._y = y_result
             self._t = t_dom
 
             toc = time.time()/60 - tic
             self._CPU_min = toc
+            self._Tg_res = y_result[:,n_comp*2*N : n_comp*2*N+N]
             if CPUtime_print:
                 print('Simulation of this step is completed.')
                 print('This took {0:9.3f} mins to run. \n'.format(toc))
 
             return y_result, self._z, t_dom
         
         # Depressurization (=Blowdown) (Open outlet only)
@@ -2250,14 +2252,15 @@
             Ts_tmp = T_feed*np.ones([len(t_dom), N])
             y_result = np.concatenate(C_tmp + q_tmp + [Tg_tmp, Ts_tmp], axis=1)
             self._y = y_result
             self._t = t_dom
 
             toc = time.time()/60 - tic
             self._CPU_min = toc
+            self._Tg_res = y_result[:,n_comp*2*N : n_comp*2*N+N]
             if CPUtime_print:
                 print('Simulation of this step is completed.')
                 print('This took {0:9.3f} mins to run. \n'.format(toc))
 
             return y_result, self._z, t_dom
```

### Comparing `pyapep-0.1.3/pyAPEP/simsep_backup.py` & `pyapep-0.1.4/pyAPEP/simsep_backup.py`

 * *Files identical despite different names*

### Comparing `pyapep-0.1.3/pyapep.egg-info/SOURCES.txt` & `pyapep-0.1.4/pyapep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyapep-0.1.3/setup.py` & `pyapep-0.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
         name='pyapep',
-        version='0.1.3',
+        version='0.1.4',
         author_email='sgasga@ulsan.ac.kr',
         description='Python package for adsorption process simulations',
         long_description_content_type='text/markdown',
         url='https://sebygaa.github.io/pyAPEP/',
         packages=setuptools.find_packages(),
         classifieres=[
             'Programming Language :: Python :: 3',
```

