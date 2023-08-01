# Comparing `tmp/quant-alchemy-0.1.4.tar.gz` & `tmp/quant-alchemy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant-alchemy-0.1.4.tar", last modified: Thu Jul 27 00:37:12 2023, max compression
+gzip compressed data, was "dist\quant-alchemy-0.1.5.tar", last modified: Tue Aug  1 22:19:25 2023, max compression
```

## Comparing `quant-alchemy-0.1.4.tar` & `quant-alchemy-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 00:37:12.899590 quant-alchemy-0.1.4/
--rw-rw-rw-   0        0        0      400 2023-07-27 00:37:12.899590 quant-alchemy-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-07-07 18:15:03.000000 quant-alchemy-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 00:37:12.894587 quant-alchemy-0.1.4/quant_alchemy/
--rw-rw-rw-   0        0        0       94 2023-07-26 18:55:50.000000 quant-alchemy-0.1.4/quant_alchemy/__init__.py
--rw-rw-rw-   0        0        0     3572 2023-07-12 19:45:17.000000 quant-alchemy-0.1.4/quant_alchemy/portfolio.py
--rw-rw-rw-   0        0        0    14755 2023-07-27 00:35:53.000000 quant-alchemy-0.1.4/quant_alchemy/timeseries.py
-drwxrwxrwx   0        0        0        0 2023-07-27 00:37:12.898588 quant-alchemy-0.1.4/quant_alchemy.egg-info/
--rw-rw-rw-   0        0        0      400 2023-07-27 00:37:12.000000 quant-alchemy-0.1.4/quant_alchemy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-07-27 00:37:12.000000 quant-alchemy-0.1.4/quant_alchemy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 00:37:12.000000 quant-alchemy-0.1.4/quant_alchemy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-27 00:37:12.000000 quant-alchemy-0.1.4/quant_alchemy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-27 00:37:12.000000 quant-alchemy-0.1.4/quant_alchemy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 00:37:12.899590 quant-alchemy-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      658 2023-07-27 00:37:04.000000 quant-alchemy-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:19:25.630711 quant-alchemy-0.1.5/
+-rw-rw-rw-   0        0        0      400 2023-08-01 22:19:25.629710 quant-alchemy-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-07-07 18:15:03.000000 quant-alchemy-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 22:19:25.622259 quant-alchemy-0.1.5/quant_alchemy/
+-rw-rw-rw-   0        0        0       94 2023-07-26 18:55:50.000000 quant-alchemy-0.1.5/quant_alchemy/__init__.py
+-rw-rw-rw-   0        0        0     3572 2023-07-12 19:45:17.000000 quant-alchemy-0.1.5/quant_alchemy/portfolio.py
+-rw-rw-rw-   0        0        0    16024 2023-08-01 20:57:12.000000 quant-alchemy-0.1.5/quant_alchemy/timeseries.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:19:25.628708 quant-alchemy-0.1.5/quant_alchemy.egg-info/
+-rw-rw-rw-   0        0        0      400 2023-08-01 22:19:25.000000 quant-alchemy-0.1.5/quant_alchemy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-08-01 22:19:25.000000 quant-alchemy-0.1.5/quant_alchemy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 22:19:25.000000 quant-alchemy-0.1.5/quant_alchemy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-08-01 22:19:25.000000 quant-alchemy-0.1.5/quant_alchemy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-01 22:19:25.000000 quant-alchemy-0.1.5/quant_alchemy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 22:19:25.630711 quant-alchemy-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      658 2023-08-01 22:19:22.000000 quant-alchemy-0.1.5/setup.py
```

### Comparing `quant-alchemy-0.1.4/quant_alchemy/portfolio.py` & `quant-alchemy-0.1.5/quant_alchemy/portfolio.py`

 * *Files identical despite different names*

### Comparing `quant-alchemy-0.1.4/quant_alchemy/timeseries.py` & `quant-alchemy-0.1.5/quant_alchemy/timeseries.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             'hourly': trading_days * hours_per_day,
             '30min': trading_days * hours_per_day * 2,
             '15min': trading_days * hours_per_day * 4,
             '5min': trading_days * hours_per_day * 12,
             '1min': trading_days * hours_per_day * 60,
         }.get(period.lower(), "Invalid period. Please choose a valid period")
 
-    def annualized_returns(self, period='daily', trading_days=252, hours_per_day=8):
+    def annualized_return(self, period='daily', trading_days=252, hours_per_day=8):
         """
         Calculate the annualized returns of the time series data.
 
         Parameters
         ----------
         period : str, optional
             The period of the time series data (default is 'daily'). ('annually', 'semi-annually', 'quarterly', 'monthly', 'weekly', 'daily', '4hourly', 'hourly', '30min', '15min', '5min', or '1min') (default is 'daily').
@@ -135,17 +135,17 @@
             float: The calculated annualized volatility.
         """
         periods = self.periods_in_year(period, trading_days, hours_per_day)
         if isinstance(periods, str):
             raise ValueError(periods)
         return self.prices.pct_change().std(ddof=1) * np.sqrt(periods)
 
-    def compound_returns(self):
+    def compound_return(self):
         """
-        This method calculates and returns the compounded returns.
+        This method calculates and returns the compounded return.
 
         Returns:
             float: The compounded return.
         """
         returns = self.returns()
         return np.expm1(np.log1p(returns).sum())
     
@@ -340,8 +340,46 @@
             float: The Gaussian VaR at the specified level. This is the return value such that 'level' percent of 
                     returns fall below this number, assuming returns follow a Gaussian distribution.
         """
         if not 0 <= level <= 100:
             raise ValueError("The 'level' should be a percentile, i.e., between 0 and 100.")
         
         returns = self.returns()
-        return -norm.ppf(level/100, loc=returns.mean(), scale=returns.std(ddof=1))
+        return -norm.ppf(level/100, loc=returns.mean(), scale=returns.std(ddof=1))
+    
+    def calculate_monthly_compound_return(self):
+        """
+        Calculates the monthly compounded return based on the closing prices.
+
+        Parameters:
+            df (pd.DataFrame): DataFrame with Date as the index and OHLC columns.
+
+        Returns:
+            A dictionary where the keys are column names and the values contains dataframes with the monthly compounded returns.
+            
+        """
+        def calculate_compound_return(returns):
+            """
+            Calculates and returns the compounded return for a series of returns.
+
+            Parameters:
+                returns (pd.Series): A series of returns.
+
+            Returns:
+                float: The compounded return.
+            """
+            return np.expm1(np.log1p(returns).sum())
+
+        result = {}
+
+        returns = self.returns()
+        returns["Year"] = returns.index.year
+        returns["Month"] = returns.index.month
+
+        for col in returns.columns:
+            compound_return = returns.groupby(["Year", "Month"])["Close"].apply(calculate_compound_return).reset_index()
+            compound_return.columns = ["Year", "Month", "Compound Return"]
+
+            result[col] = compound_return
+
+        return result
+
```

### Comparing `quant-alchemy-0.1.4/setup.py` & `quant-alchemy-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     readme = file.read()
 
 setuptools.setup(
     name="quant-alchemy",
-    version="0.1.4",
+    version="0.1.5",
     author="Eladio Rocha Vizcaino",
     author_email="eladio.rocha99@gmail.com",
     description="Package for quantitative finance.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/EladioRocha/quant-alchemy",
     project_urls={
```

