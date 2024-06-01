# Comparing `tmp/rose_pine_jupyterlab-0.1.7.tar.gz` & `tmp/rose_pine_jupyterlab-0.1.8.tar.gz`

## Comparing `rose_pine_jupyterlab-0.1.7.tar` & `rose_pine_jupyterlab-0.1.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/.copier-answers.yml
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/.yarnrc.yml
--rw-r--r--   0        0        0     4346 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/CHANGELOG.md
--rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/contributing.md
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/install.json
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/license
--rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/package.json
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/release.md
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/setup.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/tsconfig.json
--rw-r--r--   0        0        0   192922 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/yarn.lock
--rw-r--r--   0        0        0   117749 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/assets/rose-pine-dawn.png
--rw-r--r--   0        0        0   116576 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/assets/rose-pine-moon.png
--rw-r--r--   0        0        0   118302 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/assets/rose-pine.png
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/examples/example_notebook.ipynb
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/rose_pine_jupyterlab/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/rose_pine_jupyterlab/_version.py
--rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/rose_pine_jupyterlab/labextension/package.json
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/rose_pine_jupyterlab/labextension/static/517.da5b8c1b3fb547fc39bf.js
--rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/rose_pine_jupyterlab/labextension/static/remoteEntry.5d1fbf454e382a908af0.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/rose_pine_jupyterlab/labextension/static/style.js
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/rose_pine_jupyterlab/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    15556 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/rose_pine_jupyterlab/labextension/themes/rose_pine_jupyterlab/index.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/rose_pine_jupyterlab/labextension/themes/rose_pine_jupyterlab/index.js
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/src/index.ts
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/src/pallettes.d.ts
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/src/pallettes.ts
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/src/rose-pine-dawn.json
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/src/rose-pine-moon.json
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/src/rose-pine.json
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/src/templates.json
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/style/index.css
--rw-r--r--   0        0        0    15344 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/style/variables.css
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/.gitignore
--rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/readme.md
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/.copier-answers.yml
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/.yarnrc.yml
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/CHANGELOG.md
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/contributing.md
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/install.json
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/license
+-rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/package.json
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/release.md
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/setup.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/tsconfig.json
+-rw-r--r--   0        0        0   192922 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/yarn.lock
+-rw-r--r--   0        0        0   117749 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/assets/rose-pine-dawn.png
+-rw-r--r--   0        0        0   116576 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/assets/rose-pine-moon.png
+-rw-r--r--   0        0        0   118302 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/assets/rose-pine.png
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/examples/example_notebook.ipynb
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/rose_pine_jupyterlab/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/rose_pine_jupyterlab/_version.py
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/rose_pine_jupyterlab/labextension/package.json
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/rose_pine_jupyterlab/labextension/static/517.da5b8c1b3fb547fc39bf.js
+-rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/rose_pine_jupyterlab/labextension/static/remoteEntry.47afcc44ef7f4597528a.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/rose_pine_jupyterlab/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/rose_pine_jupyterlab/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    15985 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/rose_pine_jupyterlab/labextension/themes/rose_pine_jupyterlab/index.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/rose_pine_jupyterlab/labextension/themes/rose_pine_jupyterlab/index.js
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/src/index.ts
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/src/pallettes.d.ts
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/src/pallettes.ts
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/src/rose-pine-dawn.json
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/src/rose-pine-moon.json
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/src/rose-pine.json
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/src/templates.json
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/style/index.css
+-rwxr-xr-x   0        0        0    15773 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/style/variables.css
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/.gitignore
+-rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/readme.md
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 rose_pine_jupyterlab-0.1.8/PKG-INFO
```

### Comparing `rose_pine_jupyterlab-0.1.7/.pre-commit-config.yaml` & `rose_pine_jupyterlab-0.1.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.7/CHANGELOG.md` & `rose_pine_jupyterlab-0.1.8/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,45 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.1.8
+
+([Full Changelog](https://github.com/aaravind100/jupyterlab/compare/v0.1.7...670f49ce630ebd215c4822437e1fa2c809a07c1d))
+
+### Bugs fixed
+
+- improve menu test color and visibility [#12](https://github.com/aaravind100/jupyterlab/pull/12) ([@aaravind100](https://github.com/aaravind100))
+
+### Documentation improvements
+
+- docs: :memo: update contributing [#11](https://github.com/aaravind100/jupyterlab/pull/11) ([@aaravind100](https://github.com/aaravind100))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/aaravind100/jupyterlab/graphs/contributors?from=2024-05-28&to=2024-06-01&type=c))
+
+[@aaravind100](https://github.com/search?q=repo%3Aaaravind100%2Fjupyterlab+involves%3Aaaravind100+updated%3A2024-05-28..2024-06-01&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.1.7
 
 ([Full Changelog](https://github.com/aaravind100/jupyterlab/compare/v0.1.6...0a32b0bed802d97d0b34f90d856c759eaecfb4d2))
 
 ### Maintenance and upkeep improvements
 
 - Revert "fix: :bug: secret var name" [#10](https://github.com/aaravind100/jupyterlab/pull/10) ([@aaravind100](https://github.com/aaravind100))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/aaravind100/jupyterlab/graphs/contributors?from=2024-05-28&to=2024-05-28&type=c))
 
 [@aaravind100](https://github.com/search?q=repo%3Aaaravind100%2Fjupyterlab+involves%3Aaaravind100+updated%3A2024-05-28..2024-05-28&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.1.6
 
 ([Full Changelog](https://github.com/aaravind100/jupyterlab/compare/v0.1.5...d4e82be3baf220cb46ea2522ef5ca50d7cc94b62))
 
 ### Maintenance and upkeep improvements
 
 - fix: :bug: secret var name [#9](https://github.com/aaravind100/jupyterlab/pull/9) ([@aaravind100](https://github.com/aaravind100))
```

### Comparing `rose_pine_jupyterlab-0.1.7/contributing.md` & `rose_pine_jupyterlab-0.1.8/contributing.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 > Prefer using [@rose-pine/build](https://github.com/rose-pine/build) when possible
 
 This is used to generate color variant from the template file.
 
 Modify `style/variables.css` & `src/template.json` using Rosé Pine variables, then build variants:
 
 ```sh
-npx @rose-pine/build@latest -t src/templates.ts -o src/
+npx @rose-pine/build@latest -t src/templates.json -o src/
 ```
 
 ## Development install
 
 Note: You will need NodeJS to build the extension package.
 
 The `jlpm` command is JupyterLab's pinned version of
```

### Comparing `rose_pine_jupyterlab-0.1.7/license` & `rose_pine_jupyterlab-0.1.8/license`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.7/package.json` & `rose_pine_jupyterlab-0.1.8/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.1.8'"}*

```diff
@@ -180,9 +180,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.7"
+    "version": "0.1.8"
 }
```

### Comparing `rose_pine_jupyterlab-0.1.7/release.md` & `rose_pine_jupyterlab-0.1.8/release.md`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.7/tsconfig.json` & `rose_pine_jupyterlab-0.1.8/tsconfig.json`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.7/yarn.lock` & `rose_pine_jupyterlab-0.1.8/yarn.lock`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.7/assets/rose-pine-dawn.png` & `rose_pine_jupyterlab-0.1.8/assets/rose-pine-dawn.png`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.7/assets/rose-pine-moon.png` & `rose_pine_jupyterlab-0.1.8/assets/rose-pine-moon.png`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.7/assets/rose-pine.png` & `rose_pine_jupyterlab-0.1.8/assets/rose-pine.png`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.7/examples/example_notebook.ipynb` & `rose_pine_jupyterlab-0.1.8/examples/example_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.7/rose_pine_jupyterlab/__init__.py` & `rose_pine_jupyterlab-0.1.8/rose_pine_jupyterlab/__init__.py`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.7/rose_pine_jupyterlab/labextension/package.json` & `rose_pine_jupyterlab-0.1.8/rose_pine_jupyterlab/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9765625%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.47afcc44ef7f4597528a.js'}}",*

 * * "'version'": "'0.1.8'"}*

```diff
@@ -100,15 +100,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "src/**/*.{ts,tsx}"
     ],
     "homepage": "https://github.com/aaravind100/jupyterlab",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.5d1fbf454e382a908af0.js"
+            "load": "static/remoteEntry.47afcc44ef7f4597528a.js"
         },
         "extension": true,
         "outputDir": "rose_pine_jupyterlab/labextension",
         "themePath": "style/index.css"
     },
     "keywords": [
         "jupyter",
@@ -184,9 +184,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.7"
+    "version": "0.1.8"
 }
```

### Comparing `rose_pine_jupyterlab-0.1.7/rose_pine_jupyterlab/labextension/static/517.da5b8c1b3fb547fc39bf.js` & `rose_pine_jupyterlab-0.1.8/rose_pine_jupyterlab/labextension/static/517.da5b8c1b3fb547fc39bf.js`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.7/rose_pine_jupyterlab/labextension/static/remoteEntry.5d1fbf454e382a908af0.js` & `rose_pine_jupyterlab-0.1.8/rose_pine_jupyterlab/labextension/static/remoteEntry.47afcc44ef7f4597528a.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -93,15 +93,15 @@
                     var o = i[e] = i[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : a > u.from)) && (o[r] = {
                         get: () => m.e(517).then((() => () => m(517))),
                         from: a,
                         eager: !1
                     })
-                })("rose_pine_jupyterlab", "0.1.7"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("rose_pine_jupyterlab", "0.1.8"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `rose_pine_jupyterlab-0.1.7/rose_pine_jupyterlab/labextension/themes/rose_pine_jupyterlab/index.css` & `rose_pine_jupyterlab-0.1.8/style/variables.css`

 * *Files 1% similar despite different names*

```diff
@@ -83,18 +83,18 @@
 
   /* Borders
    *
    * The following variables, specify the visual styling of borders in JupyterLab.
    */
 
   --jp-border-width: 1px;
-  --jp-border-color0: var(—-rp-plt-highlight-high);
-  --jp-border-color1: var(-—rp-plt-highlight-high);
-  --jp-border-color2: var(—-rp-plt-highlight-high);
-  --jp-border-color3: var(—-rp-plt-highlight-high);
+  --jp-border-color0: var(--rp-plt-highlight-high);
+  --jp-border-color1: var(--rp-plt-highlight-high);
+  --jp-border-color2: var(--rp-plt-highlight-high);
+  --jp-border-color3: var(--rp-plt-highlight-high);
   --jp-border-radius: 2px;
 
   /* UI Fonts
    *
    * The UI font CSS variables are used for the typography all of the JupyterLab
    * user interface elements that are not directly user generated content.
    *
@@ -118,24 +118,24 @@
    * In a light theme, these go from dark to light.
    */
 
   /* Defaults use Material Design specification */
   --jp-ui-font-color0: var(--rp-plt-text);
   --jp-ui-font-color1: var(--rp-plt-subtle);
   --jp-ui-font-color2: var(--rp-plt-muted);
-  --jp-ui-font-color3: var(--rp-plt-overlay);
+  --jp-ui-font-color3: var(--rp-plt-muted);
 
   /*
    * Use these against the brand/accent/warn/error colors.
    * These will typically go from light to darker, in both a dark and light theme.
    */
 
   --jp-ui-inverse-font-color0: var(--rp-plt-base);
   --jp-ui-inverse-font-color1: var(--rp-plt-surface);
-  --jp-ui-inverse-font-color2: var(--rp-plt-overlay);
+  --jp-ui-inverse-font-color2: var(--rp-plt-muted);
   --jp-ui-inverse-font-color3: var(--rp-plt-muted);
 
   /* Content Fonts
    *
    * Content font variables are used for typography of user generated content.
    *
    * The font sizing here is done assuming that the body font size of --jp-content-font-size1
@@ -395,20 +395,25 @@
   /* Vega extension styles */
 
   --jp-vega-background: var(--rp-plt-base);
 
   /* Sidebar-related styles */
 
   --jp-sidebar-min-width: 180px;
-}
 
-/* Set the default typography for monospace elements */
-tt,
-code,
-kbd,
-samp,
-pre {
-  font-family: var(--jp-code-font-family);
-  font-size: var(--jp-code-font-size);
-  line-height: var(--jp-code-line-height);
-}
+  /* Jupyterlab git */
 
+  --jp-git-diff-deleted-color: color-mix(
+    in srgb,
+    var(--rp-plt-rose),
+    var(--rp-plt-text) 15%
+  );
+  --jp-git-diff-deleted-color1: var(--rp-plt-rose);
+  --jp-diff-deleted-color2: var(--rp-plt-rose);
+  --jp-git-diff-added-color: color-mix(
+    in srgb,
+    var(--rp-plt-foam),
+    var(--rp-plt-text) 15%
+  );
+  --jp-git-diff-added-color1: var(--rp-plt-foam);
+  --jp-diff-added-color2: var(--rp-plt-foam);
+}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rose_pine_jupyterlab-0.1.7/src/index.ts` & `rose_pine_jupyterlab-0.1.8/src/index.ts`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.7/src/pallettes.ts` & `rose_pine_jupyterlab-0.1.8/src/pallettes.ts`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.7/src/rose-pine-dawn.json` & `rose_pine_jupyterlab-0.1.8/src/rose-pine-dawn.json`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.7/src/rose-pine-moon.json` & `rose_pine_jupyterlab-0.1.8/src/rose-pine-moon.json`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.7/src/rose-pine.json` & `rose_pine_jupyterlab-0.1.8/src/rose-pine.json`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.7/src/templates.json` & `rose_pine_jupyterlab-0.1.8/src/templates.json`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.7/style/variables.css` & `rose_pine_jupyterlab-0.1.8/rose_pine_jupyterlab/labextension/themes/rose_pine_jupyterlab/index.css`

 * *Files 6% similar despite different names*

```diff
@@ -83,18 +83,18 @@
 
   /* Borders
    *
    * The following variables, specify the visual styling of borders in JupyterLab.
    */
 
   --jp-border-width: 1px;
-  --jp-border-color0: var(—-rp-plt-highlight-high);
-  --jp-border-color1: var(-—rp-plt-highlight-high);
-  --jp-border-color2: var(—-rp-plt-highlight-high);
-  --jp-border-color3: var(—-rp-plt-highlight-high);
+  --jp-border-color0: var(--rp-plt-highlight-high);
+  --jp-border-color1: var(--rp-plt-highlight-high);
+  --jp-border-color2: var(--rp-plt-highlight-high);
+  --jp-border-color3: var(--rp-plt-highlight-high);
   --jp-border-radius: 2px;
 
   /* UI Fonts
    *
    * The UI font CSS variables are used for the typography all of the JupyterLab
    * user interface elements that are not directly user generated content.
    *
@@ -118,24 +118,24 @@
    * In a light theme, these go from dark to light.
    */
 
   /* Defaults use Material Design specification */
   --jp-ui-font-color0: var(--rp-plt-text);
   --jp-ui-font-color1: var(--rp-plt-subtle);
   --jp-ui-font-color2: var(--rp-plt-muted);
-  --jp-ui-font-color3: var(--rp-plt-overlay);
+  --jp-ui-font-color3: var(--rp-plt-muted);
 
   /*
    * Use these against the brand/accent/warn/error colors.
    * These will typically go from light to darker, in both a dark and light theme.
    */
 
   --jp-ui-inverse-font-color0: var(--rp-plt-base);
   --jp-ui-inverse-font-color1: var(--rp-plt-surface);
-  --jp-ui-inverse-font-color2: var(--rp-plt-overlay);
+  --jp-ui-inverse-font-color2: var(--rp-plt-muted);
   --jp-ui-inverse-font-color3: var(--rp-plt-muted);
 
   /* Content Fonts
    *
    * Content font variables are used for typography of user generated content.
    *
    * The font sizing here is done assuming that the body font size of --jp-content-font-size1
@@ -395,8 +395,37 @@
   /* Vega extension styles */
 
   --jp-vega-background: var(--rp-plt-base);
 
   /* Sidebar-related styles */
 
   --jp-sidebar-min-width: 180px;
+
+  /* Jupyterlab git */
+
+  --jp-git-diff-deleted-color: color-mix(
+    in srgb,
+    var(--rp-plt-rose),
+    var(--rp-plt-text) 15%
+  );
+  --jp-git-diff-deleted-color1: var(--rp-plt-rose);
+  --jp-diff-deleted-color2: var(--rp-plt-rose);
+  --jp-git-diff-added-color: color-mix(
+    in srgb,
+    var(--rp-plt-foam),
+    var(--rp-plt-text) 15%
+  );
+  --jp-git-diff-added-color1: var(--rp-plt-foam);
+  --jp-diff-added-color2: var(--rp-plt-foam);
 }
+
+/* Set the default typography for monospace elements */
+tt,
+code,
+kbd,
+samp,
+pre {
+  font-family: var(--jp-code-font-family);
+  font-size: var(--jp-code-font-size);
+  line-height: var(--jp-code-line-height);
+}
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rose_pine_jupyterlab-0.1.7/.gitignore` & `rose_pine_jupyterlab-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.7/pyproject.toml` & `rose_pine_jupyterlab-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rose_pine_jupyterlab-0.1.7/readme.md` & `rose_pine_jupyterlab-0.1.8/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,13 +55,13 @@
 ## Thanks to
 
 - [aaravind100](https://github.com/aaravind100)
 
 <!-- #rose-pine-build -->
 
 ```sh
-npx @rose-pine/build@0.8.2 -t src/templates.json -o src/
+npx @rose-pine/build@0.9.1 -t src/templates.json -o src/
 ```
 
-_Generated by [@rose-pine/build@0.8.2](https://github.com/rose-pine/build)_
+_Generated by [@rose-pine/build@0.9.1](https://github.com/rose-pine/build)_
 
 <!-- /rose-pine-build -->
```

#### html2text {}

```diff
@@ -10,9 +10,9 @@
 lab. 2. Under Settings > Theme. 3. Select `RosÃ© Pine (Main/Moon/Dawn)` from
 the themes dropdown. - Note: Also works with notebook view. ## Gallery - RosÃ©
 Pine ![RosÃ© Pine](assets/rose-pine.png) - RosÃ© Pine Moon ![RosÃ© Pine Moon]
 (assets/rose-pine-moon.png) - RosÃ© Pine Dawn ![RosÃ© Pine Dawn](assets/rose-
 pine-dawn.png) ## Uninstall To remove the extension, execute: ```bash pip
 uninstall rose_pine_jupyterlab ``` ## Contributing See [CONTRIBUTING]
 (contributing.md) ## Thanks to - [aaravind100](https://github.com/aaravind100)
-```sh npx @rose-pine/build@0.8.2 -t src/templates.json -o src/ ``` _Generated
-by [@rose-pine/build@0.8.2](https://github.com/rose-pine/build)_
+```sh npx @rose-pine/build@0.9.1 -t src/templates.json -o src/ ``` _Generated
+by [@rose-pine/build@0.9.1](https://github.com/rose-pine/build)_
```

### Comparing `rose_pine_jupyterlab-0.1.7/PKG-INFO` & `rose_pine_jupyterlab-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rose_pine_jupyterlab
-Version: 0.1.7
+Version: 0.1.8
 Dynamic: Keywords
 Summary: Soho Vibes for JupyterLab
 Project-URL: Homepage, https://github.com/aaravind100/jupyterlab
 Project-URL: Bug Tracker, https://github.com/aaravind100/jupyterlab/issues
 Project-URL: Repository, https://github.com/aaravind100/jupyterlab.git
 Author-email: Ajith Aravind <ajith.aravind100@gmail.com>
 License: BSD 3-Clause License
@@ -109,13 +109,13 @@
 ## Thanks to
 
 - [aaravind100](https://github.com/aaravind100)
 
 <!-- #rose-pine-build -->
 
 ```sh
-npx @rose-pine/build@0.8.2 -t src/templates.json -o src/
+npx @rose-pine/build@0.9.1 -t src/templates.json -o src/
 ```
 
-_Generated by [@rose-pine/build@0.8.2](https://github.com/rose-pine/build)_
+_Generated by [@rose-pine/build@0.9.1](https://github.com/rose-pine/build)_
 
 <!-- /rose-pine-build -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: rose_pine_jupyterlab Version: 0.1.7 Dynamic:
+Metadata-Version: 2.3 Name: rose_pine_jupyterlab Version: 0.1.8 Dynamic:
 Keywords Summary: Soho Vibes for JupyterLab Project-URL: Homepage, https://
 github.com/aaravind100/jupyterlab Project-URL: Bug Tracker, https://github.com/
 aaravind100/jupyterlab/issues Project-URL: Repository, https://github.com/
 aaravind100/jupyterlab.git Author-email: Ajith Aravind
 gmail.com> License: BSD 3-Clause License Copyright (c) 2024, Ajith Aravind All
 rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
@@ -45,9 +45,9 @@
 lab. 2. Under Settings > Theme. 3. Select `RosÃ© Pine (Main/Moon/Dawn)` from
 the themes dropdown. - Note: Also works with notebook view. ## Gallery - RosÃ©
 Pine ![RosÃ© Pine](assets/rose-pine.png) - RosÃ© Pine Moon ![RosÃ© Pine Moon]
 (assets/rose-pine-moon.png) - RosÃ© Pine Dawn ![RosÃ© Pine Dawn](assets/rose-
 pine-dawn.png) ## Uninstall To remove the extension, execute: ```bash pip
 uninstall rose_pine_jupyterlab ``` ## Contributing See [CONTRIBUTING]
 (contributing.md) ## Thanks to - [aaravind100](https://github.com/aaravind100)
-```sh npx @rose-pine/build@0.8.2 -t src/templates.json -o src/ ``` _Generated
-by [@rose-pine/build@0.8.2](https://github.com/rose-pine/build)_
+```sh npx @rose-pine/build@0.9.1 -t src/templates.json -o src/ ``` _Generated
+by [@rose-pine/build@0.9.1](https://github.com/rose-pine/build)_
```

