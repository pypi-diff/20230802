# Comparing `tmp/evoaug-tf-0.1.0.tar.gz` & `tmp/evoaug-tf-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evoaug-tf-0.1.0.tar", last modified: Thu Jul 13 17:03:11 2023, max compression
+gzip compressed data, was "evoaug-tf-1.0.0.tar", last modified: Wed Aug  2 14:20:09 2023, max compression
```

## Comparing `evoaug-tf-0.1.0.tar` & `evoaug-tf-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yiyu      (1000) yiyu      (1000)        0 2023-07-13 17:03:11.760000 evoaug-tf-0.1.0/
--rw-r--r--   0 yiyu      (1000) yiyu      (1000)     1066 2023-07-13 17:01:27.000000 evoaug-tf-0.1.0/LICENSE
--rw-r--r--   0 yiyu      (1000) yiyu      (1000)      252 2023-07-13 17:03:11.760000 evoaug-tf-0.1.0/PKG-INFO
--rw-r--r--   0 yiyu      (1000) yiyu      (1000)      610 2023-07-13 15:45:21.000000 evoaug-tf-0.1.0/README.md
-drwxr-xr-x   0 yiyu      (1000) yiyu      (1000)        0 2023-07-13 17:03:11.760000 evoaug-tf-0.1.0/evoaug_tf/
--rw-r--r--   0 yiyu      (1000) yiyu      (1000)       43 2023-07-13 15:47:47.000000 evoaug-tf-0.1.0/evoaug_tf/__init__.py
--rw-r--r--   0 yiyu      (1000) yiyu      (1000)    13117 2023-06-14 00:59:38.000000 evoaug-tf-0.1.0/evoaug_tf/augment.py
--rw-r--r--   0 yiyu      (1000) yiyu      (1000)     6618 2023-07-13 15:53:16.000000 evoaug-tf-0.1.0/evoaug_tf/evoaug.py
-drwxr-xr-x   0 yiyu      (1000) yiyu      (1000)        0 2023-07-13 17:03:11.760000 evoaug-tf-0.1.0/evoaug_tf.egg-info/
--rw-r--r--   0 yiyu      (1000) yiyu      (1000)      252 2023-07-13 17:03:11.000000 evoaug-tf-0.1.0/evoaug_tf.egg-info/PKG-INFO
--rw-r--r--   0 yiyu      (1000) yiyu      (1000)      221 2023-07-13 17:03:11.000000 evoaug-tf-0.1.0/evoaug_tf.egg-info/SOURCES.txt
--rw-r--r--   0 yiyu      (1000) yiyu      (1000)        1 2023-07-13 17:03:11.000000 evoaug-tf-0.1.0/evoaug_tf.egg-info/dependency_links.txt
--rw-r--r--   0 yiyu      (1000) yiyu      (1000)       10 2023-07-13 17:03:11.000000 evoaug-tf-0.1.0/evoaug_tf.egg-info/top_level.txt
--rw-r--r--   0 yiyu      (1000) yiyu      (1000)       38 2023-07-13 17:03:11.760000 evoaug-tf-0.1.0/setup.cfg
--rw-r--r--   0 yiyu      (1000) yiyu      (1000)      282 2023-07-13 15:58:20.000000 evoaug-tf-0.1.0/setup.py
+drwxr-xr-x   0 yiyu      (1000) yiyu      (1000)        0 2023-08-02 14:20:09.847920 evoaug-tf-1.0.0/
+-rw-r--r--   0 yiyu      (1000) yiyu      (1000)     1066 2023-07-13 17:01:27.000000 evoaug-tf-1.0.0/LICENSE
+-rw-r--r--   0 yiyu      (1000) yiyu      (1000)      252 2023-08-02 14:20:09.847920 evoaug-tf-1.0.0/PKG-INFO
+-rw-r--r--   0 yiyu      (1000) yiyu      (1000)     3664 2023-08-02 14:17:43.000000 evoaug-tf-1.0.0/README.md
+drwxr-xr-x   0 yiyu      (1000) yiyu      (1000)        0 2023-08-02 14:20:09.847920 evoaug-tf-1.0.0/evoaug_tf/
+-rw-r--r--   0 yiyu      (1000) yiyu      (1000)       43 2023-07-13 15:47:47.000000 evoaug-tf-1.0.0/evoaug_tf/__init__.py
+-rw-r--r--   0 yiyu      (1000) yiyu      (1000)    13117 2023-06-14 00:59:38.000000 evoaug-tf-1.0.0/evoaug_tf/augment.py
+-rw-r--r--   0 yiyu      (1000) yiyu      (1000)     6568 2023-08-02 13:29:16.000000 evoaug-tf-1.0.0/evoaug_tf/evoaug.py
+drwxr-xr-x   0 yiyu      (1000) yiyu      (1000)        0 2023-08-02 14:20:09.847920 evoaug-tf-1.0.0/evoaug_tf.egg-info/
+-rw-r--r--   0 yiyu      (1000) yiyu      (1000)      252 2023-08-02 14:20:09.000000 evoaug-tf-1.0.0/evoaug_tf.egg-info/PKG-INFO
+-rw-r--r--   0 yiyu      (1000) yiyu      (1000)      221 2023-08-02 14:20:09.000000 evoaug-tf-1.0.0/evoaug_tf.egg-info/SOURCES.txt
+-rw-r--r--   0 yiyu      (1000) yiyu      (1000)        1 2023-08-02 14:20:09.000000 evoaug-tf-1.0.0/evoaug_tf.egg-info/dependency_links.txt
+-rw-r--r--   0 yiyu      (1000) yiyu      (1000)       10 2023-08-02 14:20:09.000000 evoaug-tf-1.0.0/evoaug_tf.egg-info/top_level.txt
+-rw-r--r--   0 yiyu      (1000) yiyu      (1000)       38 2023-08-02 14:20:09.847920 evoaug-tf-1.0.0/setup.cfg
+-rw-r--r--   0 yiyu      (1000) yiyu      (1000)      283 2023-08-02 13:30:11.000000 evoaug-tf-1.0.0/setup.py
```

### Comparing `evoaug-tf-0.1.0/LICENSE` & `evoaug-tf-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `evoaug-tf-0.1.0/evoaug_tf/augment.py` & `evoaug-tf-1.0.0/evoaug_tf/augment.py`

 * *Files identical despite different names*

### Comparing `evoaug-tf-0.1.0/evoaug_tf/evoaug.py` & `evoaug-tf-1.0.0/evoaug_tf/evoaug.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,20 +87,17 @@
         x, y = batch
         if self.inference_aug:
             x = self._apply_augment(x)
         else:
             if self.insert_max:
                 x = self._pad_end(x)
 
-        with tf.GradientTape() as tape:
-            y_pred = self(x, training=True)  
-            loss = self.compiled_loss(y, y_pred, regularization_losses=self.losses)
-
+        y_pred = self(x, training=True)  
+        loss = self.compiled_loss(y, y_pred, regularization_losses=self.losses)
         self.compiled_metrics.update_state(y, y_pred)
-
         return {m.name: m.result() for m in self.metrics}
 
     @tf.function
     def predict_step(self, batch):
         x = batch
         if self.inference_aug:
             x = self._apply_augment(x)
```

