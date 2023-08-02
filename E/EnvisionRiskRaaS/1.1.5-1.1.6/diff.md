# Comparing `tmp/envisionriskraas-1.1.5.tar.gz` & `tmp/envisionriskraas-1.1.6.tar.gz`

## Comparing `envisionriskraas-1.1.5.tar` & `envisionriskraas-1.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 envisionriskraas-1.1.5/src/EnvisionRiskRaaS/__init__.py
--rw-r--r--   0        0        0    86306 2020-02-02 00:00:00.000000 envisionriskraas-1.1.5/src/EnvisionRiskRaaS/core.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-1.1.5/LICENSE.txt
--rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 envisionriskraas-1.1.5/README.md
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 envisionriskraas-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     9964 2020-02-02 00:00:00.000000 envisionriskraas-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 envisionriskraas-1.1.6/src/EnvisionRiskRaaS/__init__.py
+-rw-r--r--   0        0        0    86306 2020-02-02 00:00:00.000000 envisionriskraas-1.1.6/src/EnvisionRiskRaaS/core.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-1.1.6/LICENSE.txt
+-rw-r--r--   0        0        0     8861 2020-02-02 00:00:00.000000 envisionriskraas-1.1.6/README.md
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 envisionriskraas-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 envisionriskraas-1.1.6/PKG-INFO
```

### Comparing `envisionriskraas-1.1.5/src/EnvisionRiskRaaS/core.py` & `envisionriskraas-1.1.6/src/EnvisionRiskRaaS/core.py`

 * *Files identical despite different names*

### Comparing `envisionriskraas-1.1.5/LICENSE.txt` & `envisionriskraas-1.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `envisionriskraas-1.1.5/README.md` & `envisionriskraas-1.1.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -38,62 +38,62 @@
 - <b>Regulatory Compliance:</b> Regulators often require financial institutions to maintain capital reserves based on potential losses, which are derived from P/L distributions. Hence, understanding the P/L distribution is crucial to meet these regulatory requirements.
 
 - <b>Stress Testing:</b> Stress testing involves applying extreme but plausible hypothetical scenarios to the P/L distribution to assess the portfolio’s resilience. This helps managers prepare for unexpected market events and ensure that the portfolio can withstand adverse conditions.
 
 Therefore, P/L distribution serves as a key pillar of market risk management, providing insights into potential risks, informing decision-making, enabling portfolio optimization, and ensuring regulatory compliance.
 
 ```
+#Libraries
+import EnvisionRiskRaaS as RaaS
+from datetime import date
+import matplotlib.pyplot as plt
+from scipy import stats
+import pandas as pd
+import numpy as np
+import queuelib
+
+#EnvisionRisk login
+RaaS.envrsk_auth_log_in("your username/email here", "your password here")
+
 #### Get the delta vector (simulated price change) ####
 # The term '_raw' within the function name is indicative of a key feature: 
 # the simulated price changes are denominated in the same currency as 
 # the stock. This implies that the analysis maintains the original currency 
 # perspective of the stock, allowing for more accurate and relevant 
 # insights. It enhances ease of comprehension and direct applicability, 
 # bringing us closer to the context of the actual trading environment.
+use_date = date.today()
+use_symbol = "AAPL.US"
 api_response = RAAS.envrsk_instrument_delta_vector_raw(use_date,use_symbol)
 
 # Leverage our sophisticated API to conduct an Expected-Shortfall computation, 
 # specified at a 97.5% confidence level across a single-day span, utilizing a 
 # point-in-time volatility scenario.
-api_response_es = RAAS.envrsk_instrument_expected_shortfall_raw(use_date, use_symbol, signif_level = 0.975, volatility_id = "point_in_time")
+api_response_es = RAAS.envrsk_instrument_expected_shortfall_raw(date = use_date,symbols = use_symbol, signif_level = 0.975, volatility_id = "point_in_time")
 expected_shortfall_estimate = api_response_es["Output"]["expected_shortfall"][0]
 
 #manipulate the data for the density function
 data = api_response["Output"]["PnL"]
-density = stats.gaussian_kde(data)
-
-#build a dataset spanning from min of the PnL dataset to the max.
-xs = np.linspace(min(data), max(data), 200)
-#build weights for the histogram
-weights = np.ones_like(data) / len(data)
 
-#indicate the subtitle and the caption text.
+#titles and captions
 subtitle = "Profit/Loss distribution (one day) for " + use_symbol + " as seen from the " + str(use_date)
-caption= "In the world of financial markets, price uncertainty is a key element that contributes to market risk - the risk of losses in positions arising \n
-from movements in market prices. Risk management aims to quantify this risk and devise strategies to mitigate potential losses."
+caption= "In the world of financial markets, price uncertainty is a key element that contributes to market risk - the risk of losses in positions arising \nfrom movements in market prices. Risk management aims to quantify this risk and devise strategies to mitigate potential losses."
 
-# Plot the P/L distribution
-#title
-plt.suptitle("Price Uncertainty", x=0.2875, y=1, fontsize=18)
-#subtitle
+#plot, titles, vertical line and more.
+plt.suptitle("Price Uncertainty", fontsize=18)
 plt.title(subtitle, fontsize=10, loc='left')
-
-#histogram, density and vertical line.
-plt.hist(data, weights=weights, bins=37, color="#27647B", edgecolor="#27647B",alpha = 0.75)
-plt.plot( xs, density(xs), color="#CA3542", alpha=0.5)
+sns.histplot(data, kde=True)
 plt.axvline(x = expected_shortfall_estimate, color = "#57575F", label = 'axvline - full height')
-
-#vertical line text, labels, remove tickers and insert caption
-plt.text(expected_shortfall_estimate, max(density(xs))/2, 'Expected-Shortfall (97.5%, 1 day)', ha='center', va='center',rotation='vertical', backgroundcolor='white')
+plt.text(expected_shortfall_estimate, 300, 'Expected-Shortfall (97.5%, 1 day)', ha='center', va='center',rotation='vertical', backgroundcolor='white')
 plt.xlabel("Profit/Loss (in $)")
 plt.ylabel("Density")
 plt.yticks([])
-plt.text(0.5, -0.04, caption, ha='center', size=7)
-#plot
+plt.text(5,-120, caption, ha='center', size=7)
 plt.show()
+
 ```
 
 <img height='600' style='border:0px;height:600px;' src='https://raw.githubusercontent.com/EnvisionRisk/EnvisionRiskRaaS/master/man/figures/README-plot-1.png' border='0' />
 
 <h2>API documentation</h2>
 <hr>
 You can locate our extensive API documentation <a href="https://envisionrisk.stoplight.io/docs/api-aleadomus-documentation/9ed9f79a31a4a-market-risk-as-a-service-api">here</a>. This comprehensive guide is designed to walk you through our APIs’ functionalities, providing clear instructions on how to integrate and use them effectively.
```

#### html2text {}

```diff
@@ -61,49 +61,47 @@
 understanding the P/L distribution is crucial to meet these regulatory
 requirements. - Stress Testing: Stress testing involves applying extreme but
 plausible hypothetical scenarios to the P/L distribution to assess the
 portfolioâs resilience. This helps managers prepare for unexpected market
 events and ensure that the portfolio can withstand adverse conditions.
 Therefore, P/L distribution serves as a key pillar of market risk management,
 providing insights into potential risks, informing decision-making, enabling
-portfolio optimization, and ensuring regulatory compliance. ``` #### Get the
-delta vector (simulated price change) #### # The term '_raw' within the
-function name is indicative of a key feature: # the simulated price changes are
-denominated in the same currency as # the stock. This implies that the analysis
-maintains the original currency # perspective of the stock, allowing for more
-accurate and relevant # insights. It enhances ease of comprehension and direct
+portfolio optimization, and ensuring regulatory compliance. ``` #Libraries
+import EnvisionRiskRaaS as RaaS from datetime import date import
+matplotlib.pyplot as plt from scipy import stats import pandas as pd import
+numpy as np import queuelib #EnvisionRisk login RaaS.envrsk_auth_log_in("your
+username/email here", "your password here") #### Get the delta vector
+(simulated price change) #### # The term '_raw' within the function name is
+indicative of a key feature: # the simulated price changes are denominated in
+the same currency as # the stock. This implies that the analysis maintains the
+original currency # perspective of the stock, allowing for more accurate and
+relevant # insights. It enhances ease of comprehension and direct
 applicability, # bringing us closer to the context of the actual trading
-environment. api_response = RAAS.envrsk_instrument_delta_vector_raw
-(use_date,use_symbol) # Leverage our sophisticated API to conduct an Expected-
-Shortfall computation, # specified at a 97.5% confidence level across a single-
-day span, utilizing a # point-in-time volatility scenario. api_response_es =
-RAAS.envrsk_instrument_expected_shortfall_raw(use_date, use_symbol,
-signif_level = 0.975, volatility_id = "point_in_time")
+environment. use_date = date.today() use_symbol = "AAPL.US" api_response =
+RAAS.envrsk_instrument_delta_vector_raw(use_date,use_symbol) # Leverage our
+sophisticated API to conduct an Expected-Shortfall computation, # specified at
+a 97.5% confidence level across a single-day span, utilizing a # point-in-time
+volatility scenario. api_response_es =
+RAAS.envrsk_instrument_expected_shortfall_raw(date = use_date,symbols =
+use_symbol, signif_level = 0.975, volatility_id = "point_in_time")
 expected_shortfall_estimate = api_response_es["Output"]["expected_shortfall"]
 [0] #manipulate the data for the density function data = api_response["Output"]
-["PnL"] density = stats.gaussian_kde(data) #build a dataset spanning from min
-of the PnL dataset to the max. xs = np.linspace(min(data), max(data), 200)
-#build weights for the histogram weights = np.ones_like(data) / len(data)
-#indicate the subtitle and the caption text. subtitle = "Profit/Loss
-distribution (one day) for " + use_symbol + " as seen from the " + str
-(use_date) caption= "In the world of financial markets, price uncertainty is a
-key element that contributes to market risk - the risk of losses in positions
-arising \n from movements in market prices. Risk management aims to quantify
-this risk and devise strategies to mitigate potential losses." # Plot the P/
-L distribution #title plt.suptitle("Price Uncertainty", x=0.2875, y=1,
-fontsize=18) #subtitle plt.title(subtitle, fontsize=10, loc='left') #histogram,
-density and vertical line. plt.hist(data, weights=weights, bins=37,
-color="#27647B", edgecolor="#27647B",alpha = 0.75) plt.plot( xs, density(xs),
-color="#CA3542", alpha=0.5) plt.axvline(x = expected_shortfall_estimate, color
-= "#57575F", label = 'axvline - full height') #vertical line text, labels,
-remove tickers and insert caption plt.text(expected_shortfall_estimate, max
-(density(xs))/2, 'Expected-Shortfall (97.5%, 1 day)', ha='center',
-va='center',rotation='vertical', backgroundcolor='white') plt.xlabel("Profit/
-Loss (in $)") plt.ylabel("Density") plt.yticks([]) plt.text(0.5, -0.04,
-caption, ha='center', size=7) #plot plt.show() ``` [https://
+["PnL"] #titles and captions subtitle = "Profit/Loss distribution (one day) for
+" + use_symbol + " as seen from the " + str(use_date) caption= "In the world of
+financial markets, price uncertainty is a key element that contributes to
+market risk - the risk of losses in positions arising \nfrom movements in
+market prices. Risk management aims to quantify this risk and devise strategies
+to mitigate potential losses." #plot, titles, vertical line and more.
+plt.suptitle("Price Uncertainty", fontsize=18) plt.title(subtitle, fontsize=10,
+loc='left') sns.histplot(data, kde=True) plt.axvline(x =
+expected_shortfall_estimate, color = "#57575F", label = 'axvline - full
+height') plt.text(expected_shortfall_estimate, 300, 'Expected-Shortfall (97.5%,
+1 day)', ha='center', va='center',rotation='vertical', backgroundcolor='white')
+plt.xlabel("Profit/Loss (in $)") plt.ylabel("Density") plt.yticks([]) plt.text
+(5,-120, caption, ha='center', size=7) plt.show() ``` [https://
 raw.githubusercontent.com/EnvisionRisk/EnvisionRiskRaaS/master/man/figures/
 README-plot-1.png]
 ***** API documentation *****
 ===============================================================================
 You can locate our extensive API documentation here. This comprehensive guide
 is designed to walk you through our APIsâ functionalities, providing clear
 instructions on how to integrate and use them effectively. For each API,
```

### Comparing `envisionriskraas-1.1.5/pyproject.toml` & `envisionriskraas-1.1.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EnvisionRiskRaaS"
-version = "1.1.5"
+version = "1.1.6"
 authors = [{name="EnvisionRisk", email="support@envisionrisk.com" },{name="Coptolon",email="mark@brezina.dk"},]
 keywords = ["Risk-as-a-service","Market risk","Quantitative finance"]
 description = "EnvisionRisk improves market risk management by providing predictive analytics for risk quantification, aiding strategic decisions and risk mitigation."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -16,12 +16,13 @@
     "Operating System :: OS Independent",
 ]
 
 dependencies = [ 
 "requests>= 2.31.0; python_version<'3.9'",  
 "pandas>= 2.0.2; python_version<'3.9'", 
 "typing >= 3.10.0.0; python_version<'3.9'", 
-"queuelib >= 1.5.0; python_version<'3.9'", ]
+"queuelib >= 1.5.0; python_version<'3.9'", 
+"seaborn >= 0.12; python_version<'3.9'" ]
 
 [project.urls]
 "API webpage" = "https://envisionrisk.stoplight.io/docs/api-aleadomus-documentation/cjr0z7gv4x6en-harnessing-advanced-tools-for-strategic-market-risk-management"
 "Homepage" = "https://www.envisionrisk.com/"
```

### Comparing `envisionriskraas-1.1.5/PKG-INFO` & `envisionriskraas-1.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: EnvisionRiskRaaS
-Version: 1.1.5
+Version: 1.1.6
 Summary: EnvisionRisk improves market risk management by providing predictive analytics for risk quantification, aiding strategic decisions and risk mitigation.
 Project-URL: API webpage, https://envisionrisk.stoplight.io/docs/api-aleadomus-documentation/cjr0z7gv4x6en-harnessing-advanced-tools-for-strategic-market-risk-management
 Project-URL: Homepage, https://www.envisionrisk.com/
 Author-email: EnvisionRisk <support@envisionrisk.com>, Coptolon <mark@brezina.dk>
 License-File: LICENSE.txt
 Keywords: Market risk,Quantitative finance,Risk-as-a-service
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: pandas>=2.0.2; python_version < '3.9'
 Requires-Dist: queuelib>=1.5.0; python_version < '3.9'
 Requires-Dist: requests>=2.31.0; python_version < '3.9'
+Requires-Dist: seaborn>=0.12; python_version < '3.9'
 Requires-Dist: typing>=3.10.0.0; python_version < '3.9'
 Description-Content-Type: text/markdown
 
 <h1>EnvisionRiskRaaS</h1>
 <hr>
 Delve into the world of EnvisionRisk’s Python package, your portal to our sophisticated Market Risk-as-a-Service (RaaS). This comprehensive tool allows you to tap into our cutting-edge risk management services, retrieve relevant data, perform complex calculations, and generate actionable insights, all without leaving your Python programming environment. Embrace this smarter, efficient approach to handling market risk.
 
@@ -57,62 +58,62 @@
 - <b>Regulatory Compliance:</b> Regulators often require financial institutions to maintain capital reserves based on potential losses, which are derived from P/L distributions. Hence, understanding the P/L distribution is crucial to meet these regulatory requirements.
 
 - <b>Stress Testing:</b> Stress testing involves applying extreme but plausible hypothetical scenarios to the P/L distribution to assess the portfolio’s resilience. This helps managers prepare for unexpected market events and ensure that the portfolio can withstand adverse conditions.
 
 Therefore, P/L distribution serves as a key pillar of market risk management, providing insights into potential risks, informing decision-making, enabling portfolio optimization, and ensuring regulatory compliance.
 
 ```
+#Libraries
+import EnvisionRiskRaaS as RaaS
+from datetime import date
+import matplotlib.pyplot as plt
+from scipy import stats
+import pandas as pd
+import numpy as np
+import queuelib
+
+#EnvisionRisk login
+RaaS.envrsk_auth_log_in("your username/email here", "your password here")
+
 #### Get the delta vector (simulated price change) ####
 # The term '_raw' within the function name is indicative of a key feature: 
 # the simulated price changes are denominated in the same currency as 
 # the stock. This implies that the analysis maintains the original currency 
 # perspective of the stock, allowing for more accurate and relevant 
 # insights. It enhances ease of comprehension and direct applicability, 
 # bringing us closer to the context of the actual trading environment.
+use_date = date.today()
+use_symbol = "AAPL.US"
 api_response = RAAS.envrsk_instrument_delta_vector_raw(use_date,use_symbol)
 
 # Leverage our sophisticated API to conduct an Expected-Shortfall computation, 
 # specified at a 97.5% confidence level across a single-day span, utilizing a 
 # point-in-time volatility scenario.
-api_response_es = RAAS.envrsk_instrument_expected_shortfall_raw(use_date, use_symbol, signif_level = 0.975, volatility_id = "point_in_time")
+api_response_es = RAAS.envrsk_instrument_expected_shortfall_raw(date = use_date,symbols = use_symbol, signif_level = 0.975, volatility_id = "point_in_time")
 expected_shortfall_estimate = api_response_es["Output"]["expected_shortfall"][0]
 
 #manipulate the data for the density function
 data = api_response["Output"]["PnL"]
-density = stats.gaussian_kde(data)
-
-#build a dataset spanning from min of the PnL dataset to the max.
-xs = np.linspace(min(data), max(data), 200)
-#build weights for the histogram
-weights = np.ones_like(data) / len(data)
 
-#indicate the subtitle and the caption text.
+#titles and captions
 subtitle = "Profit/Loss distribution (one day) for " + use_symbol + " as seen from the " + str(use_date)
-caption= "In the world of financial markets, price uncertainty is a key element that contributes to market risk - the risk of losses in positions arising \n
-from movements in market prices. Risk management aims to quantify this risk and devise strategies to mitigate potential losses."
+caption= "In the world of financial markets, price uncertainty is a key element that contributes to market risk - the risk of losses in positions arising \nfrom movements in market prices. Risk management aims to quantify this risk and devise strategies to mitigate potential losses."
 
-# Plot the P/L distribution
-#title
-plt.suptitle("Price Uncertainty", x=0.2875, y=1, fontsize=18)
-#subtitle
+#plot, titles, vertical line and more.
+plt.suptitle("Price Uncertainty", fontsize=18)
 plt.title(subtitle, fontsize=10, loc='left')
-
-#histogram, density and vertical line.
-plt.hist(data, weights=weights, bins=37, color="#27647B", edgecolor="#27647B",alpha = 0.75)
-plt.plot( xs, density(xs), color="#CA3542", alpha=0.5)
+sns.histplot(data, kde=True)
 plt.axvline(x = expected_shortfall_estimate, color = "#57575F", label = 'axvline - full height')
-
-#vertical line text, labels, remove tickers and insert caption
-plt.text(expected_shortfall_estimate, max(density(xs))/2, 'Expected-Shortfall (97.5%, 1 day)', ha='center', va='center',rotation='vertical', backgroundcolor='white')
+plt.text(expected_shortfall_estimate, 300, 'Expected-Shortfall (97.5%, 1 day)', ha='center', va='center',rotation='vertical', backgroundcolor='white')
 plt.xlabel("Profit/Loss (in $)")
 plt.ylabel("Density")
 plt.yticks([])
-plt.text(0.5, -0.04, caption, ha='center', size=7)
-#plot
+plt.text(5,-120, caption, ha='center', size=7)
 plt.show()
+
 ```
 
 <img height='600' style='border:0px;height:600px;' src='https://raw.githubusercontent.com/EnvisionRisk/EnvisionRiskRaaS/master/man/figures/README-plot-1.png' border='0' />
 
 <h2>API documentation</h2>
 <hr>
 You can locate our extensive API documentation <a href="https://envisionrisk.stoplight.io/docs/api-aleadomus-documentation/9ed9f79a31a4a-market-risk-as-a-service-api">here</a>. This comprehensive guide is designed to walk you through our APIs’ functionalities, providing clear instructions on how to integrate and use them effectively.
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: EnvisionRiskRaaS Version: 1.1.5 Summary:
+Metadata-Version: 2.1 Name: EnvisionRiskRaaS Version: 1.1.6 Summary:
 EnvisionRisk improves market risk management by providing predictive analytics
 for risk quantification, aiding strategic decisions and risk mitigation.
 Project-URL: API webpage, https://envisionrisk.stoplight.io/docs/api-aleadomus-
 documentation/cjr0z7gv4x6en-harnessing-advanced-tools-for-strategic-market-
 risk-management Project-URL: Homepage, https://www.envisionrisk.com/ Author-
 email: EnvisionRisk
 envisionrisk.com>, Coptolon
 brezina.dk> License-File: LICENSE.txt Keywords: Market risk,Quantitative
 finance,Risk-as-a-service Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Requires-Python: >=3.9 Requires-Dist: pandas>=2.0.2;
 python_version < '3.9' Requires-Dist: queuelib>=1.5.0; python_version < '3.9'
 Requires-Dist: requests>=2.31.0; python_version < '3.9' Requires-Dist:
-typing>=3.10.0.0; python_version < '3.9' Description-Content-Type: text/
-markdown
+seaborn>=0.12; python_version < '3.9' Requires-Dist: typing>=3.10.0.0;
+python_version < '3.9' Description-Content-Type: text/markdown
 ****** EnvisionRiskRaaS ******
 ===============================================================================
 Delve into the world of EnvisionRiskâs Python package, your portal to our
 sophisticated Market Risk-as-a-Service (RaaS). This comprehensive tool allows
 you to tap into our cutting-edge risk management services, retrieve relevant
 data, perform complex calculations, and generate actionable insights, all
 without leaving your Python programming environment. Embrace this smarter,
@@ -77,49 +77,47 @@
 understanding the P/L distribution is crucial to meet these regulatory
 requirements. - Stress Testing: Stress testing involves applying extreme but
 plausible hypothetical scenarios to the P/L distribution to assess the
 portfolioâs resilience. This helps managers prepare for unexpected market
 events and ensure that the portfolio can withstand adverse conditions.
 Therefore, P/L distribution serves as a key pillar of market risk management,
 providing insights into potential risks, informing decision-making, enabling
-portfolio optimization, and ensuring regulatory compliance. ``` #### Get the
-delta vector (simulated price change) #### # The term '_raw' within the
-function name is indicative of a key feature: # the simulated price changes are
-denominated in the same currency as # the stock. This implies that the analysis
-maintains the original currency # perspective of the stock, allowing for more
-accurate and relevant # insights. It enhances ease of comprehension and direct
+portfolio optimization, and ensuring regulatory compliance. ``` #Libraries
+import EnvisionRiskRaaS as RaaS from datetime import date import
+matplotlib.pyplot as plt from scipy import stats import pandas as pd import
+numpy as np import queuelib #EnvisionRisk login RaaS.envrsk_auth_log_in("your
+username/email here", "your password here") #### Get the delta vector
+(simulated price change) #### # The term '_raw' within the function name is
+indicative of a key feature: # the simulated price changes are denominated in
+the same currency as # the stock. This implies that the analysis maintains the
+original currency # perspective of the stock, allowing for more accurate and
+relevant # insights. It enhances ease of comprehension and direct
 applicability, # bringing us closer to the context of the actual trading
-environment. api_response = RAAS.envrsk_instrument_delta_vector_raw
-(use_date,use_symbol) # Leverage our sophisticated API to conduct an Expected-
-Shortfall computation, # specified at a 97.5% confidence level across a single-
-day span, utilizing a # point-in-time volatility scenario. api_response_es =
-RAAS.envrsk_instrument_expected_shortfall_raw(use_date, use_symbol,
-signif_level = 0.975, volatility_id = "point_in_time")
+environment. use_date = date.today() use_symbol = "AAPL.US" api_response =
+RAAS.envrsk_instrument_delta_vector_raw(use_date,use_symbol) # Leverage our
+sophisticated API to conduct an Expected-Shortfall computation, # specified at
+a 97.5% confidence level across a single-day span, utilizing a # point-in-time
+volatility scenario. api_response_es =
+RAAS.envrsk_instrument_expected_shortfall_raw(date = use_date,symbols =
+use_symbol, signif_level = 0.975, volatility_id = "point_in_time")
 expected_shortfall_estimate = api_response_es["Output"]["expected_shortfall"]
 [0] #manipulate the data for the density function data = api_response["Output"]
-["PnL"] density = stats.gaussian_kde(data) #build a dataset spanning from min
-of the PnL dataset to the max. xs = np.linspace(min(data), max(data), 200)
-#build weights for the histogram weights = np.ones_like(data) / len(data)
-#indicate the subtitle and the caption text. subtitle = "Profit/Loss
-distribution (one day) for " + use_symbol + " as seen from the " + str
-(use_date) caption= "In the world of financial markets, price uncertainty is a
-key element that contributes to market risk - the risk of losses in positions
-arising \n from movements in market prices. Risk management aims to quantify
-this risk and devise strategies to mitigate potential losses." # Plot the P/
-L distribution #title plt.suptitle("Price Uncertainty", x=0.2875, y=1,
-fontsize=18) #subtitle plt.title(subtitle, fontsize=10, loc='left') #histogram,
-density and vertical line. plt.hist(data, weights=weights, bins=37,
-color="#27647B", edgecolor="#27647B",alpha = 0.75) plt.plot( xs, density(xs),
-color="#CA3542", alpha=0.5) plt.axvline(x = expected_shortfall_estimate, color
-= "#57575F", label = 'axvline - full height') #vertical line text, labels,
-remove tickers and insert caption plt.text(expected_shortfall_estimate, max
-(density(xs))/2, 'Expected-Shortfall (97.5%, 1 day)', ha='center',
-va='center',rotation='vertical', backgroundcolor='white') plt.xlabel("Profit/
-Loss (in $)") plt.ylabel("Density") plt.yticks([]) plt.text(0.5, -0.04,
-caption, ha='center', size=7) #plot plt.show() ``` [https://
+["PnL"] #titles and captions subtitle = "Profit/Loss distribution (one day) for
+" + use_symbol + " as seen from the " + str(use_date) caption= "In the world of
+financial markets, price uncertainty is a key element that contributes to
+market risk - the risk of losses in positions arising \nfrom movements in
+market prices. Risk management aims to quantify this risk and devise strategies
+to mitigate potential losses." #plot, titles, vertical line and more.
+plt.suptitle("Price Uncertainty", fontsize=18) plt.title(subtitle, fontsize=10,
+loc='left') sns.histplot(data, kde=True) plt.axvline(x =
+expected_shortfall_estimate, color = "#57575F", label = 'axvline - full
+height') plt.text(expected_shortfall_estimate, 300, 'Expected-Shortfall (97.5%,
+1 day)', ha='center', va='center',rotation='vertical', backgroundcolor='white')
+plt.xlabel("Profit/Loss (in $)") plt.ylabel("Density") plt.yticks([]) plt.text
+(5,-120, caption, ha='center', size=7) plt.show() ``` [https://
 raw.githubusercontent.com/EnvisionRisk/EnvisionRiskRaaS/master/man/figures/
 README-plot-1.png]
 ***** API documentation *****
 ===============================================================================
 You can locate our extensive API documentation here. This comprehensive guide
 is designed to walk you through our APIsâ functionalities, providing clear
 instructions on how to integrate and use them effectively. For each API,
```

