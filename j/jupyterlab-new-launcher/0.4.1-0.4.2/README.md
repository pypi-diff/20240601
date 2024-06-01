# Comparing `tmp/jupyterlab_new_launcher-0.4.1.tar.gz` & `tmp/jupyterlab_new_launcher-0.4.2.tar.gz`

## Comparing `jupyterlab_new_launcher-0.4.1.tar` & `jupyterlab_new_launcher-0.4.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/.copier-answers.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/CHANGELOG.md
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/babel.config.js
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/jest.config.js
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/junit.xml
--rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/setup.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/tsconfig.test.json
--rw-r--r--   0        0        0   376569 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/yarn.lock
--rw-r--r--   0        0        0    54951 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/docs/images/dialog.png
--rw-r--r--   0        0        0    58321 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/docs/images/launcher.png
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/jupyter-config/server-config/jupyterlab_new_launcher.json
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/jupyterlab_new_launcher/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/jupyterlab_new_launcher/_version.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/jupyterlab_new_launcher/handlers.py
--rw-r--r--   0        0        0     6149 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/jupyterlab_new_launcher/labextension/package.json
--rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json
--rw-r--r--   0        0        0    31739 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/jupyterlab_new_launcher/labextension/static/252.3c46a26a0699bccd36cb.js
--rw-r--r--   0        0        0    11071 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/jupyterlab_new_launcher/labextension/static/728.54b87b26a387a46f2b0d.js
--rw-r--r--   0        0        0     7175 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/jupyterlab_new_launcher/labextension/static/remoteEntry.85dc567ef623d61041db.js
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/jupyterlab_new_launcher/labextension/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/jupyterlab_new_launcher/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/schema/plugin.json
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/src/commands.ts
--rw-r--r--   0        0        0     4667 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/src/database.ts
--rw-r--r--   0        0        0    10672 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/src/dialogs.tsx
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/src/handler.ts
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/src/icons.ts
--rw-r--r--   0        0        0     7318 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/src/index.ts
--rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/src/item.ts
--rw-r--r--   0        0        0    11152 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/src/launcher.tsx
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/src/model.ts
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/src/svg.d.ts
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/src/types.ts
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/src/typings.d.ts
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/src/__tests__/jupyterlab_new_launcher.spec.ts
--rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/src/components/base-table.tsx
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/src/components/card.tsx
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/src/components/section.tsx
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/src/components/table.tsx
--rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/style/index.js
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/style/webkit.raw.css
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/style/icons/code-server.svg
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/style/icons/md/LICENSE
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/style/icons/md/file.svg
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/style/icons/md/star.svg
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/ui-tests/package.json
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   148126 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/ui-tests/yarn.lock
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts
--rw-r--r--   0        0        0    27608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png
--rw-r--r--   0        0        0    28063 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png
--rw-r--r--   0        0        0    33928 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/table-context-menu-linux.png
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/table-context-menu-visible-columns-linux.png
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/.gitignore
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/LICENSE
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/README.md
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     6432 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/.copier-answers.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/CHANGELOG.md
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/babel.config.js
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/jest.config.js
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/junit.xml
+-rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/setup.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/tsconfig.test.json
+-rw-r--r--   0        0        0   376569 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/yarn.lock
+-rw-r--r--   0        0        0    54951 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/docs/images/dialog.png
+-rw-r--r--   0        0        0    58321 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/docs/images/launcher.png
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/jupyter-config/server-config/jupyterlab_new_launcher.json
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/jupyterlab_new_launcher/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/jupyterlab_new_launcher/_version.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/jupyterlab_new_launcher/handlers.py
+-rw-r--r--   0        0        0     6149 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/jupyterlab_new_launcher/labextension/package.json
+-rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json
+-rw-r--r--   0        0        0    31754 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/jupyterlab_new_launcher/labextension/static/252.12c1ec021a497826c277.js
+-rw-r--r--   0        0        0    11071 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/jupyterlab_new_launcher/labextension/static/728.54b87b26a387a46f2b0d.js
+-rw-r--r--   0        0        0     7175 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/jupyterlab_new_launcher/labextension/static/remoteEntry.007c3198a42218fd36c4.js
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/jupyterlab_new_launcher/labextension/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/jupyterlab_new_launcher/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/schema/plugin.json
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/src/commands.ts
+-rw-r--r--   0        0        0     4667 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/src/database.ts
+-rw-r--r--   0        0        0    10672 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/src/dialogs.tsx
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/src/handler.ts
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/src/icons.ts
+-rw-r--r--   0        0        0     7318 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/src/index.ts
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/src/item.ts
+-rw-r--r--   0        0        0    11152 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/src/launcher.tsx
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/src/model.ts
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/src/svg.d.ts
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/src/types.ts
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/src/typings.d.ts
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/src/__tests__/jupyterlab_new_launcher.spec.ts
+-rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/src/components/base-table.tsx
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/src/components/card.tsx
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/src/components/section.tsx
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/src/components/table.tsx
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/style/index.js
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/style/webkit.raw.css
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/style/icons/code-server.svg
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/style/icons/md/LICENSE
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/style/icons/md/file.svg
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/style/icons/md/star.svg
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/ui-tests/package.json
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   148126 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/ui-tests/yarn.lock
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts
+-rw-r--r--   0        0        0    27608 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png
+-rw-r--r--   0        0        0    28063 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png
+-rw-r--r--   0        0        0    33928 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/table-context-menu-linux.png
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/table-context-menu-visible-columns-linux.png
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/LICENSE
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/README.md
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     6432 2020-02-02 00:00:00.000000 jupyterlab_new_launcher-0.4.2/PKG-INFO
```

### Comparing `jupyterlab_new_launcher-0.4.1/.copier-answers.yml` & `jupyterlab_new_launcher-0.4.2/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/RELEASE.md` & `jupyterlab_new_launcher-0.4.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/jest.config.js` & `jupyterlab_new_launcher-0.4.2/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/package.json` & `jupyterlab_new_launcher-0.4.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.4.2'"}*

```diff
@@ -196,9 +196,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.4.1"
+    "version": "0.4.2"
 }
```

### Comparing `jupyterlab_new_launcher-0.4.1/tsconfig.json` & `jupyterlab_new_launcher-0.4.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/yarn.lock` & `jupyterlab_new_launcher-0.4.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/docs/images/dialog.png` & `jupyterlab_new_launcher-0.4.2/docs/images/dialog.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/docs/images/launcher.png` & `jupyterlab_new_launcher-0.4.2/docs/images/launcher.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/jupyterlab_new_launcher/__init__.py` & `jupyterlab_new_launcher-0.4.2/jupyterlab_new_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/jupyterlab_new_launcher/handlers.py` & `jupyterlab_new_launcher-0.4.2/jupyterlab_new_launcher/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/jupyterlab_new_launcher/labextension/package.json` & `jupyterlab_new_launcher-0.4.2/jupyterlab_new_launcher/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788194444444445%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.007c3198a42218fd36c4.js'}}",*

 * * "'version'": "'0.4.2'"}*

```diff
@@ -109,15 +109,15 @@
         "schema/*.json",
         "!**/.ipynb_checkpoints/"
     ],
     "homepage": "https://github.com/nebari-dev/jupyterlab-new-launcher",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.85dc567ef623d61041db.js",
+            "load": "static/remoteEntry.007c3198a42218fd36c4.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/launcher-extension",
             "@jupyterlab/apputils-extension:sessionDialogs"
         ],
         "extension": true,
@@ -201,9 +201,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.4.1"
+    "version": "0.4.2"
 }
```

### Comparing `jupyterlab_new_launcher-0.4.1/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig` & `jupyterlab_new_launcher-0.4.2/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.4.2'"}*

```diff
@@ -196,9 +196,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.4.1"
+    "version": "0.4.2"
 }
```

### Comparing `jupyterlab_new_launcher-0.4.1/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json` & `jupyterlab_new_launcher-0.4.2/jupyterlab_new_launcher/labextension/schemas/jupyterlab-new-launcher/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/jupyterlab_new_launcher/labextension/static/252.3c46a26a0699bccd36cb.js` & `jupyterlab_new_launcher-0.4.2/jupyterlab_new_launcher/labextension/static/252.12c1ec021a497826c277.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -42,20 +42,24 @@
                     };
                     this.command = o.command, this.args = i, this.category = o.category, this.rank = o.rank, this.kernelIconUrl = o.kernelIconUrl, this.metadata = null !== (t = o.metadata) && void 0 !== t ? t : {}, this.iconClass = r.iconClass(o.command, i), this.icon = r.icon(o.command, i), this.caption = r.caption(o.command, i), this.label = r.label(o.command, i);
                     const c = this.metadata.kernel;
                     if (c) {
                         const e = (null !== (n = c.conda_env_name) && void 0 !== n ? n : "").match(/(?<namespace>.+)-(?<duplicate>\1)-(?<environment>.+)/);
                         if (e && this.metadata) {
                             const t = e.groups;
-                            this.label = null !== (a = c.conda_language) && void 0 !== a ? a : t.environment, delete c.conda_env_name, this.metadata = {
+                            this.label = null !== (a = c.conda_language) && void 0 !== a ? a : t.environment;
+                            const n = {
+                                ...c
+                            };
+                            delete n.conda_env_name, this.metadata = {
                                 ...this.metadata,
                                 kernel: {
                                     Namespace: t.namespace,
                                     conda_env_name: t.environment,
-                                    ...c
+                                    ...n
                                 }
                             }
                         }
                     }
                     "server-proxy:open" === this.command && (null === (s = this.kernelIconUrl) || void 0 === s ? void 0 : s.endsWith("/vscode")) && (this.icon = g)
                 }
                 get starred() {
```

### Comparing `jupyterlab_new_launcher-0.4.1/jupyterlab_new_launcher/labextension/static/728.54b87b26a387a46f2b0d.js` & `jupyterlab_new_launcher-0.4.2/jupyterlab_new_launcher/labextension/static/728.54b87b26a387a46f2b0d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/jupyterlab_new_launcher/labextension/static/remoteEntry.85dc567ef623d61041db.js` & `jupyterlab_new_launcher-0.4.2/jupyterlab_new_launcher/labextension/static/remoteEntry.007c3198a42218fd36c4.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -43,18 +43,18 @@
         }), r
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        252: "3c46a26a0699bccd36cb",
+        252: "12c1ec021a497826c277",
         728: "54b87b26a387a46f2b0d"
     } [e] + ".js?v=" + {
-        252: "3c46a26a0699bccd36cb",
+        252: "12c1ec021a497826c277",
         728: "54b87b26a387a46f2b0d"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -106,15 +106,15 @@
                     var a = o[e] = o[e] || {},
                         u = a[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (a[r] = {
                         get: () => m.e(252).then((() => () => m(252))),
                         from: i,
                         eager: !1
                     })
-                })("jupyterlab-new-launcher", "0.4.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("jupyterlab-new-launcher", "0.4.2"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_new_launcher-0.4.1/jupyterlab_new_launcher/labextension/static/third-party-licenses.json` & `jupyterlab_new_launcher-0.4.2/jupyterlab_new_launcher/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/schema/plugin.json` & `jupyterlab_new_launcher-0.4.2/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/src/commands.ts` & `jupyterlab_new_launcher-0.4.2/src/commands.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/src/database.ts` & `jupyterlab_new_launcher-0.4.2/src/database.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/src/dialogs.tsx` & `jupyterlab_new_launcher-0.4.2/src/dialogs.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/src/handler.ts` & `jupyterlab_new_launcher-0.4.2/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/src/icons.ts` & `jupyterlab_new_launcher-0.4.2/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/src/index.ts` & `jupyterlab_new_launcher-0.4.2/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/src/item.ts` & `jupyterlab_new_launcher-0.4.2/src/item.ts`

 * *Files 3% similar despite different names*

```diff
@@ -53,21 +53,22 @@
         (kernel['conda_env_name'] as string | undefined) ?? ''
       ).match(/(?<namespace>.+)-(?<duplicate>\1)-(?<environment>.+)/);
       if (condaStoreMatch && this.metadata) {
         const groups = condaStoreMatch.groups!;
         this.label =
           (kernel['conda_language'] as string | undefined) ??
           groups.environment;
-        delete kernel['conda_env_name'];
+        const kernelCopy = { ...kernel };
+        delete kernelCopy['conda_env_name'];
         this.metadata = {
           ...this.metadata,
           kernel: {
             Namespace: groups.namespace,
             conda_env_name: groups.environment,
-            ...kernel
+            ...kernelCopy
           }
         };
       }
     }
     // set the code-server icon to support dark theme properly
     if (
       this.command === 'server-proxy:open' &&
```

### Comparing `jupyterlab_new_launcher-0.4.1/src/launcher.tsx` & `jupyterlab_new_launcher-0.4.2/src/launcher.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/src/model.ts` & `jupyterlab_new_launcher-0.4.2/src/model.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/src/types.ts` & `jupyterlab_new_launcher-0.4.2/src/types.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/src/components/base-table.tsx` & `jupyterlab_new_launcher-0.4.2/src/components/base-table.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/src/components/card.tsx` & `jupyterlab_new_launcher-0.4.2/src/components/card.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/src/components/section.tsx` & `jupyterlab_new_launcher-0.4.2/src/components/section.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/src/components/table.tsx` & `jupyterlab_new_launcher-0.4.2/src/components/table.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/style/base.css` & `jupyterlab_new_launcher-0.4.2/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/style/icons/code-server.svg` & `jupyterlab_new_launcher-0.4.2/style/icons/code-server.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/style/icons/md/LICENSE` & `jupyterlab_new_launcher-0.4.2/style/icons/md/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/ui-tests/README.md` & `jupyterlab_new_launcher-0.4.2/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/ui-tests/yarn.lock` & `jupyterlab_new_launcher-0.4.2/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts` & `jupyterlab_new_launcher-0.4.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png` & `jupyterlab_new_launcher-0.4.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png` & `jupyterlab_new_launcher-0.4.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-search-in-individual-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png` & `jupyterlab_new_launcher-0.4.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/launcher-with-starred-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/table-context-menu-linux.png` & `jupyterlab_new_launcher-0.4.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/table-context-menu-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/table-context-menu-visible-columns-linux.png` & `jupyterlab_new_launcher-0.4.2/ui-tests/tests/jupyterlab_new_launcher.spec.ts-snapshots/table-context-menu-visible-columns-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/.gitignore` & `jupyterlab_new_launcher-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/LICENSE` & `jupyterlab_new_launcher-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/README.md` & `jupyterlab_new_launcher-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/pyproject.toml` & `jupyterlab_new_launcher-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_new_launcher-0.4.1/PKG-INFO` & `jupyterlab_new_launcher-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-new-launcher
-Version: 0.4.1
+Version: 0.4.2
 Dynamic: Keywords
 Summary: A redesigned JupyterLab launcher
 Project-URL: Homepage, https://github.com/nebari-dev/jupyterlab-new-launcher
 Project-URL: Bug Tracker, https://github.com/nebari-dev/jupyterlab-new-launcher/issues
 Project-URL: Repository, https://github.com/nebari-dev/jupyterlab-new-launcher.git
 Author-email: Nebari development team <internal-it@quansight.com>
 License: BSD 3-Clause License
```

