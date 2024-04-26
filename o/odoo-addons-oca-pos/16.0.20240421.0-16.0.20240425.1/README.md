# Comparing `tmp/odoo_addons_oca_pos-16.0.20240421.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_pos-16.0.20240425.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1734 bytes, number of entries: 4
--rw-r--r--  2.0 unx     3426 b- defN 24-Apr-22 04:52 odoo_addons_oca_pos-16.0.20240421.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 04:52 odoo_addons_oca_pos-16.0.20240421.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-22 04:52 odoo_addons_oca_pos-16.0.20240421.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      385 b- defN 24-Apr-22 04:52 odoo_addons_oca_pos-16.0.20240421.0.dist-info/RECORD
-4 files, 3904 bytes uncompressed, 976 bytes compressed:  75.0%
+Zip file size: 1754 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     3576 b- defN 24-Apr-26 05:10 odoo_addons_oca_pos-16.0.20240425.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-26 05:10 odoo_addons_oca_pos-16.0.20240425.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-26 05:10 odoo_addons_oca_pos-16.0.20240425.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      385 b- defN 24-Apr-26 05:10 odoo_addons_oca_pos-16.0.20240425.1.dist-info/RECORD
+4 files, 4054 bytes uncompressed, 996 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_pos-16.0.20240421.0.dist-info/METADATA
+Filename: odoo_addons_oca_pos-16.0.20240425.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_pos-16.0.20240421.0.dist-info/WHEEL
+Filename: odoo_addons_oca_pos-16.0.20240425.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_pos-16.0.20240421.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_pos-16.0.20240425.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_pos-16.0.20240421.0.dist-info/RECORD
+Filename: odoo_addons_oca_pos-16.0.20240425.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_pos-16.0.20240421.0.dist-info/METADATA` & `odoo_addons_oca_pos-16.0.20240425.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-pos
-Version: 16.0.20240421.0
+Version: 16.0.20240425.1
 Summary: Meta package for oca-pos Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
 Requires-Dist: odoo-addon-pos-access-right <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-customer-comment <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-pos-daily-sales-reports-category-only <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-default-partner <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-discount-all <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-edit-order-line <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-escpos-status <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-financial-risk <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-global-discount-in-line <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-lot-barcode <16.1dev,>=16.0dev
@@ -41,14 +42,15 @@
 Requires-Dist: odoo-addon-pos-payment-terminal <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-display-default-code <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-label <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-multi-barcode <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-packaging-container-deposit <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-packaging-multi-barcode <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-quick-info <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-pos-receipt-hide-info <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-receipt-hide-price <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-receipt-replace-user-by-trigram <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-receipt-replace-user-by-trigram-hr <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-reset-search <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-sale-order-print <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-sale-product-config-no-variant <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-stock-available-online <16.1dev,>=16.0dev
```

