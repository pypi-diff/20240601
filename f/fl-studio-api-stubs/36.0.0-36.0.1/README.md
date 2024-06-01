# Comparing `tmp/fl_studio_api_stubs-36.0.0.tar.gz` & `tmp/fl_studio_api_stubs-36.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fl_studio_api_stubs-36.0.0.tar", max compression
+gzip compressed data, was "fl_studio_api_stubs-36.0.1.tar", max compression
```

## Comparing `fl_studio_api_stubs-36.0.0.tar` & `fl_studio_api_stubs-36.0.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     7642 2024-05-28 10:53:31.153757 fl_studio_api_stubs-36.0.0/LICENSE.md
--rw-r--r--   0        0        0     3962 2024-05-28 13:46:50.769735 fl_studio_api_stubs-36.0.0/README.md
--rw-r--r--   0        0        0     3893 2024-05-28 14:06:25.260400 fl_studio_api_stubs-36.0.0/pyproject.toml
--rw-r--r--   0        0        0     5514 1970-01-01 00:00:00.000000 fl_studio_api_stubs-36.0.0/PKG-INFO
+-rw-r--r--   0        0        0     7799 2024-04-08 03:54:11.613974 fl_studio_api_stubs-36.0.1/LICENSE.md
+-rw-r--r--   0        0        0     4012 2024-06-01 11:35:13.430472 fl_studio_api_stubs-36.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4060 2024-06-01 11:33:40.195360 fl_studio_api_stubs-36.0.1/README.md
+-rw-r--r--   0        0        0     5514 1970-01-01 00:00:00.000000 fl_studio_api_stubs-36.0.1/PKG-INFO
```

### Comparing `fl_studio_api_stubs-36.0.0/LICENSE.md` & `fl_studio_api_stubs-36.0.1/LICENSE.md`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-### GNU LESSER GENERAL PUBLIC LICENSE
-
-Version 3, 29 June 2007
-
-Copyright (C) 2007 Free Software Foundation, Inc.
-<https://fsf.org/>
-
-Everyone is permitted to copy and distribute verbatim copies of this
-license document, but changing it is not allowed.
-
-This version of the GNU Lesser General Public License incorporates the
-terms and conditions of version 3 of the GNU General Public License,
-supplemented by the additional permissions listed below.
-
-#### 0. Additional Definitions.
-
-As used herein, "this License" refers to version 3 of the GNU Lesser
-General Public License, and the "GNU GPL" refers to version 3 of the
-GNU General Public License.
-
-"The Library" refers to a covered work governed by this License, other
-than an Application or a Combined Work as defined below.
-
-An "Application" is any work that makes use of an interface provided
-by the Library, but which is not otherwise based on the Library.
-Defining a subclass of a class defined by the Library is deemed a mode
-of using an interface provided by the Library.
-
-A "Combined Work" is a work produced by combining or linking an
-Application with the Library. The particular version of the Library
-with which the Combined Work was made is also called the "Linked
-Version".
-
-The "Minimal Corresponding Source" for a Combined Work means the
-Corresponding Source for the Combined Work, excluding any source code
-for portions of the Combined Work that, considered in isolation, are
-based on the Application, and not on the Linked Version.
-
-The "Corresponding Application Code" for a Combined Work means the
-object code and/or source code for the Application, including any data
-and utility programs needed for reproducing the Combined Work from the
-Application, but excluding the System Libraries of the Combined Work.
-
-#### 1. Exception to Section 3 of the GNU GPL.
-
-You may convey a covered work under sections 3 and 4 of this License
-without being bound by section 3 of the GNU GPL.
-
-#### 2. Conveying Modified Versions.
-
-If you modify a copy of the Library, and, in your modifications, a
-facility refers to a function or data to be supplied by an Application
-that uses the facility (other than as an argument passed when the
-facility is invoked), then you may convey a copy of the modified
-version:
-
--   a) under this License, provided that you make a good faith effort
-    to ensure that, in the event an Application does not supply the
-    function or data, the facility still operates, and performs
-    whatever part of its purpose remains meaningful, or
--   b) under the GNU GPL, with none of the additional permissions of
-    this License applicable to that copy.
-
-#### 3. Object Code Incorporating Material from Library Header Files.
-
-The object code form of an Application may incorporate material from a
-header file that is part of the Library. You may convey such object
-code under terms of your choice, provided that, if the incorporated
-material is not limited to numerical parameters, data structure
-layouts and accessors, or small macros, inline functions and templates
-(ten or fewer lines in length), you do both of the following:
-
--   a) Give prominent notice with each copy of the object code that
-    the Library is used in it and that the Library and its use are
-    covered by this License.
--   b) Accompany the object code with a copy of the GNU GPL and this
-    license document.
-
-#### 4. Combined Works.
-
-You may convey a Combined Work under terms of your choice that, taken
-together, effectively do not restrict modification of the portions of
-the Library contained in the Combined Work and reverse engineering for
-debugging such modifications, if you also do each of the following:
-
--   a) Give prominent notice with each copy of the Combined Work that
-    the Library is used in it and that the Library and its use are
-    covered by this License.
--   b) Accompany the Combined Work with a copy of the GNU GPL and this
-    license document.
--   c) For a Combined Work that displays copyright notices during
-    execution, include the copyright notice for the Library among
-    these notices, as well as a reference directing the user to the
-    copies of the GNU GPL and this license document.
--   d) Do one of the following:
-    -   0) Convey the Minimal Corresponding Source under the terms of
-        this License, and the Corresponding Application Code in a form
-        suitable for, and under terms that permit, the user to
-        recombine or relink the Application with a modified version of
-        the Linked Version to produce a modified Combined Work, in the
-        manner specified by section 6 of the GNU GPL for conveying
-        Corresponding Source.
-    -   1) Use a suitable shared library mechanism for linking with
-        the Library. A suitable mechanism is one that (a) uses at run
-        time a copy of the Library already present on the user's
-        computer system, and (b) will operate properly with a modified
-        version of the Library that is interface-compatible with the
-        Linked Version.
--   e) Provide Installation Information, but only if you would
-    otherwise be required to provide such information under section 6
-    of the GNU GPL, and only to the extent that such information is
-    necessary to install and execute a modified version of the
-    Combined Work produced by recombining or relinking the Application
-    with a modified version of the Linked Version. (If you use option
-    4d0, the Installation Information must accompany the Minimal
-    Corresponding Source and Corresponding Application Code. If you
-    use option 4d1, you must provide the Installation Information in
-    the manner specified by section 6 of the GNU GPL for conveying
-    Corresponding Source.)
-
-#### 5. Combined Libraries.
-
-You may place library facilities that are a work based on the Library
-side by side in a single library together with other library
-facilities that are not Applications and are not covered by this
-License, and convey such a combined library under terms of your
-choice, if you do both of the following:
-
--   a) Accompany the combined library with a copy of the same work
-    based on the Library, uncombined with any other library
-    facilities, conveyed under the terms of this License.
--   b) Give prominent notice with the combined library that part of it
-    is a work based on the Library, and explaining where to find the
-    accompanying uncombined form of the same work.
-
-#### 6. Revised Versions of the GNU Lesser General Public License.
-
-The Free Software Foundation may publish revised and/or new versions
-of the GNU Lesser General Public License from time to time. Such new
-versions will be similar in spirit to the present version, but may
-differ in detail to address new problems or concerns.
-
-Each version is given a distinguishing version number. If the Library
-as you received it specifies that a certain numbered version of the
-GNU Lesser General Public License "or any later version" applies to
-it, you have the option of following the terms and conditions either
-of that published version or of any later version published by the
-Free Software Foundation. If the Library as you received it does not
-specify a version number of the GNU Lesser General Public License, you
-may choose any version of the GNU Lesser General Public License ever
-published by the Free Software Foundation.
-
-If the Library as you received it specifies that a proxy can decide
-whether future versions of the GNU Lesser General Public License shall
-apply, that proxy's public statement of acceptance of any version is
-permanent authorization for you to choose that version for the
-Library.
+### GNU LESSER GENERAL PUBLIC LICENSE
+
+Version 3, 29 June 2007
+
+Copyright (C) 2007 Free Software Foundation, Inc.
+<https://fsf.org/>
+
+Everyone is permitted to copy and distribute verbatim copies of this
+license document, but changing it is not allowed.
+
+This version of the GNU Lesser General Public License incorporates the
+terms and conditions of version 3 of the GNU General Public License,
+supplemented by the additional permissions listed below.
+
+#### 0. Additional Definitions.
+
+As used herein, "this License" refers to version 3 of the GNU Lesser
+General Public License, and the "GNU GPL" refers to version 3 of the
+GNU General Public License.
+
+"The Library" refers to a covered work governed by this License, other
+than an Application or a Combined Work as defined below.
+
+An "Application" is any work that makes use of an interface provided
+by the Library, but which is not otherwise based on the Library.
+Defining a subclass of a class defined by the Library is deemed a mode
+of using an interface provided by the Library.
+
+A "Combined Work" is a work produced by combining or linking an
+Application with the Library. The particular version of the Library
+with which the Combined Work was made is also called the "Linked
+Version".
+
+The "Minimal Corresponding Source" for a Combined Work means the
+Corresponding Source for the Combined Work, excluding any source code
+for portions of the Combined Work that, considered in isolation, are
+based on the Application, and not on the Linked Version.
+
+The "Corresponding Application Code" for a Combined Work means the
+object code and/or source code for the Application, including any data
+and utility programs needed for reproducing the Combined Work from the
+Application, but excluding the System Libraries of the Combined Work.
+
+#### 1. Exception to Section 3 of the GNU GPL.
+
+You may convey a covered work under sections 3 and 4 of this License
+without being bound by section 3 of the GNU GPL.
+
+#### 2. Conveying Modified Versions.
+
+If you modify a copy of the Library, and, in your modifications, a
+facility refers to a function or data to be supplied by an Application
+that uses the facility (other than as an argument passed when the
+facility is invoked), then you may convey a copy of the modified
+version:
+
+-   a) under this License, provided that you make a good faith effort
+    to ensure that, in the event an Application does not supply the
+    function or data, the facility still operates, and performs
+    whatever part of its purpose remains meaningful, or
+-   b) under the GNU GPL, with none of the additional permissions of
+    this License applicable to that copy.
+
+#### 3. Object Code Incorporating Material from Library Header Files.
+
+The object code form of an Application may incorporate material from a
+header file that is part of the Library. You may convey such object
+code under terms of your choice, provided that, if the incorporated
+material is not limited to numerical parameters, data structure
+layouts and accessors, or small macros, inline functions and templates
+(ten or fewer lines in length), you do both of the following:
+
+-   a) Give prominent notice with each copy of the object code that
+    the Library is used in it and that the Library and its use are
+    covered by this License.
+-   b) Accompany the object code with a copy of the GNU GPL and this
+    license document.
+
+#### 4. Combined Works.
+
+You may convey a Combined Work under terms of your choice that, taken
+together, effectively do not restrict modification of the portions of
+the Library contained in the Combined Work and reverse engineering for
+debugging such modifications, if you also do each of the following:
+
+-   a) Give prominent notice with each copy of the Combined Work that
+    the Library is used in it and that the Library and its use are
+    covered by this License.
+-   b) Accompany the Combined Work with a copy of the GNU GPL and this
+    license document.
+-   c) For a Combined Work that displays copyright notices during
+    execution, include the copyright notice for the Library among
+    these notices, as well as a reference directing the user to the
+    copies of the GNU GPL and this license document.
+-   d) Do one of the following:
+    -   0) Convey the Minimal Corresponding Source under the terms of
+        this License, and the Corresponding Application Code in a form
+        suitable for, and under terms that permit, the user to
+        recombine or relink the Application with a modified version of
+        the Linked Version to produce a modified Combined Work, in the
+        manner specified by section 6 of the GNU GPL for conveying
+        Corresponding Source.
+    -   1) Use a suitable shared library mechanism for linking with
+        the Library. A suitable mechanism is one that (a) uses at run
+        time a copy of the Library already present on the user's
+        computer system, and (b) will operate properly with a modified
+        version of the Library that is interface-compatible with the
+        Linked Version.
+-   e) Provide Installation Information, but only if you would
+    otherwise be required to provide such information under section 6
+    of the GNU GPL, and only to the extent that such information is
+    necessary to install and execute a modified version of the
+    Combined Work produced by recombining or relinking the Application
+    with a modified version of the Linked Version. (If you use option
+    4d0, the Installation Information must accompany the Minimal
+    Corresponding Source and Corresponding Application Code. If you
+    use option 4d1, you must provide the Installation Information in
+    the manner specified by section 6 of the GNU GPL for conveying
+    Corresponding Source.)
+
+#### 5. Combined Libraries.
+
+You may place library facilities that are a work based on the Library
+side by side in a single library together with other library
+facilities that are not Applications and are not covered by this
+License, and convey such a combined library under terms of your
+choice, if you do both of the following:
+
+-   a) Accompany the combined library with a copy of the same work
+    based on the Library, uncombined with any other library
+    facilities, conveyed under the terms of this License.
+-   b) Give prominent notice with the combined library that part of it
+    is a work based on the Library, and explaining where to find the
+    accompanying uncombined form of the same work.
+
+#### 6. Revised Versions of the GNU Lesser General Public License.
+
+The Free Software Foundation may publish revised and/or new versions
+of the GNU Lesser General Public License from time to time. Such new
+versions will be similar in spirit to the present version, but may
+differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number. If the Library
+as you received it specifies that a certain numbered version of the
+GNU Lesser General Public License "or any later version" applies to
+it, you have the option of following the terms and conditions either
+of that published version or of any later version published by the
+Free Software Foundation. If the Library as you received it does not
+specify a version number of the GNU Lesser General Public License, you
+may choose any version of the GNU Lesser General Public License ever
+published by the Free Software Foundation.
+
+If the Library as you received it specifies that a proxy can decide
+whether future versions of the GNU Lesser General Public License shall
+apply, that proxy's public statement of acceptance of any version is
+permanent authorization for you to choose that version for the
+Library.
```

### Comparing `fl_studio_api_stubs-36.0.0/README.md` & `fl_studio_api_stubs-36.0.1/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-# ![FL Studio API Stubs](https://raw.githubusercontent.com/IL-Group/FL-Studio-API-Stubs/main/data/readme-header.png)
-
-This repository contains stub code for functions and classes used in FL
-Studio's Python API. This includes modules used for
-
-* [MIDI Controller Scripting](https://www.image-line.com/fl-studio-learning/fl-studio-beta-online-manual/html/midi_scripting.htm)
-* [Edison Audio Scripting](https://www.image-line.com/fl-studio-learning/fl-studio-beta-online-manual/html/pianoroll_scripting_api.htm)
-* [Piano Roll Scripting](https://www.image-line.com/fl-studio-learning/fl-studio-beta-online-manual/html/plugins/editortool_run.htm)
-
-## Usage
-
-This documentation can be [viewed online](https://il-group.github.io/FL-Studio-API-Stubs/),
-or accessed by installing the package from Python's package manager Pip.
-
-For instructions, please visit the documentation website.
-
-## Contributing
-
-We'd love to have your help maintaining this project.
-
-### Feature requests and bugs
-
-If you'd like to report a bug in FL Studio, or get new features added to FL
-Studio's Python API, please create a post on the Image-Line forum. The issues
-tab for this repository should only be used for reporting issues with the
-stub code.
-
-### Issues with the API
-
-If you've spotted an issue with the API documentation or stub code, please
-open an issue and we'll get it fixed up as soon as we can. In particular,
-we're on the look out for:
-
-* Incorrect type definitions
-* Missing functions or constants
-* Confusing, missing or poorly-formatted documentation
-
-### Setting up a development environment
-
-Dependencies for this project are managed using
-[Poetry](https://python-poetry.org/). You'll need to
-[install Poetry](https://python-poetry.org/docs/#installation) to contribute to
-the project.
-
-To install dependencies for the project:
-
-```sh
-# Install dependencies for the project
-poetry install --no-root
-# Run the pre-build script
-poetry run python -m scripts.build_lib
-# Install the library
-poetry install
-```
-
-Whenever you modify documentation, you will need to rerun the pre-build script
-for your changes to be persisted.
-
-### Developing the documentation site
-
-You can trigger a build of the documentation site by running:
-
-```sh
-poetry run python -m scripts.build_docs
-```
-
-If you are using the [VS Code](https://code.visualstudio.com/) text editor,
-we recommend using the [Live Server Extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
-to serve the documentation site, since it automatically refreshes the page
-whenever you run the build command. Additionally, VS Code will automatically
-run this build command when you press `Ctrl+Shift+B`.
-
-### Understanding the repository layout
-
-In order to ensure that the documentation is of the highest quality, both
-online and in library form, the layout is a little complex.
-
-* `src/` contains the source code for all included modules, divided up based on
-  whether they are a component of MIDI Controller Scripting, Edison Scripting,
-  or Piano Roll Scripting. Each Python file contains function definitions, with
-  [docstrings](https://peps.python.org/pep-0257/) showing their behaviour.
-
-* `docs/` contains Markdown files and other assets used when building the
-  online documentation. This is merged with the layout of `src/` when building
-  documentation, so the resultant site ends up containing the documentation
-  from both directories.
-
-    * `.pages` files within the `docs/` directory contain a YAML listing for
-      the navigation of this section of the documentation. They are used to
-      re-order and rename elements within the navigation pane of the
-      documentation site.
-
-* `scripts/` contains Python scripts for performing common actions such as
-  building the documentation or building the package.
-
-* `data/` contains other assets used by the repository, such as
-  [Transdoc](https://github.com/MiguelGuthridge/transdoc) rule definitions, and
-  docstring templates.
+# ![FL Studio API Stubs](https://raw.githubusercontent.com/IL-Group/FL-Studio-API-Stubs/main/data/readme-header.png)
+
+This repository contains stub code for functions and classes used in FL
+Studio's Python API. This includes modules used for
+
+* [MIDI Controller Scripting](https://www.image-line.com/fl-studio-learning/fl-studio-beta-online-manual/html/midi_scripting.htm)
+* [Edison Audio Scripting](https://www.image-line.com/fl-studio-learning/fl-studio-beta-online-manual/html/pianoroll_scripting_api.htm)
+* [Piano Roll Scripting](https://www.image-line.com/fl-studio-learning/fl-studio-beta-online-manual/html/plugins/editortool_run.htm)
+
+## Usage
+
+This documentation can be [viewed online](https://il-group.github.io/FL-Studio-API-Stubs/),
+or accessed by installing the package from Python's package manager Pip.
+
+For instructions, please visit the documentation website.
+
+## Contributing
+
+We'd love to have your help maintaining this project.
+
+### Feature requests and bugs
+
+If you'd like to report a bug in FL Studio, or get new features added to FL
+Studio's Python API, please create a post on the Image-Line forum. The issues
+tab for this repository should only be used for reporting issues with the
+stub code.
+
+### Issues with the API
+
+If you've spotted an issue with the API documentation or stub code, please
+open an issue and we'll get it fixed up as soon as we can. In particular,
+we're on the look out for:
+
+* Incorrect type definitions
+* Missing functions or constants
+* Confusing, missing or poorly-formatted documentation
+
+### Setting up a development environment
+
+Dependencies for this project are managed using
+[Poetry](https://python-poetry.org/). You'll need to
+[install Poetry](https://python-poetry.org/docs/#installation) to contribute to
+the project.
+
+To install dependencies for the project:
+
+```sh
+# Install dependencies for the project
+poetry install --no-root
+# Run the pre-build script
+poetry run python -m scripts.build_lib
+# Install the library
+poetry install
+```
+
+Whenever you modify documentation, you will need to rerun the pre-build script
+for your changes to be persisted.
+
+### Developing the documentation site
+
+You can trigger a build of the documentation site by running:
+
+```sh
+poetry run python -m scripts.build_docs
+```
+
+If you are using the [VS Code](https://code.visualstudio.com/) text editor,
+we recommend using the [Live Server Extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
+to serve the documentation site, since it automatically refreshes the page
+whenever you run the build command. Additionally, VS Code will automatically
+run this build command when you press `Ctrl+Shift+B`.
+
+### Understanding the repository layout
+
+In order to ensure that the documentation is of the highest quality, both
+online and in library form, the layout is a little complex.
+
+* `src/` contains the source code for all included modules, divided up based on
+  whether they are a component of MIDI Controller Scripting, Edison Scripting,
+  or Piano Roll Scripting. Each Python file contains function definitions, with
+  [docstrings](https://peps.python.org/pep-0257/) showing their behaviour.
+
+* `docs/` contains Markdown files and other assets used when building the
+  online documentation. This is merged with the layout of `src/` when building
+  documentation, so the resultant site ends up containing the documentation
+  from both directories.
+
+    * `.pages` files within the `docs/` directory contain a YAML listing for
+      the navigation of this section of the documentation. They are used to
+      re-order and rename elements within the navigation pane of the
+      documentation site.
+
+* `scripts/` contains Python scripts for performing common actions such as
+  building the documentation or building the package.
+
+* `data/` contains other assets used by the repository, such as
+  [Transdoc](https://github.com/MiguelGuthridge/transdoc) rule definitions, and
+  docstring templates.
```

### Comparing `fl_studio_api_stubs-36.0.0/pyproject.toml` & `fl_studio_api_stubs-36.0.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-[tool.poetry]
-name = "fl-studio-api-stubs"
-version = "36.0.0"
-
-description = "Stub code, type definitions and documentation for the FL Studio Python API"
-readme = "README.md"
-
-authors = ["Miguel Guthridge <hello@miguelguthridge.com>"]
-license = "LGPL-3.0-only"
-
-repository = "https://github.com/IL-Group/FL-Studio-Api-Stubs/issues"
-documentation = "https://il-group.github.io/FL-Studio-API-Stubs/"
-
-keywords = [
-    "fl-studio",
-    "midi",
-    "api",
-    "documentation",
-    "stubs",
-    "fl",
-    "studio",
-    "daw",
-    "controller",
-    "image-line",
-]
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
-    "Operating System :: OS Independent",
-    "Development Status :: 5 - Production/Stable",
-    "Environment :: Other Environment",
-    "Topic :: Software Development :: Documentation",
-    "Topic :: Software Development :: Libraries :: Application Frameworks",
-    "Typing :: Typed",
-    "Typing :: Stubs Only",
-]
-include = ["py.typed"]
-
-packages = [
-    # MIDI controller scripting
-    { include = "arrangement", from = "build_lib/midi_controller_scripting" },
-    { include = "channels", from = "build_lib/midi_controller_scripting" },
-    { include = "device", from = "build_lib/midi_controller_scripting" },
-    { include = "general", from = "build_lib/midi_controller_scripting" },
-    { include = "launchMapPages", from = "build_lib/midi_controller_scripting" },
-    { include = "mixer", from = "build_lib/midi_controller_scripting" },
-    { include = "patterns", from = "build_lib/midi_controller_scripting" },
-    { include = "playlist", from = "build_lib/midi_controller_scripting" },
-    { include = "plugins", from = "build_lib/midi_controller_scripting" },
-    { include = "screen", from = "build_lib/midi_controller_scripting" },
-    { include = "transport", from = "build_lib/midi_controller_scripting" },
-    { include = "ui", from = "build_lib/midi_controller_scripting" },
-    # MIDI controller scripting extra libraries
-    { include = "midi", from = "build_lib/midi_controller_scripting" },
-    { include = "utils", from = "build_lib/midi_controller_scripting" },
-    # API stubs extra modules
-    { include = "fl_classes", from = "build_lib/midi_controller_scripting" },
-    # Edison scripting
-    { include = "enveditor", from = "build_lib/edison_scripting" },
-    # Piano roll scripting
-    { include = "flpianoroll", from = "build_lib/piano_roll_scripting" },
-]
-
-[tool.poetry.urls]
-"Bug Tracker" = "https://github.com/IL-Group/FL-Studio-Api-Stubs/issues"
-"Online Documentation" = "https://il-group.github.io/FL-Studio-API-Stubs/"
-
-
-[tool.poetry.dependencies]
-# Primary dependencies
-python = "^3.10"
-
-[tool.poetry.group.build.dependencies]
-# Build dependencies -- required to build the library
-transdoc = "^0.2.2"
-griffe = "^0.45.2"
-
-[tool.poetry.group.docs.dependencies]
-# Docs depdnencies -- required to build documentation site
-# Note build dependencies are also required
-mkdocs = "^1.4.2"
-mkdocs-gen-files = "^0.5.0"
-mkdocs-material = "^9.5.0"
-mkdocstrings = { version = ">=0.24,<0.26", extras = ["python"] }
-mkdocs-awesome-pages-plugin = "^2.9.2"
-mkdocs-section-index = "^0.3.8"
-
-[tool.poetry.group.ci.dependencies]
-# CI dependencies -- required to run continuous integration, including
-# linting, type checking, etc
-coverage = "^7.2.2"
-autopep8 = "^2.0.2"
-mypy = "^1.1.1"
-typing-extensions = "^4.5.0"
-flake8 = "^7.0.0"
-flake8-pyproject = "^1.2.3"
-pytest = ">=7.2.2,<9.0.0"
-flapi = "^1.0.1"
-
-[tool.flake8]
-exclude = [
-    '.git',
-    '__pycache__',
-    'old',
-    'build',
-    'dist',
-    'prebuild_docs',
-    'build_lib',
-]
-ignore = ['E501', 'W503']
-
-[tool.mypy]
-check_untyped_defs = true
-files = ["src", "scripts", "data"]
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "fl-studio-api-stubs"
+version = "36.0.1"
+
+description = "Stub code, type definitions and documentation for the FL Studio Python API"
+readme = "README.md"
+
+authors = ["Miguel Guthridge <hello@miguelguthridge.com>"]
+license = "LGPL-3.0-only"
+
+repository = "https://github.com/IL-Group/FL-Studio-Api-Stubs/issues"
+documentation = "https://il-group.github.io/FL-Studio-API-Stubs/"
+
+keywords = [
+    "fl-studio",
+    "midi",
+    "api",
+    "documentation",
+    "stubs",
+    "fl",
+    "studio",
+    "daw",
+    "controller",
+    "image-line",
+]
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
+    "Operating System :: OS Independent",
+    "Development Status :: 5 - Production/Stable",
+    "Environment :: Other Environment",
+    "Topic :: Software Development :: Documentation",
+    "Topic :: Software Development :: Libraries :: Application Frameworks",
+    "Typing :: Typed",
+    "Typing :: Stubs Only",
+]
+include = ["py.typed"]
+
+packages = [
+    # MIDI controller scripting
+    { include = "arrangement", from = "build_lib/midi_controller_scripting" },
+    { include = "channels", from = "build_lib/midi_controller_scripting" },
+    { include = "device", from = "build_lib/midi_controller_scripting" },
+    { include = "general", from = "build_lib/midi_controller_scripting" },
+    { include = "launchMapPages", from = "build_lib/midi_controller_scripting" },
+    { include = "mixer", from = "build_lib/midi_controller_scripting" },
+    { include = "patterns", from = "build_lib/midi_controller_scripting" },
+    { include = "playlist", from = "build_lib/midi_controller_scripting" },
+    { include = "plugins", from = "build_lib/midi_controller_scripting" },
+    { include = "screen", from = "build_lib/midi_controller_scripting" },
+    { include = "transport", from = "build_lib/midi_controller_scripting" },
+    { include = "ui", from = "build_lib/midi_controller_scripting" },
+    # MIDI controller scripting extra libraries
+    { include = "midi", from = "build_lib/midi_controller_scripting" },
+    { include = "utils", from = "build_lib/midi_controller_scripting" },
+    # API stubs extra modules
+    { include = "fl_classes", from = "build_lib/midi_controller_scripting" },
+    # Edison scripting
+    { include = "enveditor", from = "build_lib/edison_scripting" },
+    # Piano roll scripting
+    { include = "flpianoroll", from = "build_lib/piano_roll_scripting" },
+]
+
+[tool.poetry.urls]
+"Bug Tracker" = "https://github.com/IL-Group/FL-Studio-Api-Stubs/issues"
+"Online Documentation" = "https://il-group.github.io/FL-Studio-API-Stubs/"
+
+
+[tool.poetry.dependencies]
+# Primary dependencies
+python = "^3.10"
+
+[tool.poetry.group.build.dependencies]
+# Build dependencies -- required to build the library
+transdoc = "^0.2.2"
+griffe = "^0.45.2"
+
+[tool.poetry.group.docs.dependencies]
+# Docs depdnencies -- required to build documentation site
+# Note build dependencies are also required
+mkdocs = "^1.4.2"
+mkdocs-gen-files = "^0.5.0"
+mkdocs-material = "^9.5.0"
+mkdocstrings = { version = ">=0.24,<0.26", extras = ["python"] }
+mkdocs-awesome-pages-plugin = "^2.9.2"
+mkdocs-section-index = "^0.3.8"
+
+[tool.poetry.group.ci.dependencies]
+# CI dependencies -- required to run continuous integration, including
+# linting, type checking, etc
+coverage = "^7.2.2"
+autopep8 = "^2.0.2"
+mypy = "^1.1.1"
+typing-extensions = "^4.5.0"
+flake8 = "^7.0.0"
+flake8-pyproject = "^1.2.3"
+pytest = ">=7.2.2,<9.0.0"
+flapi = "^1.0.1"
+
+[tool.flake8]
+exclude = [
+    '.git',
+    '__pycache__',
+    'old',
+    'build',
+    'dist',
+    'prebuild_docs',
+    'build_lib',
+]
+ignore = ['E501', 'W503']
+
+[tool.mypy]
+check_untyped_defs = true
+files = ["src", "scripts", "data"]
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `fl_studio_api_stubs-36.0.0/PKG-INFO` & `fl_studio_api_stubs-36.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fl-studio-api-stubs
-Version: 36.0.0
+Version: 36.0.1
 Summary: Stub code, type definitions and documentation for the FL Studio Python API
 Home-page: https://github.com/IL-Group/FL-Studio-Api-Stubs/issues
 License: LGPL-3.0-only
 Keywords: fl-studio,midi,api,documentation,stubs,fl,studio,daw,controller,image-line
 Author: Miguel Guthridge
 Author-email: hello@miguelguthridge.com
 Requires-Python: >=3.10,<4.0
```

