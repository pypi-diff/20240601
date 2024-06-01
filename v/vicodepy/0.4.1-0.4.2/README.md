# Comparing `tmp/vicodepy-0.4.1.tar.gz` & `tmp/vicodepy-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vicodepy-0.4.1.tar", last modified: Fri May 31 07:53:27 2024, max compression
+gzip compressed data, was "vicodepy-0.4.2.tar", last modified: Sat Jun  1 10:38:51 2024, max compression
```

## Comparing `vicodepy-0.4.1.tar` & `vicodepy-0.4.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1372 2024-05-31 07:53:21.000000 vicodepy-0.4.1/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2024-05-31 07:53:21.000000 vicodepy-0.4.1/LICENSE
--rw-r--r--   0        0        0     2758 2024-05-31 07:53:21.000000 vicodepy-0.4.1/README.md
--rw-r--r--   0        0        0      875 2024-05-31 07:53:21.000000 vicodepy-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      818 2024-05-31 07:53:21.000000 vicodepy-0.4.1/vicodepy/__init__.py
--rw-r--r--   0        0        0      957 2024-05-31 07:53:21.000000 vicodepy-0.4.1/vicodepy/__main__.py
--rw-r--r--   0        0        0    43326 2024-05-31 07:53:21.000000 vicodepy-0.4.1/vicodepy/app.py
--rw-r--r--   0        0        0     1032 2024-05-31 07:53:21.000000 vicodepy-0.4.1/vicodepy/command.py
--rw-r--r--   0        0        0      202 2024-05-31 07:53:21.000000 vicodepy-0.4.1/vicodepy/config/config.yml
--rw-r--r--   0        0        0       43 2024-05-31 07:53:21.000000 vicodepy-0.4.1/vicodepy/style.qss
--rw-r--r--   0        0        0     3078 2024-05-31 07:53:21.000000 vicodepy-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1564 2024-06-01 10:38:44.000000 vicodepy-0.4.2/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2024-06-01 10:38:44.000000 vicodepy-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2758 2024-06-01 10:38:44.000000 vicodepy-0.4.2/README.md
+-rw-r--r--   0        0        0      896 2024-06-01 10:38:44.000000 vicodepy-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      818 2024-06-01 10:38:44.000000 vicodepy-0.4.2/vicodepy/__init__.py
+-rw-r--r--   0        0        0      957 2024-06-01 10:38:44.000000 vicodepy-0.4.2/vicodepy/__main__.py
+-rw-r--r--   0        0        0    43076 2024-06-01 10:38:44.000000 vicodepy-0.4.2/vicodepy/app.py
+-rw-r--r--   0        0        0     1323 2024-06-01 10:38:44.000000 vicodepy-0.4.2/vicodepy/command.py
+-rw-r--r--   0        0        0      202 2024-06-01 10:38:44.000000 vicodepy-0.4.2/vicodepy/config/config.yml
+-rw-r--r--   0        0        0       43 2024-06-01 10:38:44.000000 vicodepy-0.4.2/vicodepy/style.qss
+-rw-r--r--   0        0        0     3078 2024-06-01 10:38:44.000000 vicodepy-0.4.2/PKG-INFO
```

### Comparing `vicodepy-0.4.1/CHANGELOG.md` & `vicodepy-0.4.2/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGELOG
 =========
 
+0.4.2 - 2024-06-01
+------------------
+
+* The program accepts now command line arguments
+* Annotation labels can be chosen directly using the keyboard, once the annotation dialog is displayed
+
 0.4.1 - 2024-05-31
 ------------------
 
 * All supported video file formats can now be loaded
 * Annotation handles can now be clicked/dragged with the mouse
 * Improved color contrast of annotation labels
```

### Comparing `vicodepy-0.4.1/LICENSE` & `vicodepy-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vicodepy-0.4.1/README.md` & `vicodepy-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `vicodepy-0.4.1/pyproject.toml` & `vicodepy-0.4.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [project]
 name = "vicodepy"
-version = "0.4.1"
+version = "0.4.2"
 description = "Video coder for psychological experiments"
 authors = [
     { name = "Rafael Laboissière", email = "rafael.laboissiere@cnrs.fr" },
     { name = "Esteban Milleret", email = "esteban.milleret@etu.univ-grenoble-alpes.fr" },
 ]
 dependencies = [
     "PySide6==6.7.1",
     "numpy>=1.26.4",
     "pyyaml>=6.0.1",
     "colour>=0.1.5",
+    "docopt>=0.6.2",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "GPL-3.0-or-later"
```

### Comparing `vicodepy-0.4.1/vicodepy/__init__.py` & `vicodepy-0.4.2/vicodepy/__init__.py`

 * *Files identical despite different names*

### Comparing `vicodepy-0.4.1/vicodepy/__main__.py` & `vicodepy-0.4.2/vicodepy/__main__.py`

 * *Files identical despite different names*

### Comparing `vicodepy-0.4.1/vicodepy/app.py` & `vicodepy-0.4.2/vicodepy/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,14 @@
     QSlider,
     QStyle,
     QVBoxLayout,
     QWidget,
     QLabel,
     QDialog,
     QLineEdit,
-    QRadioButton,
     QColorDialog,
     QComboBox,
     QGraphicsScene,
     QGraphicsView,
     QGraphicsRectItem,
     QGraphicsItem,
     QMenu,
@@ -392,26 +391,27 @@
     def stop(self):
         """Stop player"""
         self.mediaplayer.stop()
         self.playbutton.setIcon(
             self.style().standardIcon(QStyle.StandardPixmap.SP_MediaPlay)
         )
 
-    def open_file(self):
+    def open_file(self, filename=None):
         """Open a media file in a MediaPlayer"""
 
-        dialog_txt = "Open Video File"
-        file_dialog = QFileDialog(self)
-        file_dialog.setWindowTitle(dialog_txt)
-        file_dialog.setNameFilters(self.file_name_filters)
-        file_dialog.exec()
-        # Load only the first of the selected file
-        filename = file_dialog.selectedFiles()[0]
         if not filename:
-            return
+            dialog_txt = "Open Video File"
+            file_dialog = QFileDialog(self)
+            file_dialog.setWindowTitle(dialog_txt)
+            file_dialog.setNameFilters(self.file_name_filters)
+            file_dialog.exec()
+            # Load only the first of the selected file
+            filename = file_dialog.selectedFiles()[0]
+            if not filename:
+                return
 
         # getOpenFileName returns a tuple, so use only the actual file name
         self.media = QUrl.fromLocalFile(filename)
 
         # Enable the buttons
         self.playbutton.setEnabled(True)
         self.stopbutton.setEnabled(True)
@@ -731,29 +731,29 @@
             self.scene.addItem(self.currentAnnotation)
         else:
             # End the current annotation
             agd = AnnotationGroupDialog(self)
             agd.exec()
 
             if agd.result() == AnnotationDialogCode.Accepted:
-                if agd.radio_button_2.isChecked():
+                if agd.state == "create":
                     # When creating a new group, create the group and add the
                     # current annotation to it
                     group = AnnotationGroup(
                         len(self.groups) + 1,
                         agd.group_name_text.text(),
                         agd.color,
                         self,
                     )
                     group.add_annotation(self.currentAnnotation)
                     self.add_group(group)
                 else:
                     # Otherwise, we are selecting an existing group, and will
                     # retrieve the group and add the annotation to it
-                    group = agd.combo_box_1.currentData()
+                    group = agd.combo_box.currentData()
                     group.add_annotation(self.currentAnnotation)
                 self.currentAnnotation.finish_create()
                 self.add_annotation(self.currentAnnotation)
                 self.currentAnnotation = None
             elif agd.result() == AnnotationDialogCode.Aborted:
                 self.currentAnnotation.remove()
             self.update()
@@ -1196,92 +1196,89 @@
     """Dialog to select or create a new annotation group"""
 
     def __init__(self, timeline: TimeLineWidget = None):
         super().__init__(timeline)
         self.setWindowTitle("New annotation")
 
         self.color = self.DEFAULT_COLOR
-        self.combo_box_1 = QComboBox()
+        self.combo_box = QComboBox()
         for group in timeline.groups:
-            self.combo_box_1.addItem(group.name, group)
+            self.combo_box.addItem(group.name, group)
+        self.combo_box.setEditable(True)
 
-        self.label_2 = QLabel("Group's name")
+        self.label_2 = QLabel("New label")
         self.group_name_text = QLineEdit()
 
         self.button_color_2 = QPushButton("Color")
         self.button_color_2.clicked.connect(self.on_button_color_2_clicked)
 
         self.cancel_button = QPushButton("Cancel")
         self.cancel_button.clicked.connect(self.reject)
 
         self.abort_button = QPushButton("Abort")
         self.abort_button.clicked.connect(self.abort)
 
         self.save_button = QPushButton("Save")
         self.save_button.clicked.connect(self.accept)
 
-        # Create radio buttons
-        self.radio_button_1 = QRadioButton("Select existing group")
-        self.radio_button_1.toggled.connect(self.on_radio_button_1_toggled)
-
-        self.radio_button_2 = QRadioButton("Create new group")
-        self.radio_button_2.toggled.connect(self.on_radio_button_2_toggled)
-
         # Create layout for contents
         layout = QHBoxLayout()
-        layout.addWidget(self.combo_box_1)
+        layout.addWidget(self.combo_box)
         layout.addWidget(self.label_2)
         layout.addWidget(self.group_name_text)
         layout.addWidget(self.button_color_2)
 
-        # Create layout for radio buttons
-        radio_button_layout = QHBoxLayout()
-        radio_button_layout.addWidget(self.radio_button_1)
-        radio_button_layout.addWidget(self.radio_button_2)
-
         # Create layout for main buttons
         main_button_layout = QHBoxLayout()
         main_button_layout.addWidget(self.cancel_button)
         main_button_layout.addWidget(self.abort_button)
         main_button_layout.addWidget(self.save_button)
 
         main_layout = QVBoxLayout()
-        main_layout.addLayout(radio_button_layout)
         main_layout.addLayout(layout)
         main_layout.addLayout(main_button_layout)
 
         self.setLayout(main_layout)
 
         if timeline.groups:
-            self.radio_button_1.setChecked(True)
+            self.state = "choose"
         else:
-            self.radio_button_1.setDisabled(True)
-            self.radio_button_2.setChecked(True)
+            self.state = "create"
+
+        self.set_visibility()
+
+    def accept(self):
+        if self.combo_box.currentData() or self.state == "create":
+            super().accept()
+        else:
+            self.state = "create"
+            self.group_name_text.setText(self.combo_box.currentText())
+            self.set_visibility()
+            self.group_name_text.setFocus()
 
     def abort(self):
         confirm_box = AnnotationConfirmMessageBox(self)
         if confirm_box.result() == QMessageBox.DialogCode.Accepted:
             self.done(AnnotationDialogCode.Aborted)
 
     def on_button_color_2_clicked(self):
         self.color = QColorDialog.getColor()
 
-    def on_radio_button_1_toggled(self, checked):
-        if checked:
-            self.combo_box_1.setVisible(True)
+    def set_visibility(self):
+        if self.state == "choose":
+            self.combo_box.setVisible(True)
             self.label_2.setVisible(False)
             self.group_name_text.setVisible(False)
             self.button_color_2.setVisible(False)
-
-    def on_radio_button_2_toggled(self, checked):
-        if checked:
-            self.combo_box_1.setVisible(False)
+        else:
+            self.combo_box.setVisible(False)
             self.label_2.setVisible(True)
             self.group_name_text.setVisible(True)
             self.button_color_2.setVisible(True)
+        self.save_button.setDefault(True)
 
 
 class AnnotationConfirmMessageBox(QMessageBox):
     def __init__(self, parent=None):
         super().__init__(
             QMessageBox.Icon.Warning,
             "Warning",
```

### Comparing `vicodepy-0.4.1/PKG-INFO` & `vicodepy-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vicodepy
-Version: 0.4.1
+Version: 0.4.2
 Summary: Video coder for psychological experiments
 License: GPL-3.0-or-later
 Author-email: Rafael Laboissière <rafael.laboissiere@cnrs.fr>,Esteban Milleret <esteban.milleret@etu.univ-grenoble-alpes.fr>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # ViCodePy – Video coder in Python for Experimental Psychology
```

