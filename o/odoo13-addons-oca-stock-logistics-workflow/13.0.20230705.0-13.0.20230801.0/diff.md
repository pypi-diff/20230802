# Comparing `tmp/odoo13_addons_oca_stock_logistics_workflow-13.0.20230705.0-py3-none-any.whl.zip` & `tmp/odoo13_addons_oca_stock_logistics_workflow-13.0.20230801.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2201 bytes, number of entries: 4
--rw-r--r--  2.0 unx     4317 b- defN 23-Jul-06 05:29 odoo13_addons_oca_stock_logistics_workflow-13.0.20230705.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 05:29 odoo13_addons_oca_stock_logistics_workflow-13.0.20230705.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-06 05:29 odoo13_addons_oca_stock_logistics_workflow-13.0.20230705.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      477 b- defN 23-Jul-06 05:29 odoo13_addons_oca_stock_logistics_workflow-13.0.20230705.0.dist-info/RECORD
-4 files, 4887 bytes uncompressed, 1259 bytes compressed:  74.2%
+Zip file size: 2217 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     4508 b- defN 23-Aug-02 05:37 odoo13_addons_oca_stock_logistics_workflow-13.0.20230801.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 05:37 odoo13_addons_oca_stock_logistics_workflow-13.0.20230801.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Aug-02 05:37 odoo13_addons_oca_stock_logistics_workflow-13.0.20230801.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      477 b- defN 23-Aug-02 05:37 odoo13_addons_oca_stock_logistics_workflow-13.0.20230801.0.dist-info/RECORD
+4 files, 5078 bytes uncompressed, 1275 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo13_addons_oca_stock_logistics_workflow-13.0.20230705.0.dist-info/METADATA
+Filename: odoo13_addons_oca_stock_logistics_workflow-13.0.20230801.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo13_addons_oca_stock_logistics_workflow-13.0.20230705.0.dist-info/WHEEL
+Filename: odoo13_addons_oca_stock_logistics_workflow-13.0.20230801.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo13_addons_oca_stock_logistics_workflow-13.0.20230705.0.dist-info/top_level.txt
+Filename: odoo13_addons_oca_stock_logistics_workflow-13.0.20230801.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo13_addons_oca_stock_logistics_workflow-13.0.20230705.0.dist-info/RECORD
+Filename: odoo13_addons_oca_stock_logistics_workflow-13.0.20230801.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo13_addons_oca_stock_logistics_workflow-13.0.20230705.0.dist-info/METADATA` & `odoo13_addons_oca_stock_logistics_workflow-13.0.20230801.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo13-addons-oca-stock-logistics-workflow
-Version: 13.0.20230705.0
+Version: 13.0.20230801.0
 Summary: Meta package for oca-stock-logistics-workflow Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 13.0
@@ -48,14 +48,17 @@
 Requires-Dist: odoo13-addon-stock-picking-group-by-partner-by-carrier-by-date
 Requires-Dist: odoo13-addon-stock-picking-import-serial-number
 Requires-Dist: odoo13-addon-stock-picking-invoice-link
 Requires-Dist: odoo13-addon-stock-picking-late-activity
 Requires-Dist: odoo13-addon-stock-picking-line-sequence
 Requires-Dist: odoo13-addon-stock-picking-mass-action
 Requires-Dist: odoo13-addon-stock-picking-operation-quick-change
+Requires-Dist: odoo13-addon-stock-picking-origin-reference
+Requires-Dist: odoo13-addon-stock-picking-origin-reference-purchase
+Requires-Dist: odoo13-addon-stock-picking-origin-reference-sale
 Requires-Dist: odoo13-addon-stock-picking-package-preparation
 Requires-Dist: odoo13-addon-stock-picking-product-assortment
 Requires-Dist: odoo13-addon-stock-picking-product-assortment-availability-inline
 Requires-Dist: odoo13-addon-stock-picking-product-availability-inline
 Requires-Dist: odoo13-addon-stock-picking-purchase-order-link
 Requires-Dist: odoo13-addon-stock-picking-restrict-cancel-with-orig-move
 Requires-Dist: odoo13-addon-stock-picking-return-restricted-qty
```

