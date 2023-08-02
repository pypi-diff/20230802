# Comparing `tmp/arabica-1.6.8.tar.gz` & `tmp/arabica-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arabica-1.6.8.tar", last modified: Wed Jul  5 10:35:55 2023, max compression
+gzip compressed data, was "arabica-1.6.9.tar", last modified: Wed Aug  2 20:43:20 2023, max compression
```

## Comparing `arabica-1.6.8.tar` & `arabica-1.6.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 10:35:55.961370 arabica-1.6.8/
--rw-rw-rw-   0        0        0       39 2023-06-29 19:51:45.000000 arabica-1.6.8/LICENSE
--rw-rw-rw-   0        0        0     7819 2023-07-05 10:35:55.961370 arabica-1.6.8/PKG-INFO
--rw-rw-rw-   0        0        0     7012 2023-07-05 10:30:26.000000 arabica-1.6.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 10:35:55.961370 arabica-1.6.8/arabica/
--rw-rw-rw-   0        0        0      105 2023-06-29 22:43:08.000000 arabica-1.6.8/arabica/__init__.py
--rw-rw-rw-   0        0        0    11892 2023-06-22 16:47:25.000000 arabica-1.6.8/arabica/arabica_freq.py
--rw-rw-rw-   0        0        0    31618 2023-06-29 18:51:09.000000 arabica-1.6.8/arabica/cappuccino.py
--rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.6.8/arabica/clean_ngram.py
--rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.6.8/arabica/clean_numbers.py
--rw-rw-rw-   0        0        0     8246 2023-06-17 08:04:35.000000 arabica-1.6.8/arabica/coffee_break.py
--rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.6.8/arabica/group.py
--rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.6.8/arabica/preprocess.py
--rw-rw-rw-   0        0        0      533 2023-06-17 08:02:21.000000 arabica-1.6.8/arabica/sentiment.py
--rw-rw-rw-   0        0        0      447 2023-06-22 00:51:28.000000 arabica-1.6.8/arabica/stopwords.py
-drwxrwxrwx   0        0        0        0 2023-07-05 10:35:55.961370 arabica-1.6.8/arabica.egg-info/
--rw-rw-rw-   0        0        0     7819 2023-07-05 10:35:55.000000 arabica-1.6.8/arabica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-07-05 10:35:55.000000 arabica-1.6.8/arabica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 10:35:55.000000 arabica-1.6.8/arabica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      186 2023-07-05 10:35:55.000000 arabica-1.6.8/arabica.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-05 10:35:55.000000 arabica-1.6.8/arabica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      557 2023-07-05 10:33:39.000000 arabica-1.6.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-05 10:35:55.961370 arabica-1.6.8/setup.cfg
--rw-rw-rw-   0        0        0     1152 2023-07-05 10:33:39.000000 arabica-1.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 20:43:20.074245 arabica-1.6.9/
+-rw-rw-rw-   0        0        0       39 2023-06-29 19:51:45.000000 arabica-1.6.9/LICENSE
+-rw-rw-rw-   0        0        0     8336 2023-08-02 20:43:20.074245 arabica-1.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7526 2023-08-02 20:38:35.000000 arabica-1.6.9/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 20:43:20.066875 arabica-1.6.9/arabica/
+-rw-rw-rw-   0        0        0      105 2023-06-29 22:43:08.000000 arabica-1.6.9/arabica/__init__.py
+-rw-rw-rw-   0        0        0    11892 2023-06-22 16:47:25.000000 arabica-1.6.9/arabica/arabica_freq.py
+-rw-rw-rw-   0        0        0    31618 2023-06-29 18:51:09.000000 arabica-1.6.9/arabica/cappuccino.py
+-rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.6.9/arabica/clean_ngram.py
+-rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.6.9/arabica/clean_numbers.py
+-rw-rw-rw-   0        0        0     8246 2023-06-17 08:04:35.000000 arabica-1.6.9/arabica/coffee_break.py
+-rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.6.9/arabica/group.py
+-rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.6.9/arabica/preprocess.py
+-rw-rw-rw-   0        0        0      533 2023-06-17 08:02:21.000000 arabica-1.6.9/arabica/sentiment.py
+-rw-rw-rw-   0        0        0      447 2023-06-22 00:51:28.000000 arabica-1.6.9/arabica/stopwords.py
+drwxrwxrwx   0        0        0        0 2023-08-02 20:43:20.073267 arabica-1.6.9/arabica.egg-info/
+-rw-rw-rw-   0        0        0     8336 2023-08-02 20:43:20.000000 arabica-1.6.9/arabica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-08-02 20:43:20.000000 arabica-1.6.9/arabica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 20:43:20.000000 arabica-1.6.9/arabica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      186 2023-08-02 20:43:20.000000 arabica-1.6.9/arabica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-02 20:43:20.000000 arabica-1.6.9/arabica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      557 2023-08-02 20:41:47.000000 arabica-1.6.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-02 20:43:20.075249 arabica-1.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     1152 2023-08-02 20:41:47.000000 arabica-1.6.9/setup.py
```

### Comparing `arabica-1.6.8/PKG-INFO` & `arabica-1.6.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.6.8
+Version: 1.6.9
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: OSI Approved :: Apache Software License
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
 Project-URL: Bug Tracker, https://github.com/PetrKorab/Arabica/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.9, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![pypi](https://img.shields.io/pypi/v/arabica.svg)](https://pypi.python.org/pypi/arabica)
+[![python](https://img.shields.io/pypi/pyversions/arabica.svg)](https://pypi.python.org/pypi/arabica)
+[![License: MIT](https://badgen.net/badge/license/apache-2-0/blue)]([https://opensource.org/licenses/MIT](https://opensource.org/license/apache-2-0/))
+
+
 # Arabica
 **Python package for exploratory text data analysis**
 
 Text data is often recorded as a time series with significant variability over time. Some examples of time-series text data include Twitter tweets, research article metadata, product reviews, and newspaper headlines. Arabica makes exploratory analysis of these time-series text datasets simple by providing:
 
 * **Descriptive n-gram analysis**: n-gram frequencies
 * **Time-series n-gram analysis**: n-gram frequencies over a period
 * **Text visualization**: n-gram heatmap, line plot, word cloud
 * **Sentiment analysis**: VADER sentiment classifier
+* **Financial sentiment analysis**: with FinVADER
 * **Structural breaks identification**: Jenks Optimization Method
 
 It automatically cleans data from punctuation on input. It can also apply all or a selected combination of the following cleaning operations:
 
 * Remove digits from the text
-* Remove the standard list(s) of stop words
+* Remove the standard list(s) of stopwords
 * Remove an additional list of stop words
 
 Arabica works with **texts** of languages based on the Latin alphabet, uses `cleantext` for punctuation cleaning, and enables stop words removal for languages in the `NLTK` corpus of stopwords.
 
 It reads dates in:
 
 * **US-style**: *MM/DD/YYYY* (2013-12-31, Feb-09-2009, 2013-12-31 11:46:17, etc.)
@@ -48,16 +54,14 @@
 [vaderSentiment](https://pypi.org/project/vaderSentiment) - sentiment analysis, [finvader](https://pypi.org/project/finvader) - financial sentiment analysis,
 and [jenskpy](https://pypi.org/project/jenkspy/) for breakpoint identification.
 
 To install using pip, use:
 
 `pip install arabica`
 
-
-
 ## Usage
 
 * **Import the library**:
 
 
 ``` python
 from arabica import arabica_freq
@@ -65,67 +69,67 @@
 from arabica import coffee_break 
 ```
 
 
 
 * **Choose a method:**
 
-**arabica_freq** enables a set of cleaning operations (lower casing, numbers, common stop words, and additional stop words removal) and returns a dataframe with aggregated unigrams, bigrams, and trigrams frequencies over a period.
+**arabica_freq** enables a specific set of cleaning operations (lower casing, numbers, common stop words, and additional stop words 
+removal) and returns a dataframe with aggregated unigrams, bigrams, and trigrams frequencies over a period.
 
 
 
 ``` python
 def arabica_freq(text: str,                # Text
                  time: str,                # Time
                  date_format: str,         # Date format: 'eur' - European, 'us' - American
                  time_freq: str = '',      # Aggregation period: 'Y'/'M'/'D', if no aggregation: 'ungroup'
                  max_words: int = '',      # Maximum of most frequent n-grams displayed for each period
-                 stopwords: [],            # Languages for common stop words
-                 skip: [],                 # Remove additional list of stopwords
+                 stopwords: [],            # Languages for stop words
+                 skip: [],                 # Remove additional stop words
                  numbers: bool = False,    # Remove all digits
                  lower_case: bool = False  # Lowercase text
 ) 
 ```
 
-**cappuccino** enables cleaning operations (lower casing, numbers, common stop words, and additional stop words 
+**cappuccino**  enables cleaning operations (lower casing, numbers, common stop words, and additional stop words
 removal) and provides plots for descriptive (word cloud) and time-series (heatmap, line plot) visualization.
 
 ``` python
 def cappuccino(text: str,                # Text
                time: str,                # Time
                date_format: str,         # Date format: 'eur' - European, 'us' - American
                plot: str = '',           # Chart type: 'wordcloud'/'heatmap'/'line'
                ngram: int = '',          # N-gram size, 1 = unigram, 2 = bigram, 3 = trigram
                time_freq: str = '',      # Aggregation period: 'Y'/'M', if no aggregation: 'ungroup'
                max_words int = '',       # Maximum of most frequent n-grams displayed for each period
-               stopwords: [],            # Languages for common stop words
-               skip: [] ,                # Remove additional list of stop words
+               stopwords: [],            # Languages for stop words
+               skip: [],                 # Remove additional stop words
                numbers: bool = False,    # Remove numbers
                lower_case: bool = False  # Lowercase text
-)
 ```
 
-**coffee_break** provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. The implemented models are:
-
-* **VADER** is a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. See more [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
+**coffee_break**  provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. The implemented models are:
 
-* **FinVADER** improves VADER's classification accuracy, including two financial lexicons. Available from [here](https://pypi.org/project/finvader/).
+* [VADER](https://ojs.aaai.org/index.php/ICWSM/article/view/14550) is a lexicon and rule-based sentiment classifier attuned explicitly to general language expressed in social media
+  
+* [FinVADER](https://pypi.org/project/finvader/) improves VADER's classification accuracy on financial texts, including two financial lexicons
 
-Structural breaks in the time series are identified with the **Fisher-Jenks algorithm** (Jenks, 1977. Optimal data classification for choropleth maps).
+Break points in the time series are identified with the **Fisher-Jenks algorithm** (Jenks, 1977. Optimal data classification for choropleth maps).
 
 
 ``` python
 def coffee_break(text: str,                 # Text
                  time: str,                 # Time
                  date_format: str,          # Date format: 'eur' - European, 'us' - American
                  model: str,                # Sentiment classifier, 'vader' - general language, 'finvader' - financial text                
-                 skip: [] ,                 # Remove additional list of stop words
+                 skip: [],                  # Remove additional stop words
                  preprocess: bool = False,  # Clean data from numbers and punctuation
                  time_freq: str ='',        # Aggregation period: 'Y'/'M'
-                 n_breaks: int =''          # Number of breaks: min. 2
+                 n_breaks: int =''          # Number of breakpoints: min. 2
 )
 ```
 
 ## Documentation, examples and tutorials
 
 * Read the [documentation](https://arabica.readthedocs.io/en/latest/index.html)
 
@@ -136,13 +140,13 @@
 * Sentiment Analysis and Structural Breaks in Time-Series Text Data [here](https://medium.com/towards-data-science/sentiment-analysis-and-structural-breaks-in-time-series-text-data-8109c712ca2)                        
 * Visualization Module in Arabica Speeds Up Text Data Exploration [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)                                                                                                                          
 * Text as Time Series: Arabica 1.0 Brings New Features for Exploratory Text Data Analysis [here](https://towardsdatascience.com/text-as-time-series-arabica-1-0-brings-new-features-for-exploratory-text-data-analysis-88eaabb84deb?sk=229ec0602d0b8514f25bce501ed9ecb9)   
 
 **Applications:**
 
 * **Business Intelligence:** Customer Satisfaction Measurement with N-gram and Sentiment Analysis [here](https://towardsdatascience.com/customer-satisfaction-measurement-with-n-gram-and-sentiment-analysis-547e291c13a6)                       
+* **Research meta-data description:** Research Article Meta-data Description Made Quick and Easy [here](https://pub.towardsai.net/research-article-meta-data-description-made-quick-and-easy-57754e54b550)
 * **Twitter tweets analysis**
-* **Journal meta-data description**
 
 ---
 
 Please visit [here](https://github.com/PetrKorab/arabica/issues) for any questions, issues, bugs, and suggestions.
```

### Comparing `arabica-1.6.8/README.md` & `arabica-1.6.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+[![pypi](https://img.shields.io/pypi/v/arabica.svg)](https://pypi.python.org/pypi/arabica)
+[![python](https://img.shields.io/pypi/pyversions/arabica.svg)](https://pypi.python.org/pypi/arabica)
+[![License: MIT](https://badgen.net/badge/license/apache-2-0/blue)]([https://opensource.org/licenses/MIT](https://opensource.org/license/apache-2-0/))
+
+
 # Arabica
 **Python package for exploratory text data analysis**
 
 Text data is often recorded as a time series with significant variability over time. Some examples of time-series text data include Twitter tweets, research article metadata, product reviews, and newspaper headlines. Arabica makes exploratory analysis of these time-series text datasets simple by providing:
 
 * **Descriptive n-gram analysis**: n-gram frequencies
 * **Time-series n-gram analysis**: n-gram frequencies over a period
 * **Text visualization**: n-gram heatmap, line plot, word cloud
 * **Sentiment analysis**: VADER sentiment classifier
+* **Financial sentiment analysis**: with FinVADER
 * **Structural breaks identification**: Jenks Optimization Method
 
 It automatically cleans data from punctuation on input. It can also apply all or a selected combination of the following cleaning operations:
 
 * Remove digits from the text
-* Remove the standard list(s) of stop words
+* Remove the standard list(s) of stopwords
 * Remove an additional list of stop words
 
 Arabica works with **texts** of languages based on the Latin alphabet, uses `cleantext` for punctuation cleaning, and enables stop words removal for languages in the `NLTK` corpus of stopwords.
 
 It reads dates in:
 
 * **US-style**: *MM/DD/YYYY* (2013-12-31, Feb-09-2009, 2013-12-31 11:46:17, etc.)
@@ -31,16 +37,14 @@
 [vaderSentiment](https://pypi.org/project/vaderSentiment) - sentiment analysis, [finvader](https://pypi.org/project/finvader) - financial sentiment analysis,
 and [jenskpy](https://pypi.org/project/jenkspy/) for breakpoint identification.
 
 To install using pip, use:
 
 `pip install arabica`
 
-
-
 ## Usage
 
 * **Import the library**:
 
 
 ``` python
 from arabica import arabica_freq
@@ -48,67 +52,67 @@
 from arabica import coffee_break 
 ```
 
 
 
 * **Choose a method:**
 
-**arabica_freq** enables a set of cleaning operations (lower casing, numbers, common stop words, and additional stop words removal) and returns a dataframe with aggregated unigrams, bigrams, and trigrams frequencies over a period.
+**arabica_freq** enables a specific set of cleaning operations (lower casing, numbers, common stop words, and additional stop words 
+removal) and returns a dataframe with aggregated unigrams, bigrams, and trigrams frequencies over a period.
 
 
 
 ``` python
 def arabica_freq(text: str,                # Text
                  time: str,                # Time
                  date_format: str,         # Date format: 'eur' - European, 'us' - American
                  time_freq: str = '',      # Aggregation period: 'Y'/'M'/'D', if no aggregation: 'ungroup'
                  max_words: int = '',      # Maximum of most frequent n-grams displayed for each period
-                 stopwords: [],            # Languages for common stop words
-                 skip: [],                 # Remove additional list of stopwords
+                 stopwords: [],            # Languages for stop words
+                 skip: [],                 # Remove additional stop words
                  numbers: bool = False,    # Remove all digits
                  lower_case: bool = False  # Lowercase text
 ) 
 ```
 
-**cappuccino** enables cleaning operations (lower casing, numbers, common stop words, and additional stop words 
+**cappuccino**  enables cleaning operations (lower casing, numbers, common stop words, and additional stop words
 removal) and provides plots for descriptive (word cloud) and time-series (heatmap, line plot) visualization.
 
 ``` python
 def cappuccino(text: str,                # Text
                time: str,                # Time
                date_format: str,         # Date format: 'eur' - European, 'us' - American
                plot: str = '',           # Chart type: 'wordcloud'/'heatmap'/'line'
                ngram: int = '',          # N-gram size, 1 = unigram, 2 = bigram, 3 = trigram
                time_freq: str = '',      # Aggregation period: 'Y'/'M', if no aggregation: 'ungroup'
                max_words int = '',       # Maximum of most frequent n-grams displayed for each period
-               stopwords: [],            # Languages for common stop words
-               skip: [] ,                # Remove additional list of stop words
+               stopwords: [],            # Languages for stop words
+               skip: [],                 # Remove additional stop words
                numbers: bool = False,    # Remove numbers
                lower_case: bool = False  # Lowercase text
-)
 ```
 
-**coffee_break** provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. The implemented models are:
-
-* **VADER** is a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. See more [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
+**coffee_break**  provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. The implemented models are:
 
-* **FinVADER** improves VADER's classification accuracy, including two financial lexicons. Available from [here](https://pypi.org/project/finvader/).
+* [VADER](https://ojs.aaai.org/index.php/ICWSM/article/view/14550) is a lexicon and rule-based sentiment classifier attuned explicitly to general language expressed in social media
+  
+* [FinVADER](https://pypi.org/project/finvader/) improves VADER's classification accuracy on financial texts, including two financial lexicons
 
-Structural breaks in the time series are identified with the **Fisher-Jenks algorithm** (Jenks, 1977. Optimal data classification for choropleth maps).
+Break points in the time series are identified with the **Fisher-Jenks algorithm** (Jenks, 1977. Optimal data classification for choropleth maps).
 
 
 ``` python
 def coffee_break(text: str,                 # Text
                  time: str,                 # Time
                  date_format: str,          # Date format: 'eur' - European, 'us' - American
                  model: str,                # Sentiment classifier, 'vader' - general language, 'finvader' - financial text                
-                 skip: [] ,                 # Remove additional list of stop words
+                 skip: [],                  # Remove additional stop words
                  preprocess: bool = False,  # Clean data from numbers and punctuation
                  time_freq: str ='',        # Aggregation period: 'Y'/'M'
-                 n_breaks: int =''          # Number of breaks: min. 2
+                 n_breaks: int =''          # Number of breakpoints: min. 2
 )
 ```
 
 ## Documentation, examples and tutorials
 
 * Read the [documentation](https://arabica.readthedocs.io/en/latest/index.html)
 
@@ -119,13 +123,13 @@
 * Sentiment Analysis and Structural Breaks in Time-Series Text Data [here](https://medium.com/towards-data-science/sentiment-analysis-and-structural-breaks-in-time-series-text-data-8109c712ca2)                        
 * Visualization Module in Arabica Speeds Up Text Data Exploration [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)                                                                                                                          
 * Text as Time Series: Arabica 1.0 Brings New Features for Exploratory Text Data Analysis [here](https://towardsdatascience.com/text-as-time-series-arabica-1-0-brings-new-features-for-exploratory-text-data-analysis-88eaabb84deb?sk=229ec0602d0b8514f25bce501ed9ecb9)   
 
 **Applications:**
 
 * **Business Intelligence:** Customer Satisfaction Measurement with N-gram and Sentiment Analysis [here](https://towardsdatascience.com/customer-satisfaction-measurement-with-n-gram-and-sentiment-analysis-547e291c13a6)                       
+* **Research meta-data description:** Research Article Meta-data Description Made Quick and Easy [here](https://pub.towardsai.net/research-article-meta-data-description-made-quick-and-easy-57754e54b550)
 * **Twitter tweets analysis**
-* **Journal meta-data description**
 
 ---
 
-Please visit [here](https://github.com/PetrKorab/arabica/issues) for any questions, issues, bugs, and suggestions.
+Please visit [here](https://github.com/PetrKorab/arabica/issues) for any questions, issues, bugs, and suggestions.
```

### Comparing `arabica-1.6.8/arabica/arabica_freq.py` & `arabica-1.6.9/arabica/arabica_freq.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.8/arabica/cappuccino.py` & `arabica-1.6.9/arabica/cappuccino.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.8/arabica/clean_ngram.py` & `arabica-1.6.9/arabica/clean_ngram.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.8/arabica/coffee_break.py` & `arabica-1.6.9/arabica/coffee_break.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.8/arabica/group.py` & `arabica-1.6.9/arabica/group.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.8/arabica/preprocess.py` & `arabica-1.6.9/arabica/preprocess.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.8/arabica/sentiment.py` & `arabica-1.6.9/arabica/sentiment.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.8/arabica.egg-info/PKG-INFO` & `arabica-1.6.9/arabica.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.6.8
+Version: 1.6.9
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: OSI Approved :: Apache Software License
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
 Project-URL: Bug Tracker, https://github.com/PetrKorab/Arabica/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.9, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![pypi](https://img.shields.io/pypi/v/arabica.svg)](https://pypi.python.org/pypi/arabica)
+[![python](https://img.shields.io/pypi/pyversions/arabica.svg)](https://pypi.python.org/pypi/arabica)
+[![License: MIT](https://badgen.net/badge/license/apache-2-0/blue)]([https://opensource.org/licenses/MIT](https://opensource.org/license/apache-2-0/))
+
+
 # Arabica
 **Python package for exploratory text data analysis**
 
 Text data is often recorded as a time series with significant variability over time. Some examples of time-series text data include Twitter tweets, research article metadata, product reviews, and newspaper headlines. Arabica makes exploratory analysis of these time-series text datasets simple by providing:
 
 * **Descriptive n-gram analysis**: n-gram frequencies
 * **Time-series n-gram analysis**: n-gram frequencies over a period
 * **Text visualization**: n-gram heatmap, line plot, word cloud
 * **Sentiment analysis**: VADER sentiment classifier
+* **Financial sentiment analysis**: with FinVADER
 * **Structural breaks identification**: Jenks Optimization Method
 
 It automatically cleans data from punctuation on input. It can also apply all or a selected combination of the following cleaning operations:
 
 * Remove digits from the text
-* Remove the standard list(s) of stop words
+* Remove the standard list(s) of stopwords
 * Remove an additional list of stop words
 
 Arabica works with **texts** of languages based on the Latin alphabet, uses `cleantext` for punctuation cleaning, and enables stop words removal for languages in the `NLTK` corpus of stopwords.
 
 It reads dates in:
 
 * **US-style**: *MM/DD/YYYY* (2013-12-31, Feb-09-2009, 2013-12-31 11:46:17, etc.)
@@ -48,16 +54,14 @@
 [vaderSentiment](https://pypi.org/project/vaderSentiment) - sentiment analysis, [finvader](https://pypi.org/project/finvader) - financial sentiment analysis,
 and [jenskpy](https://pypi.org/project/jenkspy/) for breakpoint identification.
 
 To install using pip, use:
 
 `pip install arabica`
 
-
-
 ## Usage
 
 * **Import the library**:
 
 
 ``` python
 from arabica import arabica_freq
@@ -65,67 +69,67 @@
 from arabica import coffee_break 
 ```
 
 
 
 * **Choose a method:**
 
-**arabica_freq** enables a set of cleaning operations (lower casing, numbers, common stop words, and additional stop words removal) and returns a dataframe with aggregated unigrams, bigrams, and trigrams frequencies over a period.
+**arabica_freq** enables a specific set of cleaning operations (lower casing, numbers, common stop words, and additional stop words 
+removal) and returns a dataframe with aggregated unigrams, bigrams, and trigrams frequencies over a period.
 
 
 
 ``` python
 def arabica_freq(text: str,                # Text
                  time: str,                # Time
                  date_format: str,         # Date format: 'eur' - European, 'us' - American
                  time_freq: str = '',      # Aggregation period: 'Y'/'M'/'D', if no aggregation: 'ungroup'
                  max_words: int = '',      # Maximum of most frequent n-grams displayed for each period
-                 stopwords: [],            # Languages for common stop words
-                 skip: [],                 # Remove additional list of stopwords
+                 stopwords: [],            # Languages for stop words
+                 skip: [],                 # Remove additional stop words
                  numbers: bool = False,    # Remove all digits
                  lower_case: bool = False  # Lowercase text
 ) 
 ```
 
-**cappuccino** enables cleaning operations (lower casing, numbers, common stop words, and additional stop words 
+**cappuccino**  enables cleaning operations (lower casing, numbers, common stop words, and additional stop words
 removal) and provides plots for descriptive (word cloud) and time-series (heatmap, line plot) visualization.
 
 ``` python
 def cappuccino(text: str,                # Text
                time: str,                # Time
                date_format: str,         # Date format: 'eur' - European, 'us' - American
                plot: str = '',           # Chart type: 'wordcloud'/'heatmap'/'line'
                ngram: int = '',          # N-gram size, 1 = unigram, 2 = bigram, 3 = trigram
                time_freq: str = '',      # Aggregation period: 'Y'/'M', if no aggregation: 'ungroup'
                max_words int = '',       # Maximum of most frequent n-grams displayed for each period
-               stopwords: [],            # Languages for common stop words
-               skip: [] ,                # Remove additional list of stop words
+               stopwords: [],            # Languages for stop words
+               skip: [],                 # Remove additional stop words
                numbers: bool = False,    # Remove numbers
                lower_case: bool = False  # Lowercase text
-)
 ```
 
-**coffee_break** provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. The implemented models are:
-
-* **VADER** is a lexicon and rule-based sentiment classifier attuned explicitly to sentiments expressed in social media. See more [here](https://ojs.aaai.org/index.php/ICWSM/article/view/14550).
+**coffee_break**  provides sentiment analysis and breakpoint identification in aggregated time series of sentiment. The implemented models are:
 
-* **FinVADER** improves VADER's classification accuracy, including two financial lexicons. Available from [here](https://pypi.org/project/finvader/).
+* [VADER](https://ojs.aaai.org/index.php/ICWSM/article/view/14550) is a lexicon and rule-based sentiment classifier attuned explicitly to general language expressed in social media
+  
+* [FinVADER](https://pypi.org/project/finvader/) improves VADER's classification accuracy on financial texts, including two financial lexicons
 
-Structural breaks in the time series are identified with the **Fisher-Jenks algorithm** (Jenks, 1977. Optimal data classification for choropleth maps).
+Break points in the time series are identified with the **Fisher-Jenks algorithm** (Jenks, 1977. Optimal data classification for choropleth maps).
 
 
 ``` python
 def coffee_break(text: str,                 # Text
                  time: str,                 # Time
                  date_format: str,          # Date format: 'eur' - European, 'us' - American
                  model: str,                # Sentiment classifier, 'vader' - general language, 'finvader' - financial text                
-                 skip: [] ,                 # Remove additional list of stop words
+                 skip: [],                  # Remove additional stop words
                  preprocess: bool = False,  # Clean data from numbers and punctuation
                  time_freq: str ='',        # Aggregation period: 'Y'/'M'
-                 n_breaks: int =''          # Number of breaks: min. 2
+                 n_breaks: int =''          # Number of breakpoints: min. 2
 )
 ```
 
 ## Documentation, examples and tutorials
 
 * Read the [documentation](https://arabica.readthedocs.io/en/latest/index.html)
 
@@ -136,13 +140,13 @@
 * Sentiment Analysis and Structural Breaks in Time-Series Text Data [here](https://medium.com/towards-data-science/sentiment-analysis-and-structural-breaks-in-time-series-text-data-8109c712ca2)                        
 * Visualization Module in Arabica Speeds Up Text Data Exploration [here](https://medium.com/towards-data-science/visualization-module-in-arabica-speeds-up-text-data-exploration-47114ad646ce)                                                                                                                          
 * Text as Time Series: Arabica 1.0 Brings New Features for Exploratory Text Data Analysis [here](https://towardsdatascience.com/text-as-time-series-arabica-1-0-brings-new-features-for-exploratory-text-data-analysis-88eaabb84deb?sk=229ec0602d0b8514f25bce501ed9ecb9)   
 
 **Applications:**
 
 * **Business Intelligence:** Customer Satisfaction Measurement with N-gram and Sentiment Analysis [here](https://towardsdatascience.com/customer-satisfaction-measurement-with-n-gram-and-sentiment-analysis-547e291c13a6)                       
+* **Research meta-data description:** Research Article Meta-data Description Made Quick and Easy [here](https://pub.towardsai.net/research-article-meta-data-description-made-quick-and-easy-57754e54b550)
 * **Twitter tweets analysis**
-* **Journal meta-data description**
 
 ---
 
 Please visit [here](https://github.com/PetrKorab/arabica/issues) for any questions, issues, bugs, and suggestions.
```

### Comparing `arabica-1.6.8/pyproject.toml` & `arabica-1.6.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "arabica"
-version = "1.6.8"
+version = "1.6.9"
 authors = [
   { name="Petr Korab", email="xpetrkorab@gmail.com" },
 ]
 description = "Python package for exploratory text data analysis"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">3.9, <3.11"
```

### Comparing `arabica-1.6.8/setup.py` & `arabica-1.6.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
     setuptools.setup(
         name="arabica",
-        version="1.6.8",
+        version="1.6.9",
         author="Petr Koráb",
         author_email="xpetrkorab@gmail.com",
         packages=["arabica"],
         description="Python package for exploratory text data analysis",
         long_description=description,
         long_description_content_type="text/markdown",
         url="https://github.com/PetrKorab/Arabica",
```

