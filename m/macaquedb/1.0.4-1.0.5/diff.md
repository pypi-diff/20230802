# Comparing `tmp/macaquedb-1.0.4.tar.gz` & `tmp/macaquedb-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macaquedb-1.0.4.tar", last modified: Mon Jul 31 18:36:26 2023, max compression
+gzip compressed data, was "macaquedb-1.0.5.tar", last modified: Wed Aug  2 14:56:31 2023, max compression
```

## Comparing `macaquedb-1.0.4.tar` & `macaquedb-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-31 18:36:26.409445 macaquedb-1.0.4/
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      223 2023-07-31 18:36:26.409282 macaquedb-1.0.4/PKG-INFO
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)     2335 2023-07-28 16:05:19.000000 macaquedb-1.0.4/README.md
-drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-31 18:36:26.407013 macaquedb-1.0.4/macaquedb/
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)    17546 2023-07-31 18:36:06.000000 macaquedb-1.0.4/macaquedb/Database.py
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       31 2023-07-21 17:03:41.000000 macaquedb-1.0.4/macaquedb/__init__.py
-drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-31 18:36:26.408925 macaquedb-1.0.4/macaquedb/database/
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      489 2023-07-21 14:36:48.000000 macaquedb-1.0.4/macaquedb/database/Image.py
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      306 2023-07-21 14:36:48.000000 macaquedb-1.0.4/macaquedb/database/Session.py
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      294 2023-07-31 15:08:30.000000 macaquedb-1.0.4/macaquedb/database/Subject.py
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-21 16:58:35.000000 macaquedb-1.0.4/macaquedb/database/__init__.py
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      451 2023-07-21 14:36:48.000000 macaquedb-1.0.4/macaquedb/database/utilities.py
-drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-31 18:36:26.407885 macaquedb-1.0.4/macaquedb.egg-info/
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      223 2023-07-31 18:36:26.000000 macaquedb-1.0.4/macaquedb.egg-info/PKG-INFO
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      377 2023-07-31 18:36:26.000000 macaquedb-1.0.4/macaquedb.egg-info/SOURCES.txt
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)        1 2023-07-31 18:36:26.000000 macaquedb-1.0.4/macaquedb.egg-info/dependency_links.txt
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       14 2023-07-31 18:36:26.000000 macaquedb-1.0.4/macaquedb.egg-info/requires.txt
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       10 2023-07-31 18:36:26.000000 macaquedb-1.0.4/macaquedb.egg-info/top_level.txt
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       38 2023-07-31 18:36:26.409502 macaquedb-1.0.4/setup.cfg
--rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      372 2023-07-31 18:36:14.000000 macaquedb-1.0.4/setup.py
+drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-08-02 14:56:31.435339 macaquedb-1.0.5/
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      223 2023-08-02 14:56:31.435121 macaquedb-1.0.5/PKG-INFO
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)     2882 2023-08-02 14:52:26.000000 macaquedb-1.0.5/README.md
+drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-08-02 14:56:31.432872 macaquedb-1.0.5/macaquedb/
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)    18297 2023-08-02 14:55:51.000000 macaquedb-1.0.5/macaquedb/Database.py
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       31 2023-07-21 17:03:41.000000 macaquedb-1.0.5/macaquedb/__init__.py
+drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-08-02 14:56:31.434772 macaquedb-1.0.5/macaquedb/database/
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      489 2023-07-21 14:36:48.000000 macaquedb-1.0.5/macaquedb/database/Image.py
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      306 2023-07-21 14:36:48.000000 macaquedb-1.0.5/macaquedb/database/Session.py
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      294 2023-07-31 15:08:30.000000 macaquedb-1.0.5/macaquedb/database/Subject.py
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)        0 2023-07-21 16:58:35.000000 macaquedb-1.0.5/macaquedb/database/__init__.py
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      451 2023-07-21 14:36:48.000000 macaquedb-1.0.5/macaquedb/database/utilities.py
+drwxr-xr-x   0 Sam.Alldritt   (504) staff       (20)        0 2023-08-02 14:56:31.433716 macaquedb-1.0.5/macaquedb.egg-info/
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      223 2023-08-02 14:56:31.000000 macaquedb-1.0.5/macaquedb.egg-info/PKG-INFO
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      377 2023-08-02 14:56:31.000000 macaquedb-1.0.5/macaquedb.egg-info/SOURCES.txt
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)        1 2023-08-02 14:56:31.000000 macaquedb-1.0.5/macaquedb.egg-info/dependency_links.txt
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       14 2023-08-02 14:56:31.000000 macaquedb-1.0.5/macaquedb.egg-info/requires.txt
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       10 2023-08-02 14:56:31.000000 macaquedb-1.0.5/macaquedb.egg-info/top_level.txt
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)       38 2023-08-02 14:56:31.435407 macaquedb-1.0.5/setup.cfg
+-rw-r--r--   0 Sam.Alldritt   (504) staff       (20)      372 2023-08-02 14:56:27.000000 macaquedb-1.0.5/setup.py
```

### Comparing `macaquedb-1.0.4/README.md` & `macaquedb-1.0.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -21,40 +21,52 @@
 ```
 This will build the tables and the .db file. This file stores the data. If we move the .db file, you need to point the interface to the new location with:
 ```
 interface.changePath('/new/path/to/database')
 ```
 ## Tables and adding data
 In the current version, we have 4 tables that are connected:
-### Subject:
+### Subjects:
 | Column Name | Data Type         |
 |-------------|------------------|
 | subject_id  | TEXT (Primary Key)|
 | site        | TEXT             |
 | sessions    | INTEGER          |
 | gender      | TEXT             |
-### Session:
+### Sessions:
 | Column Name | Data Type         | References         |
 |-------------|------------------|--------------------|
 | session_id  | TEXT (Primary Key)|                    |
 | subject_id  | TEXT             | Subject(subject_id)|
 | age         | DOUBLE           |                    |
 | site        | TEXT             |                    |
 | image_count | INT              |                    |
-### Image:
+### Images:
 | Column Name   | Data Type         | References         |
 |---------------|------------------|--------------------|
 | image_id      | TEXT (Primary Key)|                    |
 | session_id    | TEXT             | Session(session_id)|
 | subject_id    | TEXT             | Subject(subject_id)|
 | image_type    | TEXT             |                    |
 | image_subtype | TEXT             |                    |
 | image_path    | TEXT             |                    |
 | mask_path     | TEXT             |                    |
 | run_number    | INTEGER          |                    |
 | site          | TEXT             |                    |
-### JSON
+### JSONS
 | Column Name | Data Type        | References      |
 |-------------|------------------|-----------------|
 | json_id     | INTEGER (Primary Key)|               |
 | image_id    | INTEGER          | Image(image_id) |
 | json_path   | TEXT             |                 |
+
+To add data:
+```
+interface.input_site('/path/to/site-site')
+interface.input_demographics(csv_path='/path/to/csv.csv', subject_column='SubColName', session_column='SesColName', age_column='AgeColName', sex_column='SexColName')
+```
+You can also pick and choose any column you want to extract and return a pandas dataframe or just export straight to a CSV
+Extracting data:
+```
+colNamesToExtract = ("subject_id", "session_id", "age", "sex", "image_path", "run_number")
+dataframe = interface.make_csv(colNamesToExtract, '/path/to/output.csv')
+```
```

### Comparing `macaquedb-1.0.4/macaquedb/Database.py` & `macaquedb-1.0.5/macaquedb/Database.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,27 +71,36 @@
                                       subject_id=subject_id,
                                       site=site_name,
                                       image_count=image_count)
                 self.insert_session(new_session, force)
 
                 session_count += 1
 
+            elif session.startswith('anat') or session.startswith('func'):
+                unique_id = subject_id + '_001'
+                image_count = self.loop_images(
+                    session_dir=subject_dir, subject_id=subject_id, session_id=unique_id, site=site_name, force=force)
+                new_session = Session(session_id=unique_id,
+                                      subject_id=subject_id,
+                                      site=site_name,
+                                      image_count=image_count)
+                self.insert_session(new_session, force)
+
         return session_count
 
     '''
     Loop over NIFTI files in a directory and add them all to the database
     '''
 
     def loop_images(self, session_dir, subject_id, session_id, site, force=False):
         # Walk through every file in session (anat, dwi, fieldmap, func)
         image_count = 1
         for root, dirs, files in os.walk(session_dir):
             for file in files:
                 file_path = os.path.join(root, file)
-                abs_file_path = os.path.abspath(file)
                 # Get file type and subtype
                 image_type = os.path.basename(root)
 
                 if image_type == "anat":
                     if re.search(r"T1w", file):
                         image_subtype = "T1w"
                     elif re.search(r"T2w", file):
@@ -106,22 +115,30 @@
                 elif image_type == "dwi":
                     if re.search(r"AP", file) or re.search(r"ap", file):
                         image_subtype = "AP"
                     elif re.search(r"PA", file) or re.search(r"pa", file):
                         image_subtype = "PA"
                     else:
                         image_subtype = "unknown"
+
+                # Find the run
+                match = re.search(r"run[-_](\d+)?", file)
+                if match:
+                    run_number = match.group(1)
+                else:
+                    run_number = None
+
                 if is_nifti_file(file_path):
                     new_image = Image(image_id=file,
                                       session_id=session_id,
                                       subject_id=subject_id,
                                       image_type=os.path.basename(root),
                                       image_subtype=image_subtype,
-                                      image_path=abs_file_path,
-                                      run_number=image_count,
+                                      image_path=file_path,
+                                      run_number=run_number,
                                       site=site)
                     self.insert_image(new_image, force)
                     image_count += 1
 
         return image_count
 
     '''
```

