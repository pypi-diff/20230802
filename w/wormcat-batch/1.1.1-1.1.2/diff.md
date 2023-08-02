# Comparing `tmp/wormcat_batch-1.1.1.tar.gz` & `tmp/wormcat_batch-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wormcat_batch-1.1.1.tar", last modified: Tue Aug  1 20:00:28 2023, max compression
+gzip compressed data, was "wormcat_batch-1.1.2.tar", last modified: Wed Aug  2 17:17:10 2023, max compression
```

## Comparing `wormcat_batch-1.1.1.tar` & `wormcat_batch-1.1.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-08-01 20:00:28.128959 wormcat_batch-1.1.1/
--rw-r--r--   0 dan        (501) staff       (20)       95 2022-08-16 12:41:26.000000 wormcat_batch-1.1.1/MANIFEST.in
--rw-r--r--   0 dan        (501) staff       (20)      226 2023-08-01 20:00:28.128807 wormcat_batch-1.1.1/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)     2733 2023-08-01 19:34:44.000000 wormcat_batch-1.1.1/README.md
--rw-r--r--   0 dan        (501) staff       (20)       38 2023-08-01 20:00:28.129001 wormcat_batch-1.1.1/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)      692 2023-08-01 18:25:58.000000 wormcat_batch-1.1.1/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-08-01 20:00:28.127594 wormcat_batch-1.1.1/wormcat_batch/
--rw-r--r--   0 dan        (501) staff       (20)     3947 2023-08-01 17:11:31.000000 wormcat_batch-1.1.1/wormcat_batch/create_wormcat_xlsx.py
--rw-r--r--   0 dan        (501) staff       (20)     2522 2023-08-01 19:01:04.000000 wormcat_batch-1.1.1/wormcat_batch/execute_r.py
--rwxr-xr-x   0 dan        (501) staff       (20)       46 2022-08-16 12:41:26.000000 wormcat_batch-1.1.1/wormcat_batch/is_wormcat_installed.R
--rwxr-xr-x   0 dan        (501) staff       (20)     8507 2023-08-01 18:54:19.000000 wormcat_batch-1.1.1/wormcat_batch/run_wormcat_batch.py
--rwxr-xr-x   0 dan        (501) staff       (20)     1484 2023-07-31 16:25:55.000000 wormcat_batch-1.1.1/wormcat_batch/worm_cat.R
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-08-01 20:00:28.128575 wormcat_batch-1.1.1/wormcat_batch.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)      226 2023-08-01 20:00:28.000000 wormcat_batch-1.1.1/wormcat_batch.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      451 2023-08-01 20:00:28.000000 wormcat_batch-1.1.1/wormcat_batch.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-08-01 20:00:28.000000 wormcat_batch-1.1.1/wormcat_batch.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)       69 2023-08-01 20:00:28.000000 wormcat_batch-1.1.1/wormcat_batch.egg-info/entry_points.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-08-01 20:00:28.000000 wormcat_batch-1.1.1/wormcat_batch.egg-info/not-zip-safe
--rw-r--r--   0 dan        (501) staff       (20)       23 2023-08-01 20:00:28.000000 wormcat_batch-1.1.1/wormcat_batch.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)       14 2023-08-01 20:00:28.000000 wormcat_batch-1.1.1/wormcat_batch.egg-info/top_level.txt
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-08-02 17:17:10.100752 wormcat_batch-1.1.2/
+-rw-r--r--   0 dan        (501) staff       (20)      135 2023-08-02 13:35:39.000000 wormcat_batch-1.1.2/MANIFEST.in
+-rw-r--r--   0 dan        (501) staff       (20)      226 2023-08-02 17:17:10.100603 wormcat_batch-1.1.2/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)     2733 2023-08-01 19:34:44.000000 wormcat_batch-1.1.2/README.md
+-rw-r--r--   0 dan        (501) staff       (20)       38 2023-08-02 17:17:10.100790 wormcat_batch-1.1.2/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)      703 2023-08-02 17:16:21.000000 wormcat_batch-1.1.2/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-08-02 17:17:10.099310 wormcat_batch-1.1.2/wormcat_batch/
+-rw-r--r--   0 dan        (501) staff       (20)     3324 2023-08-02 16:46:39.000000 wormcat_batch-1.1.2/wormcat_batch/create_sunburst.py
+-rw-r--r--   0 dan        (501) staff       (20)     3947 2023-08-01 17:11:31.000000 wormcat_batch-1.1.2/wormcat_batch/create_wormcat_xlsx.py
+-rw-r--r--   0 dan        (501) staff       (20)     2522 2023-08-01 19:01:04.000000 wormcat_batch-1.1.2/wormcat_batch/execute_r.py
+-rwxr-xr-x   0 dan        (501) staff       (20)       46 2022-08-16 12:41:26.000000 wormcat_batch-1.1.2/wormcat_batch/is_wormcat_installed.R
+-rwxr-xr-x   0 dan        (501) staff       (20)     9162 2023-08-02 16:42:21.000000 wormcat_batch-1.1.2/wormcat_batch/run_wormcat_batch.py
+-rw-r--r--   0 dan        (501) staff       (20)   227410 2023-08-02 13:20:17.000000 wormcat_batch-1.1.2/wormcat_batch/sunburst.template
+-rwxr-xr-x   0 dan        (501) staff       (20)     1484 2023-07-31 16:25:55.000000 wormcat_batch-1.1.2/wormcat_batch/worm_cat.R
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-08-02 17:17:10.100309 wormcat_batch-1.1.2/wormcat_batch.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)      226 2023-08-02 17:17:10.000000 wormcat_batch-1.1.2/wormcat_batch.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      516 2023-08-02 17:17:10.000000 wormcat_batch-1.1.2/wormcat_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-08-02 17:17:10.000000 wormcat_batch-1.1.2/wormcat_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)       69 2023-08-02 17:17:10.000000 wormcat_batch-1.1.2/wormcat_batch.egg-info/entry_points.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-08-02 17:17:10.000000 wormcat_batch-1.1.2/wormcat_batch.egg-info/not-zip-safe
+-rw-r--r--   0 dan        (501) staff       (20)       32 2023-08-02 17:17:10.000000 wormcat_batch-1.1.2/wormcat_batch.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)       14 2023-08-02 17:17:10.000000 wormcat_batch-1.1.2/wormcat_batch.egg-info/top_level.txt
```

### Comparing `wormcat_batch-1.1.1/README.md` & `wormcat_batch-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `wormcat_batch-1.1.1/setup.py` & `wormcat_batch-1.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 # rm -rf dist
 # python setup.py sdist
 # pip install dist/wormcat_batch-1.0.1.tar.gz
 # twine check dist/*
 # twine upload --repository pypi dist/*
 
 setup(name='wormcat_batch',
-      version='1.1.1',
+      version='1.1.2',
       description='Batch processing for Wormcat data',
       url='https://github.com/dphiggs01/Wormcat_batch',
       author='Dan Higgins',
       author_email='daniel.higgins@yahoo.com',
       license='MIT',
 
       packages=['wormcat_batch'],
-      install_requires=['pandas','xlrd','xlsxwriter'],
+      install_requires=['pandas','xlrd','openpyxl','xlsxwriter'],
       entry_points={
           'console_scripts': ['wormcat_cli=wormcat_batch.run_wormcat_batch:main'],
       },
       include_package_data=True,
       zip_safe=False)
```

### Comparing `wormcat_batch-1.1.1/wormcat_batch/create_wormcat_xlsx.py` & `wormcat_batch-1.1.2/wormcat_batch/create_wormcat_xlsx.py`

 * *Files identical despite different names*

### Comparing `wormcat_batch-1.1.1/wormcat_batch/execute_r.py` & `wormcat_batch-1.1.2/wormcat_batch/execute_r.py`

 * *Files identical despite different names*

### Comparing `wormcat_batch-1.1.1/wormcat_batch/run_wormcat_batch.py` & `wormcat_batch-1.1.2/wormcat_batch/run_wormcat_batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,44 +4,47 @@
 import pandas as pd
 import shutil
 import zipfile
 import importlib.metadata
 from datetime import datetime
 from wormcat_batch.execute_r import ExecuteR
 from wormcat_batch.create_wormcat_xlsx import process_category_files
+from wormcat_batch.create_sunburst import create_sunburst
 
 import warnings
 warnings.filterwarnings('ignore', category=UserWarning, module='openpyxl')
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
-# Create CSV Files from the given Excelsheet
 def extract_csv_files(input_excel_nm, csv_file_path):
+    '''
+    Create CSV Files from the given Excel spreadsheet
+    '''
     input_excel = pd.ExcelFile(input_excel_nm)
     for sheet in input_excel.sheet_names:
         sheet_df = input_excel.parse(sheet)
         sheet_df.to_csv(f'{csv_file_path}{os.path.sep}{sheet}.csv', index=False)
 
         
-# Read CSV Files and call worm cat for each file
 def process_csv_files(csv_file_path, wormcat_out_path, annotation_file):
     '''
-    Read the Excel file and process each sheet individually through Wormcat
+    Read the csv data files and process each individually through Wormcat
     '''
     for dir_content in os.listdir(csv_file_path):
         conetnt_full_path = os.path.join(csv_file_path, dir_content)
         if os.path.isfile(conetnt_full_path):
             with open(conetnt_full_path, 'r') as file:
                 header_line = file.readline().strip()
             wormcat_input_type = header_line.replace(' ', '.')
             csv_file_nm = os.path.basename(conetnt_full_path)
             file_nm_wo_ext = csv_file_nm[:-4] # Remove .csv from file name
             title = file_nm_wo_ext.replace('_', ' ')
             wormcat_output_dir = f'{wormcat_out_path}{os.path.sep}{file_nm_wo_ext}'
             executeR = ExecuteR()
             executeR.worm_cat_fun(conetnt_full_path, wormcat_output_dir, title, annotation_file, wormcat_input_type)
+            create_sunburst(wormcat_output_dir)
     return wormcat_out_path
 
 def create_summary_spreadsheet(wormcat_out_path, annotation_file, out_xsl_file_nm):
     '''
     After all the sheets on the Excel have been executed or CSV files processed 
     create a dataframe that can be used to summarize the results.
     This dataframe is used to create the output Excel.
@@ -111,96 +114,117 @@
     '''
     with zipfile.ZipFile(zip_file_name, 'w') as zipf:
         for root, _, files in os.walk(directory_path):
             for file in files:
                 file_path = os.path.join(root, file)
                 zipf.write(file_path, os.path.relpath(file_path, directory_path))
 
+## main application functions 
 
-##########################################################
-
-def main():
-    print("Starting Wormcat Batch")
+def process_command_arguments():
+    '''
+    The process_command_arguments method validates and sets the input arguments 
+    to conform with downstream processing
+    '''
     parser = argparse.ArgumentParser()
     help_statement="wormcat_cli --input-excel <path_to_excel> | --input-csv-path <path_to_csv> --output-path <path_to_out_dir> --annotation-file 'whole_genome_v2_nov-11-2021.csv' --clean-temp False"
     parser.add_argument('-i', '--input-excel', help='Input file in Excel/Wormcat format')
     parser.add_argument('-c', '--input-csv-path', help='Input path to a collection of CSV files in Wormcat format')
     parser.add_argument('-o', '--output-path', help='Output path')
     parser.add_argument('-a', '--annotation-file', default='whole_genome_v2_nov-11-2021.csv', help='Annotation file name or path default=whole_genome_v2_nov-11-2021.csv')
-    parser.add_argument('-t', '--clean-temp', default='False', help='Remove files created while processing default=False')
+    parser.add_argument('-t', '--clean-temp', default='True', help='Remove files created while processing default=False')
 
     parser.add_argument('-v', '--version', action='version', version=f'%(prog)s v{importlib.metadata.version("wormcat_batch")}')
     args = parser.parse_args()
 
     if not args.input_excel and not args.input_csv_path:
         print(help_statement)
         print("An Excel Input file or a path to CSV files is required.")
-        return
+        sys.exit(-1)
 
     if not args.output_path:
         print(help_statement)
-        print("Output path is required.")
-        return
+        print("An Output path is required.")
+        sys.exit(-1)
 
-    if os.path.sep in args.annotation_file:
-        # Assume we are given a path to an external Annotation file
-        annotation_file_path = args.annotation_file
-    else:
+    # if args.annotation_file is not a path to an annotation file
+    # vaildate the input name and set the full path
+    if not (os.path.sep in args.annotation_file):
         wormcat_path = get_wormcat_lib()
         annotation_files = get_category_files(wormcat_path)
          
         if not args.annotation_file or not args.annotation_file in annotation_files:
             print(help_statement)
             print("Missing or incorrect annotation-file-nm.")
             print("Available names: {}".format(annotation_files))
-            return
-        annotation_file_path = f"{wormcat_path}{os.path.sep}extdata{os.path.sep}{args.annotation_file}"
+            sys.exit(-1)
+        args.annotation_file = f"{wormcat_path}{os.path.sep}extdata{os.path.sep}{args.annotation_file}"
     
+    # Support TRUE or True as input to clean temp
+    # otherwise set to False
     if args.clean_temp.lower().title() == 'True':
-        clean_temp = True
+        args.clean_temp = True
     else:
-        clean_temp = False
+        args.clean_temp = False
+
+    return args
 
-    # Create the output directory if it does not exsist
-    # Create a backup of the directory if it does exist and has content
+
+def main():
+    print("Starting Wormcat Batch")
+
+    # Validate the command line arguments
+    args = process_command_arguments()
+
+    # Create the output directory if it does not exsist.
+    # If it does exist and has content create a backup.
     create_directory(args.output_path, with_backup=True)
 
-    # If needed Extract the sreadsheet data
+    # If we are given an input_csv_path use it.
     if args.input_csv_path:
         csv_file_path = args.input_csv_path
     else:
-        # Create a directory to extrat the Spreadsheet data into CSV
+        # Else we MUST have been given an input_excel
+        # Create a directory and extract the Excel sheets as csv data
         csv_file_path = f"{args.output_path}{os.path.sep}csv_files"
         create_directory(csv_file_path)
         extract_csv_files(args.input_excel, csv_file_path)
 
     # Create a directory based on the Excel file name or CSV directory and a timestamp
     # Wormcat processing will write to this directory
     if args.input_excel:
         base_input_excel = os.path.basename(args.input_excel)
         input_data_nm = os.path.splitext(base_input_excel)[0]
     else:
         input_data_nm = os.path.basename(args.input_csv_path)
+
     timestamp = datetime.now().strftime("%Y%m%d-%H%M%S")
     output_base_dir =f"{input_data_nm}_{timestamp}"
     wormcat_out_path = f"{args.output_path}{os.path.sep}{output_base_dir}"
     create_directory(wormcat_out_path)
 
-    # Call wormcat on each CSV file
+    print(f"{args.input_excel=}")
+    print(f"{args.input_csv_path=}")
+    print(f"{args.output_path=}")
+    print(f"{args.annotation_file=}")
+    print(f"{args.clean_temp=}")
+
+    # Call Wormcat on each CSV file
     process_csv_files(csv_file_path, wormcat_out_path, args.annotation_file)
 
     # Create a summary spreadsheet of all CSV runs
     out_xsl_file_nm = f"{wormcat_out_path}{os.path.sep}Out_{input_data_nm}.xlsx"
-    create_summary_spreadsheet(wormcat_out_path, annotation_file_path, out_xsl_file_nm)
+    create_summary_spreadsheet(wormcat_out_path, args.annotation_file, out_xsl_file_nm)
     
     # Zip the results
     zip_dir_nm = f"{args.output_path}{os.path.sep}{output_base_dir}.zip"
     zip_directory(wormcat_out_path, zip_dir_nm)
     
     # If set Remove files created while processing
-    if clean_temp:
+    if args.clean_temp:
         shutil.rmtree(wormcat_out_path)
         if args.input_excel:
             shutil.rmtree(csv_file_path)
 
+
 if __name__ == '__main__':
     main()
```

### Comparing `wormcat_batch-1.1.1/wormcat_batch/worm_cat.R` & `wormcat_batch-1.1.2/wormcat_batch/worm_cat.R`

 * *Files identical despite different names*

