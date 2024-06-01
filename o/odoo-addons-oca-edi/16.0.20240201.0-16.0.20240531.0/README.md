# Comparing `tmp/odoo_addons_oca_edi-16.0.20240201.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_edi-16.0.20240531.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1424 bytes, number of entries: 4
--rw-r--r--  2.0 unx     1347 b- defN 24-Feb-03 03:52 odoo_addons_oca_edi-16.0.20240201.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-03 03:52 odoo_addons_oca_edi-16.0.20240201.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Feb-03 03:52 odoo_addons_oca_edi-16.0.20240201.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      385 b- defN 24-Feb-03 03:52 odoo_addons_oca_edi-16.0.20240201.0.dist-info/RECORD
-4 files, 1825 bytes uncompressed, 666 bytes compressed:  63.5%
+Zip file size: 1441 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     1420 b- defN 24-Jun-01 04:14 odoo_addons_oca_edi-16.0.20240531.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-01 04:14 odoo_addons_oca_edi-16.0.20240531.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Jun-01 04:14 odoo_addons_oca_edi-16.0.20240531.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      385 b- defN 24-Jun-01 04:14 odoo_addons_oca_edi-16.0.20240531.0.dist-info/RECORD
+4 files, 1898 bytes uncompressed, 683 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_edi-16.0.20240201.0.dist-info/METADATA
+Filename: odoo_addons_oca_edi-16.0.20240531.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_edi-16.0.20240201.0.dist-info/WHEEL
+Filename: odoo_addons_oca_edi-16.0.20240531.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_edi-16.0.20240201.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_edi-16.0.20240531.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_edi-16.0.20240201.0.dist-info/RECORD
+Filename: odoo_addons_oca_edi-16.0.20240531.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_edi-16.0.20240201.0.dist-info/METADATA` & `odoo_addons_oca_edi-16.0.20240531.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-edi
-Version: 16.0.20240201.0
+Version: 16.0.20240531.0
 Summary: Meta package for oca-edi Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
 Requires-Dist: odoo-addon-account-einvoice-generate <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-account-invoice-edifact <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-account-invoice-facturx <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-account-invoice-facturx-py3o <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-base-business-document-import <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-base-business-document-import-phone <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-base-ebill-payment-contract <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-base-edi <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-base-edifact <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-base-facturx <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-base-ubl <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-base-wamas-ubl <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-despatch-advice-import <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-despatch-advice-import-ubl <16.1dev,>=16.0dev
```

