# Comparing `tmp/napari_moltrack-0.0.6.tar.gz` & `tmp/napari_moltrack-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_moltrack-0.0.6.tar", last modified: Fri May 31 18:49:50 2024, max compression
+gzip compressed data, was "napari_moltrack-0.0.7.tar", last modified: Sat Jun  1 07:19:53 2024, max compression
```

## Comparing `napari_moltrack-0.0.6.tar` & `napari_moltrack-0.0.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 18:49:50.052069 napari_moltrack-0.0.6/
--rw-rw-rw-   0        0        0     1515 2024-05-29 16:12:09.000000 napari_moltrack-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      101 2024-05-29 16:12:09.000000 napari_moltrack-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     6468 2024-05-31 18:49:50.036447 napari_moltrack-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2705 2024-05-29 16:12:09.000000 napari_moltrack-0.0.6/README.md
--rw-rw-rw-   0        0        0     3406 2024-05-30 17:30:23.000000 napari_moltrack-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-31 18:49:50.052069 napari_moltrack-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-31 18:49:49.967448 napari_moltrack-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-05-31 18:49:49.989580 napari_moltrack-0.0.6/src/moltrack/
-drwxrwxrwx   0        0        0        0 2024-05-31 18:49:49.989580 napari_moltrack-0.0.6/src/moltrack/GUI/
--rw-rw-rw-   0        0        0        0 2024-05-29 16:42:16.000000 napari_moltrack-0.0.6/src/moltrack/GUI/__init__.py
--rw-rw-rw-   0        0        0    65658 2024-05-31 18:12:06.000000 napari_moltrack-0.0.6/src/moltrack/GUI/widget_ui.py
--rw-rw-rw-   0        0        0       98 2024-05-31 18:49:39.000000 napari_moltrack-0.0.6/src/moltrack/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 18:49:49.989580 napari_moltrack-0.0.6/src/moltrack/_tests/
--rw-rw-rw-   0        0        0        0 2024-05-29 16:12:09.000000 napari_moltrack-0.0.6/src/moltrack/_tests/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-05-29 16:15:26.000000 napari_moltrack-0.0.6/src/moltrack/_tests/test_widget.py
--rw-rw-rw-   0        0        0     7816 2024-05-31 18:10:07.000000 napari_moltrack-0.0.6/src/moltrack/_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-31 18:49:50.005204 napari_moltrack-0.0.6/src/moltrack/funcs/
--rw-rw-rw-   0        0        0        0 2024-05-30 07:19:51.000000 napari_moltrack-0.0.6/src/moltrack/funcs/__init__.py
--rw-rw-rw-   0        0        0     8053 2024-05-30 10:37:04.000000 napari_moltrack-0.0.6/src/moltrack/funcs/compute_utils.py
--rw-rw-rw-   0        0        0    15734 2024-05-31 17:45:32.000000 napari_moltrack-0.0.6/src/moltrack/funcs/events_utils.py
--rw-rw-rw-   0        0        0     9068 2024-05-31 18:43:16.000000 napari_moltrack-0.0.6/src/moltrack/funcs/export_utils.py
--rw-rw-rw-   0        0        0    12905 2024-05-31 09:24:15.000000 napari_moltrack-0.0.6/src/moltrack/funcs/import_utils.py
--rw-rw-rw-   0        0        0     5422 2024-05-30 10:39:02.000000 napari_moltrack-0.0.6/src/moltrack/funcs/loc_filter_utils.py
--rw-rw-rw-   0        0        0    33886 2024-05-31 17:45:56.000000 napari_moltrack-0.0.6/src/moltrack/funcs/picasso_detect_utils.py
--rw-rw-rw-   0        0        0     3282 2024-05-30 10:49:15.000000 napari_moltrack-0.0.6/src/moltrack/funcs/picasso_render_utils.py
--rw-rw-rw-   0        0        0    10414 2024-05-31 17:30:34.000000 napari_moltrack-0.0.6/src/moltrack/funcs/segmentation_events.py
--rw-rw-rw-   0        0        0    19142 2024-05-31 17:31:51.000000 napari_moltrack-0.0.6/src/moltrack/funcs/segmentation_utils.py
--rw-rw-rw-   0        0        0     4609 2024-05-31 18:48:23.000000 napari_moltrack-0.0.6/src/moltrack/funcs/tracking_utils.py
--rw-rw-rw-   0        0        0      495 2024-05-29 16:15:26.000000 napari_moltrack-0.0.6/src/moltrack/napari.yaml
-drwxrwxrwx   0        0        0        0 2024-05-31 18:49:50.036447 napari_moltrack-0.0.6/src/napari_moltrack.egg-info/
--rw-rw-rw-   0        0        0     6468 2024-05-31 18:49:49.000000 napari_moltrack-0.0.6/src/napari_moltrack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2024-05-31 18:49:49.000000 napari_moltrack-0.0.6/src/napari_moltrack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 18:49:49.000000 napari_moltrack-0.0.6/src/napari_moltrack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-05-31 18:49:49.000000 napari_moltrack-0.0.6/src/napari_moltrack.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      234 2024-05-31 18:49:49.000000 napari_moltrack-0.0.6/src/napari_moltrack.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-31 18:49:49.000000 napari_moltrack-0.0.6/src/napari_moltrack.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-31 18:49:50.036447 napari_moltrack-0.0.6/src/pygpufit/
--rw-rw-rw-   0        0        0  1982976 2024-05-21 11:03:35.000000 napari_moltrack-0.0.6/src/pygpufit/Gpufit.dll
--rw-rw-rw-   0        0        0        0 2024-05-21 11:03:35.000000 napari_moltrack-0.0.6/src/pygpufit/__init__.py
--rw-rw-rw-   0        0        0    14512 2024-05-21 11:03:35.000000 napari_moltrack-0.0.6/src/pygpufit/gpufit.py
--rw-rw-rw-   0        0        0      140 2024-05-21 11:03:35.000000 napari_moltrack-0.0.6/src/pygpufit/version.py
+drwxrwxrwx   0        0        0        0 2024-06-01 07:19:53.751804 napari_moltrack-0.0.7/
+-rw-rw-rw-   0        0        0     1515 2024-05-29 16:12:09.000000 napari_moltrack-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-05-29 16:12:09.000000 napari_moltrack-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     6468 2024-06-01 07:19:53.750834 napari_moltrack-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2705 2024-05-29 16:12:09.000000 napari_moltrack-0.0.7/README.md
+-rw-rw-rw-   0        0        0     3406 2024-05-30 17:30:23.000000 napari_moltrack-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-01 07:19:53.751804 napari_moltrack-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-01 07:19:53.683434 napari_moltrack-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-06-01 07:19:53.695432 napari_moltrack-0.0.7/src/moltrack/
+drwxrwxrwx   0        0        0        0 2024-06-01 07:19:53.698396 napari_moltrack-0.0.7/src/moltrack/GUI/
+-rw-rw-rw-   0        0        0        0 2024-05-29 16:42:16.000000 napari_moltrack-0.0.7/src/moltrack/GUI/__init__.py
+-rw-rw-rw-   0        0        0    67574 2024-06-01 07:17:47.000000 napari_moltrack-0.0.7/src/moltrack/GUI/widget_ui.py
+-rw-rw-rw-   0        0        0       98 2024-06-01 07:19:45.000000 napari_moltrack-0.0.7/src/moltrack/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 07:19:53.701389 napari_moltrack-0.0.7/src/moltrack/_tests/
+-rw-rw-rw-   0        0        0        0 2024-05-29 16:12:09.000000 napari_moltrack-0.0.7/src/moltrack/_tests/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-05-29 16:15:26.000000 napari_moltrack-0.0.7/src/moltrack/_tests/test_widget.py
+-rw-rw-rw-   0        0        0     7816 2024-05-31 18:10:07.000000 napari_moltrack-0.0.7/src/moltrack/_widget.py
+drwxrwxrwx   0        0        0        0 2024-06-01 07:19:53.719270 napari_moltrack-0.0.7/src/moltrack/funcs/
+-rw-rw-rw-   0        0        0        0 2024-05-30 07:19:51.000000 napari_moltrack-0.0.7/src/moltrack/funcs/__init__.py
+-rw-rw-rw-   0        0        0     8053 2024-05-30 10:37:04.000000 napari_moltrack-0.0.7/src/moltrack/funcs/compute_utils.py
+-rw-rw-rw-   0        0        0    15734 2024-05-31 17:45:32.000000 napari_moltrack-0.0.7/src/moltrack/funcs/events_utils.py
+-rw-rw-rw-   0        0        0     9068 2024-05-31 18:43:16.000000 napari_moltrack-0.0.7/src/moltrack/funcs/export_utils.py
+-rw-rw-rw-   0        0        0    12905 2024-05-31 09:24:15.000000 napari_moltrack-0.0.7/src/moltrack/funcs/import_utils.py
+-rw-rw-rw-   0        0        0     5422 2024-05-30 10:39:02.000000 napari_moltrack-0.0.7/src/moltrack/funcs/loc_filter_utils.py
+-rw-rw-rw-   0        0        0    33886 2024-05-31 17:45:56.000000 napari_moltrack-0.0.7/src/moltrack/funcs/picasso_detect_utils.py
+-rw-rw-rw-   0        0        0     3282 2024-05-30 10:49:15.000000 napari_moltrack-0.0.7/src/moltrack/funcs/picasso_render_utils.py
+-rw-rw-rw-   0        0        0    11810 2024-06-01 07:08:45.000000 napari_moltrack-0.0.7/src/moltrack/funcs/segmentation_events.py
+-rw-rw-rw-   0        0        0    19377 2024-06-01 06:45:42.000000 napari_moltrack-0.0.7/src/moltrack/funcs/segmentation_utils.py
+-rw-rw-rw-   0        0        0     4609 2024-05-31 18:48:23.000000 napari_moltrack-0.0.7/src/moltrack/funcs/tracking_utils.py
+-rw-rw-rw-   0        0        0      495 2024-05-29 16:15:26.000000 napari_moltrack-0.0.7/src/moltrack/napari.yaml
+drwxrwxrwx   0        0        0        0 2024-06-01 07:19:53.748839 napari_moltrack-0.0.7/src/napari_moltrack.egg-info/
+-rw-rw-rw-   0        0        0     6468 2024-06-01 07:19:53.000000 napari_moltrack-0.0.7/src/napari_moltrack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2024-06-01 07:19:53.000000 napari_moltrack-0.0.7/src/napari_moltrack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 07:19:53.000000 napari_moltrack-0.0.7/src/napari_moltrack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-06-01 07:19:53.000000 napari_moltrack-0.0.7/src/napari_moltrack.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      234 2024-06-01 07:19:53.000000 napari_moltrack-0.0.7/src/napari_moltrack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-06-01 07:19:53.000000 napari_moltrack-0.0.7/src/napari_moltrack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 07:19:53.745849 napari_moltrack-0.0.7/src/pygpufit/
+-rw-rw-rw-   0        0        0  1982976 2024-05-21 11:03:35.000000 napari_moltrack-0.0.7/src/pygpufit/Gpufit.dll
+-rw-rw-rw-   0        0        0        0 2024-05-21 11:03:35.000000 napari_moltrack-0.0.7/src/pygpufit/__init__.py
+-rw-rw-rw-   0        0        0    14512 2024-05-21 11:03:35.000000 napari_moltrack-0.0.7/src/pygpufit/gpufit.py
+-rw-rw-rw-   0        0        0      140 2024-05-21 11:03:35.000000 napari_moltrack-0.0.7/src/pygpufit/version.py
```

### Comparing `napari_moltrack-0.0.6/LICENSE` & `napari_moltrack-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.6/PKG-INFO` & `napari_moltrack-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-moltrack
-Version: 0.0.6
+Version: 0.0.7
 Summary: Single molecule tracking package for Napari
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: 
         Copyright (c) 2024, Piers Turner
         All rights reserved.
```

### Comparing `napari_moltrack-0.0.6/README.md` & `napari_moltrack-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.6/pyproject.toml` & `napari_moltrack-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.6/src/moltrack/GUI/widget_ui.py` & `napari_moltrack-0.0.7/src/moltrack/GUI/widget_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,26 +93,30 @@
         self.verticalLayout_19.setObjectName("verticalLayout_19")
         self.formLayout_21 = QtWidgets.QFormLayout()
         self.formLayout_21.setObjectName("formLayout_21")
         self.label_76 = QtWidgets.QLabel(self.tab_16)
         self.label_76.setObjectName("label_76")
         self.formLayout_21.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_76)
         self.import_picasso_type = QtWidgets.QComboBox(self.tab_16)
+        self.import_picasso_type.setEnabled(False)
+        self.import_picasso_type.setEditable(False)
         self.import_picasso_type.setObjectName("import_picasso_type")
         self.import_picasso_type.addItem("")
         self.import_picasso_type.addItem("")
         self.formLayout_21.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.import_picasso_type)
         self.label_2 = QtWidgets.QLabel(self.tab_16)
         self.label_2.setObjectName("label_2")
         self.formLayout_21.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_2)
         self.import_picasso_dataset = QtWidgets.QComboBox(self.tab_16)
+        self.import_picasso_dataset.setEnabled(False)
         self.import_picasso_dataset.setObjectName("import_picasso_dataset")
         self.formLayout_21.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.import_picasso_dataset)
         self.verticalLayout_19.addLayout(self.formLayout_21)
         self.import_picasso = QtWidgets.QPushButton(self.tab_16)
+        self.import_picasso.setEnabled(False)
         self.import_picasso.setObjectName("import_picasso")
         self.verticalLayout_19.addWidget(self.import_picasso)
         spacerItem1 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_19.addItem(spacerItem1)
         self.tabWidget_4.addTab(self.tab_16, "")
         self.verticalLayout_2.addWidget(self.tabWidget_4)
         self.import_progressbar = QtWidgets.QProgressBar(self.tab)
@@ -302,54 +306,76 @@
         spacerItem5 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout_28.addItem(spacerItem5)
         self.tabWidget_7.addTab(self.tab_24, "")
         self.tab_26 = QtWidgets.QWidget()
         self.tab_26.setObjectName("tab_26")
         self.verticalLayout_30 = QtWidgets.QVBoxLayout(self.tab_26)
         self.verticalLayout_30.setObjectName("verticalLayout_30")
+        self.label_132 = QtWidgets.QLabel(self.tab_26)
+        font = QtGui.QFont()
+        font.setBold(True)
+        font.setWeight(75)
+        self.label_132.setFont(font)
+        self.label_132.setObjectName("label_132")
+        self.verticalLayout_30.addWidget(self.label_132)
+        self.label_15 = QtWidgets.QLabel(self.tab_26)
+        self.label_15.setObjectName("label_15")
+        self.verticalLayout_30.addWidget(self.label_15)
+        self.label_17 = QtWidgets.QLabel(self.tab_26)
+        self.label_17.setObjectName("label_17")
+        self.verticalLayout_30.addWidget(self.label_17)
+        self.label_18 = QtWidgets.QLabel(self.tab_26)
+        self.label_18.setObjectName("label_18")
+        self.verticalLayout_30.addWidget(self.label_18)
+        self.label_16 = QtWidgets.QLabel(self.tab_26)
+        self.label_16.setObjectName("label_16")
+        self.verticalLayout_30.addWidget(self.label_16)
+        spacerItem6 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_30.addItem(spacerItem6)
         self.label_103 = QtWidgets.QLabel(self.tab_26)
         font = QtGui.QFont()
         font.setBold(True)
         font.setWeight(75)
         self.label_103.setFont(font)
         self.label_103.setObjectName("label_103")
         self.verticalLayout_30.addWidget(self.label_103)
         self.formLayout_26 = QtWidgets.QFormLayout()
         self.formLayout_26.setObjectName("formLayout_26")
         self.label_111 = QtWidgets.QLabel(self.tab_26)
         self.label_111.setObjectName("label_111")
         self.formLayout_26.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_111)
         self.dilatation_size = QtWidgets.QDoubleSpinBox(self.tab_26)
         self.dilatation_size.setDecimals(1)
-        self.dilatation_size.setMinimum(0.1)
+        self.dilatation_size.setMinimum(-10.0)
         self.dilatation_size.setMaximum(10.0)
+        self.dilatation_size.setSingleStep(0.1)
         self.dilatation_size.setProperty("value", 1.0)
         self.dilatation_size.setObjectName("dilatation_size")
         self.formLayout_26.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.dilatation_size)
         self.verticalLayout_30.addLayout(self.formLayout_26)
         self.dilate_segmentations = QtWidgets.QPushButton(self.tab_26)
         self.dilate_segmentations.setObjectName("dilate_segmentations")
         self.verticalLayout_30.addWidget(self.dilate_segmentations)
-        spacerItem6 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_30.addItem(spacerItem6)
+        spacerItem7 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_30.addItem(spacerItem7)
         self.label_105 = QtWidgets.QLabel(self.tab_26)
         font = QtGui.QFont()
         font.setBold(True)
         font.setWeight(75)
         self.label_105.setFont(font)
         self.label_105.setObjectName("label_105")
         self.verticalLayout_30.addWidget(self.label_105)
         self.formLayout_32 = QtWidgets.QFormLayout()
         self.formLayout_32.setObjectName("formLayout_32")
         self.label_131 = QtWidgets.QLabel(self.tab_26)
         self.label_131.setObjectName("label_131")
         self.formLayout_32.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_131)
         self.translation_size = QtWidgets.QDoubleSpinBox(self.tab_26)
         self.translation_size.setDecimals(1)
-        self.translation_size.setMinimum(0.1)
+        self.translation_size.setMinimum(0.5)
         self.translation_size.setObjectName("translation_size")
         self.formLayout_32.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.translation_size)
         self.label_9 = QtWidgets.QLabel(self.tab_26)
         self.label_9.setObjectName("label_9")
         self.formLayout_32.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_9)
         self.translation_target = QtWidgets.QComboBox(self.tab_26)
         self.translation_target.setObjectName("translation_target")
@@ -357,20 +383,20 @@
         self.translation_target.addItem("")
         self.translation_target.addItem("")
         self.formLayout_32.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.translation_target)
         self.verticalLayout_30.addLayout(self.formLayout_32)
         self.label_10 = QtWidgets.QLabel(self.tab_26)
         self.label_10.setObjectName("label_10")
         self.verticalLayout_30.addWidget(self.label_10)
-        spacerItem7 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_30.addItem(spacerItem7)
+        spacerItem8 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_30.addItem(spacerItem8)
         self.tabWidget_7.addTab(self.tab_26, "")
         self.verticalLayout_27.addWidget(self.tabWidget_7)
-        spacerItem8 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_27.addItem(spacerItem8)
+        spacerItem9 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_27.addItem(spacerItem9)
         self.tabWidget.addTab(self.tab_25, "")
         self.tab_2 = QtWidgets.QWidget()
         self.tab_2.setObjectName("tab_2")
         self.verticalLayout_3 = QtWidgets.QVBoxLayout(self.tab_2)
         self.verticalLayout_3.setObjectName("verticalLayout_3")
         self.tabWidget_6 = QtWidgets.QTabWidget(self.tab_2)
         self.tabWidget_6.setObjectName("tabWidget_6")
@@ -420,15 +446,15 @@
         self.picasso_roi_border_width.setObjectName("picasso_roi_border_width")
         self.formLayout_3.setWidget(10, QtWidgets.QFormLayout.FieldRole, self.picasso_roi_border_width)
         self.label_35 = QtWidgets.QLabel(self.tab_21)
         self.label_35.setObjectName("label_35")
         self.formLayout_3.setWidget(10, QtWidgets.QFormLayout.LabelRole, self.label_35)
         self.moltrack_window_size = QtWidgets.QSpinBox(self.tab_21)
         self.moltrack_window_size.setMaximum(100)
-        self.moltrack_window_size.setProperty("value", 5)
+        self.moltrack_window_size.setProperty("value", 7)
         self.moltrack_window_size.setObjectName("moltrack_window_size")
         self.formLayout_3.setWidget(8, QtWidgets.QFormLayout.FieldRole, self.moltrack_window_size)
         self.moltrack_window_size_label = QtWidgets.QLabel(self.tab_21)
         self.moltrack_window_size_label.setObjectName("moltrack_window_size_label")
         self.formLayout_3.setWidget(8, QtWidgets.QFormLayout.LabelRole, self.moltrack_window_size_label)
         self.moltrack_threshold = QtWidgets.QSpinBox(self.tab_21)
         self.moltrack_threshold.setMaximum(255)
@@ -492,16 +518,16 @@
         self.gridLayout_6.addWidget(self.picasso_fit, 0, 1, 1, 1)
         self.verticalLayout_23.addLayout(self.gridLayout_6)
         self.picasso_progressbar = QtWidgets.QProgressBar(self.tab_21)
         self.picasso_progressbar.setMaximumSize(QtCore.QSize(16777215, 10))
         self.picasso_progressbar.setProperty("value", 0)
         self.picasso_progressbar.setObjectName("picasso_progressbar")
         self.verticalLayout_23.addWidget(self.picasso_progressbar)
-        spacerItem9 = QtWidgets.QSpacerItem(20, 0, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.MinimumExpanding)
-        self.verticalLayout_23.addItem(spacerItem9)
+        spacerItem10 = QtWidgets.QSpacerItem(20, 0, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.MinimumExpanding)
+        self.verticalLayout_23.addItem(spacerItem10)
         self.tabWidget_6.addTab(self.tab_21, "")
         self.tab_23 = QtWidgets.QWidget()
         self.tab_23.setObjectName("tab_23")
         self.verticalLayout_26 = QtWidgets.QVBoxLayout(self.tab_23)
         self.verticalLayout_26.setObjectName("verticalLayout_26")
         self.label_92 = QtWidgets.QLabel(self.tab_23)
         font = QtGui.QFont()
@@ -614,16 +640,16 @@
         self.picasso_render_min_blur.setSingleStep(0.1)
         self.picasso_render_min_blur.setObjectName("picasso_render_min_blur")
         self.formLayout_20.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.picasso_render_min_blur)
         self.verticalLayout_25.addLayout(self.formLayout_20)
         self.picasso_render = QtWidgets.QPushButton(self.tab_20)
         self.picasso_render.setObjectName("picasso_render")
         self.verticalLayout_25.addWidget(self.picasso_render)
-        spacerItem10 = QtWidgets.QSpacerItem(413, 173, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_25.addItem(spacerItem10)
+        spacerItem11 = QtWidgets.QSpacerItem(413, 173, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_25.addItem(spacerItem11)
         self.tabWidget_6.addTab(self.tab_20, "")
         self.tab_27 = QtWidgets.QWidget()
         self.tab_27.setObjectName("tab_27")
         self.verticalLayout_29 = QtWidgets.QVBoxLayout(self.tab_27)
         self.verticalLayout_29.setObjectName("verticalLayout_29")
         self.label_80 = QtWidgets.QLabel(self.tab_27)
         font = QtGui.QFont()
@@ -640,39 +666,41 @@
         self.tracking_dataset = QtWidgets.QComboBox(self.tab_27)
         self.tracking_dataset.setObjectName("tracking_dataset")
         self.formLayout_25.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.tracking_dataset)
         self.label_98 = QtWidgets.QLabel(self.tab_27)
         self.label_98.setObjectName("label_98")
         self.formLayout_25.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_98)
         self.trackpy_search_range = QtWidgets.QDoubleSpinBox(self.tab_27)
-        self.trackpy_search_range.setProperty("value", 1.0)
+        self.trackpy_search_range.setProperty("value", 5.0)
         self.trackpy_search_range.setObjectName("trackpy_search_range")
         self.formLayout_25.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.trackpy_search_range)
         self.label_99 = QtWidgets.QLabel(self.tab_27)
         self.label_99.setObjectName("label_99")
         self.formLayout_25.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_99)
         self.trackpy_memory = QtWidgets.QSpinBox(self.tab_27)
+        self.trackpy_memory.setProperty("value", 1)
         self.trackpy_memory.setObjectName("trackpy_memory")
         self.formLayout_25.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.trackpy_memory)
         self.label_100 = QtWidgets.QLabel(self.tab_27)
         self.label_100.setObjectName("label_100")
         self.formLayout_25.setWidget(3, QtWidgets.QFormLayout.LabelRole, self.label_100)
         self.min_track_length = QtWidgets.QSpinBox(self.tab_27)
         self.min_track_length.setMinimum(1)
+        self.min_track_length.setProperty("value", 5)
         self.min_track_length.setObjectName("min_track_length")
         self.formLayout_25.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.min_track_length)
         self.verticalLayout_29.addLayout(self.formLayout_25)
         self.remove_unlinked = QtWidgets.QCheckBox(self.tab_27)
         self.remove_unlinked.setObjectName("remove_unlinked")
         self.verticalLayout_29.addWidget(self.remove_unlinked)
         self.link_localisations = QtWidgets.QPushButton(self.tab_27)
         self.link_localisations.setObjectName("link_localisations")
         self.verticalLayout_29.addWidget(self.link_localisations)
-        spacerItem11 = QtWidgets.QSpacerItem(20, 122, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_29.addItem(spacerItem11)
+        spacerItem12 = QtWidgets.QSpacerItem(20, 122, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_29.addItem(spacerItem12)
         self.tabWidget_6.addTab(self.tab_27, "")
         self.tab_22 = QtWidgets.QWidget()
         self.tab_22.setObjectName("tab_22")
         self.verticalLayout_24 = QtWidgets.QVBoxLayout(self.tab_22)
         self.verticalLayout_24.setObjectName("verticalLayout_24")
         self.label_27 = QtWidgets.QLabel(self.tab_22)
         font = QtGui.QFont()
@@ -736,20 +764,20 @@
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.picasso_vis_edge_width.addItem("")
         self.gridLayout_14.addWidget(self.picasso_vis_edge_width, 1, 3, 1, 1)
         self.verticalLayout_24.addLayout(self.gridLayout_14)
-        spacerItem12 = QtWidgets.QSpacerItem(354, 254, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_24.addItem(spacerItem12)
+        spacerItem13 = QtWidgets.QSpacerItem(354, 254, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_24.addItem(spacerItem13)
         self.tabWidget_6.addTab(self.tab_22, "")
         self.verticalLayout_3.addWidget(self.tabWidget_6)
-        spacerItem13 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_3.addItem(spacerItem13)
+        spacerItem14 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_3.addItem(spacerItem14)
         self.tabWidget.addTab(self.tab_2, "")
         self.tab_6 = QtWidgets.QWidget()
         self.tab_6.setObjectName("tab_6")
         self.verticalLayout_11 = QtWidgets.QVBoxLayout(self.tab_6)
         self.verticalLayout_11.setObjectName("verticalLayout_11")
         self.label_74 = QtWidgets.QLabel(self.tab_6)
         self.label_74.setObjectName("label_74")
@@ -783,16 +811,16 @@
         self.export_localisations.setObjectName("export_localisations")
         self.verticalLayout_11.addWidget(self.export_localisations)
         self.export_progressbar = QtWidgets.QProgressBar(self.tab_6)
         self.export_progressbar.setMaximumSize(QtCore.QSize(16777215, 10))
         self.export_progressbar.setProperty("value", 0)
         self.export_progressbar.setObjectName("export_progressbar")
         self.verticalLayout_11.addWidget(self.export_progressbar)
-        spacerItem14 = QtWidgets.QSpacerItem(354, 414, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.verticalLayout_11.addItem(spacerItem14)
+        spacerItem15 = QtWidgets.QSpacerItem(354, 414, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_11.addItem(spacerItem15)
         self.tabWidget.addTab(self.tab_6, "")
         self.verticalLayout.addWidget(self.tabWidget)
         self.label_12 = QtWidgets.QLabel(Frame)
         font = QtGui.QFont()
         font.setBold(True)
         font.setWeight(75)
         self.label_12.setFont(font)
@@ -809,15 +837,15 @@
         self.verticalLayout.addLayout(self.formLayout_2)
 
         self.retranslateUi(Frame)
         self.tabWidget.setCurrentIndex(0)
         self.tabWidget_4.setCurrentIndex(0)
         self.tabWidget_7.setCurrentIndex(0)
         self.tabWidget_6.setCurrentIndex(0)
-        self.picasso_box_size.setCurrentIndex(0)
+        self.picasso_box_size.setCurrentIndex(1)
         self.picasso_vis_size.setCurrentIndex(4)
         self.picasso_vis_opacity.setCurrentIndex(9)
         self.picasso_vis_edge_width.setCurrentIndex(0)
         QtCore.QMetaObject.connectSlotsByName(Frame)
 
     def retranslateUi(self, Frame):
         _translate = QtCore.QCoreApplication.translate
@@ -893,26 +921,31 @@
         self.label_109.setText(_translate("Frame", "Diameter"))
         self.cellpose_diameter_label.setText(_translate("Frame", "15"))
         self.cellpose_invert_images.setText(_translate("Frame", "Invert Images"))
         self.label_110.setText(_translate("Frame", "Cellpose/Omnipose Functions"))
         self.cellpose_load_model.setText(_translate("Frame", "Load Custom Model"))
         self.segment_all.setText(_translate("Frame", "Segment All Images"))
         self.segment_active.setText(_translate("Frame", "Segment Active Image"))
-        self.tabWidget_7.setTabText(self.tabWidget_7.indexOf(self.tab_24), _translate("Frame", "Cellpose"))
+        self.tabWidget_7.setTabText(self.tabWidget_7.indexOf(self.tab_24), _translate("Frame", "ML Segmentation (Cellpose)"))
+        self.label_132.setText(_translate("Frame", "Keyboard/Mouse Shortcuts"))
+        self.label_15.setText(_translate("Frame", "Add Segmentation [Space]"))
+        self.label_17.setText(_translate("Frame", "Extend Segmentation [E]"))
+        self.label_18.setText(_translate("Frame", "Join Segmentations [J]"))
+        self.label_16.setText(_translate("Frame", "Delete Segmentation [D] or [Double Click]"))
         self.label_103.setText(_translate("Frame", "Dilate Segmentations"))
         self.label_111.setText(_translate("Frame", "Pixels"))
         self.dilate_segmentations.setText(_translate("Frame", "Dilate Segmentations"))
         self.label_105.setText(_translate("Frame", "Translate Segmentations"))
         self.label_131.setText(_translate("Frame", "Translation Size (Pixels)"))
         self.label_9.setText(_translate("Frame", "Translation Target"))
         self.translation_target.setItemText(0, _translate("Frame", "Segmentation Image"))
         self.translation_target.setItemText(1, _translate("Frame", "Segmentations"))
         self.translation_target.setItemText(2, _translate("Frame", "Both"))
         self.label_10.setText(_translate("Frame", "Press [Control] + [Arrow Key] to move translation target by translation size"))
-        self.tabWidget_7.setTabText(self.tabWidget_7.indexOf(self.tab_26), _translate("Frame", "Curate"))
+        self.tabWidget_7.setTabText(self.tabWidget_7.indexOf(self.tab_26), _translate("Frame", "Edit Segmentations"))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_25), _translate("Frame", "Segment"))
         self.label_3.setText(_translate("Frame", "Detect Localisations"))
         self.label_7.setText(_translate("Frame", "Detect Mode"))
         self.smlm_detect_mode.setItemText(0, _translate("Frame", "MolTrack"))
         self.smlm_detect_mode.setItemText(1, _translate("Frame", "Picasso"))
         self.label_11.setText(_translate("Frame", "Dataset"))
         self.label_8.setText(_translate("Frame", "Frame Mode"))
```

### Comparing `napari_moltrack-0.0.6/src/moltrack/_tests/test_widget.py` & `napari_moltrack-0.0.7/src/moltrack/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.6/src/moltrack/_widget.py` & `napari_moltrack-0.0.7/src/moltrack/_widget.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.6/src/moltrack/funcs/compute_utils.py` & `napari_moltrack-0.0.7/src/moltrack/funcs/compute_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.6/src/moltrack/funcs/events_utils.py` & `napari_moltrack-0.0.7/src/moltrack/funcs/events_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.6/src/moltrack/funcs/export_utils.py` & `napari_moltrack-0.0.7/src/moltrack/funcs/export_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.6/src/moltrack/funcs/import_utils.py` & `napari_moltrack-0.0.7/src/moltrack/funcs/import_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.6/src/moltrack/funcs/loc_filter_utils.py` & `napari_moltrack-0.0.7/src/moltrack/funcs/loc_filter_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.6/src/moltrack/funcs/picasso_detect_utils.py` & `napari_moltrack-0.0.7/src/moltrack/funcs/picasso_detect_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.6/src/moltrack/funcs/picasso_render_utils.py` & `napari_moltrack-0.0.7/src/moltrack/funcs/picasso_render_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.6/src/moltrack/funcs/segmentation_events.py` & `napari_moltrack-0.0.7/src/moltrack/funcs/segmentation_events.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 
     def register_segmentation_keybinds(self, layer):
 
         layer.bind_key(key='Space', func=lambda event: self.segmentation_modify_mode(mode="add"), overwrite=True)
         layer.bind_key(key='e', func=lambda event: self.segmentation_modify_mode(mode="extend"), overwrite=True)
         layer.bind_key(key='j', func=lambda event: self.segmentation_modify_mode(mode="join"), overwrite=True)
         layer.bind_key(key='s', func=lambda event: self.segmentation_modify_mode(mode="split"), overwrite=True)
-        layer.bind_key(key='Delete', func=lambda event: self.segmentation_modify_mode(mode="delete"), overwrite=True)
-        layer.bind_key(key='Backspace', func=lambda event: self.segmentation_modify_mode(mode="delete"), overwrite=True)
-
+        layer.bind_key(key='d', func=lambda event: self.segmentation_modify_mode(mode="delete"), overwrite=True)
 
     def initialise_segLayer(self, shapes = None):
 
         layer_names = [layer.name for layer in self.viewer.layers]
 
         if "Segmentations" in layer_names:
             self.viewer.layers.remove("Segmentations")
@@ -33,14 +31,15 @@
             self.segLayer = self.viewer.add_shapes(name="Segmentations", shape_type="polygon",
                 opacity=0.5, face_color="red", edge_color="black", edge_width=1, data=shapes)
         else:
             self.segLayer = self.viewer.add_shapes(name="Segmentations", shape_type="polygon",
                 opacity=0.5, face_color="red", edge_color="black", edge_width=1)
 
         self.segLayer.mouse_drag_callbacks.append(self.seg_drag_event)
+        self.segLayer.mouse_double_click_callbacks.append(self.delete_clicked)
         self.segLayer.events.data.connect(self.update_shapes)
         self.register_segmentation_keybinds(self.segLayer)
 
         return self.segLayer
 
 
     def get_seglayer(self, shapes = None):
@@ -56,16 +55,14 @@
 
     def segmentation_modify_mode(self, viewer=None, mode = "add"):
 
         try:
 
             self.segLayer = self.get_seglayer()
 
-            print(f"Segmentation mode: {mode}")
-
             if mode == "add":
                 self.viewer.layers.selection.select_only(self.segLayer)
 
                 self.interface_mode = "segment"
                 self.segmentation_mode = "add"
                 self.segLayer.mode = "add_polygon_lasso"
                 show_info("Add (click/drag to add)")
@@ -109,24 +106,34 @@
 
 
     def remove_shapes(self, indices):
 
         if type(indices) == int:
             indices = [indices]
 
-        self.segLayer.selected_data = indices
-        self.segLayer.remove_selected()
+        if len(indices) > 0:
+
+            self.segLayer.mode = "pan_zoom"
+
+            self.segLayer.events.data.disconnect(self.update_shapes)
+
+            self.segLayer.selected_data = indices
+            self.segLayer.remove_selected()
+
+            self.segLayer.events.data.connect(self.update_shapes)
 
 
     def update_shapes(self, event):
 
         try:
 
             if event.action == "added":
 
+                self.segLayer.mode = "pan_zoom"
+
                 if self.segmentation_mode == "join":
 
                     shapes = self.segLayer.data
                     last_index = len(shapes)-1
 
                     self.remove_shapes(last_index)
 
@@ -147,44 +154,76 @@
 
                                 if union_shape is not None:
 
                                     self.remove_shapes([shape_index1, shape_index2])
                                     shapes = self.segLayer.data.copy()
                                     shapes.append(union_shape)
                                     self.segLayer.data = shapes
+                                    self.segLayer.refresh()
 
                     self.join_coords = None
 
                 if self.segmentation_mode == "extend":
 
+                    extend_shapes = False
+
                     if hasattr(self, "extend_indices"):
 
                         if type(self.extend_indices) == list:
 
                             if len(self.extend_indices) == 2:
 
-                                shape_index, extend_index = self.extend_indices
+                                extend_shapes = True
 
-                                shapes = self.segLayer.data.copy()
+                    if extend_shapes:
 
-                                target = shapes[shape_index].copy()
-                                extension = shapes[extend_index].copy()
+                        shape_index, extend_index = self.extend_indices
 
-                                if len(target) > 4 and len(extension) > 4:
+                        shapes = self.segLayer.data.copy()
+
+                        target = shapes[shape_index].copy()
+                        extension = shapes[extend_index].copy()
+
+                        if len(target) > 4 and len(extension) > 4:
+
+                            union_shape = self.join_shapes(target, extension)
 
-                                    union_shape = self.join_shapes(target, extension)
+                            if union_shape is not None:
 
-                                    if union_shape is not None:
+                                self.segLayer.events.data.disconnect(self.update_shapes)
+                                self.segLayer.selected_data = [shape_index, extend_index]
+                                self.segLayer.remove_selected()
+                                self.segLayer.add(union_shape, shape_type="polygon")
+                                self.segLayer.events.data.connect(self.update_shapes)
 
-                                        self.segLayer.events.data.disconnect(self.update_shapes)
-                                        self.segLayer.add(union_shape, shape_type="polygon")
-                                        self.segLayer.events.data.connect(self.update_shapes)
+                    else:
+
+                        shapes = self.segLayer.data.copy()
+                        last_index = len(shapes)-1
+                        self.remove_shapes(last_index)
 
                     self.extend_indices = None
 
+            if event.action in ["added", "changed"]:
+                self.segLayer.mode = "pan_zoom"
+
+        except:
+            print(traceback.format_exc())
+            pass
+
+    def delete_clicked(self, viewer=None, event=None):
+
+        try:
+
+            coords = self.segLayer.world_to_data(event.position)
+            shape_index = self.segLayer.get_value(coords)[0]
+
+            if shape_index is not None:
+                self.remove_shapes([shape_index])
+
         except:
             print(traceback.format_exc())
             pass
 
 
     def seg_drag_event(self, viwer = None, event = None):
 
@@ -249,49 +288,55 @@
 
                         shapes = self.segLayer.data.copy()
                         last_index = len(shapes)-1
 
                         self.extend_indices = [shape_index, last_index]
 
 
-
-    def join_shapes(self, shape1, shape2, simplify = True):
+    def join_shapes(self, shape1, shape2, simplify = True, buffer = 1):
 
         union_shape = None
 
         try:
 
             if shape1.shape[1] == 2:
+
                 shape1 = Polygon(shape1)
                 shape2 = Polygon(shape2)
 
+                shape1 = shape1.buffer(buffer)
+                shape2 = shape2.buffer(buffer)
+
                 if shape1.intersects(shape2):
 
                     union_polygon = unary_union([shape1, shape2])
+                    union_polygon = union_polygon.buffer(-buffer)
 
                     if simplify == True:
-                        print("Simplify")
                         union_polygon = union_polygon.simplify(0.1)
 
                     union_shape = np.array(union_polygon.exterior.coords)
 
                     union_shape = union_shape[1:]
                     union_shape = union_shape.astype(float)
 
             else:
                 frame_index = shape1[0, 0]
                 shape1 = Polygon(shape1[:, 1:])
                 shape2 = Polygon(shape2[:, 1:])
 
+                shape1 = shape1.buffer(buffer)
+                shape2 = shape2.buffer(buffer)
+
                 if shape1.intersects(shape2):
 
                     union_polygon = unary_union([shape1, shape2])
+                    union_polygon = union_polygon.buffer(-buffer)
 
                     if simplify == True:
-                        print("Simplify")
                         union_polygon = union_polygon.simplify(0.1)
 
                     union_shape = np.array(union_polygon.exterior.coords)
                     union_shape = np.insert(union_shape, 0, frame_index, axis=1)
 
                     union_shape = union_shape[1:]
                     union_shape = union_shape.astype(float)
```

### Comparing `napari_moltrack-0.0.6/src/moltrack/funcs/segmentation_utils.py` & `napari_moltrack-0.0.7/src/moltrack/funcs/segmentation_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -482,65 +482,70 @@
 
         try:
 
             layer_names = [layer.name for layer in self.viewer.layers]
 
             buffer = float(self.gui.dilatation_size.value())
 
-            if "Segmentations" in layer_names and filter:
+            if "Segmentations" in layer_names:
 
                 self.update_ui(init=True)
 
-                segLayer = self.viewer.layers["Segmentations"]
+                segLayer = self.segLayer
 
                 segmentations = segLayer.data.copy()
                 shape_types = segLayer.shape_type
 
                 segmentations = [seg for seg, shape in zip(segmentations, shape_types) if shape == "polygon"]
+                segmentations = [seg for seg in segmentations if len(seg) > 4]
 
                 for index, seg in enumerate(segmentations):
 
-                    ndim = segmentations[0].shape[1]
+                    try:
 
-                    if ndim == 2:
+                        ndim = seg.shape[1]
 
-                        seg = np.fliplr(seg)
-                        poly = Polygon(seg)
-                        poly = poly.buffer(buffer)
-
-                        if simplify == True:
-                            poly = poly.simplify(0.1)
-
-                        seg = np.array(poly.exterior.coords)
-                        seg = np.fliplr(seg)
-                        seg = seg.astype(float)
-                        seg = seg[:-1]
-                        segmentations[index] = seg
-
-                    if ndim == 3:
-
-                        frame = int(seg[0, 0])
-                        seg = seg[:, 1:]
-                        seg = np.fliplr(seg)
-                        poly = Polygon(seg)
-                        poly = poly.buffer(buffer)
-
-                        if simplify == True:
-                            poly = poly.simplify(0.1)
-
-                        seg = np.array(poly.exterior.coords)
-                        seg = np.fliplr(seg)
-                        seg = seg.astype(float)
-                        seg = seg[:-1]
-                        seg = np.insert(seg, 0, frame, axis=1)
-                        segmentations[index] = seg
+                        if ndim == 2:
 
+                            seg = np.fliplr(seg)
+                            poly = Polygon(seg)
+                            poly = poly.buffer(buffer)
+
+                            if simplify == True:
+                                poly = poly.simplify(0.1)
+
+                            seg = np.array(poly.exterior.coords)
+                            seg = np.fliplr(seg)
+                            seg = seg.astype(float)
+                            seg = seg[:-1]
+                            segmentations[index] = seg
+
+                        elif ndim == 3:
+
+                            frame = int(seg[0, 0])
+                            seg = seg[:, 1:]
+                            seg = np.fliplr(seg)
+                            poly = Polygon(seg)
+                            poly = poly.buffer(buffer)
+
+                            if simplify == True:
+                                poly = poly.simplify(0.1)
+
+                            seg = np.array(poly.exterior.coords)
+                            seg = np.fliplr(seg)
+                            seg = seg.astype(float)
+                            seg = seg[:-1]
+                            seg = np.insert(seg, 0, frame, axis=1)
+                            segmentations[index] = seg
+
+                    except:
+                        pass
 
                 # update layer
-                segLayer.data = []
+                segLayer.mode = "pan_zoom"
                 segLayer.data = segmentations
 
                 self.update_ui()
 
         except:
             self.update_ui()
             print(traceback.format_exc())
```

### Comparing `napari_moltrack-0.0.6/src/moltrack/funcs/tracking_utils.py` & `napari_moltrack-0.0.7/src/moltrack/funcs/tracking_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.6/src/napari_moltrack.egg-info/PKG-INFO` & `napari_moltrack-0.0.7/src/napari_moltrack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-moltrack
-Version: 0.0.6
+Version: 0.0.7
 Summary: Single molecule tracking package for Napari
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: 
         Copyright (c) 2024, Piers Turner
         All rights reserved.
```

### Comparing `napari_moltrack-0.0.6/src/napari_moltrack.egg-info/SOURCES.txt` & `napari_moltrack-0.0.7/src/napari_moltrack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.6/src/pygpufit/Gpufit.dll` & `napari_moltrack-0.0.7/src/pygpufit/Gpufit.dll`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.6/src/pygpufit/gpufit.py` & `napari_moltrack-0.0.7/src/pygpufit/gpufit.py`

 * *Files identical despite different names*

