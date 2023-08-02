# Comparing `tmp/coziepy-0.0.2.tar.gz` & `tmp/coziepy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coziepy-0.0.2.tar", last modified: Thu Jul 20 14:37:03 2023, max compression
+gzip compressed data, was "coziepy-0.0.3.tar", last modified: Wed Aug  2 18:19:25 2023, max compression
```

## Comparing `coziepy-0.0.2.tar` & `coziepy-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 14:37:03.630741 coziepy-0.0.2/
--rw-rw-rw-   0        0        0    35823 2023-04-01 08:53:49.000000 coziepy-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       11 2023-07-20 14:26:44.000000 coziepy-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      978 2023-07-20 14:37:03.627741 coziepy-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      391 2023-07-20 07:53:27.000000 coziepy-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 14:37:03.541648 coziepy-0.0.2/coziepy/
--rw-rw-rw-   0        0        0       74 2023-07-19 06:43:46.000000 coziepy-0.0.2/coziepy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 14:37:03.613858 coziepy-0.0.2/coziepy/cozie/
--rw-rw-rw-   0        0        0        0 2023-07-19 06:42:23.000000 coziepy-0.0.2/coziepy/cozie/__init__.py
--rw-rw-rw-   0        0        0    15133 2023-07-20 14:34:08.000000 coziepy-0.0.2/coziepy/cozie/cozie.py
-drwxrwxrwx   0        0        0        0 2023-07-20 14:37:03.621930 coziepy-0.0.2/coziepy/cozieplot/
--rw-rw-rw-   0        0        0        0 2023-07-19 06:42:23.000000 coziepy-0.0.2/coziepy/cozieplot/__init__.py
--rw-rw-rw-   0        0        0    45702 2023-07-20 14:33:15.000000 coziepy-0.0.2/coziepy/cozieplot/cozieplot.py
--rw-rw-rw-   0        0        0        6 2023-07-19 06:44:29.000000 coziepy-0.0.2/coziepy/coziepy.py
-drwxrwxrwx   0        0        0        0 2023-07-20 14:37:03.604772 coziepy-0.0.2/coziepy.egg-info/
--rw-rw-rw-   0        0        0      978 2023-07-20 14:37:03.000000 coziepy-0.0.2/coziepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-07-20 14:37:03.000000 coziepy-0.0.2/coziepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 14:37:03.000000 coziepy-0.0.2/coziepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      229 2023-07-20 14:37:03.000000 coziepy-0.0.2/coziepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-20 14:37:03.000000 coziepy-0.0.2/coziepy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1243 2023-07-20 14:36:27.000000 coziepy-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-20 14:37:03.630741 coziepy-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      273 2023-07-20 14:29:39.000000 coziepy-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 18:19:25.951647 coziepy-0.0.3/
+-rw-rw-rw-   0        0        0    35823 2023-04-01 08:53:49.000000 coziepy-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       11 2023-07-20 14:26:44.000000 coziepy-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1464 2023-08-02 18:19:25.949638 coziepy-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      877 2023-07-20 14:56:03.000000 coziepy-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 18:19:25.907632 coziepy-0.0.3/coziepy/
+-rw-rw-rw-   0        0        0       74 2023-07-19 06:43:46.000000 coziepy-0.0.3/coziepy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 18:19:25.937632 coziepy-0.0.3/coziepy/cozie/
+-rw-rw-rw-   0        0        0        0 2023-07-19 06:42:23.000000 coziepy-0.0.3/coziepy/cozie/__init__.py
+-rw-rw-rw-   0        0        0    15133 2023-07-20 14:34:08.000000 coziepy-0.0.3/coziepy/cozie/cozie.py
+drwxrwxrwx   0        0        0        0 2023-08-02 18:19:25.944631 coziepy-0.0.3/coziepy/cozieplot/
+-rw-rw-rw-   0        0        0        0 2023-07-19 06:42:23.000000 coziepy-0.0.3/coziepy/cozieplot/__init__.py
+-rw-rw-rw-   0        0        0    45700 2023-07-20 16:27:06.000000 coziepy-0.0.3/coziepy/cozieplot/cozieplot.py
+-rw-rw-rw-   0        0        0        6 2023-07-19 06:44:29.000000 coziepy-0.0.3/coziepy/coziepy.py
+drwxrwxrwx   0        0        0        0 2023-08-02 18:19:25.930634 coziepy-0.0.3/coziepy.egg-info/
+-rw-rw-rw-   0        0        0     1464 2023-08-02 18:19:25.000000 coziepy-0.0.3/coziepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-08-02 18:19:25.000000 coziepy-0.0.3/coziepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 18:19:25.000000 coziepy-0.0.3/coziepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      245 2023-08-02 18:19:25.000000 coziepy-0.0.3/coziepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-08-02 18:19:25.000000 coziepy-0.0.3/coziepy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1269 2023-08-02 18:13:29.000000 coziepy-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-02 18:19:25.952634 coziepy-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      273 2023-07-20 14:29:39.000000 coziepy-0.0.3/setup.py
```

### Comparing `coziepy-0.0.2/LICENSE` & `coziepy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `coziepy-0.0.2/coziepy/cozie/cozie.py` & `coziepy-0.0.3/coziepy/cozie/cozie.py`

 * *Files identical despite different names*

### Comparing `coziepy-0.0.2/coziepy/cozieplot/cozieplot.py` & `coziepy-0.0.3/coziepy/cozieplot/cozieplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
     # Plot timestamp difference (index-timestamp -lambda-timestamp)- histogram
     if len(df2['dTL'].values)>1: # Skip the histogram if there is not at least two values in the dataframe.
       axs[2][1].hist(df2['dTL'].values, bins=100, edgecolor='black')
       axs[2][1].set_xlabel('Duration [min]') 
       axs[2][1].set_ylabel('Counts [#]')
       axs[2][1].set_title('Duration between Timestamps (Histogram)')
 
-    plt.show()
+    #plt.show()
     
     return fig, axs
   
   def ts_inspection2(self, column_name, id_participant):  
     """
     Function to plot time-series data in detail for one participant
     Arguments
@@ -280,15 +280,15 @@
             df_participant[modality].max(),
             ]
     fig.add_trace(go.Bar(x = x_bar, y=y_bar),
                   row=2, col=2)
     fig.update_yaxes(title_text=modality, row=2, col=2)
 
     fig.update_layout(height=1200, width=1200, title_text=modality)
-    fig.show()
+    #fig.show()
     return fig
 
   def cohort_survey_count_bar(self, valid_votes = True):
     """
     Function to plot bar chart of ws_survey_count for all participants
     
     Arguments
@@ -329,15 +329,15 @@
     # Every 7th ticklable shows the month and day
     ticklabels[::7] = [item.strftime('%b %d') for item in df2.index[::7]]
     ax.xaxis.set_major_formatter(ticker.FixedFormatter(ticklabels))
     plt.gcf().autofmt_xdate()
 
     ax.legend(loc=(1.05, 0.5))
 
-    plt.show()
+    #plt.show()
     return fig, ax
   
 
   def cohort_survey_count_bar2(self, participant_list=None, valid_votes=True):
     """
     Function to plot bar chart of ws_survey_count for all participants
     
@@ -381,15 +381,15 @@
                 title=f'ws_survey_count counts daily, individual {valid_votes_title}',
                 width = 800,
                 height = 400)
     fig.update_layout(yaxis_title = "ws_survey_count [#]",
                       title_x=0.5,
                       xaxis_title = 'Date',
                       legend_title = 'Participants')
-    fig.show()
+    #fig.show()
     return fig
 
     
   def cohort_all_survey_count_bar(self, valid_votes=True):
     """
     Function to plot bar chart of the sum of ws_survey_count for all participants
     
@@ -422,15 +422,15 @@
     ax.set_ylabel('Counts') 
     ax.set_xlabel('Date')
 
     ax.xaxis.set_major_locator(mdates.WeekdayLocator())
     ax.xaxis.set_major_formatter(mdates.DateFormatter('%b %d'))
     ax.tick_params(axis='x', labelrotation=0) # Rotate xlabel
 
-    plt.show()
+    #plt.show()
     return fig, ax
   
    
   def cohort_all_survey_count_bar2(self, valid_votes=True):
     """
     Function to plot bar chart of the sum of ws_survey_count for all participants using Plotly
     
@@ -462,15 +462,15 @@
                 title=f'ws_survey_count counts daily, all participants {valid_votes_title}',
                 width = 800,
                 height = 400)
     fig.update_layout(yaxis_title = "ws_survey_count [#]",
                       title_x=0.5,
                       xaxis_title = 'Date',
                       legend_title = 'Participants')
-    fig.show()
+    #fig.show()
     return fig
 
   def cohort_individual_survey_count_bar(self, participant_list=None, valid_votes=True):
     """
     Function to plot bar chart of ws_survey_count for individual participants
     
     Arguments
@@ -544,15 +544,15 @@
                 title=f'ws_survey_count counts daily, all participants {valid_votes_title}',
                 width = 800,
                 height = 400)
     fig.update_layout(yaxis_title = "ws_survey_count [#]",
                       title_x=0.5,
                       xaxis_title = 'Date',
                       legend_title = 'Participants')
-    fig.show()
+    #fig.show()
     return fig
 
   def cohort_survey_count_line(self, valid_votes=True):
     """
     Function to plot bar chart of the sum of ws_survey_count for all participants using Matplotlib
     
     Arguments
@@ -638,15 +638,15 @@
       fig.add_trace(go.Scatter(x=df2.index, y=df2["ws_survey_count_count"], name=id_participant, mode='lines'))
 
     fig.update_layout(title = f'Cohort cummulative ws_survey_count, individual {valid_votes_title}',
                       yaxis_title = 'Cummulative ws_survey_count [#]',
                       title_x=0.5,
                       xaxis_title = 'Date',
                       legend_title = 'Participants')
-    fig.show()
+    #fig.show()
     return fig
 
   def cohort_all_survey_count_line(self, valid_votes=True):
     """
     Function to plot line chart of the cumsum of ws_survey_count for all participants using Matplotlib
     
     Arguments
@@ -679,15 +679,14 @@
           xlabel='Date', 
           ax=ax,
           figsize=(25, 7))
     )
     ax.legend(["All participants"])
     ax.set_xlim([df.index[0], df.index[-1]])
 
-    plt.show()
     return fig, ax
 
   def cohort_all_survey_count_line2(self, valid_votes=True):
     """
     Function to plot line chart of the cumsum of ws_survey_count for all participants using Plotly
     
     Arguments
@@ -715,15 +714,15 @@
     fig.add_trace(go.Scatter(x=df.index, y=df["ws_survey_count_count"], name="All Participants", mode='lines'))
     fig.update_layout(title = f'Cohort cummulative ws_survey_count, all participants {valid_votes_title}',
                       yaxis_title = 'Cummulative ws_survey_count [#]',
                       title_x=0.5,
                       xaxis_title = 'Date',
                       legend_title = 'Participants',
                       showlegend=True)
-    fig.show()
+    #fig.show()
     return fig
   
   def cohort_all_survey_count_line3(self, participant_list=None, valid_votes=True):
     """
     Function to plot line chart of the cumsum of ws_survey_count for entire cohort and individual participants using Plotly
     
     Arguments
@@ -766,15 +765,15 @@
                       showlegend=True)
     
     # Plot data for individual participants
     for id_participant in participant_list:
       df2 = df[df["id_participant"]==id_participant]
       fig.add_trace(go.Scatter(x=df2.index, y=df2["ws_survey_count_count"], name=id_participant, mode='lines'))
 
-    fig.show()
+    #fig.show()
     return fig
   
   def cohort_dt_swarm(self, participant_list=None, threshold=None, valid_votes=True):
     """
     Function to plot swarm chart of the time between two ws_survey_count timestmaps for 
     individual participants with Matplotlib/Seaborn
     
@@ -813,15 +812,15 @@
     ax.set_title(f"Duration between two micro-survey responses {valid_votes_title}")
 
     # Draw red line
     if threshold != None:
       (xmin, xmax) = ax.get_xlim()
       ax.hlines(threshold, xmin, xmax, colors="red")
       
-    plt.show()
+    #plt.show()
     return fig, ax
   
 
   def cohort_dt_swarm2(self, participant_list=None, threshold=None, valid_votes=True):
     """
     Function to plot swarm chart of the time between two ws_survey_count timestmaps for 
     individual participants with Plotly
@@ -853,15 +852,15 @@
     fig.update_layout(title = f'Cohort cummulative ws_survey_count, all participants {valid_votes_title}',
                       title_x=0.5,
                       yaxis_title = 'Duration between two micro-survey responses [min]',
                       xaxis_title = 'Participants',
                       showlegend=True,
                       yaxis_range=[0,1200])
     fig.add_hline(y=55, line_width=1, line_dash="solid", line_color="red")
-    fig.show()
+    #fig.show()
 
     return fig
 
   def cohort_dt_hist(self, threshold=None, valid_votes=True):
     """
     Function to plot histogram of the time between two ws_survey_count timestmaps 
     for individual participants with Matplotlib/Seaborn
@@ -901,15 +900,15 @@
     _=ax.set_xticks(ticks)
     _=ax.set_xticklabels(labels)
 
     # Draw red line
     if threshold != None:
       (ymin, ymax) = ax.get_ylim()
       ax.vlines(threshold, ymin, ymax, colors="red")
-    plt.show()
+    #plt.show()
     return fig, ax
   
   def cohort_dt_hist2(self, threshold=None, valid_votes=True):
     """
     Function to swarm chart chart of the time between two ws_survey_count timestmaps for individual participants with Matplotlib/Seaborn
     
     Arguments
@@ -950,15 +949,15 @@
                       width = 800,
                       height = 400)
     
     if threshold != None:
       threshold = threshold/60
       fig.add_vline(x=threshold, line_width=1, line_dash="solid", line_color="red")
 
-    fig.show()
+    #fig.show()
     return fig
   
   def cohort_threshold_undercut(self, threshold, valid_votes=True):
     """
     Function to plot bar chart of cummulative thresholed exeedances per participant
     
     Arguments
@@ -988,15 +987,15 @@
                           title=f'Instances where the duration between two watch survey responses that are less than {threshold} min {valid_votes_title}', 
                           ylabel='Counts [x]', 
                           xlabel='Participants', 
                           figsize=(25, 7))
     )
     ax.tick_params(axis='x', labelrotation=0)
 
-    plt.show()
+    #plt.show()
     return fig, ax
   
   def cohort_threshold_undercut2(self, threshold, valid_votes=True):
     """
     Function to plot bar chart of cummulative thresholed exeedances per participant
     
     Arguments
@@ -1025,16 +1024,15 @@
                 barmode='group',
                 title=f'Instances where the duration between two watch survey responses that are less than {threshold} min {valid_votes_title}',
                 width = 800,
                 height = 400)
     fig.update_layout(yaxis_title = "Counts [#]",
                       title_x=0.5,
                       xaxis_title = 'Participants')
-    fig.show()
-
+    #fig.show()
     return fig
   
   def cohort_treshold_report(self, threshold, valid_votes=True):
     """
     Function to print some stats about the threshold of duration between two cote_counts
     
     Arguments
@@ -1133,15 +1131,15 @@
 
     # Remove redundant tick labels
     axs[number_of_rows-1,0].set_xticks([])
     axs[number_of_rows-1,0].set_yticks([])
     axs[number_of_rows-1,1].set_xticks([])
     axs[number_of_rows-1,1].set_yticks([])
 
-    plt.show()
+    #plt.show()
 
     return fig, axs
 
 
   def cohort_ws_inspection2(self, ws_questions, valid_votes=True): 
     """
     Function to plot bar chart with the responses to the watch surveys for the entire cohort with Matplotlib
@@ -1239,10 +1237,9 @@
     trace2 = go.Bar(x=['A','B','C'], y=[3,8,5])
     fig.add_trace(trace2, number_of_rows, 1)
     fig.update_xaxes(title_text='Questions', row=number_of_rows, col=1)
     fig.update_yaxes(title_text='Counts [#]', row=number_of_rows, col=1)
 
     fig.update_layout(height=1400, width=1000, showlegend = False)
 
-    fig.show()
-
+    #fig.show()
     return fig
```

### Comparing `coziepy-0.0.2/pyproject.toml` & `coziepy-0.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coziepy"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Mario Frei", email="mario.frei@gmx.net" },
 ]
 description = "A package for processing and visualizing data collected with the Cozie-Apple app"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -17,24 +17,25 @@
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "arrow >= 1.2.3",
     "DateTime >= 5.2",
     "fastparquet >= 2023.7.0",
+    "folium >= 0.14.0",
     "influxdb >= 5.3.1",
-    "matplotlib >= 3.7.2",
+    "matplotlib >= 3.7.1",
     "matplotlib-inline >= 0.1.6",
-    "numpy >= 1.25.1",
+    "numpy >= 1.24.0",
     "packaging >= 23.1",
-    "pandas >= 2.0.3",
-    "plotly >= 5.15.0",
-    "pyarrow >= 12.0.1",
-    "pytz >= 2023.3",
-    "requests >= 2.31.0",
+    "pandas >= 2.0.0",
+    "plotly >= 5.13.0",
+    "pyarrow >= 9.0.0",
+    "pytz >= 2022.7.0",
+    "requests >= 2.27.0",
     "seaborn >= 0.12.2",
 ]
 
 [project.urls]
 homepage = "https://www.cozie-apple.app/"
 repository = "https://github.com/cozie-app/cozie-wizard/issues"
```

