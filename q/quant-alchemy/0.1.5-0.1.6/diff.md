# Comparing `tmp/quant-alchemy-0.1.5.tar.gz` & `tmp/quant-alchemy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\quant-alchemy-0.1.5.tar", last modified: Tue Aug  1 22:19:25 2023, max compression
+gzip compressed data, was "quant-alchemy-0.1.6.tar", last modified: Tue Aug  1 23:48:46 2023, max compression
```

## Comparing `quant-alchemy-0.1.5.tar` & `quant-alchemy-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 22:19:25.630711 quant-alchemy-0.1.5/
--rw-rw-rw-   0        0        0      400 2023-08-01 22:19:25.629710 quant-alchemy-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-07-07 18:15:03.000000 quant-alchemy-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 22:19:25.622259 quant-alchemy-0.1.5/quant_alchemy/
--rw-rw-rw-   0        0        0       94 2023-07-26 18:55:50.000000 quant-alchemy-0.1.5/quant_alchemy/__init__.py
--rw-rw-rw-   0        0        0     3572 2023-07-12 19:45:17.000000 quant-alchemy-0.1.5/quant_alchemy/portfolio.py
--rw-rw-rw-   0        0        0    16024 2023-08-01 20:57:12.000000 quant-alchemy-0.1.5/quant_alchemy/timeseries.py
-drwxrwxrwx   0        0        0        0 2023-08-01 22:19:25.628708 quant-alchemy-0.1.5/quant_alchemy.egg-info/
--rw-rw-rw-   0        0        0      400 2023-08-01 22:19:25.000000 quant-alchemy-0.1.5/quant_alchemy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-08-01 22:19:25.000000 quant-alchemy-0.1.5/quant_alchemy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 22:19:25.000000 quant-alchemy-0.1.5/quant_alchemy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-08-01 22:19:25.000000 quant-alchemy-0.1.5/quant_alchemy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-08-01 22:19:25.000000 quant-alchemy-0.1.5/quant_alchemy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 22:19:25.630711 quant-alchemy-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      658 2023-08-01 22:19:22.000000 quant-alchemy-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 23:48:46.854793 quant-alchemy-0.1.6/
+-rw-rw-rw-   0        0        0      400 2023-08-01 23:48:46.853798 quant-alchemy-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-07-07 18:15:03.000000 quant-alchemy-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 23:48:46.847797 quant-alchemy-0.1.6/quant_alchemy/
+-rw-rw-rw-   0        0        0       94 2023-07-26 18:55:50.000000 quant-alchemy-0.1.6/quant_alchemy/__init__.py
+-rw-rw-rw-   0        0        0     3572 2023-07-12 19:45:17.000000 quant-alchemy-0.1.6/quant_alchemy/portfolio.py
+-rw-rw-rw-   0        0        0    16021 2023-08-01 23:45:46.000000 quant-alchemy-0.1.6/quant_alchemy/timeseries.py
+drwxrwxrwx   0        0        0        0 2023-08-01 23:48:46.852797 quant-alchemy-0.1.6/quant_alchemy.egg-info/
+-rw-rw-rw-   0        0        0      400 2023-08-01 23:48:46.000000 quant-alchemy-0.1.6/quant_alchemy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-08-01 23:48:46.000000 quant-alchemy-0.1.6/quant_alchemy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 23:48:46.000000 quant-alchemy-0.1.6/quant_alchemy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-08-01 23:48:46.000000 quant-alchemy-0.1.6/quant_alchemy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-01 23:48:46.000000 quant-alchemy-0.1.6/quant_alchemy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 23:48:46.854793 quant-alchemy-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      658 2023-08-01 23:48:35.000000 quant-alchemy-0.1.6/setup.py
```

### Comparing `quant-alchemy-0.1.5/quant_alchemy/portfolio.py` & `quant-alchemy-0.1.6/quant_alchemy/portfolio.py`

 * *Files identical despite different names*

### Comparing `quant-alchemy-0.1.5/quant_alchemy/timeseries.py` & `quant-alchemy-0.1.6/quant_alchemy/timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,17 +251,17 @@
         Returns:
             float: The Sharpe ratio of the time series data.
         """
         periods = self.periods_in_year(period, trading_days, hours_per_day)
         if isinstance(periods, str):
             raise ValueError(periods)
         
-        annualized_returns = self.annualized_returns(period, trading_days, hours_per_day)
+        annualized_return = self.annualized_return(period, trading_days, hours_per_day)
         annualized_volatility = self.annualized_volatility(period, trading_days, hours_per_day)
-        return (annualized_returns - risk_free_rate) / annualized_volatility
+        return (annualized_return - risk_free_rate) / annualized_volatility
 
     def semideviation(self, threshold=0.0):
         """
         Calculates semideviation of the returns that are less than the provided threshold.
 
         Parameters:
             threshold (float, optional): The reference value below which a return is considered as underperforming.
```

### Comparing `quant-alchemy-0.1.5/setup.py` & `quant-alchemy-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     readme = file.read()
 
 setuptools.setup(
     name="quant-alchemy",
-    version="0.1.5",
+    version="0.1.6",
     author="Eladio Rocha Vizcaino",
     author_email="eladio.rocha99@gmail.com",
     description="Package for quantitative finance.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/EladioRocha/quant-alchemy",
     project_urls={
```

