# Comparing `tmp/wwpdb_utils_emdb-1.8.2.tar.gz` & `tmp/wwpdb_utils_emdb-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb_utils_emdb-1.8.2.tar", last modified: Thu Apr 25 19:45:39 2024, max compression
+gzip compressed data, was "wwpdb_utils_emdb-1.9.tar", last modified: Fri May 31 22:36:43 2024, max compression
```

## Comparing `wwpdb_utils_emdb-1.8.2.tar` & `wwpdb_utils_emdb-1.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 19:45:39.864299 wwpdb_utils_emdb-1.8.2/
--rw-r--r--   0 vsts      (1001) docker     (127)      106 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)      960 2024-04-25 19:45:39.864299 wwpdb_utils_emdb-1.8.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-25 19:45:39.868299 wwpdb_utils_emdb-1.8.2/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2310 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 19:45:39.860299 wwpdb_utils_emdb-1.8.2/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 19:45:39.860299 wwpdb_utils_emdb-1.8.2/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 19:45:39.860299 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/
--rw-r--r--   0 vsts      (1001) docker     (127)      322 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/EmdbSchema.py
--rw-r--r--   0 vsts      (1001) docker     (127)      145 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 19:45:39.860299 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/atomcheck/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/atomcheck/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7031 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/atomcheck/atomcheck.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 19:45:39.860299 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/checkemupload/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/checkemupload/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19243 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/checkemupload/checkemupload.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 19:45:39.864299 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/cif_emdb_translator/
--rwxr-xr-x   0 vsts      (1001) docker     (127)      139 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/cif_emdb_translator/README.md
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/cif_emdb_translator/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)   676892 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
--rw-r--r--   0 vsts      (1001) docker     (127)  2304974 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/cif_emdb_translator/emdb.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1196 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2490 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 19:45:39.864299 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/data/
--rw-r--r--   0 vsts      (1001) docker     (127)   221515 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/data/emdb-v3.xsd
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 19:45:39.864299 wwpdb_utils_emdb-1.8.2/wwpdb.utils.emdb.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)      960 2024-04-25 19:45:39.000000 wwpdb_utils_emdb-1.8.2/wwpdb.utils.emdb.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      947 2024-04-25 19:45:39.000000 wwpdb_utils_emdb-1.8.2/wwpdb.utils.emdb.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-25 19:45:39.000000 wwpdb_utils_emdb-1.8.2/wwpdb.utils.emdb.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       87 2024-04-25 19:45:39.000000 wwpdb_utils_emdb-1.8.2/wwpdb.utils.emdb.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-25 19:45:26.000000 wwpdb_utils_emdb-1.8.2/wwpdb.utils.emdb.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      101 2024-04-25 19:45:39.000000 wwpdb_utils_emdb-1.8.2/wwpdb.utils.emdb.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-25 19:45:39.000000 wwpdb_utils_emdb-1.8.2/wwpdb.utils.emdb.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 22:36:43.244602 wwpdb_utils_emdb-1.9/
+-rw-r--r--   0 vsts      (1001) docker     (127)      106 2024-05-31 22:35:33.000000 wwpdb_utils_emdb-1.9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)      958 2024-05-31 22:36:43.244602 wwpdb_utils_emdb-1.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-05-31 22:35:33.000000 wwpdb_utils_emdb-1.9/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-05-31 22:36:43.244602 wwpdb_utils_emdb-1.9/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2310 2024-05-31 22:35:33.000000 wwpdb_utils_emdb-1.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 22:36:43.236601 wwpdb_utils_emdb-1.9/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-31 22:35:33.000000 wwpdb_utils_emdb-1.9/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 22:36:43.236601 wwpdb_utils_emdb-1.9/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-31 22:35:33.000000 wwpdb_utils_emdb-1.9/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 22:36:43.236601 wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)      322 2024-05-31 22:35:33.000000 wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/EmdbSchema.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      143 2024-05-31 22:35:33.000000 wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 22:36:43.240602 wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/atomcheck/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-31 22:35:33.000000 wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/atomcheck/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7031 2024-05-31 22:35:33.000000 wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/atomcheck/atomcheck.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 22:36:43.240602 wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/checkemupload/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-31 22:35:33.000000 wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/checkemupload/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26321 2024-05-31 22:35:33.000000 wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/checkemupload/checkemupload.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 22:36:43.244602 wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/cif_emdb_translator/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      139 2024-05-31 22:35:33.000000 wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/cif_emdb_translator/README.md
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 22:35:33.000000 wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/cif_emdb_translator/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)   677969 2024-05-31 22:35:33.000000 wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)  2304974 2024-05-31 22:35:33.000000 wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/cif_emdb_translator/emdb.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1196 2024-05-31 22:35:33.000000 wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2490 2024-05-31 22:35:33.000000 wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 22:36:43.244602 wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/data/
+-rw-r--r--   0 vsts      (1001) docker     (127)   221515 2024-05-31 22:35:33.000000 wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/data/emdb-v3.xsd
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-31 22:36:43.244602 wwpdb_utils_emdb-1.9/wwpdb.utils.emdb.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)      958 2024-05-31 22:36:43.000000 wwpdb_utils_emdb-1.9/wwpdb.utils.emdb.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      947 2024-05-31 22:36:43.000000 wwpdb_utils_emdb-1.9/wwpdb.utils.emdb.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-31 22:36:43.000000 wwpdb_utils_emdb-1.9/wwpdb.utils.emdb.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       87 2024-05-31 22:36:43.000000 wwpdb_utils_emdb-1.9/wwpdb.utils.emdb.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-31 22:36:23.000000 wwpdb_utils_emdb-1.9/wwpdb.utils.emdb.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      101 2024-05-31 22:36:43.000000 wwpdb_utils_emdb-1.9/wwpdb.utils.emdb.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-31 22:36:43.000000 wwpdb_utils_emdb-1.9/wwpdb.utils.emdb.egg-info/top_level.txt
```

### Comparing `wwpdb_utils_emdb-1.8.2/PKG-INFO` & `wwpdb_utils_emdb-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.emdb
-Version: 1.8.2
+Version: 1.9
 Summary: wwPDB EMDB to XML converter
 Home-page: https://github.com/rcsb/py-wwpdb_utils_config
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb_utils_emdb-1.8.2/setup.py` & `wwpdb_utils_emdb-1.9/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/atomcheck/atomcheck.py` & `wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/atomcheck/atomcheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py` & `wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1474,15 +1474,15 @@
             """
             Helper function that returns the schema construct for the given cif category
 
             Parameters:
             @param cif_item: full name of the cif category, e.g. _em_admin.title
             """
             xsd = ""
-            if cif_item in const.MMCIF_TO_XSD:
+            if cif_item in const.MMCIF_TO_XSD:  # pylint: disable=possibly-used-before-assignment
                 xsd = const.MMCIF_TO_XSD[cif_item]
             else:
                 txt = u"CIF item (%s) not found in the MMCIF_TO_XSD dictionary." % cif_item
                 self.current_entry_log.error_logs.append(self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.error_title + txt))
                 self.log_formatted(self.error_log_string, "(" + self.entry_in_translation_log.id + ")" + const.REQUIRED_ALERT + txt)
             return xsd
 
@@ -1727,15 +1727,15 @@
                     if res_type is not None:
                         if units is not None:
                             constructed_cif_value = constructor(valueOf_=fmt_cif_value, units=units, res_type=res_type)
                         else:
                             constructed_cif_value = constructor(valueOf_=fmt_cif_value, res_type=res_type)
                 else:
                     constructed_cif_value = fmt_cif_value
-                setter_func(constructed_cif_value)
+                setter_func(constructed_cif_value)  # pylint: disable=possibly-used-before-assignment
                 log(cif_item, setter_func, fmt_cif_value, soft_name=soft_name)
             else:
                 log(cif_item, setter_func, parent_el_req=parent_el_req, soft_name=soft_name)
 
         def make_list_of_dicts(cif_category, key_item, cif_list=None, min_length=3):
             """
             Create a dictionary from a cif category where
@@ -3084,15 +3084,15 @@
                                     correct_acc_code = "EMD-" + acc_code
                                     corrected = True
                                 if acc_code.find("EMDB") != -1:
                                     # acc_code is in a EMDB-xxxx format - remove B
                                     correct_acc_code = acc_code.replace("B", "")
                                     corrected = True
                                 if corrected:
-                                    set_cif_value(emdb_ref.set_emdb_id, "access_code", const.EM_DB_REFERENCE, cif_list=emdb_ref_in, cif_value=correct_acc_code)
+                                    set_cif_value(emdb_ref.set_emdb_id, "access_code", const.EM_DB_REFERENCE, cif_list=emdb_ref_in, cif_value=correct_acc_code)  # pylint: disable=possibly-used-before-assignment
                                     txt = u"emdb_id is set to (%s) as (_em_db_reference.access_code) is (%s)." % (correct_acc_code, acc_code)
                                     self.current_entry_log.warn_logs.append(
                                         self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.warn_title + txt)
                                     )
                                     self.log_formatted(self.warn_log_string, const.CHANGE_MADE + txt)
                         else:
                             txt = u"Cannot set crossreference emdb_id as the required value for (_em_db_reference.access_code) is not given."
@@ -3152,15 +3152,15 @@
                                     # db_id is given as e.g. D_1000232117; should be EMD-xxxx
                                     txt = u"emdb_id cannot be set as the value for (_pdbx_database_related.db_id) is given as (%s)." % db_id
                                     self.current_entry_log.error_logs.append(
                                         self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.error_title + txt)
                                     )
                                     self.log_formatted(self.error_log_string, const.REQUIRED_ALERT + txt)
                                 if corrected:
-                                    set_cif_value(cross_ref.set_emdb_id, "db_id", const.PDBX_DATABASE_RELATED, cif_list=rel_in, cif_value=correct_db_id)
+                                    set_cif_value(cross_ref.set_emdb_id, "db_id", const.PDBX_DATABASE_RELATED, cif_list=rel_in, cif_value=correct_db_id)  # pylint: disable=possibly-used-before-assignment
                                     txt = u"emdb_id is set to (%s) as the value for (_pdbx_database_related.db_id) is given as (%s)." % (correct_db_id, db_id)
                                     self.current_entry_log.warn_logs.append(
                                         self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.change_title + txt)
                                     )
                                     self.log_formatted(self.warn_log_string, const.CHANGE_MADE + txt)
                         else:
                             set_cif_value(cross_ref.set_emdb_id, "db_id", const.PDBX_DATABASE_RELATED, cif_list=rel_in)
@@ -5553,15 +5553,15 @@
                     p_mol.original_tagname_ = "protein_or_peptide"
                     # base
                     set_base_mol_with_dict(p_mol, ent_in, ent_id_in, src_dicts)
                     # element 1
                     rec_exp_dict_in = get_rec_exp_dict(ent_id_in, src_dicts, ent_poly_in, is_supramolecule=False)
                     set_el_recombinant_expression(p_mol, ent_id_in, rec_exp_dict_in)
                     # element 2
-                    set_el_enantiomer(p_mol, ent_type_in)
+                    set_el_enantiomer(p_mol, ent_type_in)  # pylint: disable=possibly-used-before-assignment
                     # element 3
                     set_el_sequence(p_mol, ent_poly_in, ent_id_in, ent_ref_dict)
                     # element 4
                     set_el_ec_number(p_mol, ent_in)
 
                 def set_saccharide_mol_type(poly_mol, ent_in, ent_id_in, src_dicts):
                     """
@@ -6044,15 +6044,15 @@
                         """
                         XSD: <xs:element name="details" type="xs:string" minOccurs="0" >
                         CIF: _em_shadowing.details 'rotary shadowing'
                         """
                         set_cif_value(shadow.set_details, "details", const.EM_SHADOWING, cif_list=shadow_in)
 
                     # element 1
-                    set_el_material(shadow, shadow_in)
+                    set_el_material(shadow, shadow_in)  # pylint: disable=possibly-used-before-assignment
                     # element 2
                     set_el_angle(shadow, shadow_in)
                     # element 3
                     set_el_thickness(shadow, shadow_in)
                     # element 4
                     set_el_details(shadow, shadow_in)
 
@@ -6238,15 +6238,15 @@
                                     cif_list=pretreat_in,
                                     constructor=emdb.pressureType,
                                     fmt=lambda x: float(x) * 0.001,
                                     units=const.U_KPA,
                                 )
 
                             # element 1
-                            set_el_type(pretreat, pretreat_in)
+                            set_el_type(pretreat, pretreat_in)  # pylint: disable=possibly-used-before-assignment
                             # element 2
                             set_el_time(pretreat, pretreat_in)
                             # element 3
                             set_el_atmosphere(pretreat, pretreat_in)
                             # element 4
                             set_el_pressure(pretreat, pretreat_in)
 
@@ -6264,15 +6264,15 @@
                     def set_el_details(grid, grid_in):
                         """
                         XSD: <xs:element name="details" type="xs:string" minOccurs="0">
                         CIF: _em_sample_support.details ?
                         """
                         set_cif_value(grid.set_details, "details", const.EM_SAMPLE_SUPPORT, cif_list=grid_in)
 
-                    grid_id_in = get_cif_value(const.K_ID, const.EM_SAMPLE_SUPPORT, grid_in)
+                    grid_id_in = get_cif_value(const.K_ID, const.EM_SAMPLE_SUPPORT, grid_in)  # pylint: disable=possibly-used-before-assignment
                     # element 1
                     set_el_model(grid, grid_in)
                     # element 2
                     set_el_material(grid, grid_in)
                     # element 3
                     set_el_mesh(grid, grid_in)
                     # element 4
@@ -6518,15 +6518,15 @@
                     # element 1
                     set_el_fiducial_type()
                     # element 2
                     set_el_manufacturer(fid, fid_in)
                     # element 3
                     set_el_diameter(fid, fid_in)
 
-                fs_present = get_cif_value("fiducial_markers", const.EM_TOMOGRAPHY_SPECIMEN, tom_prep_in)
+                fs_present = get_cif_value("fiducial_markers", const.EM_TOMOGRAPHY_SPECIMEN, tom_prep_in)  # pylint: disable=possibly-used-before-assignment
                 if tom_id_in in fid_dict_in and fs_present == "YES":
                     fid_list = emdb.fiducial_markers_listType()
                     fid_list_in = fid_dict_in[tom_id_in]
                     for fid_in in fid_list_in:
                         fid = emdb.fiducial_marker_type()
                         set_fiducial_marker_type(fid, fid_in)
                         if fid.has__content():
@@ -6656,15 +6656,15 @@
                         """
                         XSD: <xs:element name="details" type="xs:string" minOccurs="0"/>
                         CIF: _em_ultramicrotomy.details ?
                         """
                         set_cif_value(u_tome.set_details, "details", const.EM_ULTRAMICROTOMY, cif_list=u_tome_in)
 
                     # element 1
-                    set_el_instrument(u_tome, u_tome_in)
+                    set_el_instrument(u_tome, u_tome_in)  # Will be inherited from caller scope.  #  pylint: disable=used-before-assignment
                     # element 2
                     set_el_temperature(u_tome, u_tome_in)
                     # element 3
                     set_el_final_thickness(u_tome, u_tome_in)
                     # element 4
                     set_el_details(u_tome, u_tome_in)
 
@@ -6790,15 +6790,15 @@
                         if current_details is not None:
                             all_details = ". ".join((current_details, details_txt))
                         else:
                             all_details = details_txt
                         set_cif_value(fib.set_details, "details", const.EM_FOCUSED_ION_BEAM, cif_list=fib_in, cif_value=all_details)
 
                     # element 1
-                    details_txt = set_el_instrument(fib, fib_in)
+                    details_txt = set_el_instrument(fib, fib_in)  # Will be inherited from caller scope.  #  pylint: disable=used-before-assignment
                     # element 2
                     set_el_ion(fib, fib_in, details_txt)
                     # element 3
                     set_el_voltage(fib, fib_in)
                     # element 4
                     set_el_current(fib, fib_in)
                     # element 5
@@ -6812,22 +6812,22 @@
                     # element 9
                     set_el_final_thickness(fib, fib_in)
                     # element 10
                     set_el_details(fib, fib_in, details_txt)
 
                 sec_in = get_cif_value("sectioning", const.EM_TOMOGRAPHY_SPECIMEN, tom_prep_in)
                 if sec_in is not None:
-                    if sec_in == "ULTRAMICROTOMY" and tom_id_in in u_tome_dict_in:
+                    if sec_in == "ULTRAMICROTOMY" and tom_id_in in u_tome_dict_in:  # Ordering sets this  #  pylint: disable=possibly-used-before-assignment
                         u_tome_in = u_tome_dict_in[tom_id_in]
                         u_tome = emdb.ultramicrotomyType()
                         set_ultramicrotomy_type(u_tome)
                         if u_tome.has__content():
                             tom_prep.set_sectioning(emdb.sectioningType(ultramicrotomy=u_tome))
                     elif sec_in == "FOCUSED ION BEAM" and tom_id_in in fib_dict_in:
-                        fib_in = fib_dict_in[tom_id_in]
+                        fib_in = fib_dict_in[tom_id_in]  # fib_in must be set before calling set_focused_ion_beam_type
                         fib = emdb.focused_ion_beamType()
                         set_focused_ion_beam_type(fib)
                         if fib.has__content():
                             tom_prep.set_sectioning(emdb.sectioningType(focused_ion_beam=fib))
                     elif sec_in == "NO SECTIONING":
                         # XSD: choice 3: <xs:element name="other_sectioning" type="xs:string"/>
                         tom_prep.set_sectioning(emdb.sectioningType(other_sectioning=sec_in))
@@ -6935,15 +6935,15 @@
                     """
                     XSD:<xs:element name="details" type="xs:string" minOccurs="0">
                     CIF: _em_crystal_formation.details
                     """
                     set_cif_value(cryst.set_details, "details", const.EM_CRYSTAL_FORMATION, cif_list=cryst_in)
 
                 # element 1
-                set_el_lipid_protein_ratio(cryst, cryst_in)
+                set_el_lipid_protein_ratio(cryst, cryst_in)  # Will never happen but should be passed to function.  #  pylint: disable=possibly-used-before-assignment
                 # element 2
                 set_el_lipid_mixture(cryst, cryst_in)
                 # element 3
                 set_el_instrument(cryst, cryst_in)
                 # element 4
                 set_el_atmosphere(cryst, cryst_in)
                 # element 5
@@ -6952,15 +6952,15 @@
                 set_el_time(cryst, cryst_in)
                 # element 7
                 set_el_details(cryst, cryst_in)
 
             cryst_dict_in = make_dict(const.EM_CRYSTAL_FORMATION, const.K_SPECIMEN_ID)
 
             if sp_id_in in cryst_dict_in:
-                cryst_in = cryst_dict_in[sp_id_in]
+                cryst_in = cryst_dict_in[sp_id_in]  # must be set before set_crystal_formation_type
                 cryst = emdb.crystal_formationType()
                 set_crystal_formation_type(cryst)
                 if cryst.has__content():
                     cryst_prep.set_crystal_formation(cryst)
 
         def set_classification(ip_id_in, final_class_dict_in, cat_soft_dict_in):
             """
@@ -9149,19 +9149,19 @@
                             "final_rec_dict_in": non_st_dicts["final_rec_dict_in"],
                             "cat_soft_dict_in": non_st_dicts["cat_soft_dict_in"],
                             "p_sym_dict_in": non_st_dicts["p_sym_dict_in"],
                             "h_sym_dict_in": non_st_dicts["h_sym_dict_in"],
                         }
                         set_final_reconstruction(spfr, ip_id_in, final_rec_dicts)
                         # element 1
-                        set_el_number_images_used(spfr, f_rec_in)
+                        set_el_number_images_used(spfr, f_rec_in)  # Will never happen but should be passed to function.  #  pylint: disable=possibly-used-before-assignment
 
                     final_rec_dict_in = non_st_dicts["final_rec_dict_in"]
                     if ip_id_in in final_rec_dict_in:
-                        f_rec_in = final_rec_dict_in[ip_id_in]
+                        f_rec_in = final_rec_dict_in[ip_id_in]  # used in set_non_subtom_final_reconstruction_type
                         spfr = emdb.non_subtom_final_reconstruction_type()
                         set_non_subtom_final_rec_type(spfr)
                         im_proc.set_final_reconstruction(spfr)
 
                 def set_single_part_im_proc_specs(ip_id_in, im_proc, sp_dict_list):
                     """
                     Set elements specific for single particle image processing add group
```

### Comparing `wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/cif_emdb_translator/emdb.py` & `wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/cif_emdb_translator/emdb.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py` & `wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py` & `wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/data/emdb-v3.xsd` & `wwpdb_utils_emdb-1.9/wwpdb/utils/emdb/data/emdb-v3.xsd`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_emdb-1.8.2/wwpdb.utils.emdb.egg-info/PKG-INFO` & `wwpdb_utils_emdb-1.9/wwpdb.utils.emdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.emdb
-Version: 1.8.2
+Version: 1.9
 Summary: wwPDB EMDB to XML converter
 Home-page: https://github.com/rcsb/py-wwpdb_utils_config
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb_utils_emdb-1.8.2/wwpdb.utils.emdb.egg-info/SOURCES.txt` & `wwpdb_utils_emdb-1.9/wwpdb.utils.emdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

