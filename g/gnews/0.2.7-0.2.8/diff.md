# Comparing `tmp/gnews-0.2.7.tar.gz` & `tmp/gnews-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnews-0.2.7.tar", last modified: Fri Nov 12 10:43:31 2021, max compression
+gzip compressed data, was "gnews-0.2.8.tar", last modified: Wed Aug  2 14:38:15 2023, max compression
```

## Comparing `gnews-0.2.7.tar` & `gnews-0.2.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 10:43:31.335326 gnews-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2021-11-12 10:43:19.000000 gnews-0.2.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)    16446 2021-11-12 10:43:31.335326 gnews-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15236 2021-11-12 10:43:19.000000 gnews-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 10:43:31.331326 gnews-0.2.7/gnews/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-11-12 10:43:19.000000 gnews-0.2.7/gnews/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6013 2021-11-12 10:43:19.000000 gnews-0.2.7/gnews/gnews.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 10:43:31.331326 gnews-0.2.7/gnews/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-12 10:43:19.000000 gnews-0.2.7/gnews/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24441 2021-11-12 10:43:19.000000 gnews-0.2.7/gnews/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2291 2021-11-12 10:43:19.000000 gnews-0.2.7/gnews/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-12 10:43:31.331326 gnews-0.2.7/gnews.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16446 2021-11-12 10:43:30.000000 gnews-0.2.7/gnews.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      277 2021-11-12 10:43:31.000000 gnews-0.2.7/gnews.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-12 10:43:30.000000 gnews-0.2.7/gnews.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      124 2021-11-12 10:43:30.000000 gnews-0.2.7/gnews.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-11-12 10:43:30.000000 gnews-0.2.7/gnews.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-12 10:43:31.335326 gnews-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2021-11-12 10:43:19.000000 gnews-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:15.423370 gnews-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-02 14:38:04.000000 gnews-0.2.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17336 2023-08-02 14:38:15.423370 gnews-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16112 2023-08-02 14:38:04.000000 gnews-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:15.415369 gnews-0.2.8/gnews/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-02 14:38:04.000000 gnews-0.2.8/gnews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-08-02 14:38:04.000000 gnews-0.2.8/gnews/gnews.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:15.415369 gnews-0.2.8/gnews/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:04.000000 gnews-0.2.8/gnews/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24441 2023-08-02 14:38:04.000000 gnews-0.2.8/gnews/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-08-02 14:38:04.000000 gnews-0.2.8/gnews/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:15.415369 gnews-0.2.8/gnews.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17336 2023-08-02 14:38:15.000000 gnews-0.2.8/gnews.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-02 14:38:15.000000 gnews-0.2.8/gnews.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:38:15.000000 gnews-0.2.8/gnews.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-02 14:38:15.000000 gnews-0.2.8/gnews.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-02 14:38:15.000000 gnews-0.2.8/gnews.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:38:15.423370 gnews-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-08-02 14:38:04.000000 gnews-0.2.8/setup.py
```

### Comparing `gnews-0.2.7/LICENSE.txt` & `gnews-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gnews-0.2.7/PKG-INFO` & `gnews-0.2.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,65 +1,75 @@
 Metadata-Version: 2.1
 Name: gnews
-Version: 0.2.7
+Version: 0.2.8
 Summary: Provide an API to search for articles on Google News and returns a usable JSON response.
 Home-page: https://github.com/ranahaani/GNews/
 Author: Muhammad Abdullah
 Author-email: ranahaani@gmail.com
-License: UNKNOWN
 Project-URL: Documentation, https://github.com/ranahaani/GNews/blob/master/README.md
 Project-URL: Source, https://github.com/ranahaani/GNews/
 Project-URL: Tracker, https://github.com/ranahaani/GNews/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 [![Download][download-sheild]][download-url]
 [![LinkedIn][linkedin-shield]][linkedin-url]
 
+
+
 <!-- PROJECT LOGO -->
 <br />
 <p align="center">
   <a href="https://github.com/ranahaani/GNews">
     <img src="https://github.com/ranahaani/GNews/raw/master/imgs/logo.png" alt="GNews">
   </a>
-
+  
+  
+  
 <h3 align="center">GNews</h3>
 
   <p align="center">
     A Happy and lightweight Python Package that Provide an API to search for articles on Google News and returns a usable JSON response!
-    <br />
+    <br />    
     <a href="https://github.com/ranahaani/GNews"><strong>Explore the docs »</strong></a>
     <br />
     <br />
+    If you like <b> GNews </b> or if it is useful to you, show your support by buying me a coffee.
+    <br />
+    <a href="https://www.buymeacoffee.com/ranahaani" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" ></a>
+    <br />
+    <br />
     <a href="https://github.com/ranahaani/GNews/blob/master/README.md">View Demo</a>
     ·
     <a href="https://github.com/ranahaani/GNews/issues">Report Bug</a>
     ·
     <a href="https://github.com/ranahaani/GNews/issues">Request Feature</a>
+
   </p>
 
+
 <!-- TABLE OF CONTENTS -->
 <details open="open">
    <summary>Table of Contents</summary>
    <ol>
       <li>
          <a href="#about-gnews">About</a>
          <ul>
@@ -122,14 +132,16 @@
 Google News cover across **141+ countries** with **41+ languages**. On the bottom left side of the Google News page you
 may find a `Language & region` section where you can find all of the supported combinations.
 
 ### Demo
 
 [![GNews Demo][demo-gif]](https://github.com/ranahaani/GNews)
 
+
+
 <!-- GETTING STARTED -->
 
 ## Getting Started
 
 This is an example of how you may give instructions on setting up your project locally. To get a local copy up and
 running follow these simple example steps.
 
@@ -145,15 +157,15 @@
 
 1. Install [docker and docker-compose](https://docs.docker.com/get-docker/).
 2. Set-up your .env environment placing the mongo db credentials.
 3. Run `docker-compose up --build`
 
 #### Install using clone
 
-1. Clone this repository `virtualenv gnews`
+1. Clone this repository `https://github.com/ranahaani/GNews.git`
 2. Start your virtual environment `virtualenv gnews`
 3. Install the requirements with `pip install -r requirements.txt`
 
 <!-- USAGE EXAMPLES -->
 
 ### Example usage
 
@@ -194,40 +206,44 @@
 ### Get news by geo location
 
 * `GNews.get_news_by_location(location)`
 * location can be name of city/state/country
 
 ### Results specification
 
-* It's possible to pass proxy, country, language, period, exclude websites and size during initialization
+* It's possible to pass proxy, country, language, period, start date, end date exclude websites and size during initialization
 
 ```python
-google_news = GNews(language='en', country='US', period='7d', max_results=10, exclude_websites=['yahoo.com', 'cnn.com'],
+google_news = GNews(language='en', country='US', period='7d', start_date=None, end_date=None, max_results=10, exclude_websites=['yahoo.com', 'cnn.com'],
                     proxy=proxy)
 ```
 
 * Or change it to an existing object
 
 ```python
 google_news.period = '7d'  # News from last 7 days
-google_news.results = 10  # number of responses across a keyword
+google_news.max_results = 10  # number of responses across a keyword
 google_news.country = 'United States'  # News from a specific country 
 google_news.language = 'english'  # News in a specific language
 google_news.exclude_websites = ['yahoo.com', 'cnn.com']  # Exclude news from specific website i.e Yahoo.com and CNN.com
+google_news.start_date = (2020, 1, 1) # Search from 1st Jan 2020
+google_news.end_date = (2020, 3, 1) # Search until 1st March 2020
 ```
 
 The format of the timeframe is a string comprised of a number, followed by a letter representing the time operator. For
 example 1y would signify 1 year. Full list of operators below:
 
 ```
  - h = hours (eg: 12h)
  - d = days (eg: 7d)
  - m = months (eg: 6m)
  - y = years (eg: 1y)
  ```
+ 
+Setting the start and end dates can be done by passing in either a datetime or a tuple in the form (YYYY, MM, DD).
 
 #### Supported Countries
 
 ```python
 print(google_news.AVAILABLE_COUNTRIES)
 
 {'Australia': 'AU', 'Botswana': 'BW', 'Canada ': 'CA', 'Ethiopia': 'ET', 'Ghana': 'GH', 'India ': 'IN',
@@ -363,14 +379,18 @@
 
 ## Contact
 
 Muhammad Abdullah - [@ranahaani](https://twitter.com/ranahaani) - ranahaani@gmail.com
 
 Project Link: [https://github.com/ranahaani/GNews](https://github.com/ranahaani/GNews)
 
+Project Link: [https://github.com/ranahaani/GNews](https://github.com/ranahaani/GNews)
+
+[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/ranahaani)
+
 [contributors-shield]: https://img.shields.io/github/contributors/ranahaani/GNews.svg?style=for-the-badge
 
 [contributors-url]: https://github.com/ranahaani/GNews/graphs/contributors
 
 [forks-shield]: https://img.shields.io/github/forks/ranahaani/GNews.svg?style=for-the-badge
 
 [forks-url]: https://github.com/ranahaani/GNews/network/members
@@ -392,9 +412,7 @@
 [download-url]: https://pypistats.org/packages/gnews
 
 [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
 
 [linkedin-url]: https://linkedin.com/in/ranahaani
 
 [demo-gif]: https://github.com/ranahaani/GNews/raw/master/imgs/gnews.gif
-
-
```

#### html2text {}

```diff
@@ -1,33 +1,38 @@
-Metadata-Version: 2.1 Name: gnews Version: 0.2.7 Summary: Provide an API to
+Metadata-Version: 2.1 Name: gnews Version: 0.2.8 Summary: Provide an API to
 search for articles on Google News and returns a usable JSON response. Home-
 page: https://github.com/ranahaani/GNews/ Author: Muhammad Abdullah Author-
-email: ranahaani@gmail.com License: UNKNOWN Project-URL: Documentation, https:/
-/github.com/ranahaani/GNews/blob/master/README.md Project-URL: Source, https://
-github.com/ranahaani/GNews/ Project-URL: Tracker, https://github.com/ranahaani/
-GNews/issues Platform: UNKNOWN Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.2 Classifier: Programming Language :: Python :: 3.3 Classifier:
-Programming Language :: Python :: 3.4 Classifier: Programming Language ::
-Python :: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Description-Content-Type: text/markdown License-File: LICENSE.txt
-[![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
-shield]][issues-url] [![MIT License][license-shield]][license-url] [![Download]
-[download-sheild]][download-url] [![LinkedIn][linkedin-shield]][linkedin-url]
+email: ranahaani@gmail.com Project-URL: Documentation, https://github.com/
+ranahaani/GNews/blob/master/README.md Project-URL: Source, https://github.com/
+ranahaani/GNews/ Project-URL: Tracker, https://github.com/ranahaani/GNews/
+issues Classifier: Development Status :: 5 - Production/Stable Classifier:
+Intended Audience :: Developers Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.2 Classifier: Programming
+Language :: Python :: 3.3 Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Description-Content-Type: text/markdown License-File:
+LICENSE.txt [![Contributors][contributors-shield]][contributors-url] [![Forks]
+[forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues]
+[issues-shield]][issues-url] [![MIT License][license-shield]][license-url] [!
+[Download][download-sheild]][download-url] [![LinkedIn][linkedin-shield]]
+[linkedin-url]
                                     [GNews]
                                 **** GNews ****
    A Happy and lightweight Python Package that Provide an API to search for
          articles on Google News and returns a usable JSON response!
                              Explore_the_docs_Â»
 
+ If you like GNews or if it is useful to you, show your support by buying me a
+                                   coffee.
+                              [Buy_Me_A_Coffee]
+
                   View_Demo Â· Report_Bug Â· Request_Feature
   Table of Contents
    1. About
           o Demo
    2. Getting_Started
           o Installation
           o Setup_with_Docker
@@ -55,54 +60,59 @@
 combinations. ### Demo [![GNews Demo][demo-gif]](https://github.com/ranahaani/
 GNews)  ## Getting Started This is an example of how you may give instructions
 on setting up your project locally. To get a local copy up and running follow
 these simple example steps. ### Installation ``` shell pip install gnews ```
 ### Setup with Docker #### Developing with docker 1. Install [docker and
 docker-compose](https://docs.docker.com/get-docker/). 2. Set-up your .env
 environment placing the mongo db credentials. 3. Run `docker-compose up --
-build` #### Install using clone 1. Clone this repository `virtualenv gnews` 2.
-Start your virtual environment `virtualenv gnews` 3. Install the requirements
-with `pip install -r requirements.txt`  ### Example usage ```python from gnews
-import GNews google_news = GNews() pakistan_news = google_news.get_news
-('Pakistan') print(pakistan_news[0]) ``` ``` [{ 'publisher': 'Aljazeera.com',
-'description': 'Pakistan accuses India of stoking conflict in Indian Ocean '
-'Aljazeera.com', 'published date': 'Tue, 16 Feb 2021 11:50:43 GMT', 'title':
-'Pakistan accuses India of stoking conflict in Indian Ocean - '
-'Aljazeera.com', 'url': 'https://www.aljazeera.com/news/2021/2/16/pakistan-
-accuses-india-of-nuclearizing-indian-ocean' }, ...] ``` ### Get top news *
-`GNews.get_top_news()` ### Get news by keyword * `GNews.get_news(keyword)` ###
-Get news by major topic * `GNews.get_news_by_topic(topic)` * Available topics:
-` WORLD, NATION, BUSINESS, TECHNOLOGY, ENTERTAINMENT, SPORTS, SCIENCE, HEALTH.`
-### Get news by geo location * `GNews.get_news_by_location(location)` *
-location can be name of city/state/country ### Results specification * It's
-possible to pass proxy, country, language, period, exclude websites and size
-during initialization ```python google_news = GNews(language='en',
-country='US', period='7d', max_results=10, exclude_websites=['yahoo.com',
-'cnn.com'], proxy=proxy) ``` * Or change it to an existing object ```python
-google_news.period = '7d' # News from last 7 days google_news.results = 10 #
-number of responses across a keyword google_news.country = 'United States' #
+build` #### Install using clone 1. Clone this repository `https://github.com/
+ranahaani/GNews.git` 2. Start your virtual environment `virtualenv gnews` 3.
+Install the requirements with `pip install -r requirements.txt`  ### Example
+usage ```python from gnews import GNews google_news = GNews() pakistan_news =
+google_news.get_news('Pakistan') print(pakistan_news[0]) ``` ``` [
+{ 'publisher': 'Aljazeera.com', 'description': 'Pakistan accuses India of
+stoking conflict in Indian Ocean ' 'Aljazeera.com', 'published date': 'Tue, 16
+Feb 2021 11:50:43 GMT', 'title': 'Pakistan accuses India of stoking conflict in
+Indian Ocean - ' 'Aljazeera.com', 'url': 'https://www.aljazeera.com/news/2021/
+2/16/pakistan-accuses-india-of-nuclearizing-indian-ocean' }, ...] ``` ### Get
+top news * `GNews.get_top_news()` ### Get news by keyword * `GNews.get_news
+(keyword)` ### Get news by major topic * `GNews.get_news_by_topic(topic)` *
+Available topics:` WORLD, NATION, BUSINESS, TECHNOLOGY, ENTERTAINMENT, SPORTS,
+SCIENCE, HEALTH.` ### Get news by geo location * `GNews.get_news_by_location
+(location)` * location can be name of city/state/country ### Results
+specification * It's possible to pass proxy, country, language, period, start
+date, end date exclude websites and size during initialization ```python
+google_news = GNews(language='en', country='US', period='7d', start_date=None,
+end_date=None, max_results=10, exclude_websites=['yahoo.com', 'cnn.com'],
+proxy=proxy) ``` * Or change it to an existing object ```python
+google_news.period = '7d' # News from last 7 days google_news.max_results = 10
+# number of responses across a keyword google_news.country = 'United States' #
 News from a specific country google_news.language = 'english' # News in a
 specific language google_news.exclude_websites = ['yahoo.com', 'cnn.com'] #
-Exclude news from specific website i.e Yahoo.com and CNN.com ``` The format of
-the timeframe is a string comprised of a number, followed by a letter
+Exclude news from specific website i.e Yahoo.com and CNN.com
+google_news.start_date = (2020, 1, 1) # Search from 1st Jan 2020
+google_news.end_date = (2020, 3, 1) # Search until 1st March 2020 ``` The
+format of the timeframe is a string comprised of a number, followed by a letter
 representing the time operator. For example 1y would signify 1 year. Full list
 of operators below: ``` - h = hours (eg: 12h) - d = days (eg: 7d) - m = months
-(eg: 6m) - y = years (eg: 1y) ``` #### Supported Countries ```python print
-(google_news.AVAILABLE_COUNTRIES) {'Australia': 'AU', 'Botswana': 'BW', 'Canada
-': 'CA', 'Ethiopia': 'ET', 'Ghana': 'GH', 'India ': 'IN', 'Indonesia': 'ID',
-'Ireland': 'IE', 'Israel ': 'IL', 'Kenya': 'KE', 'Latvia': 'LV', 'Malaysia':
-'MY', 'Namibia': 'NA', 'New Zealand': 'NZ', 'Nigeria': 'NG', 'Pakistan': 'PK',
-'Philippines': 'PH', 'Singapore': 'SG', 'South Africa': 'ZA', 'Tanzania': 'TZ',
-'Uganda': 'UG', 'United Kingdom': 'GB', 'United States': 'US', 'Zimbabwe':
-'ZW', 'Czech Republic': 'CZ', 'Germany': 'DE', 'Austria': 'AT', 'Switzerland':
-'CH', 'Argentina': 'AR', 'Chile': 'CL', 'Colombia': 'CO', 'Cuba': 'CU',
-'Mexico': 'MX', 'Peru': 'PE', 'Venezuela': 'VE', 'Belgium ': 'BE', 'France':
-'FR', 'Morocco': 'MA', 'Senegal': 'SN', 'Italy': 'IT', 'Lithuania': 'LT',
-'Hungary': 'HU', 'Netherlands': 'NL', 'Norway': 'NO', 'Poland': 'PL', 'Brazil':
-'BR', 'Portugal': 'PT', 'Romania': 'RO', 'Slovakia': 'SK', 'Slovenia': 'SI',
+(eg: 6m) - y = years (eg: 1y) ``` Setting the start and end dates can be done
+by passing in either a datetime or a tuple in the form (YYYY, MM, DD). ####
+Supported Countries ```python print(google_news.AVAILABLE_COUNTRIES)
+{'Australia': 'AU', 'Botswana': 'BW', 'Canada ': 'CA', 'Ethiopia': 'ET',
+'Ghana': 'GH', 'India ': 'IN', 'Indonesia': 'ID', 'Ireland': 'IE', 'Israel ':
+'IL', 'Kenya': 'KE', 'Latvia': 'LV', 'Malaysia': 'MY', 'Namibia': 'NA', 'New
+Zealand': 'NZ', 'Nigeria': 'NG', 'Pakistan': 'PK', 'Philippines': 'PH',
+'Singapore': 'SG', 'South Africa': 'ZA', 'Tanzania': 'TZ', 'Uganda': 'UG',
+'United Kingdom': 'GB', 'United States': 'US', 'Zimbabwe': 'ZW', 'Czech
+Republic': 'CZ', 'Germany': 'DE', 'Austria': 'AT', 'Switzerland': 'CH',
+'Argentina': 'AR', 'Chile': 'CL', 'Colombia': 'CO', 'Cuba': 'CU', 'Mexico':
+'MX', 'Peru': 'PE', 'Venezuela': 'VE', 'Belgium ': 'BE', 'France': 'FR',
+'Morocco': 'MA', 'Senegal': 'SN', 'Italy': 'IT', 'Lithuania': 'LT', 'Hungary':
+'HU', 'Netherlands': 'NL', 'Norway': 'NO', 'Poland': 'PL', 'Brazil': 'BR',
+'Portugal': 'PT', 'Romania': 'RO', 'Slovakia': 'SK', 'Slovenia': 'SI',
 'Sweden': 'SE', 'Vietnam': 'VN', 'Turkey': 'TR', 'Greece': 'GR', 'Bulgaria':
 'BG', 'Russia': 'RU', 'Ukraine ': 'UA', 'Serbia': 'RS', 'United Arab Emirates':
 'AE', 'Saudi Arabia': 'SA', 'Lebanon': 'LB', 'Egypt': 'EG', 'Bangladesh': 'BD',
 'Thailand': 'TH', 'China': 'CN', 'Taiwan': 'TW', 'Hong Kong': 'HK', 'Japan':
 'JP', 'Republic of Korea': 'KR'} ``` #### Supported Languages ```python print
 (google_news.AVAILABLE_LANGUAGES) {'english': 'en', 'indonesian': 'id',
 'czech': 'cs', 'german': 'de', 'spanish': 'es-419', 'french': 'fr', 'italian':
@@ -164,15 +174,18 @@
 Any contributions you make are **greatly appreciated**. 1. Fork the Project 2.
 Create your Feature Branch (`git checkout -b feature/AmazingFeature`) 3. Commit
 your Changes (`git commit -m 'Add some AmazingFeature'`) 4. Push to the Branch
 (`git push origin feature/AmazingFeature`) 5. Open a Pull Request  ## License
 Distributed under the MIT License. See `LICENSE` for more information.  ##
 Contact Muhammad Abdullah - [@ranahaani](https://twitter.com/ranahaani) -
 ranahaani@gmail.com Project Link: [https://github.com/ranahaani/GNews](https://
-github.com/ranahaani/GNews) [contributors-shield]: https://img.shields.io/
+github.com/ranahaani/GNews) Project Link: [https://github.com/ranahaani/GNews]
+(https://github.com/ranahaani/GNews) [!["Buy Me A Coffee"](https://
+www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://
+www.buymeacoffee.com/ranahaani) [contributors-shield]: https://img.shields.io/
 github/contributors/ranahaani/GNews.svg?style=for-the-badge [contributors-url]:
 https://github.com/ranahaani/GNews/graphs/contributors [forks-shield]: https://
 img.shields.io/github/forks/ranahaani/GNews.svg?style=for-the-badge [forks-
 url]: https://github.com/ranahaani/GNews/network/members [stars-shield]: https:
 //img.shields.io/github/stars/ranahaani/GNews.svg?style=for-the-badge [stars-
 url]: https://github.com/ranahaani/GNews/stargazers [issues-shield]: https://
 img.shields.io/github/issues/ranahaani/GNews.svg?style=for-the-badge [issues-
```

### Comparing `gnews-0.2.7/README.md` & `gnews-0.2.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,36 +2,47 @@
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 [![Download][download-sheild]][download-url]
 [![LinkedIn][linkedin-shield]][linkedin-url]
 
+
+
 <!-- PROJECT LOGO -->
 <br />
 <p align="center">
   <a href="https://github.com/ranahaani/GNews">
     <img src="https://github.com/ranahaani/GNews/raw/master/imgs/logo.png" alt="GNews">
   </a>
-
+  
+  
+  
 <h3 align="center">GNews</h3>
 
   <p align="center">
     A Happy and lightweight Python Package that Provide an API to search for articles on Google News and returns a usable JSON response!
-    <br />
+    <br />    
     <a href="https://github.com/ranahaani/GNews"><strong>Explore the docs »</strong></a>
     <br />
     <br />
+    If you like <b> GNews </b> or if it is useful to you, show your support by buying me a coffee.
+    <br />
+    <a href="https://www.buymeacoffee.com/ranahaani" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" ></a>
+    <br />
+    <br />
     <a href="https://github.com/ranahaani/GNews/blob/master/README.md">View Demo</a>
     ·
     <a href="https://github.com/ranahaani/GNews/issues">Report Bug</a>
     ·
     <a href="https://github.com/ranahaani/GNews/issues">Request Feature</a>
+
   </p>
 
+
 <!-- TABLE OF CONTENTS -->
 <details open="open">
    <summary>Table of Contents</summary>
    <ol>
       <li>
          <a href="#about-gnews">About</a>
          <ul>
@@ -94,14 +105,16 @@
 Google News cover across **141+ countries** with **41+ languages**. On the bottom left side of the Google News page you
 may find a `Language & region` section where you can find all of the supported combinations.
 
 ### Demo
 
 [![GNews Demo][demo-gif]](https://github.com/ranahaani/GNews)
 
+
+
 <!-- GETTING STARTED -->
 
 ## Getting Started
 
 This is an example of how you may give instructions on setting up your project locally. To get a local copy up and
 running follow these simple example steps.
 
@@ -117,15 +130,15 @@
 
 1. Install [docker and docker-compose](https://docs.docker.com/get-docker/).
 2. Set-up your .env environment placing the mongo db credentials.
 3. Run `docker-compose up --build`
 
 #### Install using clone
 
-1. Clone this repository `virtualenv gnews`
+1. Clone this repository `https://github.com/ranahaani/GNews.git`
 2. Start your virtual environment `virtualenv gnews`
 3. Install the requirements with `pip install -r requirements.txt`
 
 <!-- USAGE EXAMPLES -->
 
 ### Example usage
 
@@ -166,40 +179,44 @@
 ### Get news by geo location
 
 * `GNews.get_news_by_location(location)`
 * location can be name of city/state/country
 
 ### Results specification
 
-* It's possible to pass proxy, country, language, period, exclude websites and size during initialization
+* It's possible to pass proxy, country, language, period, start date, end date exclude websites and size during initialization
 
 ```python
-google_news = GNews(language='en', country='US', period='7d', max_results=10, exclude_websites=['yahoo.com', 'cnn.com'],
+google_news = GNews(language='en', country='US', period='7d', start_date=None, end_date=None, max_results=10, exclude_websites=['yahoo.com', 'cnn.com'],
                     proxy=proxy)
 ```
 
 * Or change it to an existing object
 
 ```python
 google_news.period = '7d'  # News from last 7 days
-google_news.results = 10  # number of responses across a keyword
+google_news.max_results = 10  # number of responses across a keyword
 google_news.country = 'United States'  # News from a specific country 
 google_news.language = 'english'  # News in a specific language
 google_news.exclude_websites = ['yahoo.com', 'cnn.com']  # Exclude news from specific website i.e Yahoo.com and CNN.com
+google_news.start_date = (2020, 1, 1) # Search from 1st Jan 2020
+google_news.end_date = (2020, 3, 1) # Search until 1st March 2020
 ```
 
 The format of the timeframe is a string comprised of a number, followed by a letter representing the time operator. For
 example 1y would signify 1 year. Full list of operators below:
 
 ```
  - h = hours (eg: 12h)
  - d = days (eg: 7d)
  - m = months (eg: 6m)
  - y = years (eg: 1y)
  ```
+ 
+Setting the start and end dates can be done by passing in either a datetime or a tuple in the form (YYYY, MM, DD).
 
 #### Supported Countries
 
 ```python
 print(google_news.AVAILABLE_COUNTRIES)
 
 {'Australia': 'AU', 'Botswana': 'BW', 'Canada ': 'CA', 'Ethiopia': 'ET', 'Ghana': 'GH', 'India ': 'IN',
@@ -335,14 +352,18 @@
 
 ## Contact
 
 Muhammad Abdullah - [@ranahaani](https://twitter.com/ranahaani) - ranahaani@gmail.com
 
 Project Link: [https://github.com/ranahaani/GNews](https://github.com/ranahaani/GNews)
 
+Project Link: [https://github.com/ranahaani/GNews](https://github.com/ranahaani/GNews)
+
+[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/ranahaani)
+
 [contributors-shield]: https://img.shields.io/github/contributors/ranahaani/GNews.svg?style=for-the-badge
 
 [contributors-url]: https://github.com/ranahaani/GNews/graphs/contributors
 
 [forks-shield]: https://img.shields.io/github/forks/ranahaani/GNews.svg?style=for-the-badge
 
 [forks-url]: https://github.com/ranahaani/GNews/network/members
```

#### html2text {}

```diff
@@ -4,14 +4,18 @@
 [download-sheild]][download-url] [![LinkedIn][linkedin-shield]][linkedin-url]
                                     [GNews]
                                 **** GNews ****
    A Happy and lightweight Python Package that Provide an API to search for
          articles on Google News and returns a usable JSON response!
                              Explore_the_docs_Â»
 
+ If you like GNews or if it is useful to you, show your support by buying me a
+                                   coffee.
+                              [Buy_Me_A_Coffee]
+
                   View_Demo Â· Report_Bug Â· Request_Feature
   Table of Contents
    1. About
           o Demo
    2. Getting_Started
           o Installation
           o Setup_with_Docker
@@ -39,54 +43,59 @@
 combinations. ### Demo [![GNews Demo][demo-gif]](https://github.com/ranahaani/
 GNews)  ## Getting Started This is an example of how you may give instructions
 on setting up your project locally. To get a local copy up and running follow
 these simple example steps. ### Installation ``` shell pip install gnews ```
 ### Setup with Docker #### Developing with docker 1. Install [docker and
 docker-compose](https://docs.docker.com/get-docker/). 2. Set-up your .env
 environment placing the mongo db credentials. 3. Run `docker-compose up --
-build` #### Install using clone 1. Clone this repository `virtualenv gnews` 2.
-Start your virtual environment `virtualenv gnews` 3. Install the requirements
-with `pip install -r requirements.txt`  ### Example usage ```python from gnews
-import GNews google_news = GNews() pakistan_news = google_news.get_news
-('Pakistan') print(pakistan_news[0]) ``` ``` [{ 'publisher': 'Aljazeera.com',
-'description': 'Pakistan accuses India of stoking conflict in Indian Ocean '
-'Aljazeera.com', 'published date': 'Tue, 16 Feb 2021 11:50:43 GMT', 'title':
-'Pakistan accuses India of stoking conflict in Indian Ocean - '
-'Aljazeera.com', 'url': 'https://www.aljazeera.com/news/2021/2/16/pakistan-
-accuses-india-of-nuclearizing-indian-ocean' }, ...] ``` ### Get top news *
-`GNews.get_top_news()` ### Get news by keyword * `GNews.get_news(keyword)` ###
-Get news by major topic * `GNews.get_news_by_topic(topic)` * Available topics:
-` WORLD, NATION, BUSINESS, TECHNOLOGY, ENTERTAINMENT, SPORTS, SCIENCE, HEALTH.`
-### Get news by geo location * `GNews.get_news_by_location(location)` *
-location can be name of city/state/country ### Results specification * It's
-possible to pass proxy, country, language, period, exclude websites and size
-during initialization ```python google_news = GNews(language='en',
-country='US', period='7d', max_results=10, exclude_websites=['yahoo.com',
-'cnn.com'], proxy=proxy) ``` * Or change it to an existing object ```python
-google_news.period = '7d' # News from last 7 days google_news.results = 10 #
-number of responses across a keyword google_news.country = 'United States' #
+build` #### Install using clone 1. Clone this repository `https://github.com/
+ranahaani/GNews.git` 2. Start your virtual environment `virtualenv gnews` 3.
+Install the requirements with `pip install -r requirements.txt`  ### Example
+usage ```python from gnews import GNews google_news = GNews() pakistan_news =
+google_news.get_news('Pakistan') print(pakistan_news[0]) ``` ``` [
+{ 'publisher': 'Aljazeera.com', 'description': 'Pakistan accuses India of
+stoking conflict in Indian Ocean ' 'Aljazeera.com', 'published date': 'Tue, 16
+Feb 2021 11:50:43 GMT', 'title': 'Pakistan accuses India of stoking conflict in
+Indian Ocean - ' 'Aljazeera.com', 'url': 'https://www.aljazeera.com/news/2021/
+2/16/pakistan-accuses-india-of-nuclearizing-indian-ocean' }, ...] ``` ### Get
+top news * `GNews.get_top_news()` ### Get news by keyword * `GNews.get_news
+(keyword)` ### Get news by major topic * `GNews.get_news_by_topic(topic)` *
+Available topics:` WORLD, NATION, BUSINESS, TECHNOLOGY, ENTERTAINMENT, SPORTS,
+SCIENCE, HEALTH.` ### Get news by geo location * `GNews.get_news_by_location
+(location)` * location can be name of city/state/country ### Results
+specification * It's possible to pass proxy, country, language, period, start
+date, end date exclude websites and size during initialization ```python
+google_news = GNews(language='en', country='US', period='7d', start_date=None,
+end_date=None, max_results=10, exclude_websites=['yahoo.com', 'cnn.com'],
+proxy=proxy) ``` * Or change it to an existing object ```python
+google_news.period = '7d' # News from last 7 days google_news.max_results = 10
+# number of responses across a keyword google_news.country = 'United States' #
 News from a specific country google_news.language = 'english' # News in a
 specific language google_news.exclude_websites = ['yahoo.com', 'cnn.com'] #
-Exclude news from specific website i.e Yahoo.com and CNN.com ``` The format of
-the timeframe is a string comprised of a number, followed by a letter
+Exclude news from specific website i.e Yahoo.com and CNN.com
+google_news.start_date = (2020, 1, 1) # Search from 1st Jan 2020
+google_news.end_date = (2020, 3, 1) # Search until 1st March 2020 ``` The
+format of the timeframe is a string comprised of a number, followed by a letter
 representing the time operator. For example 1y would signify 1 year. Full list
 of operators below: ``` - h = hours (eg: 12h) - d = days (eg: 7d) - m = months
-(eg: 6m) - y = years (eg: 1y) ``` #### Supported Countries ```python print
-(google_news.AVAILABLE_COUNTRIES) {'Australia': 'AU', 'Botswana': 'BW', 'Canada
-': 'CA', 'Ethiopia': 'ET', 'Ghana': 'GH', 'India ': 'IN', 'Indonesia': 'ID',
-'Ireland': 'IE', 'Israel ': 'IL', 'Kenya': 'KE', 'Latvia': 'LV', 'Malaysia':
-'MY', 'Namibia': 'NA', 'New Zealand': 'NZ', 'Nigeria': 'NG', 'Pakistan': 'PK',
-'Philippines': 'PH', 'Singapore': 'SG', 'South Africa': 'ZA', 'Tanzania': 'TZ',
-'Uganda': 'UG', 'United Kingdom': 'GB', 'United States': 'US', 'Zimbabwe':
-'ZW', 'Czech Republic': 'CZ', 'Germany': 'DE', 'Austria': 'AT', 'Switzerland':
-'CH', 'Argentina': 'AR', 'Chile': 'CL', 'Colombia': 'CO', 'Cuba': 'CU',
-'Mexico': 'MX', 'Peru': 'PE', 'Venezuela': 'VE', 'Belgium ': 'BE', 'France':
-'FR', 'Morocco': 'MA', 'Senegal': 'SN', 'Italy': 'IT', 'Lithuania': 'LT',
-'Hungary': 'HU', 'Netherlands': 'NL', 'Norway': 'NO', 'Poland': 'PL', 'Brazil':
-'BR', 'Portugal': 'PT', 'Romania': 'RO', 'Slovakia': 'SK', 'Slovenia': 'SI',
+(eg: 6m) - y = years (eg: 1y) ``` Setting the start and end dates can be done
+by passing in either a datetime or a tuple in the form (YYYY, MM, DD). ####
+Supported Countries ```python print(google_news.AVAILABLE_COUNTRIES)
+{'Australia': 'AU', 'Botswana': 'BW', 'Canada ': 'CA', 'Ethiopia': 'ET',
+'Ghana': 'GH', 'India ': 'IN', 'Indonesia': 'ID', 'Ireland': 'IE', 'Israel ':
+'IL', 'Kenya': 'KE', 'Latvia': 'LV', 'Malaysia': 'MY', 'Namibia': 'NA', 'New
+Zealand': 'NZ', 'Nigeria': 'NG', 'Pakistan': 'PK', 'Philippines': 'PH',
+'Singapore': 'SG', 'South Africa': 'ZA', 'Tanzania': 'TZ', 'Uganda': 'UG',
+'United Kingdom': 'GB', 'United States': 'US', 'Zimbabwe': 'ZW', 'Czech
+Republic': 'CZ', 'Germany': 'DE', 'Austria': 'AT', 'Switzerland': 'CH',
+'Argentina': 'AR', 'Chile': 'CL', 'Colombia': 'CO', 'Cuba': 'CU', 'Mexico':
+'MX', 'Peru': 'PE', 'Venezuela': 'VE', 'Belgium ': 'BE', 'France': 'FR',
+'Morocco': 'MA', 'Senegal': 'SN', 'Italy': 'IT', 'Lithuania': 'LT', 'Hungary':
+'HU', 'Netherlands': 'NL', 'Norway': 'NO', 'Poland': 'PL', 'Brazil': 'BR',
+'Portugal': 'PT', 'Romania': 'RO', 'Slovakia': 'SK', 'Slovenia': 'SI',
 'Sweden': 'SE', 'Vietnam': 'VN', 'Turkey': 'TR', 'Greece': 'GR', 'Bulgaria':
 'BG', 'Russia': 'RU', 'Ukraine ': 'UA', 'Serbia': 'RS', 'United Arab Emirates':
 'AE', 'Saudi Arabia': 'SA', 'Lebanon': 'LB', 'Egypt': 'EG', 'Bangladesh': 'BD',
 'Thailand': 'TH', 'China': 'CN', 'Taiwan': 'TW', 'Hong Kong': 'HK', 'Japan':
 'JP', 'Republic of Korea': 'KR'} ``` #### Supported Languages ```python print
 (google_news.AVAILABLE_LANGUAGES) {'english': 'en', 'indonesian': 'id',
 'czech': 'cs', 'german': 'de', 'spanish': 'es-419', 'french': 'fr', 'italian':
@@ -148,15 +157,18 @@
 Any contributions you make are **greatly appreciated**. 1. Fork the Project 2.
 Create your Feature Branch (`git checkout -b feature/AmazingFeature`) 3. Commit
 your Changes (`git commit -m 'Add some AmazingFeature'`) 4. Push to the Branch
 (`git push origin feature/AmazingFeature`) 5. Open a Pull Request  ## License
 Distributed under the MIT License. See `LICENSE` for more information.  ##
 Contact Muhammad Abdullah - [@ranahaani](https://twitter.com/ranahaani) -
 ranahaani@gmail.com Project Link: [https://github.com/ranahaani/GNews](https://
-github.com/ranahaani/GNews) [contributors-shield]: https://img.shields.io/
+github.com/ranahaani/GNews) Project Link: [https://github.com/ranahaani/GNews]
+(https://github.com/ranahaani/GNews) [!["Buy Me A Coffee"](https://
+www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://
+www.buymeacoffee.com/ranahaani) [contributors-shield]: https://img.shields.io/
 github/contributors/ranahaani/GNews.svg?style=for-the-badge [contributors-url]:
 https://github.com/ranahaani/GNews/graphs/contributors [forks-shield]: https://
 img.shields.io/github/forks/ranahaani/GNews.svg?style=for-the-badge [forks-
 url]: https://github.com/ranahaani/GNews/network/members [stars-shield]: https:
 //img.shields.io/github/stars/ranahaani/GNews.svg?style=for-the-badge [stars-
 url]: https://github.com/ranahaani/GNews/stargazers [issues-shield]: https://
 img.shields.io/github/issues/ranahaani/GNews.svg?style=for-the-badge [issues-
```

### Comparing `gnews-0.2.7/gnews/utils/constants.py` & `gnews-0.2.8/gnews/utils/constants.py`

 * *Files identical despite different names*

### Comparing `gnews-0.2.7/gnews/utils/utils.py` & `gnews-0.2.8/gnews/utils/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,26 @@
 import hashlib
 import json
 import logging
 import re
 
-import pip
 import pymongo
 import requests
+from gnews.utils.constants import AVAILABLE_COUNTRIES, AVAILABLE_LANGUAGES, GOOGLE_NEWS_REGEX
 from pymongo import MongoClient
 
-from gnews.utils.constants import AVAILABLE_LANGUAGES, AVAILABLE_COUNTRIES, GOOGLE_NEWS_REGEX
-
-
 
 def lang_mapping(lang):
     return AVAILABLE_LANGUAGES.get(lang)
 
 
 def country_mapping(country):
     return AVAILABLE_COUNTRIES.get(country)
 
 
-def import_or_install(package):
-    try:
-        __import__(package)
-    except ImportError:
-        if hasattr(pip, 'main'):
-            pip.main(['install', package])
-        else:
-            pip._internal.main(['install', package])
-
-
 def connect_database(db_user, db_pw, db_name, collection_name):
     """Mongo DB Establish Cluster Connection"""
 
     # .env file Structure:
 
     # DB_USER="..."
     # DB_PW="..."
```

### Comparing `gnews-0.2.7/gnews.egg-info/PKG-INFO` & `gnews-0.2.8/gnews.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,65 +1,75 @@
 Metadata-Version: 2.1
 Name: gnews
-Version: 0.2.7
+Version: 0.2.8
 Summary: Provide an API to search for articles on Google News and returns a usable JSON response.
 Home-page: https://github.com/ranahaani/GNews/
 Author: Muhammad Abdullah
 Author-email: ranahaani@gmail.com
-License: UNKNOWN
 Project-URL: Documentation, https://github.com/ranahaani/GNews/blob/master/README.md
 Project-URL: Source, https://github.com/ranahaani/GNews/
 Project-URL: Tracker, https://github.com/ranahaani/GNews/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 [![Download][download-sheild]][download-url]
 [![LinkedIn][linkedin-shield]][linkedin-url]
 
+
+
 <!-- PROJECT LOGO -->
 <br />
 <p align="center">
   <a href="https://github.com/ranahaani/GNews">
     <img src="https://github.com/ranahaani/GNews/raw/master/imgs/logo.png" alt="GNews">
   </a>
-
+  
+  
+  
 <h3 align="center">GNews</h3>
 
   <p align="center">
     A Happy and lightweight Python Package that Provide an API to search for articles on Google News and returns a usable JSON response!
-    <br />
+    <br />    
     <a href="https://github.com/ranahaani/GNews"><strong>Explore the docs »</strong></a>
     <br />
     <br />
+    If you like <b> GNews </b> or if it is useful to you, show your support by buying me a coffee.
+    <br />
+    <a href="https://www.buymeacoffee.com/ranahaani" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" ></a>
+    <br />
+    <br />
     <a href="https://github.com/ranahaani/GNews/blob/master/README.md">View Demo</a>
     ·
     <a href="https://github.com/ranahaani/GNews/issues">Report Bug</a>
     ·
     <a href="https://github.com/ranahaani/GNews/issues">Request Feature</a>
+
   </p>
 
+
 <!-- TABLE OF CONTENTS -->
 <details open="open">
    <summary>Table of Contents</summary>
    <ol>
       <li>
          <a href="#about-gnews">About</a>
          <ul>
@@ -122,14 +132,16 @@
 Google News cover across **141+ countries** with **41+ languages**. On the bottom left side of the Google News page you
 may find a `Language & region` section where you can find all of the supported combinations.
 
 ### Demo
 
 [![GNews Demo][demo-gif]](https://github.com/ranahaani/GNews)
 
+
+
 <!-- GETTING STARTED -->
 
 ## Getting Started
 
 This is an example of how you may give instructions on setting up your project locally. To get a local copy up and
 running follow these simple example steps.
 
@@ -145,15 +157,15 @@
 
 1. Install [docker and docker-compose](https://docs.docker.com/get-docker/).
 2. Set-up your .env environment placing the mongo db credentials.
 3. Run `docker-compose up --build`
 
 #### Install using clone
 
-1. Clone this repository `virtualenv gnews`
+1. Clone this repository `https://github.com/ranahaani/GNews.git`
 2. Start your virtual environment `virtualenv gnews`
 3. Install the requirements with `pip install -r requirements.txt`
 
 <!-- USAGE EXAMPLES -->
 
 ### Example usage
 
@@ -194,40 +206,44 @@
 ### Get news by geo location
 
 * `GNews.get_news_by_location(location)`
 * location can be name of city/state/country
 
 ### Results specification
 
-* It's possible to pass proxy, country, language, period, exclude websites and size during initialization
+* It's possible to pass proxy, country, language, period, start date, end date exclude websites and size during initialization
 
 ```python
-google_news = GNews(language='en', country='US', period='7d', max_results=10, exclude_websites=['yahoo.com', 'cnn.com'],
+google_news = GNews(language='en', country='US', period='7d', start_date=None, end_date=None, max_results=10, exclude_websites=['yahoo.com', 'cnn.com'],
                     proxy=proxy)
 ```
 
 * Or change it to an existing object
 
 ```python
 google_news.period = '7d'  # News from last 7 days
-google_news.results = 10  # number of responses across a keyword
+google_news.max_results = 10  # number of responses across a keyword
 google_news.country = 'United States'  # News from a specific country 
 google_news.language = 'english'  # News in a specific language
 google_news.exclude_websites = ['yahoo.com', 'cnn.com']  # Exclude news from specific website i.e Yahoo.com and CNN.com
+google_news.start_date = (2020, 1, 1) # Search from 1st Jan 2020
+google_news.end_date = (2020, 3, 1) # Search until 1st March 2020
 ```
 
 The format of the timeframe is a string comprised of a number, followed by a letter representing the time operator. For
 example 1y would signify 1 year. Full list of operators below:
 
 ```
  - h = hours (eg: 12h)
  - d = days (eg: 7d)
  - m = months (eg: 6m)
  - y = years (eg: 1y)
  ```
+ 
+Setting the start and end dates can be done by passing in either a datetime or a tuple in the form (YYYY, MM, DD).
 
 #### Supported Countries
 
 ```python
 print(google_news.AVAILABLE_COUNTRIES)
 
 {'Australia': 'AU', 'Botswana': 'BW', 'Canada ': 'CA', 'Ethiopia': 'ET', 'Ghana': 'GH', 'India ': 'IN',
@@ -363,14 +379,18 @@
 
 ## Contact
 
 Muhammad Abdullah - [@ranahaani](https://twitter.com/ranahaani) - ranahaani@gmail.com
 
 Project Link: [https://github.com/ranahaani/GNews](https://github.com/ranahaani/GNews)
 
+Project Link: [https://github.com/ranahaani/GNews](https://github.com/ranahaani/GNews)
+
+[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/ranahaani)
+
 [contributors-shield]: https://img.shields.io/github/contributors/ranahaani/GNews.svg?style=for-the-badge
 
 [contributors-url]: https://github.com/ranahaani/GNews/graphs/contributors
 
 [forks-shield]: https://img.shields.io/github/forks/ranahaani/GNews.svg?style=for-the-badge
 
 [forks-url]: https://github.com/ranahaani/GNews/network/members
@@ -392,9 +412,7 @@
 [download-url]: https://pypistats.org/packages/gnews
 
 [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
 
 [linkedin-url]: https://linkedin.com/in/ranahaani
 
 [demo-gif]: https://github.com/ranahaani/GNews/raw/master/imgs/gnews.gif
-
-
```

#### html2text {}

```diff
@@ -1,33 +1,38 @@
-Metadata-Version: 2.1 Name: gnews Version: 0.2.7 Summary: Provide an API to
+Metadata-Version: 2.1 Name: gnews Version: 0.2.8 Summary: Provide an API to
 search for articles on Google News and returns a usable JSON response. Home-
 page: https://github.com/ranahaani/GNews/ Author: Muhammad Abdullah Author-
-email: ranahaani@gmail.com License: UNKNOWN Project-URL: Documentation, https:/
-/github.com/ranahaani/GNews/blob/master/README.md Project-URL: Source, https://
-github.com/ranahaani/GNews/ Project-URL: Tracker, https://github.com/ranahaani/
-GNews/issues Platform: UNKNOWN Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.2 Classifier: Programming Language :: Python :: 3.3 Classifier:
-Programming Language :: Python :: 3.4 Classifier: Programming Language ::
-Python :: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Description-Content-Type: text/markdown License-File: LICENSE.txt
-[![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
-shield]][issues-url] [![MIT License][license-shield]][license-url] [![Download]
-[download-sheild]][download-url] [![LinkedIn][linkedin-shield]][linkedin-url]
+email: ranahaani@gmail.com Project-URL: Documentation, https://github.com/
+ranahaani/GNews/blob/master/README.md Project-URL: Source, https://github.com/
+ranahaani/GNews/ Project-URL: Tracker, https://github.com/ranahaani/GNews/
+issues Classifier: Development Status :: 5 - Production/Stable Classifier:
+Intended Audience :: Developers Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.2 Classifier: Programming
+Language :: Python :: 3.3 Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Description-Content-Type: text/markdown License-File:
+LICENSE.txt [![Contributors][contributors-shield]][contributors-url] [![Forks]
+[forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues]
+[issues-shield]][issues-url] [![MIT License][license-shield]][license-url] [!
+[Download][download-sheild]][download-url] [![LinkedIn][linkedin-shield]]
+[linkedin-url]
                                     [GNews]
                                 **** GNews ****
    A Happy and lightweight Python Package that Provide an API to search for
          articles on Google News and returns a usable JSON response!
                              Explore_the_docs_Â»
 
+ If you like GNews or if it is useful to you, show your support by buying me a
+                                   coffee.
+                              [Buy_Me_A_Coffee]
+
                   View_Demo Â· Report_Bug Â· Request_Feature
   Table of Contents
    1. About
           o Demo
    2. Getting_Started
           o Installation
           o Setup_with_Docker
@@ -55,54 +60,59 @@
 combinations. ### Demo [![GNews Demo][demo-gif]](https://github.com/ranahaani/
 GNews)  ## Getting Started This is an example of how you may give instructions
 on setting up your project locally. To get a local copy up and running follow
 these simple example steps. ### Installation ``` shell pip install gnews ```
 ### Setup with Docker #### Developing with docker 1. Install [docker and
 docker-compose](https://docs.docker.com/get-docker/). 2. Set-up your .env
 environment placing the mongo db credentials. 3. Run `docker-compose up --
-build` #### Install using clone 1. Clone this repository `virtualenv gnews` 2.
-Start your virtual environment `virtualenv gnews` 3. Install the requirements
-with `pip install -r requirements.txt`  ### Example usage ```python from gnews
-import GNews google_news = GNews() pakistan_news = google_news.get_news
-('Pakistan') print(pakistan_news[0]) ``` ``` [{ 'publisher': 'Aljazeera.com',
-'description': 'Pakistan accuses India of stoking conflict in Indian Ocean '
-'Aljazeera.com', 'published date': 'Tue, 16 Feb 2021 11:50:43 GMT', 'title':
-'Pakistan accuses India of stoking conflict in Indian Ocean - '
-'Aljazeera.com', 'url': 'https://www.aljazeera.com/news/2021/2/16/pakistan-
-accuses-india-of-nuclearizing-indian-ocean' }, ...] ``` ### Get top news *
-`GNews.get_top_news()` ### Get news by keyword * `GNews.get_news(keyword)` ###
-Get news by major topic * `GNews.get_news_by_topic(topic)` * Available topics:
-` WORLD, NATION, BUSINESS, TECHNOLOGY, ENTERTAINMENT, SPORTS, SCIENCE, HEALTH.`
-### Get news by geo location * `GNews.get_news_by_location(location)` *
-location can be name of city/state/country ### Results specification * It's
-possible to pass proxy, country, language, period, exclude websites and size
-during initialization ```python google_news = GNews(language='en',
-country='US', period='7d', max_results=10, exclude_websites=['yahoo.com',
-'cnn.com'], proxy=proxy) ``` * Or change it to an existing object ```python
-google_news.period = '7d' # News from last 7 days google_news.results = 10 #
-number of responses across a keyword google_news.country = 'United States' #
+build` #### Install using clone 1. Clone this repository `https://github.com/
+ranahaani/GNews.git` 2. Start your virtual environment `virtualenv gnews` 3.
+Install the requirements with `pip install -r requirements.txt`  ### Example
+usage ```python from gnews import GNews google_news = GNews() pakistan_news =
+google_news.get_news('Pakistan') print(pakistan_news[0]) ``` ``` [
+{ 'publisher': 'Aljazeera.com', 'description': 'Pakistan accuses India of
+stoking conflict in Indian Ocean ' 'Aljazeera.com', 'published date': 'Tue, 16
+Feb 2021 11:50:43 GMT', 'title': 'Pakistan accuses India of stoking conflict in
+Indian Ocean - ' 'Aljazeera.com', 'url': 'https://www.aljazeera.com/news/2021/
+2/16/pakistan-accuses-india-of-nuclearizing-indian-ocean' }, ...] ``` ### Get
+top news * `GNews.get_top_news()` ### Get news by keyword * `GNews.get_news
+(keyword)` ### Get news by major topic * `GNews.get_news_by_topic(topic)` *
+Available topics:` WORLD, NATION, BUSINESS, TECHNOLOGY, ENTERTAINMENT, SPORTS,
+SCIENCE, HEALTH.` ### Get news by geo location * `GNews.get_news_by_location
+(location)` * location can be name of city/state/country ### Results
+specification * It's possible to pass proxy, country, language, period, start
+date, end date exclude websites and size during initialization ```python
+google_news = GNews(language='en', country='US', period='7d', start_date=None,
+end_date=None, max_results=10, exclude_websites=['yahoo.com', 'cnn.com'],
+proxy=proxy) ``` * Or change it to an existing object ```python
+google_news.period = '7d' # News from last 7 days google_news.max_results = 10
+# number of responses across a keyword google_news.country = 'United States' #
 News from a specific country google_news.language = 'english' # News in a
 specific language google_news.exclude_websites = ['yahoo.com', 'cnn.com'] #
-Exclude news from specific website i.e Yahoo.com and CNN.com ``` The format of
-the timeframe is a string comprised of a number, followed by a letter
+Exclude news from specific website i.e Yahoo.com and CNN.com
+google_news.start_date = (2020, 1, 1) # Search from 1st Jan 2020
+google_news.end_date = (2020, 3, 1) # Search until 1st March 2020 ``` The
+format of the timeframe is a string comprised of a number, followed by a letter
 representing the time operator. For example 1y would signify 1 year. Full list
 of operators below: ``` - h = hours (eg: 12h) - d = days (eg: 7d) - m = months
-(eg: 6m) - y = years (eg: 1y) ``` #### Supported Countries ```python print
-(google_news.AVAILABLE_COUNTRIES) {'Australia': 'AU', 'Botswana': 'BW', 'Canada
-': 'CA', 'Ethiopia': 'ET', 'Ghana': 'GH', 'India ': 'IN', 'Indonesia': 'ID',
-'Ireland': 'IE', 'Israel ': 'IL', 'Kenya': 'KE', 'Latvia': 'LV', 'Malaysia':
-'MY', 'Namibia': 'NA', 'New Zealand': 'NZ', 'Nigeria': 'NG', 'Pakistan': 'PK',
-'Philippines': 'PH', 'Singapore': 'SG', 'South Africa': 'ZA', 'Tanzania': 'TZ',
-'Uganda': 'UG', 'United Kingdom': 'GB', 'United States': 'US', 'Zimbabwe':
-'ZW', 'Czech Republic': 'CZ', 'Germany': 'DE', 'Austria': 'AT', 'Switzerland':
-'CH', 'Argentina': 'AR', 'Chile': 'CL', 'Colombia': 'CO', 'Cuba': 'CU',
-'Mexico': 'MX', 'Peru': 'PE', 'Venezuela': 'VE', 'Belgium ': 'BE', 'France':
-'FR', 'Morocco': 'MA', 'Senegal': 'SN', 'Italy': 'IT', 'Lithuania': 'LT',
-'Hungary': 'HU', 'Netherlands': 'NL', 'Norway': 'NO', 'Poland': 'PL', 'Brazil':
-'BR', 'Portugal': 'PT', 'Romania': 'RO', 'Slovakia': 'SK', 'Slovenia': 'SI',
+(eg: 6m) - y = years (eg: 1y) ``` Setting the start and end dates can be done
+by passing in either a datetime or a tuple in the form (YYYY, MM, DD). ####
+Supported Countries ```python print(google_news.AVAILABLE_COUNTRIES)
+{'Australia': 'AU', 'Botswana': 'BW', 'Canada ': 'CA', 'Ethiopia': 'ET',
+'Ghana': 'GH', 'India ': 'IN', 'Indonesia': 'ID', 'Ireland': 'IE', 'Israel ':
+'IL', 'Kenya': 'KE', 'Latvia': 'LV', 'Malaysia': 'MY', 'Namibia': 'NA', 'New
+Zealand': 'NZ', 'Nigeria': 'NG', 'Pakistan': 'PK', 'Philippines': 'PH',
+'Singapore': 'SG', 'South Africa': 'ZA', 'Tanzania': 'TZ', 'Uganda': 'UG',
+'United Kingdom': 'GB', 'United States': 'US', 'Zimbabwe': 'ZW', 'Czech
+Republic': 'CZ', 'Germany': 'DE', 'Austria': 'AT', 'Switzerland': 'CH',
+'Argentina': 'AR', 'Chile': 'CL', 'Colombia': 'CO', 'Cuba': 'CU', 'Mexico':
+'MX', 'Peru': 'PE', 'Venezuela': 'VE', 'Belgium ': 'BE', 'France': 'FR',
+'Morocco': 'MA', 'Senegal': 'SN', 'Italy': 'IT', 'Lithuania': 'LT', 'Hungary':
+'HU', 'Netherlands': 'NL', 'Norway': 'NO', 'Poland': 'PL', 'Brazil': 'BR',
+'Portugal': 'PT', 'Romania': 'RO', 'Slovakia': 'SK', 'Slovenia': 'SI',
 'Sweden': 'SE', 'Vietnam': 'VN', 'Turkey': 'TR', 'Greece': 'GR', 'Bulgaria':
 'BG', 'Russia': 'RU', 'Ukraine ': 'UA', 'Serbia': 'RS', 'United Arab Emirates':
 'AE', 'Saudi Arabia': 'SA', 'Lebanon': 'LB', 'Egypt': 'EG', 'Bangladesh': 'BD',
 'Thailand': 'TH', 'China': 'CN', 'Taiwan': 'TW', 'Hong Kong': 'HK', 'Japan':
 'JP', 'Republic of Korea': 'KR'} ``` #### Supported Languages ```python print
 (google_news.AVAILABLE_LANGUAGES) {'english': 'en', 'indonesian': 'id',
 'czech': 'cs', 'german': 'de', 'spanish': 'es-419', 'french': 'fr', 'italian':
@@ -164,15 +174,18 @@
 Any contributions you make are **greatly appreciated**. 1. Fork the Project 2.
 Create your Feature Branch (`git checkout -b feature/AmazingFeature`) 3. Commit
 your Changes (`git commit -m 'Add some AmazingFeature'`) 4. Push to the Branch
 (`git push origin feature/AmazingFeature`) 5. Open a Pull Request  ## License
 Distributed under the MIT License. See `LICENSE` for more information.  ##
 Contact Muhammad Abdullah - [@ranahaani](https://twitter.com/ranahaani) -
 ranahaani@gmail.com Project Link: [https://github.com/ranahaani/GNews](https://
-github.com/ranahaani/GNews) [contributors-shield]: https://img.shields.io/
+github.com/ranahaani/GNews) Project Link: [https://github.com/ranahaani/GNews]
+(https://github.com/ranahaani/GNews) [!["Buy Me A Coffee"](https://
+www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://
+www.buymeacoffee.com/ranahaani) [contributors-shield]: https://img.shields.io/
 github/contributors/ranahaani/GNews.svg?style=for-the-badge [contributors-url]:
 https://github.com/ranahaani/GNews/graphs/contributors [forks-shield]: https://
 img.shields.io/github/forks/ranahaani/GNews.svg?style=for-the-badge [forks-
 url]: https://github.com/ranahaani/GNews/network/members [stars-shield]: https:
 //img.shields.io/github/stars/ranahaani/GNews.svg?style=for-the-badge [stars-
 url]: https://github.com/ranahaani/GNews/stargazers [issues-shield]: https://
 img.shields.io/github/issues/ranahaani/GNews.svg?style=for-the-badge [issues-
```

### Comparing `gnews-0.2.7/setup.py` & `gnews-0.2.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='gnews',
-    version='0.2.7',
+    version='0.2.8',
     author="Muhammad Abdullah",
     author_email="ranahaani@gmail.com",
     description='Provide an API to search for articles on Google News and returns a usable JSON response.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=requirements,
@@ -31,11 +31,12 @@
         'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
 )
```

