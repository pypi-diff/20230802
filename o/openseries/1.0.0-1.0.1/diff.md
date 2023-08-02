# Comparing `tmp/openseries-1.0.0-py3-none-any.whl.zip` & `tmp/openseries-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 53868 bytes, number of entries: 15
+Zip file size: 53979 bytes, number of entries: 15
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 openseries/__init__.py
 -rw-r--r--  2.0 unx     9970 b- defN 80-Jan-01 00:00 openseries/datefixer.py
 -rw-r--r--  2.0 unx   115141 b- defN 80-Jan-01 00:00 openseries/frame.py
 -rw-r--r--  2.0 unx     1119 b- defN 80-Jan-01 00:00 openseries/load_plotly.py
 -rw-r--r--  2.0 unx      178 b- defN 80-Jan-01 00:00 openseries/plotly_captor_logo.json
 -rw-r--r--  2.0 unx     1429 b- defN 80-Jan-01 00:00 openseries/plotly_layouts.json
 -rw-r--r--  2.0 unx     4404 b- defN 80-Jan-01 00:00 openseries/risk.py
 -rw-r--r--  2.0 unx    84385 b- defN 80-Jan-01 00:00 openseries/series.py
 -rw-r--r--  2.0 unx    13878 b- defN 80-Jan-01 00:00 openseries/sim_price.py
 -rw-r--r--  2.0 unx    14673 b- defN 80-Jan-01 00:00 openseries/stoch_processes.py
 -rw-r--r--  2.0 unx     6698 b- defN 80-Jan-01 00:00 openseries/types.py
--rw-r--r--  2.0 unx     1521 b- defN 80-Jan-01 00:00 openseries-1.0.0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx    47713 b- defN 80-Jan-01 00:00 openseries-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 openseries-1.0.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1200 b- defN 16-Jan-01 00:00 openseries-1.0.0.dist-info/RECORD
-15 files, 302397 bytes uncompressed, 51908 bytes compressed:  82.8%
+-rw-r--r--  2.0 unx     1521 b- defN 80-Jan-01 00:00 openseries-1.0.1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx    47927 b- defN 80-Jan-01 00:00 openseries-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 openseries-1.0.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1200 b- defN 16-Jan-01 00:00 openseries-1.0.1.dist-info/RECORD
+15 files, 302611 bytes uncompressed, 52019 bytes compressed:  82.8%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: openseries/stoch_processes.py
 Comment: 
 
 Filename: openseries/types.py
 Comment: 
 
-Filename: openseries-1.0.0.dist-info/LICENSE.md
+Filename: openseries-1.0.1.dist-info/LICENSE.md
 Comment: 
 
-Filename: openseries-1.0.0.dist-info/METADATA
+Filename: openseries-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: openseries-1.0.0.dist-info/WHEEL
+Filename: openseries-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: openseries-1.0.0.dist-info/RECORD
+Filename: openseries-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `openseries-1.0.0.dist-info/LICENSE.md` & `openseries-1.0.1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `openseries-1.0.0.dist-info/METADATA` & `openseries-1.0.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openseries
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package for simple financial time series analysis.
 Home-page: https://github.com/CaptorAB/OpenSeries
 License: BSD-3-Clause
 Keywords: python,python3,plotly,pandas,finance,fintech,data-science,timeseries,timeseries-data,timeseries-analysis,investment,investment-analysis,investing
 Author: Martin Karrin
 Author-email: martin.karrin@captor.se
 Requires-Python: >=3.10,<3.12
@@ -23,18 +23,16 @@
 Requires-Dist: numpy (>=1.25.1,<2.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: plotly (>=5.15.0,<6.0.0)
 Requires-Dist: pydantic (>=1.10.11,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-stdnum (>=1.18,<2.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Requires-Dist: statsmodels (>=0.13.5,<0.14.0)
-Requires-Dist: urllib3 (>=1.26.9,<2.0.0)
 Project-URL: Repository, https://github.com/CaptorAB/OpenSeries
 Description-Content-Type: text/markdown
 
 <img src="https://sales.captor.se/captor_logo_sv_1600_icketransparent.png" alt="Captor
 Fund Management AB"
 width="81" height="100" align="left" float="right"/><br/>
 
@@ -46,49 +44,53 @@
 [![Python version](https://img.shields.io/pypi/pyversions/openseries.svg)](https://www.python.org/)
 ![GitHub Action Test Suite](https://github.com/CaptorAB/OpenSeries/actions/workflows/test.yml/badge.svg)
 ![Coverage](https://cdn.jsdelivr.net/gh/CaptorAB/OpenSeries@master/coverage.svg)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/en/stable/index.html)
 ![pylint](https://github.com/CaptorAB/OpenSeries/actions/workflows/pylint.yml/badge.svg)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
-**OpenSeries** is a project with tools to perform timeseries analysis on a single
+**OpenSeries** is a project with tools to analyse financial timeseries of a single
 asset or a group of assets. It is solely made for daily or less frequent data.
 
 <span style="font-size:2em;">[Changelog](https://github.com/CaptorAB/OpenSeries/blob/master/CHANGELOG.md)</span>
 
 
 ## Basic Usage
 
 To install:
 
 ```
 pip install openseries
 ```
 
-An overview of an OpenTimeSeries object is shown in the below example. My preference
-is to instantiate an object from a constructing class methods such as this.
+An overview of an OpenTimeSeries object is shown in the below example. It shows how to
+create an object from a constructing classmethod. The design aligns with how we within
+our fund company's code base have a subclass of OpenTimeSeries with class methods
+for our different data sources. Combined with some additional tools it allows us to
+efficiently present investment cases to clients.
+
 The OpenTimeSeries and OpenFrame classes are both subclasses of
 the [Pydantic BaseModel](https://docs.pydantic.dev/usage/models/).
 
 To make use of some tools available in the [Pandas](https://pandas.pydata.org/) library
 the [OpenTimeSeries](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/series.py)
 and [OpenFrame](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/frame.py)
 classes have an attribute `tsdf`
 which is a DataFrame constructed from the raw data in the lists `dates` and `values`.
 
-```
+```python
 from openseries.series import OpenTimeSeries
-```
+import yfinance as yf
+
+msft=yf.Ticker("MSFT")
+history=msft.history(period="max")
+series=OpenTimeSeries.from_df(history.loc[:, "Close"])
+_=series.value_to_log().set_new_label("Microsoft Log Returns of Close Prices")
+_,_=series.plot_series()
 
-```
-series = OpenTimeSeries.from_arrays(
-    name="Timeseries",
-    dates=["2023-05-08", "2023-05-09", "2023-05-10", "2023-05-11", "2023-05-12"],
-    values=[90.2533, 89.9977, 90.1052, 90.9142, 90.5574],
-)
 ```
 
 ### Sample output using the OpenFrame.all_properties() method:
 ```
                        Scilla Global Equity C (simulation+fund) Global Low Volatility index, SEK
                                                 ValueType.PRICE                  ValueType.PRICE
 Total return                                           3.641282                         1.946319
@@ -126,51 +128,54 @@
 These instructions assume that you
 have a compatible Python version installed on your machine and that you are OK
 to install this project in a virtual environment. If not, feel free to do it your
 own way.
 
 ### Windows Powershell
 
-```
+```powershell
 git clone https://github.com/CaptorAB/OpenSeries.git
 cd OpenSeries
 ./make.ps1 -task make
 ```
 
 ### Mac Terminal/Linux
 
-```
+```bash
 git clone https://github.com/CaptorAB/OpenSeries.git
 cd OpenSeries
 make
 source source_me
 make install
+
 ```
 
 ## Testing and Linting / Type-checking
 
 Flake8, Black and Pylint checking is embedded in the pre-commit hook but not mypy. All
 packages are used in the project's GitHub workflows and are run when the `lint`
 alternative is chosen in the below commands.
 The silenced error codes can be found in the
 [pyproject.toml](https://github.com/CaptorAB/OpenSeries/blob/master/pyproject.toml)
 file.
 
 ### Windows Powershell
 
-```
+```powershell
 ./make.ps1 -task test
 ./make.ps1 -task lint
+
 ```
 
 ### Mac Terminal/Linux
 
-```
+```bash
 make test
 make lint
+
 ```
 
 
 ## Table of Contents
 
 - [Basic Usage](#basic-usage)
 - [Development Instructions](#development-instructions)
```

## Comparing `openseries-1.0.0.dist-info/RECORD` & `openseries-1.0.1.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -5,11 +5,11 @@
 openseries/plotly_captor_logo.json,sha256=pGMuPVu4cEO3ZsCH1wU03hxqbIQkHFNoJUs1k1WK89Y,178
 openseries/plotly_layouts.json,sha256=xhrMOqW8LXb4QMtPiNBGdkPX518OHThiIJ68jpQk524,1429
 openseries/risk.py,sha256=_NJd8V-6pMx8pTodW-QpGKlmCDbCn4TsEjieKnCkIxU,4404
 openseries/series.py,sha256=Xw7ppt2bCVspkjYIqZKcMNfVIlrsmrnV7XWtp99qxrg,84385
 openseries/sim_price.py,sha256=dWzmj22nq4TW4BZBwP8Ajtid_g322No6D_m7t5bT8No,13878
 openseries/stoch_processes.py,sha256=6O4C_nC2iBseWggvDDC2gTpTqS5fI5nfjSRpccaazLE,14673
 openseries/types.py,sha256=t5xeqoD-e9fm0aU5I9chbzLcZ-MHmb9-jInCz3NrIfk,6698
-openseries-1.0.0.dist-info/LICENSE.md,sha256=NJjeq3wyB7EnnHLmsdK1EK6zT00T1eB3FgAmHAPT_vM,1521
-openseries-1.0.0.dist-info/METADATA,sha256=DfsJ-HSIyPGdL_33nJK7OhCSuEStkm6duUGhnTA1rNQ,47713
-openseries-1.0.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-openseries-1.0.0.dist-info/RECORD,,
+openseries-1.0.1.dist-info/LICENSE.md,sha256=NJjeq3wyB7EnnHLmsdK1EK6zT00T1eB3FgAmHAPT_vM,1521
+openseries-1.0.1.dist-info/METADATA,sha256=PTN4E6RKx3YEmLLohbkKawOJZJPsbrE4B-wjRUxiWwM,47927
+openseries-1.0.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+openseries-1.0.1.dist-info/RECORD,,
```

