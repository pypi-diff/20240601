# Comparing `tmp/monaco-qt-0.1.7.tar.gz` & `tmp/monaco_qt-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monaco-qt-0.1.7.tar", last modified: Mon Apr  3 01:00:55 2023, max compression
+gzip compressed data, was "monaco_qt-0.1.8.tar", last modified: Sat Jun  1 21:42:34 2024, max compression
```

## Comparing `monaco-qt-0.1.7.tar` & `monaco_qt-0.1.8.tar`

### file list

```diff
@@ -1,977 +1,977 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.648529 monaco-qt-0.1.7/
--rw-rw-rw-   0        0        0     1603 2023-04-03 01:00:55.648031 monaco-qt-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      835 2023-01-09 05:00:48.000000 monaco-qt-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.672530 monaco-qt-0.1.7/monaco/
--rw-rw-rw-   0        0        0      174 2023-04-03 00:23:27.000000 monaco-qt-0.1.7/monaco/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.676032 monaco-qt-0.1.7/monaco/_pyinstaller/
--rw-rw-rw-   0        0        0        0 2023-04-03 00:24:25.000000 monaco-qt-0.1.7/monaco/_pyinstaller/__init__.py
--rw-rw-rw-   0        0        0       96 2023-04-03 00:27:34.000000 monaco-qt-0.1.7/monaco/_pyinstaller/hook-monaco.py
--rw-rw-rw-   0        0        0      612 2022-07-12 00:37:02.000000 monaco-qt-0.1.7/monaco/index.html
--rw-rw-rw-   0        0        0     1681 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/index.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.684528 monaco-qt-0.1.7/monaco/monaco-editor/
--rw-rw-rw-   0        0        0    96665 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/CHANGELOG.md
--rw-rw-rw-   0        0        0     1119 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/LICENSE
--rw-rw-rw-   0        0        0     5116 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/README.md
--rw-rw-rw-   0        0        0    63512 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/ThirdPartyNotices.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.467530 monaco-qt-0.1.7/monaco/monaco-editor/min/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.685531 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.469028 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/base/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.468028 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/base/browser/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.468528 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/base/browser/ui/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.468528 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/base/browser/ui/codicons/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.687031 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/base/browser/ui/codicons/codicon/
--rw-rw-rw-   0        0        0    70776 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/base/browser/ui/codicons/codicon/codicon.ttf
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.688531 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/base/worker/
--rw-rw-rw-   0        0        0   283886 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/base/worker/workerMain.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.526031 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.691529 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/abap/
--rw-rw-rw-   0        0        0    15097 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/abap/abap.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.693531 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/apex/
--rw-rw-rw-   0        0        0     4886 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/apex/apex.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.695030 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/azcli/
--rw-rw-rw-   0        0        0     1784 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/azcli/azcli.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.696529 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/bat/
--rw-rw-rw-   0        0        0     2777 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/bat/bat.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.698029 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/bicep/
--rw-rw-rw-   0        0        0     3473 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/bicep/bicep.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.699029 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/cameligo/
--rw-rw-rw-   0        0        0     3127 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/cameligo/cameligo.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.700029 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/clojure/
--rw-rw-rw-   0        0        0    10583 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/clojure/clojure.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.701529 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/coffee/
--rw-rw-rw-   0        0        0     4528 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/coffee/coffee.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.705032 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/cpp/
--rw-rw-rw-   0        0        0     6380 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/cpp/cpp.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.708030 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/csharp/
--rw-rw-rw-   0        0        0     5462 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/csharp/csharp.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.710031 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/csp/
--rw-rw-rw-   0        0        0     2351 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/csp/csp.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.712035 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/css/
--rw-rw-rw-   0        0        0     5441 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/css/css.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.713530 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/dart/
--rw-rw-rw-   0        0        0     5184 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/dart/dart.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.714530 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/dockerfile/
--rw-rw-rw-   0        0        0     2815 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/dockerfile/dockerfile.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.716031 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/ecl/
--rw-rw-rw-   0        0        0     6274 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/ecl/ecl.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.717531 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/elixir/
--rw-rw-rw-   0        0        0    10697 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/elixir/elixir.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.719532 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/flow9/
--rw-rw-rw-   0        0        0     2746 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/flow9/flow9.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.721029 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/freemarker2/
--rw-rw-rw-   0        0        0    17278 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/freemarker2/freemarker2.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.722530 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/fsharp/
--rw-rw-rw-   0        0        0     3921 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/fsharp/fsharp.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.724532 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/go/
--rw-rw-rw-   0        0        0     3587 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/go/go.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.726530 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/graphql/
--rw-rw-rw-   0        0        0     3200 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/graphql/graphql.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.728031 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/handlebars/
--rw-rw-rw-   0        0        0     7954 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/handlebars/handlebars.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.729530 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/hcl/
--rw-rw-rw-   0        0        0     4522 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/hcl/hcl.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.731531 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/html/
--rw-rw-rw-   0        0        0     6006 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/html/html.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.733032 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/ini/
--rw-rw-rw-   0        0        0     2033 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/ini/ini.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.736029 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/java/
--rw-rw-rw-   0        0        0     4155 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/java/java.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.740531 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/javascript/
--rw-rw-rw-   0        0        0     7235 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/javascript/javascript.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.741540 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/julia/
--rw-rw-rw-   0        0        0     8163 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/julia/julia.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.745030 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/kotlin/
--rw-rw-rw-   0        0        0     4377 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/kotlin/kotlin.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.747532 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/less/
--rw-rw-rw-   0        0        0     4830 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/less/less.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.749029 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/lexon/
--rw-rw-rw-   0        0        0     3373 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/lexon/lexon.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.750529 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/liquid/
--rw-rw-rw-   0        0        0     5132 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/liquid/liquid.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.754030 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/lua/
--rw-rw-rw-   0        0        0     3055 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/lua/lua.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.756531 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/m3/
--rw-rw-rw-   0        0        0     3747 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/m3/m3.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.760533 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/markdown/
--rw-rw-rw-   0        0        0     4730 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/markdown/markdown.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.762530 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/mips/
--rw-rw-rw-   0        0        0     3513 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/mips/mips.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.764042 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/msdax/
--rw-rw-rw-   0        0        0     5848 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/msdax/msdax.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.768531 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/mysql/
--rw-rw-rw-   0        0        0    12193 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/mysql/mysql.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.771530 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/objective-c/
--rw-rw-rw-   0        0        0     3350 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/objective-c/objective-c.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.776532 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/pascal/
--rw-rw-rw-   0        0        0     3933 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/pascal/pascal.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.779032 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/pascaligo/
--rw-rw-rw-   0        0        0     2944 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/pascaligo/pascaligo.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.782534 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/perl/
--rw-rw-rw-   0        0        0     9189 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/perl/perl.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.784043 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/pgsql/
--rw-rw-rw-   0        0        0    14340 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/pgsql/pgsql.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.786531 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/php/
--rw-rw-rw-   0        0        0     8959 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/php/php.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.788531 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/pla/
--rw-rw-rw-   0        0        0     2615 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/pla/pla.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.790532 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/postiats/
--rw-rw-rw-   0        0        0     8798 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/postiats/postiats.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.795031 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/powerquery/
--rw-rw-rw-   0        0        0    17885 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/powerquery/powerquery.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.797531 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/powershell/
--rw-rw-rw-   0        0        0     4215 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/powershell/powershell.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.799030 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/protobuf/
--rw-rw-rw-   0        0        0     9989 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/protobuf/protobuf.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.802030 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/pug/
--rw-rw-rw-   0        0        0     5760 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/pug/pug.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.804031 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/python/
--rw-rw-rw-   0        0        0     4759 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/python/python.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.805529 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/qsharp/
--rw-rw-rw-   0        0        0     3862 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/qsharp/qsharp.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.807031 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/r/
--rw-rw-rw-   0        0        0     4059 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/r/r.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.808531 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/razor/
--rw-rw-rw-   0        0        0     9948 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/razor/razor.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.810532 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/redis/
--rw-rw-rw-   0        0        0     4492 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/redis/redis.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.813031 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/redshift/
--rw-rw-rw-   0        0        0    12742 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/redshift/redshift.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.814531 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/restructuredtext/
--rw-rw-rw-   0        0        0     4851 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/restructuredtext/restructuredtext.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.817530 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/ruby/
--rw-rw-rw-   0        0        0     9438 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/ruby/ruby.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.819033 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/rust/
--rw-rw-rw-   0        0        0     5094 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/rust/rust.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.820532 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/sb/
--rw-rw-rw-   0        0        0     2759 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/sb/sb.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.823031 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/scala/
--rw-rw-rw-   0        0        0     8254 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/scala/scala.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.824530 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/scheme/
--rw-rw-rw-   0        0        0     2705 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/scheme/scheme.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.826528 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/scss/
--rw-rw-rw-   0        0        0     7342 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/scss/scss.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.830031 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/shell/
--rw-rw-rw-   0        0        0     4009 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/shell/shell.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.832029 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/solidity/
--rw-rw-rw-   0        0        0    19539 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/solidity/solidity.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.834531 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/sophia/
--rw-rw-rw-   0        0        0     3702 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/sophia/sophia.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.837530 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/sparql/
--rw-rw-rw-   0        0        0     3490 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/sparql/sparql.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.839030 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/sql/
--rw-rw-rw-   0        0        0    11229 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/sql/sql.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.840532 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/st/
--rw-rw-rw-   0        0        0     8320 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/st/st.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.842529 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/swift/
--rw-rw-rw-   0        0        0     6111 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/swift/swift.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.844529 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/systemverilog/
--rw-rw-rw-   0        0        0     8555 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/systemverilog/systemverilog.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.846029 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/tcl/
--rw-rw-rw-   0        0        0     4503 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/tcl/tcl.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.847530 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/twig/
--rw-rw-rw-   0        0        0     6906 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/twig/twig.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.849031 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/typescript/
--rw-rw-rw-   0        0        0     6567 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/typescript/typescript.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.850537 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/vb/
--rw-rw-rw-   0        0        0     6721 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/vb/vb.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.852030 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/xml/
--rw-rw-rw-   0        0        0     3579 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/xml/xml.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.853529 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/yaml/
--rw-rw-rw-   0        0        0     4478 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/yaml/yaml.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.886531 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/
--rw-rw-rw-   0        0        0    77307 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.css
--rw-rw-rw-   0        0        0  2918322 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.js
--rw-rw-rw-   0        0        0    96566 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.nls.de.js
--rw-rw-rw-   0        0        0    97319 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.nls.es.js
--rw-rw-rw-   0        0        0   106136 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.nls.fr.js
--rw-rw-rw-   0        0        0    99139 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.nls.it.js
--rw-rw-rw-   0        0        0   199359 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.nls.ja.js
--rw-rw-rw-   0        0        0    77655 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.nls.js
--rw-rw-rw-   0        0        0   165466 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.nls.ko.js
--rw-rw-rw-   0        0        0   412899 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.nls.ru.js
--rw-rw-rw-   0        0        0   126176 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.nls.zh-cn.js
--rw-rw-rw-   0        0        0   128706 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.nls.zh-tw.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.530532 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/language/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.893032 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/language/css/
--rw-rw-rw-   0        0        0    34114 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/language/css/cssMode.js
--rw-rw-rw-   0        0        0   752287 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/language/css/cssWorker.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.899531 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/language/html/
--rw-rw-rw-   0        0        0    34867 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/language/html/htmlMode.js
--rw-rw-rw-   0        0        0   446862 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/language/html/htmlWorker.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.907031 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/language/json/
--rw-rw-rw-   0        0        0    40310 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/language/json/jsonMode.js
--rw-rw-rw-   0        0        0   129160 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/language/json/jsonWorker.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.910038 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/language/typescript/
--rw-rw-rw-   0        0        0    22808 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/language/typescript/tsMode.js
--rw-rw-rw-   0        0        0  4761155 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/language/typescript/tsWorker.js
--rw-rw-rw-   0        0        0    33214 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/min/vs/loader.js
--rw-rw-rw-   0        0        0   296660 2022-07-11 15:07:46.000000 monaco-qt-0.1.7/monaco/monaco-editor/monaco.d.ts
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.659529 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.534031 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.535030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.536530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.537533 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.538030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.929030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/
--rw-rw-rw-   0        0        0    19414 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.mjs
--rw-rw-rw-   0        0        0    15178 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.mjs.map
--rw-rw-rw-   0        0        0    22396 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.umd.js
--rw-rw-rw-   0        0        0    15515 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.umd.js.map
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.950048 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/
--rw-rw-rw-   0        0        0      319 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/any-map.d.ts
--rw-rw-rw-   0        0        0     1546 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/binary-search.d.ts
--rw-rw-rw-   0        0        0      349 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/by-source.d.ts
--rw-rw-rw-   0        0        0       82 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/resolve.d.ts
--rw-rw-rw-   0        0        0      166 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/sort.d.ts
--rw-rw-rw-   0        0        0      783 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/sourcemap-segment.d.ts
--rw-rw-rw-   0        0        0      152 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/strip-filename.d.ts
--rw-rw-rw-   0        0        0     3614 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/trace-mapping.d.ts
--rw-rw-rw-   0        0        0     2218 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/types.d.ts
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.559530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.540530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.984029 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/
--rw-rw-rw-   0        0        0     9207 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/gen-mapping.mjs
--rw-rw-rw-   0        0        0    21472 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/gen-mapping.mjs.map
--rw-rw-rw-   0        0        0    10824 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/gen-mapping.umd.js
--rw-rw-rw-   0        0        0    21687 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/gen-mapping.umd.js.map
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.991530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/types/
--rw-rw-rw-   0        0        0     3672 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/types/gen-mapping.d.ts
--rw-rw-rw-   0        0        0      569 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/types/sourcemap-segment.d.ts
--rw-rw-rw-   0        0        0      820 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/types/types.d.ts
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.543531 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.000531 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/dist/
--rw-rw-rw-   0        0        0     9040 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/dist/resolve-uri.mjs
--rw-rw-rw-   0        0        0    14811 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/dist/resolve-uri.mjs.map
--rw-rw-rw-   0        0        0    10337 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/dist/resolve-uri.umd.js
--rw-rw-rw-   0        0        0    14848 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/dist/resolve-uri.umd.js.map
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.003532 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/dist/types/
--rw-rw-rw-   0        0        0      150 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/dist/types/resolve-uri.d.ts
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.546529 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/set-array/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.012029 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/
--rw-rw-rw-   0        0        0     1475 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/set-array.mjs
--rw-rw-rw-   0        0        0     2631 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/set-array.mjs.map
--rw-rw-rw-   0        0        0     2153 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/set-array.umd.js
--rw-rw-rw-   0        0        0     2675 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/set-array.umd.js.map
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.015529 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/types/
--rw-rw-rw-   0        0        0      971 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/types/set-array.d.ts
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.550532 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/source-map/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.061529 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/
--rw-rw-rw-   0        0        0    32713 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/source-map.mjs
--rw-rw-rw-   0        0        0    77701 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/source-map.mjs.map
--rw-rw-rw-   0        0        0    36850 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/source-map.umd.js
--rw-rw-rw-   0        0        0    77717 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/source-map.umd.js.map
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.064531 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/types/
--rw-rw-rw-   0        0        0     1443 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/types/source-map.d.ts
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.554530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.073544 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/dist/
--rw-rw-rw-   0        0        0     5279 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/dist/sourcemap-codec.mjs
--rw-rw-rw-   0        0        0     6099 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/dist/sourcemap-codec.mjs.map
--rw-rw-rw-   0        0        0     6390 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/dist/sourcemap-codec.umd.js
--rw-rw-rw-   0        0        0     6145 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/dist/sourcemap-codec.umd.js.map
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.075030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/dist/types/
--rw-rw-rw-   0        0        0      455 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/dist/types/sourcemap-codec.d.ts
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.560531 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.082030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/
--rw-rw-rw-   0        0        0    21727 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.mjs
--rw-rw-rw-   0        0        0    47615 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.mjs.map
--rw-rw-rw-   0        0        0    24859 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.umd.js
--rw-rw-rw-   0        0        0    47881 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.umd.js.map
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.096036 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/
--rw-rw-rw-   0        0        0      319 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/any-map.d.ts
--rw-rw-rw-   0        0        0     1546 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/binary-search.d.ts
--rw-rw-rw-   0        0        0      349 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/by-source.d.ts
--rw-rw-rw-   0        0        0       82 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/resolve.d.ts
--rw-rw-rw-   0        0        0      166 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/sort.d.ts
--rw-rw-rw-   0        0        0      783 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/sourcemap-segment.d.ts
--rw-rw-rw-   0        0        0      152 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/strip-filename.d.ts
--rw-rw-rw-   0        0        0     3730 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/trace-mapping.d.ts
--rw-rw-rw-   0        0        0     2656 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/types.d.ts
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.564531 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@tootallnate/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.566031 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@tootallnate/once/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.110530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@tootallnate/once/dist/
--rw-rw-rw-   0        0        0      407 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@tootallnate/once/dist/index.d.ts
--rw-rw-rw-   0        0        0      846 2023-01-09 05:07:11.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@tootallnate/once/dist/index.js
--rw-rw-rw-   0        0        0      824 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@tootallnate/once/dist/index.js.map
--rw-rw-rw-   0        0        0     7853 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@tootallnate/once/dist/overloaded-parameters.d.ts
--rw-rw-rw-   0        0        0      126 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@tootallnate/once/dist/overloaded-parameters.js
--rw-rw-rw-   0        0        0      134 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@tootallnate/once/dist/overloaded-parameters.js.map
--rw-rw-rw-   0        0        0     1015 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@tootallnate/once/dist/types.d.ts
--rw-rw-rw-   0        0        0      110 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@tootallnate/once/dist/types.js
--rw-rw-rw-   0        0        0      102 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@tootallnate/once/dist/types.js.map
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.568531 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@typescript/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.569029 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@typescript/vfs/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.125030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@typescript/vfs/dist/
--rw-rw-rw-   0        0        0     4989 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@typescript/vfs/dist/index.d.ts
--rw-rw-rw-   0        0        0      184 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@typescript/vfs/dist/index.js
--rw-rw-rw-   0        0        0    21880 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.cjs.development.js
--rw-rw-rw-   0        0        0    40397 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.cjs.development.js.map
--rw-rw-rw-   0        0        0     9069 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.cjs.production.min.js
--rw-rw-rw-   0        0        0    30984 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.cjs.production.min.js.map
--rw-rw-rw-   0        0        0    21435 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.esm.js
--rw-rw-rw-   0        0        0    40372 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.esm.js.map
--rw-rw-rw-   0        0        0    21755 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.globals.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.576531 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.155530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn/dist/
--rw-rw-rw-   0        0        0     6200 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn/dist/acorn.d.ts
--rw-rw-rw-   0        0        0   217774 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn/dist/acorn.js
--rw-rw-rw-   0        0        0   207097 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn/dist/acorn.mjs
--rw-rw-rw-   0        0        0       49 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn/dist/acorn.mjs.d.ts
--rw-rw-rw-   0        0        0     3285 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn/dist/bin.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.571532 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-globals/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.572030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-globals/node_modules/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.573044 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.137028 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/
--rw-rw-rw-   0        0        0     5224 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/acorn.d.ts
--rw-rw-rw-   0        0        0   200010 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/acorn.js
--rw-rw-rw-   0        0        0   392402 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/acorn.js.map
--rw-rw-rw-   0        0        0   190128 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/acorn.mjs
--rw-rw-rw-   0        0        0       49 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/acorn.mjs.d.ts
--rw-rw-rw-   0        0        0   392368 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/acorn.mjs.map
--rw-rw-rw-   0        0        0     2291 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/bin.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.574530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-walk/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.145532 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-walk/dist/
--rw-rw-rw-   0        0        0     2559 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-walk/dist/walk.d.ts
--rw-rw-rw-   0        0        0    16001 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-walk/dist/walk.js
--rw-rw-rw-   0        0        0    29054 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-walk/dist/walk.js.map
--rw-rw-rw-   0        0        0    14560 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-walk/dist/walk.mjs
--rw-rw-rw-   0        0        0    29031 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-walk/dist/walk.mjs.map
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.578530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/agent-base/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.579030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/agent-base/dist/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.166539 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/agent-base/dist/src/
--rw-rw-rw-   0        0        0     3197 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/agent-base/dist/src/index.d.ts
--rw-rw-rw-   0        0        0     7910 2023-01-09 05:07:11.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/agent-base/dist/src/index.js
--rw-rw-rw-   0        0        0     5824 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/agent-base/dist/src/index.js.map
--rw-rw-rw-   0        0        0      299 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/agent-base/dist/src/promisify.d.ts
--rw-rw-rw-   0        0        0      495 2023-01-09 05:07:11.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/agent-base/dist/src/promisify.js
--rw-rw-rw-   0        0        0      499 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/agent-base/dist/src/promisify.js.map
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.580530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/cliui/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.169531 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/cliui/build/
--rw-rw-rw-   0        0        0     9953 2023-01-09 05:07:11.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/cliui/build/index.cjs
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.172529 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/cliui/build/lib/
--rw-rw-rw-   0        0        0     9667 2023-01-09 05:07:11.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/cliui/build/lib/index.js
--rw-rw-rw-   0        0        0     1011 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/cliui/build/lib/string-utils.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.582029 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/diff/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.173529 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/diff/dist/
--rw-rw-rw-   0        0        0    48351 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/diff/dist/diff.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.584531 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/escalade/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.178030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/escalade/dist/
--rw-rw-rw-   0        0        0      534 2023-01-09 05:07:11.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/escalade/dist/index.js
--rw-rw-rw-   0        0        0      517 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/escalade/dist/index.mjs
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.586030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/esprima/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.179530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/esprima/dist/
--rw-rw-rw-   0        0        0   283567 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/esprima/dist/esprima.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.587030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/http-proxy-agent/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.192031 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/http-proxy-agent/dist/
--rw-rw-rw-   0        0        0      941 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/http-proxy-agent/dist/agent.d.ts
--rw-rw-rw-   0        0        0     6608 2023-01-09 05:07:11.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/http-proxy-agent/dist/agent.js
--rw-rw-rw-   0        0        0     3781 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/http-proxy-agent/dist/agent.js.map
--rw-rw-rw-   0        0        0      872 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/http-proxy-agent/dist/index.d.ts
--rw-rw-rw-   0        0        0      571 2023-01-09 05:07:11.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/http-proxy-agent/dist/index.js
--rw-rw-rw-   0        0        0      359 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/http-proxy-agent/dist/index.js.map
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.589031 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/https-proxy-agent/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.207030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/https-proxy-agent/dist/
--rw-rw-rw-   0        0        0     1126 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/https-proxy-agent/dist/agent.d.ts
--rw-rw-rw-   0        0        0     7841 2023-01-09 05:07:11.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/https-proxy-agent/dist/agent.js
--rw-rw-rw-   0        0        0     4367 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/https-proxy-agent/dist/agent.js.map
--rw-rw-rw-   0        0        0      970 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/https-proxy-agent/dist/index.d.ts
--rw-rw-rw-   0        0        0      579 2023-01-09 05:07:11.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/https-proxy-agent/dist/index.js
--rw-rw-rw-   0        0        0      362 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/https-proxy-agent/dist/index.js.map
--rw-rw-rw-   0        0        0      233 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/https-proxy-agent/dist/parse-proxy-response.d.ts
--rw-rw-rw-   0        0        0     2460 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/https-proxy-agent/dist/parse-proxy-response.js
--rw-rw-rw-   0        0        0     1904 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/https-proxy-agent/dist/parse-proxy-response.js.map
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.591031 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/human-signals/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.591530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/human-signals/build/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.220033 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/human-signals/build/src/
--rw-rw-rw-   0        0        0     4268 2023-01-09 05:07:11.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/human-signals/build/src/core.js
--rw-rw-rw-   0        0        0    10551 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/human-signals/build/src/core.js.map
--rw-rw-rw-   0        0        0     1528 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/human-signals/build/src/main.js
--rw-rw-rw-   0        0        0     4047 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/human-signals/build/src/main.js.map
--rw-rw-rw-   0        0        0      590 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/human-signals/build/src/realtime.js
--rw-rw-rw-   0        0        0     1245 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/human-signals/build/src/realtime.js.map
--rw-rw-rw-   0        0        0      778 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/human-signals/build/src/signals.js
--rw-rw-rw-   0        0        0     2054 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/human-signals/build/src/signals.js.map
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.593530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/js-yaml/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.224537 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/js-yaml/dist/
--rw-rw-rw-   0        0        0   114359 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/js-yaml/dist/js-yaml.js
--rw-rw-rw-   0        0        0    39430 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/js-yaml/dist/js-yaml.min.js
--rw-rw-rw-   0        0        0   107533 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/js-yaml/dist/js-yaml.mjs
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.595030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/lunr/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.236029 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/lunr/build/
--rw-rw-rw-   0        0        0      142 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/lunr/build/bower.json.template
--rw-rw-rw-   0        0        0      204 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/lunr/build/component.json.template
--rw-rw-rw-   0        0        0      165 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/lunr/build/jsdoc.conf.json
--rw-rw-rw-   0        0        0      726 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/lunr/build/package.json.template
--rw-rw-rw-   0        0        0     1758 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/lunr/build/release.sh
--rw-rw-rw-   0        0        0      873 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/lunr/build/wrapper_end
--rw-rw-rw-   0        0        0      175 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/lunr/build/wrapper_start
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.597030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/make-error/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.238032 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/make-error/dist/
--rw-rw-rw-   0        0        0     2793 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/make-error/dist/make-error.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.598529 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/nwsapi/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.243030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/nwsapi/dist/
--rw-rw-rw-   0        0        0        0 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/nwsapi/dist/lint.log
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.600030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/pretty-quick/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.276032 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/pretty-quick/dist/
--rw-rw-rw-   0        0        0      698 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/pretty-quick/dist/createIgnorer.js
--rw-rw-rw-   0        0        0      670 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/pretty-quick/dist/createMatcher.js
--rw-rw-rw-   0        0        0     2817 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/pretty-quick/dist/index.js
--rw-rw-rw-   0        0        0      389 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/pretty-quick/dist/isSupportedExtension.js
--rw-rw-rw-   0        0        0     1980 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/pretty-quick/dist/processFiles.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.294031 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/pretty-quick/dist/scms/
--rw-rw-rw-   0        0        0     3275 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/pretty-quick/dist/scms/git.js
--rw-rw-rw-   0        0        0     1605 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/pretty-quick/dist/scms/hg.js
--rw-rw-rw-   0        0        0     1423 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/pretty-quick/dist/scms/index.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.602531 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/psl/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.303029 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/psl/dist/
--rw-rw-rw-   0        0        0   162079 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/psl/dist/psl.js
--rw-rw-rw-   0        0        0   136713 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/psl/dist/psl.min.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.604531 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/shiki/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.321530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/shiki/dist/
--rw-rw-rw-   0        0        0    99926 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/shiki/dist/index.browser.mjs
--rw-rw-rw-   0        0        0    10176 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/shiki/dist/index.d.ts
--rw-rw-rw-   0        0        0    74524 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/shiki/dist/index.esm.js
--rw-rw-rw-   0        0        0   100069 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/shiki/dist/index.iife.js
--rw-rw-rw-   0        0        0    74853 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/shiki/dist/index.js
--rw-rw-rw-   0        0        0   100111 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/shiki/dist/index.jsdelivr.iife.js
--rw-rw-rw-   0        0        0   100100 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/shiki/dist/index.unpkg.iife.js
--rw-rw-rw-   0        0        0   471543 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/shiki/dist/onig.wasm
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.606030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/source-map/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.335030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/source-map/dist/
--rw-rw-rw-   0        0        0   272874 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/source-map/dist/source-map.debug.js
--rw-rw-rw-   0        0        0   106973 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/source-map/dist/source-map.js
--rw-rw-rw-   0        0        0    27111 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/source-map/dist/source-map.min.js
--rw-rw-rw-   0        0        0   257409 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/source-map/dist/source-map.min.js.map
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.608030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/terser/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.348030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/terser/dist/
--rw-rw-rw-   0        0        0   964344 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/terser/dist/bundle.min.js
--rw-rw-rw-   0        0        0      284 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/terser/dist/package.json
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.613031 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.624530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/
--rw-rw-rw-   0        0        0       31 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/bin-cwd.d.ts
--rw-rw-rw-   0        0        0      215 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/bin-cwd.js
--rw-rw-rw-   0        0        0      305 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/bin-cwd.js.map
--rw-rw-rw-   0        0        0       31 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/bin-esm.d.ts
--rw-rw-rw-   0        0        0      211 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/bin-esm.js
--rw-rw-rw-   0        0        0      301 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/bin-esm.js.map
--rw-rw-rw-   0        0        0       31 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/bin-script-deprecated.d.ts
--rw-rw-rw-   0        0        0      363 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/bin-script-deprecated.js
--rw-rw-rw-   0        0        0      535 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/bin-script-deprecated.js.map
--rw-rw-rw-   0        0        0       31 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/bin-script.d.ts
--rw-rw-rw-   0        0        0      221 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/bin-script.js
--rw-rw-rw-   0        0        0      314 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/bin-script.js.map
--rw-rw-rw-   0        0        0       31 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/bin-transpile.d.ts
--rw-rw-rw-   0        0        0      227 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/bin-transpile.js
--rw-rw-rw-   0        0        0      325 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/bin-transpile.js.map
--rw-rw-rw-   0        0        0      513 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/bin.d.ts
--rw-rw-rw-   0        0        0    26506 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/bin.js
--rw-rw-rw-   0        0        0    41981 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/bin.js.map
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.692030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/
--rw-rw-rw-   0        0        0       11 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/argv-payload.d.ts
--rw-rw-rw-   0        0        0      734 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/argv-payload.js
--rw-rw-rw-   0        0        0     1187 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/argv-payload.js.map
--rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/child-entrypoint.d.ts
--rw-rw-rw-   0        0        0     1066 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/child-entrypoint.js
--rw-rw-rw-   0        0        0     1856 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/child-entrypoint.js.map
--rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/child-loader.d.ts
--rw-rw-rw-   0        0        0     1347 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/child-loader.js
--rw-rw-rw-   0        0        0     2103 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/child-loader.js.map
--rw-rw-rw-   0        0        0      305 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/child-require.d.ts
--rw-rw-rw-   0        0        0     1054 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/child-require.js
--rw-rw-rw-   0        0        0     1884 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/child-require.js.map
--rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/spawn-child.d.ts
--rw-rw-rw-   0        0        0     1895 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/spawn-child.js
--rw-rw-rw-   0        0        0     3196 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/spawn-child.js.map
--rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/cjs-resolve-hooks.d.ts
--rw-rw-rw-   0        0        0     1331 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/cjs-resolve-hooks.js
--rw-rw-rw-   0        0        0     2982 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/cjs-resolve-hooks.js.map
--rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/configuration.d.ts
--rw-rw-rw-   0        0        0    13874 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/configuration.js
--rw-rw-rw-   0        0        0    22936 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/configuration.js.map
--rw-rw-rw-   0        0        0     2073 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/esm.d.ts
--rw-rw-rw-   0        0        0    11087 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/esm.js
--rw-rw-rw-   0        0        0    21075 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/esm.js.map
--rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/file-extensions.d.ts
--rw-rw-rw-   0        0        0     5702 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/file-extensions.js
--rw-rw-rw-   0        0        0     9477 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/file-extensions.js.map
--rw-rw-rw-   0        0        0    11689 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/index.d.ts
--rw-rw-rw-   0        0        0    45986 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/index.js
--rw-rw-rw-   0        0        0    89796 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/index.js.map
--rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/module-type-classifier.d.ts
--rw-rw-rw-   0        0        0     2363 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/module-type-classifier.js
--rw-rw-rw-   0        0        0     4897 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/module-type-classifier.js.map
--rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/node-module-type-classifier.d.ts
--rw-rw-rw-   0        0        0     1515 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/node-module-type-classifier.js
--rw-rw-rw-   0        0        0     2169 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/node-module-type-classifier.js.map
--rw-rw-rw-   0        0        0     2888 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/repl.d.ts
--rw-rw-rw-   0        0        0    21715 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/repl.js
--rw-rw-rw-   0        0        0    39064 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/repl.js.map
--rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/resolver-functions.d.ts
--rw-rw-rw-   0        0        0     7574 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/resolver-functions.js
--rw-rw-rw-   0        0        0    13596 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/resolver-functions.js.map
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.771030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/transpilers/
--rw-rw-rw-   0        0        0      470 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/transpilers/swc.d.ts
--rw-rw-rw-   0        0        0     8796 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/transpilers/swc.js
--rw-rw-rw-   0        0        0    14644 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/transpilers/swc.js.map
--rw-rw-rw-   0        0        0     1008 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/transpilers/types.d.ts
--rw-rw-rw-   0        0        0      110 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/transpilers/types.js
--rw-rw-rw-   0        0        0     2176 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/transpilers/types.js.map
--rw-rw-rw-   0        0        0     3305 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/ts-compiler-types.d.ts
--rw-rw-rw-   0        0        0      122 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/ts-compiler-types.js
--rw-rw-rw-   0        0        0     6349 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/ts-compiler-types.js.map
--rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/ts-internals.d.ts
--rw-rw-rw-   0        0        0    12325 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/ts-internals.js
--rw-rw-rw-   0        0        0    22287 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/ts-internals.js.map
--rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/ts-transpile-module.d.ts
--rw-rw-rw-   0        0        0     4941 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/ts-transpile-module.js
--rw-rw-rw-   0        0        0     9092 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/ts-transpile-module.js.map
--rw-rw-rw-   0        0        0      464 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/tsconfig-schema.d.ts
--rw-rw-rw-   0        0        0      120 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/tsconfig-schema.js
--rw-rw-rw-   0        0        0      887 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/tsconfig-schema.js.map
--rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/tsconfigs.d.ts
--rw-rw-rw-   0        0        0     1435 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/tsconfigs.js
--rw-rw-rw-   0        0        0     2442 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/tsconfigs.js.map
--rw-rw-rw-   0        0        0      118 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/util.d.ts
--rw-rw-rw-   0        0        0     6140 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/util.js
--rw-rw-rw-   0        0        0     9523 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/util.js.map
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.616032 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/node_modules/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.614030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/node_modules/acorn-walk/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.777029 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/node_modules/acorn-walk/dist/
--rw-rw-rw-   0        0        0     2605 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/node_modules/acorn-walk/dist/walk.d.ts
--rw-rw-rw-   0        0        0    16002 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/node_modules/acorn-walk/dist/walk.js
--rw-rw-rw-   0        0        0    14559 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/node_modules/acorn-walk/dist/walk.mjs
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.617031 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/node_modules/diff/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.780530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/node_modules/diff/dist/
--rw-rw-rw-   0        0        0    48402 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/node_modules/diff/dist/diff.js
--rw-rw-rw-   0        0        0    16978 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/node_modules/diff/dist/diff.min.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.620031 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.783028 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/
--rw-rw-rw-   0        0        0     1458 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/index.d.ts
--rw-rw-rw-   0        0        0     5753 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/index.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.786030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/
--rw-rw-rw-   0        0        0     3674 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/application.d.ts
--rw-rw-rw-   0        0        0    14980 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/application.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.823529 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/
--rw-rw-rw-   0        0        0      225 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/components.d.ts
--rw-rw-rw-   0        0        0      420 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/components.js
--rw-rw-rw-   0        0        0     4143 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/context.d.ts
--rw-rw-rw-   0        0        0     7550 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/context.js
--rw-rw-rw-   0        0        0      389 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/convert-expression.d.ts
--rw-rw-rw-   0        0        0     1954 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/convert-expression.js
--rw-rw-rw-   0        0        0      437 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/converter-events.d.ts
--rw-rw-rw-   0        0        0      455 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/converter-events.js
--rw-rw-rw-   0        0        0     4748 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/converter.d.ts
--rw-rw-rw-   0        0        0    18456 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/converter.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.833530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/
--rw-rw-rw-   0        0        0      867 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/comment.d.ts
--rw-rw-rw-   0        0        0     9047 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/comment.js
--rw-rw-rw-   0        0        0      167 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/index-signature.d.ts
--rw-rw-rw-   0        0        0     1806 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/index-signature.js
--rw-rw-rw-   0        0        0      976 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/signature.d.ts
--rw-rw-rw-   0        0        0    10164 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/signature.js
--rw-rw-rw-   0        0        0      183 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/index.d.ts
--rw-rw-rw-   0        0        0      873 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/index.js
--rw-rw-rw-   0        0        0      388 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/jsdoc.d.ts
--rw-rw-rw-   0        0        0     4141 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/jsdoc.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.868532 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/
--rw-rw-rw-   0        0        0     2482 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/CategoryPlugin.d.ts
--rw-rw-rw-   0        0        0     9936 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/CategoryPlugin.js
--rw-rw-rw-   0        0        0     2299 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/CommentPlugin.d.ts
--rw-rw-rw-   0        0        0    17773 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/CommentPlugin.js
--rw-rw-rw-   0        0        0     1029 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/DecoratorPlugin.d.ts
--rw-rw-rw-   0        0        0     4975 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/DecoratorPlugin.js
--rw-rw-rw-   0        0        0     2793 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/GroupPlugin.d.ts
--rw-rw-rw-   0        0        0     7239 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/GroupPlugin.js
--rw-rw-rw-   0        0        0     1570 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/ImplementsPlugin.d.ts
--rw-rw-rw-   0        0        0    14961 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/ImplementsPlugin.js
--rw-rw-rw-   0        0        0      921 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/InheritDocPlugin.d.ts
--rw-rw-rw-   0        0        0     4047 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/InheritDocPlugin.js
--rw-rw-rw-   0        0        0      851 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/PackagePlugin.d.ts
--rw-rw-rw-   0        0        0     5284 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/PackagePlugin.js
--rw-rw-rw-   0        0        0     3434 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/SourceLinkPlugin.d.ts
--rw-rw-rw-   0        0        0     9769 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/SourceLinkPlugin.js
--rw-rw-rw-   0        0        0     1712 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/SourcePlugin.d.ts
--rw-rw-rw-   0        0        0     6449 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/SourcePlugin.js
--rw-rw-rw-   0        0        0      825 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/TypePlugin.d.ts
--rw-rw-rw-   0        0        0     4594 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/TypePlugin.js
--rw-rw-rw-   0        0        0      502 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/index.d.ts
--rw-rw-rw-   0        0        0     2171 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/index.js
--rw-rw-rw-   0        0        0      184 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/symbols.d.ts
--rw-rw-rw-   0        0        0    31944 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/symbols.js
--rw-rw-rw-   0        0        0      535 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/types.d.ts
--rw-rw-rw-   0        0        0    31395 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/types.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.882531 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/
--rw-rw-rw-   0        0        0     1121 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/base-path.d.ts
--rw-rw-rw-   0        0        0     3068 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/base-path.js
--rw-rw-rw-   0        0        0      403 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/nodes.d.ts
--rw-rw-rw-   0        0        0     1048 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/nodes.js
--rw-rw-rw-   0        0        0      397 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/reflections.d.ts
--rw-rw-rw-   0        0        0     3415 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/reflections.js
--rw-rw-rw-   0        0        0      135 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/symbols.d.ts
--rw-rw-rw-   0        0        0      380 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/symbols.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.894029 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/
--rw-rw-rw-   0        0        0      823 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/ReflectionCategory.d.ts
--rw-rw-rw-   0        0        0      923 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/ReflectionCategory.js
--rw-rw-rw-   0        0        0     1874 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/ReflectionGroup.d.ts
--rw-rw-rw-   0        0        0     1047 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/ReflectionGroup.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.903033 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/comments/
--rw-rw-rw-   0        0        0     2078 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/comments/comment.d.ts
--rw-rw-rw-   0        0        0     3083 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/comments/comment.js
--rw-rw-rw-   0        0        0       73 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/comments/index.d.ts
--rw-rw-rw-   0        0        0      420 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/comments/index.js
--rw-rw-rw-   0        0        0      541 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/comments/tag.d.ts
--rw-rw-rw-   0        0        0      498 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/comments/tag.js
--rw-rw-rw-   0        0        0      202 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/index.d.ts
--rw-rw-rw-   0        0        0     1067 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/index.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.936530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/
--rw-rw-rw-   0        0        0     8213 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/abstract.d.ts
--rw-rw-rw-   0        0        0    13360 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/abstract.js
--rw-rw-rw-   0        0        0     1486 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/container.d.ts
--rw-rw-rw-   0        0        0     1192 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/container.js
--rw-rw-rw-   0        0        0     4204 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/declaration.d.ts
--rw-rw-rw-   0        0        0     3639 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/declaration.js
--rw-rw-rw-   0        0        0      687 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/index.d.ts
--rw-rw-rw-   0        0        0     2783 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/index.js
--rw-rw-rw-   0        0        0     1052 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/kind.d.ts
--rw-rw-rw-   0        0        0     3535 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/kind.js
--rw-rw-rw-   0        0        0      764 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/parameter.d.ts
--rw-rw-rw-   0        0        0     1078 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/parameter.js
--rw-rw-rw-   0        0        0     3759 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/project.d.ts
--rw-rw-rw-   0        0        0     8239 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/project.js
--rw-rw-rw-   0        0        0     1807 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/reference.d.ts
--rw-rw-rw-   0        0        0     3190 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/reference.js
--rw-rw-rw-   0        0        0     1931 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/signature.d.ts
--rw-rw-rw-   0        0        0     2075 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/signature.js
--rw-rw-rw-   0        0        0      770 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/type-parameter.d.ts
--rw-rw-rw-   0        0        0      765 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/type-parameter.js
--rw-rw-rw-   0        0        0       89 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/utils.d.ts
--rw-rw-rw-   0        0        0     1068 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/utils.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.948031 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/
--rw-rw-rw-   0        0        0     1894 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/directory.d.ts
--rw-rw-rw-   0        0        0     2007 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/directory.js
--rw-rw-rw-   0        0        0     2305 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/file.d.ts
--rw-rw-rw-   0        0        0     1099 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/file.js
--rw-rw-rw-   0        0        0      178 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/index.d.ts
--rw-rw-rw-   0        0        0      652 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/index.js
--rw-rw-rw-   0        0        0      113 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/repository.d.ts
--rw-rw-rw-   0        0        0      366 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/repository.js
--rw-rw-rw-   0        0        0    14055 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/types.d.ts
--rw-rw-rw-   0        0        0    28742 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/types.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.965529 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/
--rw-rw-rw-   0        0        0     1891 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/components.d.ts
--rw-rw-rw-   0        0        0     2489 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/components.js
--rw-rw-rw-   0        0        0     3638 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/events.d.ts
--rw-rw-rw-   0        0        0     2608 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/events.js
--rw-rw-rw-   0        0        0      448 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/index.d.ts
--rw-rw-rw-   0        0        0     1585 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/index.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.968530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/models/
--rw-rw-rw-   0        0        0      379 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/models/UrlMapping.d.ts
--rw-rw-rw-   0        0        0      292 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/models/UrlMapping.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.984529 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/
--rw-rw-rw-   0        0        0      559 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/AssetsPlugin.d.ts
--rw-rw-rw-   0        0        0     2862 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/AssetsPlugin.js
--rw-rw-rw-   0        0        0      596 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/JavascriptIndexPlugin.d.ts
--rw-rw-rw-   0        0        0     4324 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/JavascriptIndexPlugin.js
--rw-rw-rw-   0        0        0      972 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/LegendPlugin.d.ts
--rw-rw-rw-   0        0        0     9734 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/LegendPlugin.js
--rw-rw-rw-   0        0        0     2534 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/MarkedLinksPlugin.d.ts
--rw-rw-rw-   0        0        0     7176 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/MarkedLinksPlugin.js
--rw-rw-rw-   0        0        0      271 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/index.d.ts
--rw-rw-rw-   0        0        0     1172 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/index.js
--rw-rw-rw-   0        0        0     7435 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/renderer.d.ts
--rw-rw-rw-   0        0        0    12106 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/renderer.js
--rw-rw-rw-   0        0        0     1786 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/theme.d.ts
--rw-rw-rw-   0        0        0     1524 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/theme.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.990031 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/
--rw-rw-rw-   0        0        0     2065 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/MarkedPlugin.d.ts
--rw-rw-rw-   0        0        0     7378 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/MarkedPlugin.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.995530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/
--rw-rw-rw-   0        0        0     4357 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/DefaultTheme.d.ts
--rw-rw-rw-   0        0        0    11183 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/DefaultTheme.js
--rw-rw-rw-   0        0        0     4066 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/DefaultThemeRenderContext.d.ts
--rw-rw-rw-   0        0        0     4072 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/DefaultThemeRenderContext.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:54.999030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/layouts/
--rw-rw-rw-   0        0        0      343 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/layouts/default.d.ts
--rw-rw-rw-   0        0        0     2692 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/layouts/default.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.089030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/
--rw-rw-rw-   0        0        0      216 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/analytics.d.ts
--rw-rw-rw-   0        0        0      895 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/analytics.js
--rw-rw-rw-   0        0        0      119 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/anchor-icon.d.ts
--rw-rw-rw-   0        0        0      902 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/anchor-icon.js
--rw-rw-rw-   0        0        0      291 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/breadcrumb.d.ts
--rw-rw-rw-   0        0        0      665 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/breadcrumb.js
--rw-rw-rw-   0        0        0      292 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/comment.d.ts
--rw-rw-rw-   0        0        0     1321 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/comment.js
--rw-rw-rw-   0        0        0      335 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/footer.d.ts
--rw-rw-rw-   0        0        0     2075 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/footer.js
--rw-rw-rw-   0        0        0      336 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/header.d.ts
--rw-rw-rw-   0        0        0     4296 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/header.js
--rw-rw-rw-   0        0        0      298 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/hierarchy.d.ts
--rw-rw-rw-   0        0        0      545 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/hierarchy.js
--rw-rw-rw-   0        0        0      303 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/index.d.ts
--rw-rw-rw-   0        0        0     2442 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/index.js
--rw-rw-rw-   0        0        0      292 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.d.ts
--rw-rw-rw-   0        0        0      303 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.declaration.d.ts
--rw-rw-rw-   0        0        0     1695 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.declaration.js
--rw-rw-rw-   0        0        0      309 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.getterSetter.d.ts
--rw-rw-rw-   0        0        0     1397 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.getterSetter.js
--rw-rw-rw-   0        0        0     1275 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.js
--rw-rw-rw-   0        0        0      304 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.reference.d.ts
--rw-rw-rw-   0        0        0      886 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.reference.js
--rw-rw-rw-   0        0        0      363 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.signature.body.d.ts
--rw-rw-rw-   0        0        0     2395 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.signature.body.js
--rw-rw-rw-   0        0        0      413 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.signature.title.d.ts
--rw-rw-rw-   0        0        0     1852 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.signature.title.js
--rw-rw-rw-   0        0        0      307 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.signatures.d.ts
--rw-rw-rw-   0        0        0      870 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.signatures.js
--rw-rw-rw-   0        0        0      347 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.sources.d.ts
--rw-rw-rw-   0        0        0     1484 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.sources.js
--rw-rw-rw-   0        0        0      293 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/members.d.ts
--rw-rw-rw-   0        0        0      290 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/members.group.d.ts
--rw-rw-rw-   0        0        0     1051 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/members.group.js
--rw-rw-rw-   0        0        0      892 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/members.js
--rw-rw-rw-   0        0        0      334 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/navigation.d.ts
--rw-rw-rw-   0        0        0     4914 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/navigation.js
--rw-rw-rw-   0        0        0      295 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/parameter.d.ts
--rw-rw-rw-   0        0        0     6080 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/parameter.js
--rw-rw-rw-   0        0        0      266 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/type.d.ts
--rw-rw-rw-   0        0        0    17751 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/type.js
--rw-rw-rw-   0        0        0      265 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/typeAndParent.d.ts
--rw-rw-rw-   0        0        0     1448 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/typeAndParent.js
--rw-rw-rw-   0        0        0      319 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/typeParameters.d.ts
--rw-rw-rw-   0        0        0     1014 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/typeParameters.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.095530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/templates/
--rw-rw-rw-   0        0        0      362 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/templates/index.d.ts
--rw-rw-rw-   0        0        0      400 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/templates/index.js
--rw-rw-rw-   0        0        0      361 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/templates/reflection.d.ts
--rw-rw-rw-   0        0        0     3365 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/templates/reflection.js
--rw-rw-rw-   0        0        0     1066 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/lib.d.ts
--rw-rw-rw-   0        0        0     3114 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/lib.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.113031 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/
--rw-rw-rw-   0        0        0     2611 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/components.d.ts
--rw-rw-rw-   0        0        0     1976 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/components.js
--rw-rw-rw-   0        0        0     1072 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/events.d.ts
--rw-rw-rw-   0        0        0      589 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/events.js
--rw-rw-rw-   0        0        0      968 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/index.d.ts
--rw-rw-rw-   0        0        0     5662 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/index.js
--rw-rw-rw-   0        0        0     9064 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/schema.d.ts
--rw-rw-rw-   0        0        0     1203 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/schema.js
--rw-rw-rw-   0        0        0     1291 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializer.d.ts
--rw-rw-rw-   0        0        0     4537 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializer.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.130530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.150530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/comments/
--rw-rw-rw-   0        0        0      511 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/comments/comment-tag.d.ts
--rw-rw-rw-   0        0        0      828 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/comments/comment-tag.js
--rw-rw-rw-   0        0        0      477 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/comments/comment.d.ts
--rw-rw-rw-   0        0        0      986 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/comments/comment.js
--rw-rw-rw-   0        0        0      101 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/comments/index.d.ts
--rw-rw-rw-   0        0        0      504 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/comments/index.js
--rw-rw-rw-   0        0        0      518 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/decorator.d.ts
--rw-rw-rw-   0        0        0     1013 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/decorator.js
--rw-rw-rw-   0        0        0      241 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/index.d.ts
--rw-rw-rw-   0        0        0     1142 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/index.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.187031 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/models/
--rw-rw-rw-   0        0        0      267 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/models/decorator-wrapper.d.ts
--rw-rw-rw-   0        0        0      365 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/models/decorator-wrapper.js
--rw-rw-rw-   0        0        0      125 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/models/index.d.ts
--rw-rw-rw-   0        0        0      576 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/models/index.js
--rw-rw-rw-   0        0        0      307 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/models/source-reference-wrapper.d.ts
--rw-rw-rw-   0        0        0      411 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/models/source-reference-wrapper.js
--rw-rw-rw-   0        0        0      597 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflection-category.d.ts
--rw-rw-rw-   0        0        0     1018 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflection-category.js
--rw-rw-rw-   0        0        0      554 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflection-group.d.ts
--rw-rw-rw-   0        0        0     1126 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflection-group.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.223529 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/
--rw-rw-rw-   0        0        0      423 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/abstract.d.ts
--rw-rw-rw-   0        0        0     1686 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/abstract.js
--rw-rw-rw-   0        0        0      640 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/container.d.ts
--rw-rw-rw-   0        0        0     1116 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/container.js
--rw-rw-rw-   0        0        0      538 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/declaration.d.ts
--rw-rw-rw-   0        0        0     1775 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/declaration.js
--rw-rw-rw-   0        0        0      209 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/index.d.ts
--rw-rw-rw-   0        0        0     1092 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/index.js
--rw-rw-rw-   0        0        0      476 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/parameter.d.ts
--rw-rw-rw-   0        0        0      706 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/parameter.js
--rw-rw-rw-   0        0        0      532 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/reference.d.ts
--rw-rw-rw-   0        0        0      855 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/reference.js
--rw-rw-rw-   0        0        0      476 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/signature.d.ts
--rw-rw-rw-   0        0        0      964 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/signature.js
--rw-rw-rw-   0        0        0      508 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/type-parameter.d.ts
--rw-rw-rw-   0        0        0      759 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/type-parameter.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.236533 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/sources/
--rw-rw-rw-   0        0        0       73 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/sources/index.d.ts
--rw-rw-rw-   0        0        0      362 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/sources/index.js
--rw-rw-rw-   0        0        0      519 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/sources/source-reference.d.ts
--rw-rw-rw-   0        0        0      789 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/sources/source-reference.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.339530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/
--rw-rw-rw-   0        0        0      357 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/abstract.d.ts
--rw-rw-rw-   0        0        0      524 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/abstract.js
--rw-rw-rw-   0        0        0      504 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/array.d.ts
--rw-rw-rw-   0        0        0      684 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/array.js
--rw-rw-rw-   0        0        0      459 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/conditional.d.ts
--rw-rw-rw-   0        0        0      801 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/conditional.js
--rw-rw-rw-   0        0        0      571 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/index.d.ts
--rw-rw-rw-   0        0        0     1688 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/index.js
--rw-rw-rw-   0        0        0      468 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/indexed-access.d.ts
--rw-rw-rw-   0        0        0      656 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/indexed-access.js
--rw-rw-rw-   0        0        0      432 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/inferred.d.ts
--rw-rw-rw-   0        0        0      678 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/inferred.js
--rw-rw-rw-   0        0        0      560 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/intersection.d.ts
--rw-rw-rw-   0        0        0      721 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/intersection.js
--rw-rw-rw-   0        0        0      536 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/intrinsic.d.ts
--rw-rw-rw-   0        0        0      669 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/intrinsic.js
--rw-rw-rw-   0        0        0      388 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/literal.d.ts
--rw-rw-rw-   0        0        0      812 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/literal.js
--rw-rw-rw-   0        0        0      379 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/mapped.d.ts
--rw-rw-rw-   0        0        0      823 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/mapped.js
--rw-rw-rw-   0        0        0      528 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/optional.d.ts
--rw-rw-rw-   0        0        0      699 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/optional.js
--rw-rw-rw-   0        0        0      404 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/predicate.d.ts
--rw-rw-rw-   0        0        0      696 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/predicate.js
--rw-rw-rw-   0        0        0      372 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/query.d.ts
--rw-rw-rw-   0        0        0      548 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/query.js
--rw-rw-rw-   0        0        0      433 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/reference.d.ts
--rw-rw-rw-   0        0        0      935 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/reference.js
--rw-rw-rw-   0        0        0      417 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/reflection.d.ts
--rw-rw-rw-   0        0        0      618 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/reflection.js
--rw-rw-rw-   0        0        0      496 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/rest.d.ts
--rw-rw-rw-   0        0        0      679 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/rest.js
--rw-rw-rw-   0        0        0      452 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/template-literal.d.ts
--rw-rw-rw-   0        0        0      700 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/template-literal.js
--rw-rw-rw-   0        0        0      692 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/tuple.d.ts
--rw-rw-rw-   0        0        0     1138 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/tuple.js
--rw-rw-rw-   0        0        0      428 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/type-operator.d.ts
--rw-rw-rw-   0        0        0      614 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/type-operator.js
--rw-rw-rw-   0        0        0      504 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/union.d.ts
--rw-rw-rw-   0        0        0      686 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/union.js
--rw-rw-rw-   0        0        0      520 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/unknown.d.ts
--rw-rw-rw-   0        0        0      659 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/unknown.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.439030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/
--rw-rw-rw-   0        0        0     2414 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/array.d.ts
--rw-rw-rw-   0        0        0     4474 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/array.js
--rw-rw-rw-   0        0        0     3017 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/component.d.ts
--rw-rw-rw-   0        0        0     5920 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/component.js
--rw-rw-rw-   0        0        0     1659 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/entry-point.d.ts
--rw-rw-rw-   0        0        0    10766 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/entry-point.js
--rw-rw-rw-   0        0        0      304 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/enum.d.ts
--rw-rw-rw-   0        0        0      757 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/enum.js
--rw-rw-rw-   0        0        0     4284 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/events.d.ts
--rw-rw-rw-   0        0        0    12855 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/events.js
--rw-rw-rw-   0        0        0     1403 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/fs.d.ts
--rw-rw-rw-   0        0        0     4427 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/fs.js
--rw-rw-rw-   0        0        0     1421 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/general.d.ts
--rw-rw-rw-   0        0        0      711 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/general.js
--rw-rw-rw-   0        0        0      367 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/highlighter.d.ts
--rw-rw-rw-   0        0        0     6776 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/highlighter.js
--rw-rw-rw-   0        0        0     2325 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/hooks.d.ts
--rw-rw-rw-   0        0        0     3767 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/hooks.js
--rw-rw-rw-   0        0        0     1350 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/index.d.ts
--rw-rw-rw-   0        0        0     6465 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/index.js
--rw-rw-rw-   0        0        0     1894 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/jsx.d.ts
--rw-rw-rw-   0        0        0    25309 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/jsx.elements.d.ts
--rw-rw-rw-   0        0        0      139 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/jsx.elements.js
--rw-rw-rw-   0        0        0     3737 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/jsx.js
--rw-rw-rw-   0        0        0     3550 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/loggers.d.ts
--rw-rw-rw-   0        0        0     7007 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/loggers.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.458529 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/
--rw-rw-rw-   0        0        0    11114 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/declaration.d.ts
--rw-rw-rw-   0        0        0    13000 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/declaration.js
--rw-rw-rw-   0        0        0      205 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/help.d.ts
--rw-rw-rw-   0        0        0     2565 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/help.js
--rw-rw-rw-   0        0        0      652 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/index.d.ts
--rw-rw-rw-   0        0        0     1390 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/index.js
--rw-rw-rw-   0        0        0     8353 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/options.d.ts
--rw-rw-rw-   0        0        0     9136 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/options.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.474533 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/
--rw-rw-rw-   0        0        0      408 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/arguments.d.ts
--rw-rw-rw-   0        0        0     3674 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/arguments.js
--rw-rw-rw-   0        0        0      135 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/index.d.ts
--rw-rw-rw-   0        0        0      664 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/index.js
--rw-rw-rw-   0        0        0      503 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/tsconfig.d.ts
--rw-rw-rw-   0        0        0     3251 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/tsconfig.js
--rw-rw-rw-   0        0        0     1204 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/typedoc.d.ts
--rw-rw-rw-   0        0        0     3498 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/typedoc.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.484532 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/sources/
--rw-rw-rw-   0        0        0       47 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/sources/index.d.ts
--rw-rw-rw-   0        0        0      284 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/sources/index.js
--rw-rw-rw-   0        0        0      126 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/sources/typedoc.d.ts
--rw-rw-rw-   0        0        0    16281 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/sources/typedoc.js
--rw-rw-rw-   0        0        0     1088 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/package-manifest.d.ts
--rw-rw-rw-   0        0        0     9116 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/package-manifest.js
--rw-rw-rw-   0        0        0      387 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/paths.d.ts
--rw-rw-rw-   0        0        0     1094 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/paths.js
--rw-rw-rw-   0        0        0      209 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/plugins.d.ts
--rw-rw-rw-   0        0        0     3942 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/plugins.js
--rw-rw-rw-   0        0        0      576 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/sort.d.ts
--rw-rw-rw-   0        0        0     5191 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/sort.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.498030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/validation/
--rw-rw-rw-   0        0        0      261 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/validation/documentation.d.ts
--rw-rw-rw-   0        0        0     3672 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/validation/documentation.js
--rw-rw-rw-   0        0        0      218 2023-01-09 05:07:14.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/validation/exports.d.ts
--rw-rw-rw-   0        0        0     6277 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/validation/exports.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.649529 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/url-parse/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.506530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/url-parse/dist/
--rw-rw-rw-   0        0        0    21134 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/url-parse/dist/url-parse.js
--rw-rw-rw-   0        0        0     6736 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/url-parse/dist/url-parse.min.js
--rw-rw-rw-   0        0        0     9809 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/url-parse/dist/url-parse.min.js.map
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.650529 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/workerpool/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.521529 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/workerpool/dist/
--rw-rw-rw-   0        0        0     6544 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/workerpool/dist/worker.js
--rw-rw-rw-   0        0        0    10647 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/workerpool/dist/worker.js.map
--rw-rw-rw-   0        0        0    51236 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/workerpool/dist/workerpool.js
--rw-rw-rw-   0        0        0    86665 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/workerpool/dist/workerpool.js.map
--rw-rw-rw-   0        0        0    20624 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/workerpool/dist/workerpool.min.js
--rw-rw-rw-   0        0        0      815 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/workerpool/dist/workerpool.min.js.LICENSE.txt
--rw-rw-rw-   0        0        0    68373 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/workerpool/dist/workerpool.min.js.map
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.652029 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/y18n/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.522529 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/y18n/build/
--rw-rw-rw-   0        0        0     6783 2023-01-09 05:07:11.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/y18n/build/index.cjs
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.525530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/y18n/build/lib/
--rw-rw-rw-   0        0        0      192 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/y18n/build/lib/cjs.js
--rw-rw-rw-   0        0        0     6268 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/y18n/build/lib/index.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.527530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/y18n/build/lib/platform-shims/
--rw-rw-rw-   0        0        0      377 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/y18n/build/lib/platform-shims/node.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.660029 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.539029 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/
--rw-rw-rw-   0        0        0   107596 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/index.cjs
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.569531 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/
--rw-rw-rw-   0        0        0     2477 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/argsert.js
--rw-rw-rw-   0        0        0    15435 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/command.js
--rw-rw-rw-   0        0        0     1392 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/completion-templates.js
--rw-rw-rw-   0        0        0     5529 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/completion.js
--rw-rw-rw-   0        0        0     2190 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/middleware.js
--rw-rw-rw-   0        0        0     1060 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/parse-command.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.572031 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/typings/
--rw-rw-rw-   0        0        0      308 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/typings/common-types.js
--rw-rw-rw-   0        0        0       11 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/typings/yargs-parser-types.js
--rw-rw-rw-   0        0        0    19829 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/usage.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.596530 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/utils/
--rw-rw-rw-   0        0        0     2049 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/utils/apply-extends.js
--rw-rw-rw-   0        0        0      155 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/utils/is-promise.js
--rw-rw-rw-   0        0        0      731 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/utils/levenshtein.js
--rw-rw-rw-   0        0        0      299 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/utils/obj-filter.js
--rw-rw-rw-   0        0        0      436 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/utils/process-argv.js
--rw-rw-rw-   0        0        0      386 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/utils/set-blocking.js
--rw-rw-rw-   0        0        0      321 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/utils/which-module.js
--rw-rw-rw-   0        0        0    12201 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/validation.js
--rw-rw-rw-   0        0        0    42229 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/yargs-factory.js
--rw-rw-rw-   0        0        0      181 2023-01-09 05:07:13.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/yerror.js
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:53.658031 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs-parser/
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.529030 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs-parser/build/
--rw-rw-rw-   0        0        0    41467 2023-01-09 05:07:11.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs-parser/build/index.cjs
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.537029 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs-parser/build/lib/
--rw-rw-rw-   0        0        0     2023 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs-parser/build/lib/index.js
--rw-rw-rw-   0        0        0     1795 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs-parser/build/lib/string-utils.js
--rw-rw-rw-   0        0        0     1004 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs-parser/build/lib/tokenize-arg-string.js
--rw-rw-rw-   0        0        0       11 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs-parser/build/lib/yargs-parser-types.js
--rw-rw-rw-   0        0        0    45688 2023-01-09 05:07:12.000000 monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs-parser/build/lib/yargs-parser.js
--rw-rw-rw-   0        0        0     2234 2023-01-09 05:31:27.000000 monaco-qt-0.1.7/monaco/monaco-editor/package.json
--rw-rw-rw-   0        0        0     3436 2023-01-09 05:46:15.000000 monaco-qt-0.1.7/monaco/monaco_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-03 01:00:55.646530 monaco-qt-0.1.7/monaco_qt.egg-info/
--rw-rw-rw-   0        0        0     1603 2023-04-03 01:00:53.000000 monaco-qt-0.1.7/monaco_qt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    56210 2023-04-03 01:00:53.000000 monaco-qt-0.1.7/monaco_qt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 01:00:53.000000 monaco-qt-0.1.7/monaco_qt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-03 01:00:53.000000 monaco-qt-0.1.7/monaco_qt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2023-04-03 01:00:53.000000 monaco-qt-0.1.7/monaco_qt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-03 01:00:53.000000 monaco-qt-0.1.7/monaco_qt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-03 01:00:55.649029 monaco-qt-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1528 2023-04-03 01:00:27.000000 monaco-qt-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:34.667395 monaco_qt-0.1.8/
+-rw-rw-rw-   0        0        0     1624 2024-06-01 21:42:34.666395 monaco_qt-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      835 2023-01-09 05:00:48.000000 monaco_qt-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.700852 monaco_qt-0.1.8/monaco/
+-rw-rw-rw-   0        0        0      174 2023-04-03 00:23:27.000000 monaco_qt-0.1.8/monaco/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.702851 monaco_qt-0.1.8/monaco/_pyinstaller/
+-rw-rw-rw-   0        0        0        0 2023-04-03 00:24:25.000000 monaco_qt-0.1.8/monaco/_pyinstaller/__init__.py
+-rw-rw-rw-   0        0        0       96 2023-04-03 00:27:34.000000 monaco_qt-0.1.8/monaco/_pyinstaller/hook-monaco.py
+-rw-rw-rw-   0        0        0      612 2022-07-12 00:37:02.000000 monaco_qt-0.1.8/monaco/index.html
+-rw-rw-rw-   0        0        0     1681 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/index.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.713850 monaco_qt-0.1.8/monaco/monaco-editor/
+-rw-rw-rw-   0        0        0    96665 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1119 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/LICENSE
+-rw-rw-rw-   0        0        0     5116 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/README.md
+-rw-rw-rw-   0        0        0    63512 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/ThirdPartyNotices.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.524961 monaco_qt-0.1.8/monaco/monaco-editor/min/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.714851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.527958 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/base/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.526959 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/base/browser/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.526959 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/base/browser/ui/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.527958 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/base/browser/ui/codicons/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.715849 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/base/browser/ui/codicons/codicon/
+-rw-rw-rw-   0        0        0    70776 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/base/browser/ui/codicons/codicon/codicon.ttf
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.717849 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/base/worker/
+-rw-rw-rw-   0        0        0   283886 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/base/worker/workerMain.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.589851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.720852 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/abap/
+-rw-rw-rw-   0        0        0    15097 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/abap/abap.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.721852 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/apex/
+-rw-rw-rw-   0        0        0     4886 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/apex/apex.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.722851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/azcli/
+-rw-rw-rw-   0        0        0     1784 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/azcli/azcli.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.723850 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/bat/
+-rw-rw-rw-   0        0        0     2777 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/bat/bat.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.724850 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/bicep/
+-rw-rw-rw-   0        0        0     3473 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/bicep/bicep.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.726853 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/cameligo/
+-rw-rw-rw-   0        0        0     3127 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/cameligo/cameligo.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.728853 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/clojure/
+-rw-rw-rw-   0        0        0    10583 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/clojure/clojure.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.730851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/coffee/
+-rw-rw-rw-   0        0        0     4528 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/coffee/coffee.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.731852 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/cpp/
+-rw-rw-rw-   0        0        0     6380 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/cpp/cpp.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.733853 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/csharp/
+-rw-rw-rw-   0        0        0     5462 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/csharp/csharp.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.734851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/csp/
+-rw-rw-rw-   0        0        0     2351 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/csp/csp.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.735850 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/css/
+-rw-rw-rw-   0        0        0     5441 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/css/css.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.736850 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/dart/
+-rw-rw-rw-   0        0        0     5184 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/dart/dart.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.738850 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/dockerfile/
+-rw-rw-rw-   0        0        0     2815 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/dockerfile/dockerfile.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.739850 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/ecl/
+-rw-rw-rw-   0        0        0     6274 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/ecl/ecl.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.741851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/elixir/
+-rw-rw-rw-   0        0        0    10697 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/elixir/elixir.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.743849 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/flow9/
+-rw-rw-rw-   0        0        0     2746 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/flow9/flow9.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.744850 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/freemarker2/
+-rw-rw-rw-   0        0        0    17278 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/freemarker2/freemarker2.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.746851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/fsharp/
+-rw-rw-rw-   0        0        0     3921 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/fsharp/fsharp.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.748853 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/go/
+-rw-rw-rw-   0        0        0     3587 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/go/go.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.750851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/graphql/
+-rw-rw-rw-   0        0        0     3200 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/graphql/graphql.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.751850 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/handlebars/
+-rw-rw-rw-   0        0        0     7954 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/handlebars/handlebars.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.753850 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/hcl/
+-rw-rw-rw-   0        0        0     4522 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/hcl/hcl.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.754851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/html/
+-rw-rw-rw-   0        0        0     6006 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/html/html.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.756851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/ini/
+-rw-rw-rw-   0        0        0     2033 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/ini/ini.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.757855 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/java/
+-rw-rw-rw-   0        0        0     4155 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/java/java.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.759851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/javascript/
+-rw-rw-rw-   0        0        0     7235 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/javascript/javascript.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.761852 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/julia/
+-rw-rw-rw-   0        0        0     8163 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/julia/julia.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.763851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/kotlin/
+-rw-rw-rw-   0        0        0     4377 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/kotlin/kotlin.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.764852 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/less/
+-rw-rw-rw-   0        0        0     4830 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/less/less.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.766849 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/lexon/
+-rw-rw-rw-   0        0        0     3373 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/lexon/lexon.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.767851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/liquid/
+-rw-rw-rw-   0        0        0     5132 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/liquid/liquid.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.769852 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/lua/
+-rw-rw-rw-   0        0        0     3055 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/lua/lua.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.770850 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/m3/
+-rw-rw-rw-   0        0        0     3747 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/m3/m3.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.771852 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/markdown/
+-rw-rw-rw-   0        0        0     4730 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/markdown/markdown.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.773855 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/mips/
+-rw-rw-rw-   0        0        0     3513 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/mips/mips.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.775850 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/msdax/
+-rw-rw-rw-   0        0        0     5848 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/msdax/msdax.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.777850 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/mysql/
+-rw-rw-rw-   0        0        0    12193 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/mysql/mysql.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.778849 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/objective-c/
+-rw-rw-rw-   0        0        0     3350 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/objective-c/objective-c.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.779848 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/pascal/
+-rw-rw-rw-   0        0        0     3933 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/pascal/pascal.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.781852 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/pascaligo/
+-rw-rw-rw-   0        0        0     2944 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/pascaligo/pascaligo.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.784850 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/perl/
+-rw-rw-rw-   0        0        0     9189 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/perl/perl.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.785850 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/pgsql/
+-rw-rw-rw-   0        0        0    14340 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/pgsql/pgsql.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.786849 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/php/
+-rw-rw-rw-   0        0        0     8959 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/php/php.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.788851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/pla/
+-rw-rw-rw-   0        0        0     2615 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/pla/pla.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.790851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/postiats/
+-rw-rw-rw-   0        0        0     8798 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/postiats/postiats.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.791849 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/powerquery/
+-rw-rw-rw-   0        0        0    17885 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/powerquery/powerquery.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.792850 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/powershell/
+-rw-rw-rw-   0        0        0     4215 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/powershell/powershell.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.793851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/protobuf/
+-rw-rw-rw-   0        0        0     9989 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/protobuf/protobuf.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.796852 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/pug/
+-rw-rw-rw-   0        0        0     5760 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/pug/pug.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.797851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/python/
+-rw-rw-rw-   0        0        0     4759 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/python/python.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.798849 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/qsharp/
+-rw-rw-rw-   0        0        0     3862 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/qsharp/qsharp.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.799849 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/r/
+-rw-rw-rw-   0        0        0     4059 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/r/r.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.800849 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/razor/
+-rw-rw-rw-   0        0        0     9948 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/razor/razor.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.802852 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/redis/
+-rw-rw-rw-   0        0        0     4492 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/redis/redis.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.803852 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/redshift/
+-rw-rw-rw-   0        0        0    12742 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/redshift/redshift.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.805850 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/restructuredtext/
+-rw-rw-rw-   0        0        0     4851 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/restructuredtext/restructuredtext.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.807853 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/ruby/
+-rw-rw-rw-   0        0        0     9438 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/ruby/ruby.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.809851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/rust/
+-rw-rw-rw-   0        0        0     5094 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/rust/rust.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.811852 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/sb/
+-rw-rw-rw-   0        0        0     2759 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/sb/sb.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.812851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/scala/
+-rw-rw-rw-   0        0        0     8254 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/scala/scala.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.813849 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/scheme/
+-rw-rw-rw-   0        0        0     2705 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/scheme/scheme.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.814849 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/scss/
+-rw-rw-rw-   0        0        0     7342 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/scss/scss.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.817853 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/shell/
+-rw-rw-rw-   0        0        0     4009 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/shell/shell.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.819851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/solidity/
+-rw-rw-rw-   0        0        0    19539 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/solidity/solidity.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.820852 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/sophia/
+-rw-rw-rw-   0        0        0     3702 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/sophia/sophia.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.821852 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/sparql/
+-rw-rw-rw-   0        0        0     3490 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/sparql/sparql.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.823851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/sql/
+-rw-rw-rw-   0        0        0    11229 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/sql/sql.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.824851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/st/
+-rw-rw-rw-   0        0        0     8320 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/st/st.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.826850 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/swift/
+-rw-rw-rw-   0        0        0     6111 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/swift/swift.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.827849 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/systemverilog/
+-rw-rw-rw-   0        0        0     8555 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/systemverilog/systemverilog.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.828849 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/tcl/
+-rw-rw-rw-   0        0        0     4503 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/tcl/tcl.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.829850 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/twig/
+-rw-rw-rw-   0        0        0     6906 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/twig/twig.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.831852 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/typescript/
+-rw-rw-rw-   0        0        0     6567 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/typescript/typescript.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.833851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/vb/
+-rw-rw-rw-   0        0        0     6721 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/vb/vb.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.834850 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/xml/
+-rw-rw-rw-   0        0        0     3579 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/xml/xml.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.835850 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/yaml/
+-rw-rw-rw-   0        0        0     4478 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/yaml/yaml.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.862850 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/
+-rw-rw-rw-   0        0        0    77307 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.css
+-rw-rw-rw-   0        0        0  2918322 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.js
+-rw-rw-rw-   0        0        0    96566 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.nls.de.js
+-rw-rw-rw-   0        0        0    97319 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.nls.es.js
+-rw-rw-rw-   0        0        0   106136 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.nls.fr.js
+-rw-rw-rw-   0        0        0    99139 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.nls.it.js
+-rw-rw-rw-   0        0        0   199359 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.nls.ja.js
+-rw-rw-rw-   0        0        0    77655 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.nls.js
+-rw-rw-rw-   0        0        0   165466 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.nls.ko.js
+-rw-rw-rw-   0        0        0   412899 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.nls.ru.js
+-rw-rw-rw-   0        0        0   126176 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.nls.zh-cn.js
+-rw-rw-rw-   0        0        0   128706 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.nls.zh-tw.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.593853 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/language/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.865851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/language/css/
+-rw-rw-rw-   0        0        0    34114 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/language/css/cssMode.js
+-rw-rw-rw-   0        0        0   752287 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/language/css/cssWorker.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.869851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/language/html/
+-rw-rw-rw-   0        0        0    34867 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/language/html/htmlMode.js
+-rw-rw-rw-   0        0        0   446862 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/language/html/htmlWorker.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.874851 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/language/json/
+-rw-rw-rw-   0        0        0    40310 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/language/json/jsonMode.js
+-rw-rw-rw-   0        0        0   129160 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/language/json/jsonWorker.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.876850 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/language/typescript/
+-rw-rw-rw-   0        0        0    22808 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/language/typescript/tsMode.js
+-rw-rw-rw-   0        0        0  4761155 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/language/typescript/tsWorker.js
+-rw-rw-rw-   0        0        0    33214 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/min/vs/loader.js
+-rw-rw-rw-   0        0        0   296660 2022-07-11 15:07:46.000000 monaco_qt-0.1.8/monaco/monaco-editor/monaco.d.ts
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.678851 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.596851 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.596851 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.597851 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.597851 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.598849 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.950702 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/
+-rw-rw-rw-   0        0        0    19414 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.mjs
+-rw-rw-rw-   0        0        0    15178 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.mjs.map
+-rw-rw-rw-   0        0        0    22396 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.umd.js
+-rw-rw-rw-   0        0        0    15515 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.umd.js.map
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:23.096701 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/
+-rw-rw-rw-   0        0        0      319 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/any-map.d.ts
+-rw-rw-rw-   0        0        0     1546 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/binary-search.d.ts
+-rw-rw-rw-   0        0        0      349 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/by-source.d.ts
+-rw-rw-rw-   0        0        0       82 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/resolve.d.ts
+-rw-rw-rw-   0        0        0      166 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/sort.d.ts
+-rw-rw-rw-   0        0        0      783 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/sourcemap-segment.d.ts
+-rw-rw-rw-   0        0        0      152 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/strip-filename.d.ts
+-rw-rw-rw-   0        0        0     3614 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/trace-mapping.d.ts
+-rw-rw-rw-   0        0        0     2218 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/types.d.ts
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.611850 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.602856 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:23.185703 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/
+-rw-rw-rw-   0        0        0     9207 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/gen-mapping.mjs
+-rw-rw-rw-   0        0        0    21472 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/gen-mapping.mjs.map
+-rw-rw-rw-   0        0        0    10824 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/gen-mapping.umd.js
+-rw-rw-rw-   0        0        0    21687 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/gen-mapping.umd.js.map
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:23.229700 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/types/
+-rw-rw-rw-   0        0        0     3672 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/types/gen-mapping.d.ts
+-rw-rw-rw-   0        0        0      569 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/types/sourcemap-segment.d.ts
+-rw-rw-rw-   0        0        0      820 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/types/types.d.ts
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.603851 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:23.320275 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/dist/
+-rw-rw-rw-   0        0        0     9040 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/dist/resolve-uri.mjs
+-rw-rw-rw-   0        0        0    14811 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/dist/resolve-uri.mjs.map
+-rw-rw-rw-   0        0        0    10337 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/dist/resolve-uri.umd.js
+-rw-rw-rw-   0        0        0    14848 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/dist/resolve-uri.umd.js.map
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:23.328741 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/dist/types/
+-rw-rw-rw-   0        0        0      150 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/dist/types/resolve-uri.d.ts
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.605850 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/set-array/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:23.431621 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/
+-rw-rw-rw-   0        0        0     1475 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/set-array.mjs
+-rw-rw-rw-   0        0        0     2631 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/set-array.mjs.map
+-rw-rw-rw-   0        0        0     2153 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/set-array.umd.js
+-rw-rw-rw-   0        0        0     2675 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/set-array.umd.js.map
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:23.440620 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/types/
+-rw-rw-rw-   0        0        0      971 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/types/set-array.d.ts
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.608852 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/source-map/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:23.528620 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/
+-rw-rw-rw-   0        0        0    32713 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/source-map.mjs
+-rw-rw-rw-   0        0        0    77701 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/source-map.mjs.map
+-rw-rw-rw-   0        0        0    36850 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/source-map.umd.js
+-rw-rw-rw-   0        0        0    77717 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/source-map.umd.js.map
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:23.541624 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/types/
+-rw-rw-rw-   0        0        0     1443 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/types/source-map.d.ts
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.610852 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:23.617143 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/dist/
+-rw-rw-rw-   0        0        0     5279 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/dist/sourcemap-codec.mjs
+-rw-rw-rw-   0        0        0     6099 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/dist/sourcemap-codec.mjs.map
+-rw-rw-rw-   0        0        0     6390 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/dist/sourcemap-codec.umd.js
+-rw-rw-rw-   0        0        0     6145 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/dist/sourcemap-codec.umd.js.map
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:23.632141 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/dist/types/
+-rw-rw-rw-   0        0        0      455 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/dist/types/sourcemap-codec.d.ts
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.611850 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:23.736260 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/
+-rw-rw-rw-   0        0        0    21727 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.mjs
+-rw-rw-rw-   0        0        0    47615 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.mjs.map
+-rw-rw-rw-   0        0        0    24859 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.umd.js
+-rw-rw-rw-   0        0        0    47881 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.umd.js.map
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:23.794260 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/
+-rw-rw-rw-   0        0        0      319 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/any-map.d.ts
+-rw-rw-rw-   0        0        0     1546 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/binary-search.d.ts
+-rw-rw-rw-   0        0        0      349 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/by-source.d.ts
+-rw-rw-rw-   0        0        0       82 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/resolve.d.ts
+-rw-rw-rw-   0        0        0      166 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/sort.d.ts
+-rw-rw-rw-   0        0        0      783 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/sourcemap-segment.d.ts
+-rw-rw-rw-   0        0        0      152 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/strip-filename.d.ts
+-rw-rw-rw-   0        0        0     3730 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/trace-mapping.d.ts
+-rw-rw-rw-   0        0        0     2656 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/types.d.ts
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.612851 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@tootallnate/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.613851 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@tootallnate/once/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:23.912773 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@tootallnate/once/dist/
+-rw-rw-rw-   0        0        0      407 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@tootallnate/once/dist/index.d.ts
+-rw-rw-rw-   0        0        0      846 2023-01-09 05:07:11.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@tootallnate/once/dist/index.js
+-rw-rw-rw-   0        0        0      824 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@tootallnate/once/dist/index.js.map
+-rw-rw-rw-   0        0        0     7853 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@tootallnate/once/dist/overloaded-parameters.d.ts
+-rw-rw-rw-   0        0        0      126 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@tootallnate/once/dist/overloaded-parameters.js
+-rw-rw-rw-   0        0        0      134 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@tootallnate/once/dist/overloaded-parameters.js.map
+-rw-rw-rw-   0        0        0     1015 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@tootallnate/once/dist/types.d.ts
+-rw-rw-rw-   0        0        0      110 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@tootallnate/once/dist/types.js
+-rw-rw-rw-   0        0        0      102 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@tootallnate/once/dist/types.js.map
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.614853 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@typescript/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.616854 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@typescript/vfs/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:24.163323 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@typescript/vfs/dist/
+-rw-rw-rw-   0        0        0     4989 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@typescript/vfs/dist/index.d.ts
+-rw-rw-rw-   0        0        0      184 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@typescript/vfs/dist/index.js
+-rw-rw-rw-   0        0        0    21880 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.cjs.development.js
+-rw-rw-rw-   0        0        0    40397 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.cjs.development.js.map
+-rw-rw-rw-   0        0        0     9069 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.cjs.production.min.js
+-rw-rw-rw-   0        0        0    30984 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.cjs.production.min.js.map
+-rw-rw-rw-   0        0        0    21435 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.esm.js
+-rw-rw-rw-   0        0        0    40372 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.esm.js.map
+-rw-rw-rw-   0        0        0    21755 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.globals.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.620852 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:25.239952 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn/dist/
+-rw-rw-rw-   0        0        0     6200 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn/dist/acorn.d.ts
+-rw-rw-rw-   0        0        0   217774 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn/dist/acorn.js
+-rw-rw-rw-   0        0        0   207097 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn/dist/acorn.mjs
+-rw-rw-rw-   0        0        0       49 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn/dist/acorn.mjs.d.ts
+-rw-rw-rw-   0        0        0     3285 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn/dist/bin.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.617852 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-globals/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.618851 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-globals/node_modules/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.618851 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:24.686741 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/
+-rw-rw-rw-   0        0        0     5224 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/acorn.d.ts
+-rw-rw-rw-   0        0        0   200010 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/acorn.js
+-rw-rw-rw-   0        0        0   392402 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/acorn.js.map
+-rw-rw-rw-   0        0        0   190128 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/acorn.mjs
+-rw-rw-rw-   0        0        0       49 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/acorn.mjs.d.ts
+-rw-rw-rw-   0        0        0   392368 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/acorn.mjs.map
+-rw-rw-rw-   0        0        0     2291 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/bin.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.619851 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-walk/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:24.792438 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-walk/dist/
+-rw-rw-rw-   0        0        0     2559 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-walk/dist/walk.d.ts
+-rw-rw-rw-   0        0        0    16001 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-walk/dist/walk.js
+-rw-rw-rw-   0        0        0    29054 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-walk/dist/walk.js.map
+-rw-rw-rw-   0        0        0    14560 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-walk/dist/walk.mjs
+-rw-rw-rw-   0        0        0    29031 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-walk/dist/walk.mjs.map
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.623853 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/agent-base/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.624851 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/agent-base/dist/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:25.349102 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/agent-base/dist/src/
+-rw-rw-rw-   0        0        0     3197 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/agent-base/dist/src/index.d.ts
+-rw-rw-rw-   0        0        0     7910 2023-01-09 05:07:11.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/agent-base/dist/src/index.js
+-rw-rw-rw-   0        0        0     5824 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/agent-base/dist/src/index.js.map
+-rw-rw-rw-   0        0        0      299 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/agent-base/dist/src/promisify.d.ts
+-rw-rw-rw-   0        0        0      495 2023-01-09 05:07:11.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/agent-base/dist/src/promisify.js
+-rw-rw-rw-   0        0        0      499 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/agent-base/dist/src/promisify.js.map
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.625850 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/cliui/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:25.366949 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/cliui/build/
+-rw-rw-rw-   0        0        0     9953 2023-01-09 05:07:11.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/cliui/build/index.cjs
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:25.406981 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/cliui/build/lib/
+-rw-rw-rw-   0        0        0     9667 2023-01-09 05:07:11.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/cliui/build/lib/index.js
+-rw-rw-rw-   0        0        0     1011 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/cliui/build/lib/string-utils.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.626850 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/diff/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:25.438981 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/diff/dist/
+-rw-rw-rw-   0        0        0    48351 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/diff/dist/diff.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.627850 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/escalade/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:25.473985 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/escalade/dist/
+-rw-rw-rw-   0        0        0      534 2023-01-09 05:07:11.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/escalade/dist/index.js
+-rw-rw-rw-   0        0        0      517 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/escalade/dist/index.mjs
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.629854 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/esprima/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:25.541499 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/esprima/dist/
+-rw-rw-rw-   0        0        0   283567 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/esprima/dist/esprima.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.631305 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/http-proxy-agent/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:25.641497 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/http-proxy-agent/dist/
+-rw-rw-rw-   0        0        0      941 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/http-proxy-agent/dist/agent.d.ts
+-rw-rw-rw-   0        0        0     6608 2023-01-09 05:07:11.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/http-proxy-agent/dist/agent.js
+-rw-rw-rw-   0        0        0     3781 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/http-proxy-agent/dist/agent.js.map
+-rw-rw-rw-   0        0        0      872 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/http-proxy-agent/dist/index.d.ts
+-rw-rw-rw-   0        0        0      571 2023-01-09 05:07:11.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/http-proxy-agent/dist/index.js
+-rw-rw-rw-   0        0        0      359 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/http-proxy-agent/dist/index.js.map
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.631850 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/https-proxy-agent/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:25.804687 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/https-proxy-agent/dist/
+-rw-rw-rw-   0        0        0     1126 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/https-proxy-agent/dist/agent.d.ts
+-rw-rw-rw-   0        0        0     7841 2023-01-09 05:07:11.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/https-proxy-agent/dist/agent.js
+-rw-rw-rw-   0        0        0     4367 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/https-proxy-agent/dist/agent.js.map
+-rw-rw-rw-   0        0        0      970 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/https-proxy-agent/dist/index.d.ts
+-rw-rw-rw-   0        0        0      579 2023-01-09 05:07:11.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/https-proxy-agent/dist/index.js
+-rw-rw-rw-   0        0        0      362 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/https-proxy-agent/dist/index.js.map
+-rw-rw-rw-   0        0        0      233 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/https-proxy-agent/dist/parse-proxy-response.d.ts
+-rw-rw-rw-   0        0        0     2460 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/https-proxy-agent/dist/parse-proxy-response.js
+-rw-rw-rw-   0        0        0     1904 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/https-proxy-agent/dist/parse-proxy-response.js.map
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.632850 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/human-signals/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.632850 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/human-signals/build/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:25.919963 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/human-signals/build/src/
+-rw-rw-rw-   0        0        0     4268 2023-01-09 05:07:11.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/human-signals/build/src/core.js
+-rw-rw-rw-   0        0        0    10551 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/human-signals/build/src/core.js.map
+-rw-rw-rw-   0        0        0     1528 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/human-signals/build/src/main.js
+-rw-rw-rw-   0        0        0     4047 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/human-signals/build/src/main.js.map
+-rw-rw-rw-   0        0        0      590 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/human-signals/build/src/realtime.js
+-rw-rw-rw-   0        0        0     1245 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/human-signals/build/src/realtime.js.map
+-rw-rw-rw-   0        0        0      778 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/human-signals/build/src/signals.js
+-rw-rw-rw-   0        0        0     2054 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/human-signals/build/src/signals.js.map
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.633851 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/js-yaml/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:26.041688 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/js-yaml/dist/
+-rw-rw-rw-   0        0        0   114359 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/js-yaml/dist/js-yaml.js
+-rw-rw-rw-   0        0        0    39430 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/js-yaml/dist/js-yaml.min.js
+-rw-rw-rw-   0        0        0   107533 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/js-yaml/dist/js-yaml.mjs
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.634850 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/lunr/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:26.129687 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/lunr/build/
+-rw-rw-rw-   0        0        0      142 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/lunr/build/bower.json.template
+-rw-rw-rw-   0        0        0      204 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/lunr/build/component.json.template
+-rw-rw-rw-   0        0        0      165 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/lunr/build/jsdoc.conf.json
+-rw-rw-rw-   0        0        0      726 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/lunr/build/package.json.template
+-rw-rw-rw-   0        0        0     1758 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/lunr/build/release.sh
+-rw-rw-rw-   0        0        0      873 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/lunr/build/wrapper_end
+-rw-rw-rw-   0        0        0      175 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/lunr/build/wrapper_start
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.636854 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/make-error/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:26.156152 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/make-error/dist/
+-rw-rw-rw-   0        0        0     2793 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/make-error/dist/make-error.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.637853 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/nwsapi/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:26.156686 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/nwsapi/dist/
+-rw-rw-rw-   0        0        0        0 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/nwsapi/dist/lint.log
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.638851 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/pretty-quick/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:26.239687 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/pretty-quick/dist/
+-rw-rw-rw-   0        0        0      698 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/pretty-quick/dist/createIgnorer.js
+-rw-rw-rw-   0        0        0      670 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/pretty-quick/dist/createMatcher.js
+-rw-rw-rw-   0        0        0     2817 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/pretty-quick/dist/index.js
+-rw-rw-rw-   0        0        0      389 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/pretty-quick/dist/isSupportedExtension.js
+-rw-rw-rw-   0        0        0     1980 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/pretty-quick/dist/processFiles.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:26.295688 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/pretty-quick/dist/scms/
+-rw-rw-rw-   0        0        0     3275 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/pretty-quick/dist/scms/git.js
+-rw-rw-rw-   0        0        0     1605 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/pretty-quick/dist/scms/hg.js
+-rw-rw-rw-   0        0        0     1423 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/pretty-quick/dist/scms/index.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.639850 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/psl/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:26.393198 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/psl/dist/
+-rw-rw-rw-   0        0        0   162079 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/psl/dist/psl.js
+-rw-rw-rw-   0        0        0   136713 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/psl/dist/psl.min.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.640850 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/shiki/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:26.660769 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/shiki/dist/
+-rw-rw-rw-   0        0        0    99926 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/shiki/dist/index.browser.mjs
+-rw-rw-rw-   0        0        0    10176 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/shiki/dist/index.d.ts
+-rw-rw-rw-   0        0        0    74524 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/shiki/dist/index.esm.js
+-rw-rw-rw-   0        0        0   100069 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/shiki/dist/index.iife.js
+-rw-rw-rw-   0        0        0    74853 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/shiki/dist/index.js
+-rw-rw-rw-   0        0        0   100111 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/shiki/dist/index.jsdelivr.iife.js
+-rw-rw-rw-   0        0        0   100100 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/shiki/dist/index.unpkg.iife.js
+-rw-rw-rw-   0        0        0   471543 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/shiki/dist/onig.wasm
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.641850 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/source-map/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:26.831887 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/source-map/dist/
+-rw-rw-rw-   0        0        0   272874 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/source-map/dist/source-map.debug.js
+-rw-rw-rw-   0        0        0   106973 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/source-map/dist/source-map.js
+-rw-rw-rw-   0        0        0    27111 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/source-map/dist/source-map.min.js
+-rw-rw-rw-   0        0        0   257409 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/source-map/dist/source-map.min.js.map
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.643853 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/terser/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:26.885880 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/terser/dist/
+-rw-rw-rw-   0        0        0   964344 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/terser/dist/bundle.min.js
+-rw-rw-rw-   0        0        0      284 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/terser/dist/package.json
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.646852 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:27.660650 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/
+-rw-rw-rw-   0        0        0       31 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/bin-cwd.d.ts
+-rw-rw-rw-   0        0        0      215 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/bin-cwd.js
+-rw-rw-rw-   0        0        0      305 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/bin-cwd.js.map
+-rw-rw-rw-   0        0        0       31 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/bin-esm.d.ts
+-rw-rw-rw-   0        0        0      211 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/bin-esm.js
+-rw-rw-rw-   0        0        0      301 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/bin-esm.js.map
+-rw-rw-rw-   0        0        0       31 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/bin-script-deprecated.d.ts
+-rw-rw-rw-   0        0        0      363 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/bin-script-deprecated.js
+-rw-rw-rw-   0        0        0      535 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/bin-script-deprecated.js.map
+-rw-rw-rw-   0        0        0       31 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/bin-script.d.ts
+-rw-rw-rw-   0        0        0      221 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/bin-script.js
+-rw-rw-rw-   0        0        0      314 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/bin-script.js.map
+-rw-rw-rw-   0        0        0       31 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/bin-transpile.d.ts
+-rw-rw-rw-   0        0        0      227 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/bin-transpile.js
+-rw-rw-rw-   0        0        0      325 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/bin-transpile.js.map
+-rw-rw-rw-   0        0        0      513 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/bin.d.ts
+-rw-rw-rw-   0        0        0    26506 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/bin.js
+-rw-rw-rw-   0        0        0    41981 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/bin.js.map
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:27.816143 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/
+-rw-rw-rw-   0        0        0       11 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/argv-payload.d.ts
+-rw-rw-rw-   0        0        0      734 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/argv-payload.js
+-rw-rw-rw-   0        0        0     1187 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/argv-payload.js.map
+-rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/child-entrypoint.d.ts
+-rw-rw-rw-   0        0        0     1066 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/child-entrypoint.js
+-rw-rw-rw-   0        0        0     1856 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/child-entrypoint.js.map
+-rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/child-loader.d.ts
+-rw-rw-rw-   0        0        0     1347 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/child-loader.js
+-rw-rw-rw-   0        0        0     2103 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/child-loader.js.map
+-rw-rw-rw-   0        0        0      305 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/child-require.d.ts
+-rw-rw-rw-   0        0        0     1054 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/child-require.js
+-rw-rw-rw-   0        0        0     1884 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/child-require.js.map
+-rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/spawn-child.d.ts
+-rw-rw-rw-   0        0        0     1895 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/spawn-child.js
+-rw-rw-rw-   0        0        0     3196 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/spawn-child.js.map
+-rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/cjs-resolve-hooks.d.ts
+-rw-rw-rw-   0        0        0     1331 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/cjs-resolve-hooks.js
+-rw-rw-rw-   0        0        0     2982 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/cjs-resolve-hooks.js.map
+-rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/configuration.d.ts
+-rw-rw-rw-   0        0        0    13874 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/configuration.js
+-rw-rw-rw-   0        0        0    22936 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/configuration.js.map
+-rw-rw-rw-   0        0        0     2073 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/esm.d.ts
+-rw-rw-rw-   0        0        0    11087 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/esm.js
+-rw-rw-rw-   0        0        0    21075 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/esm.js.map
+-rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/file-extensions.d.ts
+-rw-rw-rw-   0        0        0     5702 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/file-extensions.js
+-rw-rw-rw-   0        0        0     9477 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/file-extensions.js.map
+-rw-rw-rw-   0        0        0    11689 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/index.d.ts
+-rw-rw-rw-   0        0        0    45986 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/index.js
+-rw-rw-rw-   0        0        0    89796 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/index.js.map
+-rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/module-type-classifier.d.ts
+-rw-rw-rw-   0        0        0     2363 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/module-type-classifier.js
+-rw-rw-rw-   0        0        0     4897 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/module-type-classifier.js.map
+-rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/node-module-type-classifier.d.ts
+-rw-rw-rw-   0        0        0     1515 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/node-module-type-classifier.js
+-rw-rw-rw-   0        0        0     2169 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/node-module-type-classifier.js.map
+-rw-rw-rw-   0        0        0     2888 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/repl.d.ts
+-rw-rw-rw-   0        0        0    21715 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/repl.js
+-rw-rw-rw-   0        0        0    39064 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/repl.js.map
+-rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/resolver-functions.d.ts
+-rw-rw-rw-   0        0        0     7574 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/resolver-functions.js
+-rw-rw-rw-   0        0        0    13596 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/resolver-functions.js.map
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:27.872144 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/transpilers/
+-rw-rw-rw-   0        0        0      470 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/transpilers/swc.d.ts
+-rw-rw-rw-   0        0        0     8796 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/transpilers/swc.js
+-rw-rw-rw-   0        0        0    14644 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/transpilers/swc.js.map
+-rw-rw-rw-   0        0        0     1008 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/transpilers/types.d.ts
+-rw-rw-rw-   0        0        0      110 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/transpilers/types.js
+-rw-rw-rw-   0        0        0     2176 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/transpilers/types.js.map
+-rw-rw-rw-   0        0        0     3305 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/ts-compiler-types.d.ts
+-rw-rw-rw-   0        0        0      122 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/ts-compiler-types.js
+-rw-rw-rw-   0        0        0     6349 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/ts-compiler-types.js.map
+-rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/ts-internals.d.ts
+-rw-rw-rw-   0        0        0    12325 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/ts-internals.js
+-rw-rw-rw-   0        0        0    22287 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/ts-internals.js.map
+-rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/ts-transpile-module.d.ts
+-rw-rw-rw-   0        0        0     4941 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/ts-transpile-module.js
+-rw-rw-rw-   0        0        0     9092 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/ts-transpile-module.js.map
+-rw-rw-rw-   0        0        0      464 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/tsconfig-schema.d.ts
+-rw-rw-rw-   0        0        0      120 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/tsconfig-schema.js
+-rw-rw-rw-   0        0        0      887 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/tsconfig-schema.js.map
+-rw-rw-rw-   0        0        0       11 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/tsconfigs.d.ts
+-rw-rw-rw-   0        0        0     1435 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/tsconfigs.js
+-rw-rw-rw-   0        0        0     2442 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/tsconfigs.js.map
+-rw-rw-rw-   0        0        0      118 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/util.d.ts
+-rw-rw-rw-   0        0        0     6140 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/util.js
+-rw-rw-rw-   0        0        0     9523 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/util.js.map
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.647852 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/node_modules/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.647852 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/node_modules/acorn-walk/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:27.924141 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/node_modules/acorn-walk/dist/
+-rw-rw-rw-   0        0        0     2605 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/node_modules/acorn-walk/dist/walk.d.ts
+-rw-rw-rw-   0        0        0    16002 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/node_modules/acorn-walk/dist/walk.js
+-rw-rw-rw-   0        0        0    14559 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/node_modules/acorn-walk/dist/walk.mjs
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.648851 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/node_modules/diff/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:27.979659 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/node_modules/diff/dist/
+-rw-rw-rw-   0        0        0    48402 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/node_modules/diff/dist/diff.js
+-rw-rw-rw-   0        0        0    16978 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/node_modules/diff/dist/diff.min.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.650854 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:28.008660 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/
+-rw-rw-rw-   0        0        0     1458 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/index.d.ts
+-rw-rw-rw-   0        0        0     5753 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/index.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:28.041661 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/
+-rw-rw-rw-   0        0        0     3674 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/application.d.ts
+-rw-rw-rw-   0        0        0    14980 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/application.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:28.266696 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/
+-rw-rw-rw-   0        0        0      225 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/components.d.ts
+-rw-rw-rw-   0        0        0      420 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/components.js
+-rw-rw-rw-   0        0        0     4143 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/context.d.ts
+-rw-rw-rw-   0        0        0     7550 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/context.js
+-rw-rw-rw-   0        0        0      389 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/convert-expression.d.ts
+-rw-rw-rw-   0        0        0     1954 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/convert-expression.js
+-rw-rw-rw-   0        0        0      437 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/converter-events.d.ts
+-rw-rw-rw-   0        0        0      455 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/converter-events.js
+-rw-rw-rw-   0        0        0     4748 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/converter.d.ts
+-rw-rw-rw-   0        0        0    18456 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/converter.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:28.345699 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/
+-rw-rw-rw-   0        0        0      867 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/comment.d.ts
+-rw-rw-rw-   0        0        0     9047 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/comment.js
+-rw-rw-rw-   0        0        0      167 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/index-signature.d.ts
+-rw-rw-rw-   0        0        0     1806 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/index-signature.js
+-rw-rw-rw-   0        0        0      976 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/signature.d.ts
+-rw-rw-rw-   0        0        0    10164 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/signature.js
+-rw-rw-rw-   0        0        0      183 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/index.d.ts
+-rw-rw-rw-   0        0        0      873 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/index.js
+-rw-rw-rw-   0        0        0      388 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/jsdoc.d.ts
+-rw-rw-rw-   0        0        0     4141 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/jsdoc.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:28.756759 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/
+-rw-rw-rw-   0        0        0     2482 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/CategoryPlugin.d.ts
+-rw-rw-rw-   0        0        0     9936 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/CategoryPlugin.js
+-rw-rw-rw-   0        0        0     2299 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/CommentPlugin.d.ts
+-rw-rw-rw-   0        0        0    17773 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/CommentPlugin.js
+-rw-rw-rw-   0        0        0     1029 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/DecoratorPlugin.d.ts
+-rw-rw-rw-   0        0        0     4975 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/DecoratorPlugin.js
+-rw-rw-rw-   0        0        0     2793 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/GroupPlugin.d.ts
+-rw-rw-rw-   0        0        0     7239 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/GroupPlugin.js
+-rw-rw-rw-   0        0        0     1570 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/ImplementsPlugin.d.ts
+-rw-rw-rw-   0        0        0    14961 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/ImplementsPlugin.js
+-rw-rw-rw-   0        0        0      921 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/InheritDocPlugin.d.ts
+-rw-rw-rw-   0        0        0     4047 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/InheritDocPlugin.js
+-rw-rw-rw-   0        0        0      851 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/PackagePlugin.d.ts
+-rw-rw-rw-   0        0        0     5284 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/PackagePlugin.js
+-rw-rw-rw-   0        0        0     3434 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/SourceLinkPlugin.d.ts
+-rw-rw-rw-   0        0        0     9769 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/SourceLinkPlugin.js
+-rw-rw-rw-   0        0        0     1712 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/SourcePlugin.d.ts
+-rw-rw-rw-   0        0        0     6449 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/SourcePlugin.js
+-rw-rw-rw-   0        0        0      825 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/TypePlugin.d.ts
+-rw-rw-rw-   0        0        0     4594 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/TypePlugin.js
+-rw-rw-rw-   0        0        0      502 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/index.d.ts
+-rw-rw-rw-   0        0        0     2171 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/index.js
+-rw-rw-rw-   0        0        0      184 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/symbols.d.ts
+-rw-rw-rw-   0        0        0    31944 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/symbols.js
+-rw-rw-rw-   0        0        0      535 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/types.d.ts
+-rw-rw-rw-   0        0        0    31395 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/types.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:28.855280 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/
+-rw-rw-rw-   0        0        0     1121 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/base-path.d.ts
+-rw-rw-rw-   0        0        0     3068 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/base-path.js
+-rw-rw-rw-   0        0        0      403 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/nodes.d.ts
+-rw-rw-rw-   0        0        0     1048 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/nodes.js
+-rw-rw-rw-   0        0        0      397 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/reflections.d.ts
+-rw-rw-rw-   0        0        0     3415 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/reflections.js
+-rw-rw-rw-   0        0        0      135 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/symbols.d.ts
+-rw-rw-rw-   0        0        0      380 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/symbols.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:28.957281 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/
+-rw-rw-rw-   0        0        0      823 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/ReflectionCategory.d.ts
+-rw-rw-rw-   0        0        0      923 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/ReflectionCategory.js
+-rw-rw-rw-   0        0        0     1874 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/ReflectionGroup.d.ts
+-rw-rw-rw-   0        0        0     1047 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/ReflectionGroup.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:29.027282 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/comments/
+-rw-rw-rw-   0        0        0     2078 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/comments/comment.d.ts
+-rw-rw-rw-   0        0        0     3083 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/comments/comment.js
+-rw-rw-rw-   0        0        0       73 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/comments/index.d.ts
+-rw-rw-rw-   0        0        0      420 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/comments/index.js
+-rw-rw-rw-   0        0        0      541 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/comments/tag.d.ts
+-rw-rw-rw-   0        0        0      498 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/comments/tag.js
+-rw-rw-rw-   0        0        0      202 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/index.d.ts
+-rw-rw-rw-   0        0        0     1067 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/index.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:29.405629 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/
+-rw-rw-rw-   0        0        0     8213 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/abstract.d.ts
+-rw-rw-rw-   0        0        0    13360 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/abstract.js
+-rw-rw-rw-   0        0        0     1486 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/container.d.ts
+-rw-rw-rw-   0        0        0     1192 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/container.js
+-rw-rw-rw-   0        0        0     4204 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/declaration.d.ts
+-rw-rw-rw-   0        0        0     3639 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/declaration.js
+-rw-rw-rw-   0        0        0      687 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/index.d.ts
+-rw-rw-rw-   0        0        0     2783 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/index.js
+-rw-rw-rw-   0        0        0     1052 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/kind.d.ts
+-rw-rw-rw-   0        0        0     3535 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/kind.js
+-rw-rw-rw-   0        0        0      764 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/parameter.d.ts
+-rw-rw-rw-   0        0        0     1078 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/parameter.js
+-rw-rw-rw-   0        0        0     3759 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/project.d.ts
+-rw-rw-rw-   0        0        0     8239 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/project.js
+-rw-rw-rw-   0        0        0     1807 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/reference.d.ts
+-rw-rw-rw-   0        0        0     3190 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/reference.js
+-rw-rw-rw-   0        0        0     1931 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/signature.d.ts
+-rw-rw-rw-   0        0        0     2075 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/signature.js
+-rw-rw-rw-   0        0        0      770 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/type-parameter.d.ts
+-rw-rw-rw-   0        0        0      765 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/type-parameter.js
+-rw-rw-rw-   0        0        0       89 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/utils.d.ts
+-rw-rw-rw-   0        0        0     1068 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/utils.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:29.541153 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/
+-rw-rw-rw-   0        0        0     1894 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/directory.d.ts
+-rw-rw-rw-   0        0        0     2007 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/directory.js
+-rw-rw-rw-   0        0        0     2305 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/file.d.ts
+-rw-rw-rw-   0        0        0     1099 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/file.js
+-rw-rw-rw-   0        0        0      178 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/index.d.ts
+-rw-rw-rw-   0        0        0      652 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/index.js
+-rw-rw-rw-   0        0        0      113 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/repository.d.ts
+-rw-rw-rw-   0        0        0      366 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/repository.js
+-rw-rw-rw-   0        0        0    14055 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/types.d.ts
+-rw-rw-rw-   0        0        0    28742 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/types.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:29.720339 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/
+-rw-rw-rw-   0        0        0     1891 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/components.d.ts
+-rw-rw-rw-   0        0        0     2489 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/components.js
+-rw-rw-rw-   0        0        0     3638 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/events.d.ts
+-rw-rw-rw-   0        0        0     2608 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/events.js
+-rw-rw-rw-   0        0        0      448 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/index.d.ts
+-rw-rw-rw-   0        0        0     1585 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/index.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:29.752343 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/models/
+-rw-rw-rw-   0        0        0      379 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/models/UrlMapping.d.ts
+-rw-rw-rw-   0        0        0      292 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/models/UrlMapping.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:29.932345 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/
+-rw-rw-rw-   0        0        0      559 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/AssetsPlugin.d.ts
+-rw-rw-rw-   0        0        0     2862 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/AssetsPlugin.js
+-rw-rw-rw-   0        0        0      596 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/JavascriptIndexPlugin.d.ts
+-rw-rw-rw-   0        0        0     4324 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/JavascriptIndexPlugin.js
+-rw-rw-rw-   0        0        0      972 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/LegendPlugin.d.ts
+-rw-rw-rw-   0        0        0     9734 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/LegendPlugin.js
+-rw-rw-rw-   0        0        0     2534 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/MarkedLinksPlugin.d.ts
+-rw-rw-rw-   0        0        0     7176 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/MarkedLinksPlugin.js
+-rw-rw-rw-   0        0        0      271 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/index.d.ts
+-rw-rw-rw-   0        0        0     1172 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/index.js
+-rw-rw-rw-   0        0        0     7435 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/renderer.d.ts
+-rw-rw-rw-   0        0        0    12106 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/renderer.js
+-rw-rw-rw-   0        0        0     1786 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/theme.d.ts
+-rw-rw-rw-   0        0        0     1524 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/theme.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:29.998340 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/
+-rw-rw-rw-   0        0        0     2065 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/MarkedPlugin.d.ts
+-rw-rw-rw-   0        0        0     7378 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/MarkedPlugin.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:30.064340 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/
+-rw-rw-rw-   0        0        0     4357 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/DefaultTheme.d.ts
+-rw-rw-rw-   0        0        0    11183 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/DefaultTheme.js
+-rw-rw-rw-   0        0        0     4066 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/DefaultThemeRenderContext.d.ts
+-rw-rw-rw-   0        0        0     4072 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/DefaultThemeRenderContext.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:30.088339 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/layouts/
+-rw-rw-rw-   0        0        0      343 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/layouts/default.d.ts
+-rw-rw-rw-   0        0        0     2692 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/layouts/default.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:30.627389 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/
+-rw-rw-rw-   0        0        0      216 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/analytics.d.ts
+-rw-rw-rw-   0        0        0      895 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/analytics.js
+-rw-rw-rw-   0        0        0      119 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/anchor-icon.d.ts
+-rw-rw-rw-   0        0        0      902 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/anchor-icon.js
+-rw-rw-rw-   0        0        0      291 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/breadcrumb.d.ts
+-rw-rw-rw-   0        0        0      665 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/breadcrumb.js
+-rw-rw-rw-   0        0        0      292 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/comment.d.ts
+-rw-rw-rw-   0        0        0     1321 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/comment.js
+-rw-rw-rw-   0        0        0      335 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/footer.d.ts
+-rw-rw-rw-   0        0        0     2075 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/footer.js
+-rw-rw-rw-   0        0        0      336 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/header.d.ts
+-rw-rw-rw-   0        0        0     4296 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/header.js
+-rw-rw-rw-   0        0        0      298 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/hierarchy.d.ts
+-rw-rw-rw-   0        0        0      545 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/hierarchy.js
+-rw-rw-rw-   0        0        0      303 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/index.d.ts
+-rw-rw-rw-   0        0        0     2442 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/index.js
+-rw-rw-rw-   0        0        0      292 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.d.ts
+-rw-rw-rw-   0        0        0      303 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.declaration.d.ts
+-rw-rw-rw-   0        0        0     1695 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.declaration.js
+-rw-rw-rw-   0        0        0      309 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.getterSetter.d.ts
+-rw-rw-rw-   0        0        0     1397 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.getterSetter.js
+-rw-rw-rw-   0        0        0     1275 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.js
+-rw-rw-rw-   0        0        0      304 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.reference.d.ts
+-rw-rw-rw-   0        0        0      886 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.reference.js
+-rw-rw-rw-   0        0        0      363 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.signature.body.d.ts
+-rw-rw-rw-   0        0        0     2395 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.signature.body.js
+-rw-rw-rw-   0        0        0      413 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.signature.title.d.ts
+-rw-rw-rw-   0        0        0     1852 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.signature.title.js
+-rw-rw-rw-   0        0        0      307 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.signatures.d.ts
+-rw-rw-rw-   0        0        0      870 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.signatures.js
+-rw-rw-rw-   0        0        0      347 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.sources.d.ts
+-rw-rw-rw-   0        0        0     1484 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.sources.js
+-rw-rw-rw-   0        0        0      293 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/members.d.ts
+-rw-rw-rw-   0        0        0      290 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/members.group.d.ts
+-rw-rw-rw-   0        0        0     1051 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/members.group.js
+-rw-rw-rw-   0        0        0      892 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/members.js
+-rw-rw-rw-   0        0        0      334 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/navigation.d.ts
+-rw-rw-rw-   0        0        0     4914 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/navigation.js
+-rw-rw-rw-   0        0        0      295 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/parameter.d.ts
+-rw-rw-rw-   0        0        0     6080 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/parameter.js
+-rw-rw-rw-   0        0        0      266 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/type.d.ts
+-rw-rw-rw-   0        0        0    17751 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/type.js
+-rw-rw-rw-   0        0        0      265 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/typeAndParent.d.ts
+-rw-rw-rw-   0        0        0     1448 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/typeAndParent.js
+-rw-rw-rw-   0        0        0      319 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/typeParameters.d.ts
+-rw-rw-rw-   0        0        0     1014 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/typeParameters.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:30.675770 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/templates/
+-rw-rw-rw-   0        0        0      362 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/templates/index.d.ts
+-rw-rw-rw-   0        0        0      400 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/templates/index.js
+-rw-rw-rw-   0        0        0      361 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/templates/reflection.d.ts
+-rw-rw-rw-   0        0        0     3365 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/templates/reflection.js
+-rw-rw-rw-   0        0        0     1066 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/lib.d.ts
+-rw-rw-rw-   0        0        0     3114 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/lib.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:30.830208 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/
+-rw-rw-rw-   0        0        0     2611 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/components.d.ts
+-rw-rw-rw-   0        0        0     1976 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/components.js
+-rw-rw-rw-   0        0        0     1072 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/events.d.ts
+-rw-rw-rw-   0        0        0      589 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/events.js
+-rw-rw-rw-   0        0        0      968 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/index.d.ts
+-rw-rw-rw-   0        0        0     5662 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/index.js
+-rw-rw-rw-   0        0        0     9064 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/schema.d.ts
+-rw-rw-rw-   0        0        0     1203 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/schema.js
+-rw-rw-rw-   0        0        0     1291 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializer.d.ts
+-rw-rw-rw-   0        0        0     4537 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializer.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:31.032204 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:31.117204 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/comments/
+-rw-rw-rw-   0        0        0      511 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/comments/comment-tag.d.ts
+-rw-rw-rw-   0        0        0      828 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/comments/comment-tag.js
+-rw-rw-rw-   0        0        0      477 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/comments/comment.d.ts
+-rw-rw-rw-   0        0        0      986 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/comments/comment.js
+-rw-rw-rw-   0        0        0      101 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/comments/index.d.ts
+-rw-rw-rw-   0        0        0      504 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/comments/index.js
+-rw-rw-rw-   0        0        0      518 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/decorator.d.ts
+-rw-rw-rw-   0        0        0     1013 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/decorator.js
+-rw-rw-rw-   0        0        0      241 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/index.d.ts
+-rw-rw-rw-   0        0        0     1142 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/index.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:31.184203 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/models/
+-rw-rw-rw-   0        0        0      267 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/models/decorator-wrapper.d.ts
+-rw-rw-rw-   0        0        0      365 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/models/decorator-wrapper.js
+-rw-rw-rw-   0        0        0      125 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/models/index.d.ts
+-rw-rw-rw-   0        0        0      576 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/models/index.js
+-rw-rw-rw-   0        0        0      307 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/models/source-reference-wrapper.d.ts
+-rw-rw-rw-   0        0        0      411 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/models/source-reference-wrapper.js
+-rw-rw-rw-   0        0        0      597 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflection-category.d.ts
+-rw-rw-rw-   0        0        0     1018 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflection-category.js
+-rw-rw-rw-   0        0        0      554 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflection-group.d.ts
+-rw-rw-rw-   0        0        0     1126 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflection-group.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:31.595790 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/
+-rw-rw-rw-   0        0        0      423 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/abstract.d.ts
+-rw-rw-rw-   0        0        0     1686 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/abstract.js
+-rw-rw-rw-   0        0        0      640 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/container.d.ts
+-rw-rw-rw-   0        0        0     1116 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/container.js
+-rw-rw-rw-   0        0        0      538 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/declaration.d.ts
+-rw-rw-rw-   0        0        0     1775 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/declaration.js
+-rw-rw-rw-   0        0        0      209 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/index.d.ts
+-rw-rw-rw-   0        0        0     1092 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/index.js
+-rw-rw-rw-   0        0        0      476 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/parameter.d.ts
+-rw-rw-rw-   0        0        0      706 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/parameter.js
+-rw-rw-rw-   0        0        0      532 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/reference.d.ts
+-rw-rw-rw-   0        0        0      855 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/reference.js
+-rw-rw-rw-   0        0        0      476 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/signature.d.ts
+-rw-rw-rw-   0        0        0      964 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/signature.js
+-rw-rw-rw-   0        0        0      508 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/type-parameter.d.ts
+-rw-rw-rw-   0        0        0      759 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/type-parameter.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:31.819968 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/sources/
+-rw-rw-rw-   0        0        0       73 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/sources/index.d.ts
+-rw-rw-rw-   0        0        0      362 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/sources/index.js
+-rw-rw-rw-   0        0        0      519 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/sources/source-reference.d.ts
+-rw-rw-rw-   0        0        0      789 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/sources/source-reference.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:33.111309 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/
+-rw-rw-rw-   0        0        0      357 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/abstract.d.ts
+-rw-rw-rw-   0        0        0      524 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/abstract.js
+-rw-rw-rw-   0        0        0      504 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/array.d.ts
+-rw-rw-rw-   0        0        0      684 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/array.js
+-rw-rw-rw-   0        0        0      459 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/conditional.d.ts
+-rw-rw-rw-   0        0        0      801 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/conditional.js
+-rw-rw-rw-   0        0        0      571 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/index.d.ts
+-rw-rw-rw-   0        0        0     1688 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/index.js
+-rw-rw-rw-   0        0        0      468 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/indexed-access.d.ts
+-rw-rw-rw-   0        0        0      656 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/indexed-access.js
+-rw-rw-rw-   0        0        0      432 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/inferred.d.ts
+-rw-rw-rw-   0        0        0      678 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/inferred.js
+-rw-rw-rw-   0        0        0      560 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/intersection.d.ts
+-rw-rw-rw-   0        0        0      721 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/intersection.js
+-rw-rw-rw-   0        0        0      536 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/intrinsic.d.ts
+-rw-rw-rw-   0        0        0      669 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/intrinsic.js
+-rw-rw-rw-   0        0        0      388 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/literal.d.ts
+-rw-rw-rw-   0        0        0      812 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/literal.js
+-rw-rw-rw-   0        0        0      379 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/mapped.d.ts
+-rw-rw-rw-   0        0        0      823 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/mapped.js
+-rw-rw-rw-   0        0        0      528 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/optional.d.ts
+-rw-rw-rw-   0        0        0      699 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/optional.js
+-rw-rw-rw-   0        0        0      404 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/predicate.d.ts
+-rw-rw-rw-   0        0        0      696 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/predicate.js
+-rw-rw-rw-   0        0        0      372 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/query.d.ts
+-rw-rw-rw-   0        0        0      548 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/query.js
+-rw-rw-rw-   0        0        0      433 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/reference.d.ts
+-rw-rw-rw-   0        0        0      935 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/reference.js
+-rw-rw-rw-   0        0        0      417 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/reflection.d.ts
+-rw-rw-rw-   0        0        0      618 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/reflection.js
+-rw-rw-rw-   0        0        0      496 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/rest.d.ts
+-rw-rw-rw-   0        0        0      679 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/rest.js
+-rw-rw-rw-   0        0        0      452 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/template-literal.d.ts
+-rw-rw-rw-   0        0        0      700 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/template-literal.js
+-rw-rw-rw-   0        0        0      692 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/tuple.d.ts
+-rw-rw-rw-   0        0        0     1138 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/tuple.js
+-rw-rw-rw-   0        0        0      428 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/type-operator.d.ts
+-rw-rw-rw-   0        0        0      614 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/type-operator.js
+-rw-rw-rw-   0        0        0      504 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/union.d.ts
+-rw-rw-rw-   0        0        0      686 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/union.js
+-rw-rw-rw-   0        0        0      520 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/unknown.d.ts
+-rw-rw-rw-   0        0        0      659 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/unknown.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:33.667335 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/
+-rw-rw-rw-   0        0        0     2414 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/array.d.ts
+-rw-rw-rw-   0        0        0     4474 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/array.js
+-rw-rw-rw-   0        0        0     3017 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/component.d.ts
+-rw-rw-rw-   0        0        0     5920 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/component.js
+-rw-rw-rw-   0        0        0     1659 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/entry-point.d.ts
+-rw-rw-rw-   0        0        0    10766 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/entry-point.js
+-rw-rw-rw-   0        0        0      304 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/enum.d.ts
+-rw-rw-rw-   0        0        0      757 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/enum.js
+-rw-rw-rw-   0        0        0     4284 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/events.d.ts
+-rw-rw-rw-   0        0        0    12855 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/events.js
+-rw-rw-rw-   0        0        0     1403 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/fs.d.ts
+-rw-rw-rw-   0        0        0     4427 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/fs.js
+-rw-rw-rw-   0        0        0     1421 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/general.d.ts
+-rw-rw-rw-   0        0        0      711 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/general.js
+-rw-rw-rw-   0        0        0      367 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/highlighter.d.ts
+-rw-rw-rw-   0        0        0     6776 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/highlighter.js
+-rw-rw-rw-   0        0        0     2325 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/hooks.d.ts
+-rw-rw-rw-   0        0        0     3767 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/hooks.js
+-rw-rw-rw-   0        0        0     1350 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/index.d.ts
+-rw-rw-rw-   0        0        0     6465 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/index.js
+-rw-rw-rw-   0        0        0     1894 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/jsx.d.ts
+-rw-rw-rw-   0        0        0    25309 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/jsx.elements.d.ts
+-rw-rw-rw-   0        0        0      139 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/jsx.elements.js
+-rw-rw-rw-   0        0        0     3737 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/jsx.js
+-rw-rw-rw-   0        0        0     3550 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/loggers.d.ts
+-rw-rw-rw-   0        0        0     7007 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/loggers.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:33.791459 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/
+-rw-rw-rw-   0        0        0    11114 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/declaration.d.ts
+-rw-rw-rw-   0        0        0    13000 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/declaration.js
+-rw-rw-rw-   0        0        0      205 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/help.d.ts
+-rw-rw-rw-   0        0        0     2565 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/help.js
+-rw-rw-rw-   0        0        0      652 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/index.d.ts
+-rw-rw-rw-   0        0        0     1390 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/index.js
+-rw-rw-rw-   0        0        0     8353 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/options.d.ts
+-rw-rw-rw-   0        0        0     9136 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/options.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:33.891457 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/
+-rw-rw-rw-   0        0        0      408 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/arguments.d.ts
+-rw-rw-rw-   0        0        0     3674 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/arguments.js
+-rw-rw-rw-   0        0        0      135 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/index.d.ts
+-rw-rw-rw-   0        0        0      664 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/index.js
+-rw-rw-rw-   0        0        0      503 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/tsconfig.d.ts
+-rw-rw-rw-   0        0        0     3251 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/tsconfig.js
+-rw-rw-rw-   0        0        0     1204 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/typedoc.d.ts
+-rw-rw-rw-   0        0        0     3498 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/typedoc.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:33.931458 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/sources/
+-rw-rw-rw-   0        0        0       47 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/sources/index.d.ts
+-rw-rw-rw-   0        0        0      284 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/sources/index.js
+-rw-rw-rw-   0        0        0      126 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/sources/typedoc.d.ts
+-rw-rw-rw-   0        0        0    16281 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/sources/typedoc.js
+-rw-rw-rw-   0        0        0     1088 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/package-manifest.d.ts
+-rw-rw-rw-   0        0        0     9116 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/package-manifest.js
+-rw-rw-rw-   0        0        0      387 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/paths.d.ts
+-rw-rw-rw-   0        0        0     1094 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/paths.js
+-rw-rw-rw-   0        0        0      209 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/plugins.d.ts
+-rw-rw-rw-   0        0        0     3942 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/plugins.js
+-rw-rw-rw-   0        0        0      576 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/sort.d.ts
+-rw-rw-rw-   0        0        0     5191 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/sort.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:33.978462 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/validation/
+-rw-rw-rw-   0        0        0      261 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/validation/documentation.d.ts
+-rw-rw-rw-   0        0        0     3672 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/validation/documentation.js
+-rw-rw-rw-   0        0        0      218 2023-01-09 05:07:14.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/validation/exports.d.ts
+-rw-rw-rw-   0        0        0     6277 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/validation/exports.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.668851 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/url-parse/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:34.032998 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/url-parse/dist/
+-rw-rw-rw-   0        0        0    21134 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/url-parse/dist/url-parse.js
+-rw-rw-rw-   0        0        0     6736 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/url-parse/dist/url-parse.min.js
+-rw-rw-rw-   0        0        0     9809 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/url-parse/dist/url-parse.min.js.map
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.672854 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/workerpool/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:34.159588 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/workerpool/dist/
+-rw-rw-rw-   0        0        0     6544 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/workerpool/dist/worker.js
+-rw-rw-rw-   0        0        0    10647 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/workerpool/dist/worker.js.map
+-rw-rw-rw-   0        0        0    51236 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/workerpool/dist/workerpool.js
+-rw-rw-rw-   0        0        0    86665 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/workerpool/dist/workerpool.js.map
+-rw-rw-rw-   0        0        0    20624 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/workerpool/dist/workerpool.min.js
+-rw-rw-rw-   0        0        0      815 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/workerpool/dist/workerpool.min.js.LICENSE.txt
+-rw-rw-rw-   0        0        0    68373 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/workerpool/dist/workerpool.min.js.map
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.673850 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/y18n/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:34.174587 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/y18n/build/
+-rw-rw-rw-   0        0        0     6783 2023-01-09 05:07:11.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/y18n/build/index.cjs
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:34.202590 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/y18n/build/lib/
+-rw-rw-rw-   0        0        0      192 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/y18n/build/lib/cjs.js
+-rw-rw-rw-   0        0        0     6268 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/y18n/build/lib/index.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:34.215590 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/y18n/build/lib/platform-shims/
+-rw-rw-rw-   0        0        0      377 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/y18n/build/lib/platform-shims/node.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.679851 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:34.335589 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/
+-rw-rw-rw-   0        0        0   107596 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/index.cjs
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:34.528996 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/
+-rw-rw-rw-   0        0        0     2477 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/argsert.js
+-rw-rw-rw-   0        0        0    15435 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/command.js
+-rw-rw-rw-   0        0        0     1392 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/completion-templates.js
+-rw-rw-rw-   0        0        0     5529 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/completion.js
+-rw-rw-rw-   0        0        0     2190 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/middleware.js
+-rw-rw-rw-   0        0        0     1060 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/parse-command.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:34.551478 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/typings/
+-rw-rw-rw-   0        0        0      308 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/typings/common-types.js
+-rw-rw-rw-   0        0        0       11 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/typings/yargs-parser-types.js
+-rw-rw-rw-   0        0        0    19829 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/usage.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:34.642392 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/utils/
+-rw-rw-rw-   0        0        0     2049 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/utils/apply-extends.js
+-rw-rw-rw-   0        0        0      155 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/utils/is-promise.js
+-rw-rw-rw-   0        0        0      731 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/utils/levenshtein.js
+-rw-rw-rw-   0        0        0      299 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/utils/obj-filter.js
+-rw-rw-rw-   0        0        0      436 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/utils/process-argv.js
+-rw-rw-rw-   0        0        0      386 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/utils/set-blocking.js
+-rw-rw-rw-   0        0        0      321 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/utils/which-module.js
+-rw-rw-rw-   0        0        0    12201 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/validation.js
+-rw-rw-rw-   0        0        0    42229 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/yargs-factory.js
+-rw-rw-rw-   0        0        0      181 2023-01-09 05:07:13.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/yerror.js
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:22.676855 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs-parser/
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:34.235591 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs-parser/build/
+-rw-rw-rw-   0        0        0    41467 2023-01-09 05:07:11.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs-parser/build/index.cjs
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:34.302589 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs-parser/build/lib/
+-rw-rw-rw-   0        0        0     2023 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs-parser/build/lib/index.js
+-rw-rw-rw-   0        0        0     1795 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs-parser/build/lib/string-utils.js
+-rw-rw-rw-   0        0        0     1004 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs-parser/build/lib/tokenize-arg-string.js
+-rw-rw-rw-   0        0        0       11 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs-parser/build/lib/yargs-parser-types.js
+-rw-rw-rw-   0        0        0    45688 2023-01-09 05:07:12.000000 monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs-parser/build/lib/yargs-parser.js
+-rw-rw-rw-   0        0        0     2234 2023-01-09 05:31:27.000000 monaco_qt-0.1.8/monaco/monaco-editor/package.json
+-rw-rw-rw-   0        0        0     3562 2024-06-01 21:41:07.000000 monaco_qt-0.1.8/monaco/monaco_widget.py
+drwxrwxrwx   0        0        0        0 2024-06-01 21:42:34.664392 monaco_qt-0.1.8/monaco_qt.egg-info/
+-rw-rw-rw-   0        0        0     1624 2024-06-01 21:42:22.000000 monaco_qt-0.1.8/monaco_qt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    56210 2024-06-01 21:42:22.000000 monaco_qt-0.1.8/monaco_qt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 21:42:22.000000 monaco_qt-0.1.8/monaco_qt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-06-01 21:42:22.000000 monaco_qt-0.1.8/monaco_qt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-06-01 21:42:22.000000 monaco_qt-0.1.8/monaco_qt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-06-01 21:42:22.000000 monaco_qt-0.1.8/monaco_qt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 21:42:34.667395 monaco_qt-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1528 2024-06-01 21:41:41.000000 monaco_qt-0.1.8/setup.py
```

### Comparing `monaco-qt-0.1.7/PKG-INFO` & `monaco_qt-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monaco-qt
-Version: 0.1.7
+Version: 0.1.8
 Summary: The Monaco editor as a Qt Widget
 Home-page: https://github.com/DaelonSuzuka/monaco-qt
 Author: David Kincaid
 Author-email: dlkincaid0@gmail.com
 Keywords: qtstrap,qt,pyqt,monaco,text editor
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Widget Sets
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+Requires-Dist: QtPy
 
 # monaco-qt
 
 [![license](https://img.shields.io/pypi/l/monaco-qt.svg)](./LICENSE)
 [![pypi version](https://img.shields.io/pypi/v/monaco-qt.svg)](https://pypi.org/project/monaco-qt/)
 [![PyPI status](https://img.shields.io/pypi/status/monaco-qt.svg)](https://github.com/DaelonSuzuka/monaco-qt/)
```

### Comparing `monaco-qt-0.1.7/README.md` & `monaco_qt-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/index.html` & `monaco_qt-0.1.8/monaco/index.html`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/index.js` & `monaco_qt-0.1.8/monaco/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/CHANGELOG.md` & `monaco_qt-0.1.8/monaco/monaco-editor/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/LICENSE` & `monaco_qt-0.1.8/monaco/monaco-editor/LICENSE`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/README.md` & `monaco_qt-0.1.8/monaco/monaco-editor/README.md`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/ThirdPartyNotices.txt` & `monaco_qt-0.1.8/monaco/monaco-editor/ThirdPartyNotices.txt`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/base/browser/ui/codicons/codicon/codicon.ttf` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/base/browser/ui/codicons/codicon/codicon.ttf`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/base/worker/workerMain.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/base/worker/workerMain.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/abap/abap.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/abap/abap.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/apex/apex.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/apex/apex.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/azcli/azcli.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/azcli/azcli.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/bat/bat.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/bat/bat.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/bicep/bicep.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/bicep/bicep.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/cameligo/cameligo.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/cameligo/cameligo.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/clojure/clojure.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/clojure/clojure.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/coffee/coffee.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/coffee/coffee.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/cpp/cpp.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/cpp/cpp.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/csharp/csharp.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/csharp/csharp.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/csp/csp.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/csp/csp.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/css/css.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/css/css.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/dart/dart.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/dart/dart.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/dockerfile/dockerfile.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/dockerfile/dockerfile.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/ecl/ecl.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/ecl/ecl.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/elixir/elixir.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/elixir/elixir.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/flow9/flow9.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/flow9/flow9.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/freemarker2/freemarker2.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/freemarker2/freemarker2.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/fsharp/fsharp.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/fsharp/fsharp.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/go/go.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/go/go.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/graphql/graphql.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/graphql/graphql.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/handlebars/handlebars.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/handlebars/handlebars.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/hcl/hcl.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/hcl/hcl.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/html/html.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/html/html.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/ini/ini.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/ini/ini.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/java/java.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/java/java.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/javascript/javascript.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/javascript/javascript.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/julia/julia.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/julia/julia.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/kotlin/kotlin.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/kotlin/kotlin.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/less/less.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/less/less.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/lexon/lexon.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/lexon/lexon.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/liquid/liquid.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/liquid/liquid.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/lua/lua.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/lua/lua.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/m3/m3.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/m3/m3.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/markdown/markdown.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/markdown/markdown.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/mips/mips.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/mips/mips.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/msdax/msdax.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/msdax/msdax.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/mysql/mysql.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/mysql/mysql.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/objective-c/objective-c.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/objective-c/objective-c.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/pascal/pascal.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/pascal/pascal.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/pascaligo/pascaligo.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/pascaligo/pascaligo.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/perl/perl.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/perl/perl.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/pgsql/pgsql.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/pgsql/pgsql.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/php/php.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/php/php.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/pla/pla.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/pla/pla.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/postiats/postiats.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/postiats/postiats.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/powerquery/powerquery.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/powerquery/powerquery.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/powershell/powershell.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/powershell/powershell.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/protobuf/protobuf.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/protobuf/protobuf.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/pug/pug.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/pug/pug.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/python/python.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/python/python.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/qsharp/qsharp.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/qsharp/qsharp.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/r/r.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/r/r.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/razor/razor.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/razor/razor.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/redis/redis.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/redis/redis.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/redshift/redshift.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/redshift/redshift.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/restructuredtext/restructuredtext.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/restructuredtext/restructuredtext.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/ruby/ruby.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/ruby/ruby.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/rust/rust.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/rust/rust.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/sb/sb.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/sb/sb.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/scala/scala.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/scala/scala.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/scheme/scheme.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/scheme/scheme.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/scss/scss.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/scss/scss.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/shell/shell.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/shell/shell.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/solidity/solidity.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/solidity/solidity.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/sophia/sophia.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/sophia/sophia.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/sparql/sparql.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/sparql/sparql.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/sql/sql.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/sql/sql.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/st/st.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/st/st.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/swift/swift.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/swift/swift.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/systemverilog/systemverilog.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/systemverilog/systemverilog.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/tcl/tcl.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/tcl/tcl.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/twig/twig.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/twig/twig.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/typescript/typescript.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/typescript/typescript.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/vb/vb.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/vb/vb.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/xml/xml.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/xml/xml.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/basic-languages/yaml/yaml.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/basic-languages/yaml/yaml.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.css` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.css`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.nls.de.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.nls.de.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.nls.es.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.nls.es.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.nls.fr.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.nls.fr.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.nls.it.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.nls.it.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.nls.ja.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.nls.ja.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.nls.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.nls.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.nls.ko.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.nls.ko.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.nls.ru.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.nls.ru.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.nls.zh-cn.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.nls.zh-cn.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/editor/editor.main.nls.zh-tw.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/editor/editor.main.nls.zh-tw.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/language/css/cssMode.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/language/css/cssMode.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/language/css/cssWorker.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/language/css/cssWorker.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/language/html/htmlMode.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/language/html/htmlMode.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/language/html/htmlWorker.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/language/html/htmlWorker.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/language/json/jsonMode.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/language/json/jsonMode.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/language/json/jsonWorker.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/language/json/jsonWorker.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/language/typescript/tsMode.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/language/typescript/tsMode.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/language/typescript/tsWorker.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/language/typescript/tsWorker.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/min/vs/loader.js` & `monaco_qt-0.1.8/monaco/monaco-editor/min/vs/loader.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/monaco.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/monaco.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.mjs` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.mjs`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.mjs.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.mjs.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.umd.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.umd.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.umd.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.umd.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/binary-search.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/binary-search.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/sourcemap-segment.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/sourcemap-segment.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/trace-mapping.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/trace-mapping.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/types.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@cspotcode/source-map-support/node_modules/@jridgewell/trace-mapping/dist/types/types.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/gen-mapping.mjs` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/gen-mapping.mjs`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/gen-mapping.mjs.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/gen-mapping.mjs.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/gen-mapping.umd.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/gen-mapping.umd.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/gen-mapping.umd.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/gen-mapping.umd.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/types/gen-mapping.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/types/gen-mapping.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/types/sourcemap-segment.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/types/sourcemap-segment.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/types/types.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/gen-mapping/dist/types/types.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/dist/resolve-uri.mjs` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/dist/resolve-uri.mjs`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/dist/resolve-uri.mjs.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/dist/resolve-uri.mjs.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/dist/resolve-uri.umd.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/dist/resolve-uri.umd.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/dist/resolve-uri.umd.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/resolve-uri/dist/resolve-uri.umd.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/set-array.mjs` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/set-array.mjs`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/set-array.mjs.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/set-array.mjs.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/set-array.umd.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/set-array.umd.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/set-array.umd.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/set-array.umd.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/types/set-array.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/set-array/dist/types/set-array.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/source-map.mjs` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/source-map.mjs`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/source-map.mjs.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/source-map.mjs.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/source-map.umd.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/source-map.umd.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/source-map.umd.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/source-map.umd.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/types/source-map.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/source-map/dist/types/source-map.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/dist/sourcemap-codec.mjs` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/dist/sourcemap-codec.mjs`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/dist/sourcemap-codec.mjs.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/dist/sourcemap-codec.mjs.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/dist/sourcemap-codec.umd.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/dist/sourcemap-codec.umd.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/dist/sourcemap-codec.umd.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/sourcemap-codec/dist/sourcemap-codec.umd.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.mjs` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.mjs`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.mjs.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.mjs.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.umd.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.umd.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.umd.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/trace-mapping.umd.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/binary-search.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/binary-search.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/sourcemap-segment.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/sourcemap-segment.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/trace-mapping.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/trace-mapping.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/types.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@jridgewell/trace-mapping/dist/types/types.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@tootallnate/once/dist/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@tootallnate/once/dist/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@tootallnate/once/dist/index.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@tootallnate/once/dist/index.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@tootallnate/once/dist/overloaded-parameters.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@tootallnate/once/dist/overloaded-parameters.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@tootallnate/once/dist/types.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@tootallnate/once/dist/types.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@typescript/vfs/dist/index.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@typescript/vfs/dist/index.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.cjs.development.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.cjs.development.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.cjs.development.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.cjs.development.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.cjs.production.min.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.cjs.production.min.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.cjs.production.min.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.cjs.production.min.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.esm.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.esm.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.esm.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.esm.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.globals.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/@typescript/vfs/dist/vfs.globals.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn/dist/acorn.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn/dist/acorn.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn/dist/acorn.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn/dist/acorn.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn/dist/acorn.mjs` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn/dist/acorn.mjs`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn/dist/bin.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn/dist/bin.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/acorn.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/acorn.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/acorn.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/acorn.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/acorn.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/acorn.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/acorn.mjs` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/acorn.mjs`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/acorn.mjs.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/acorn.mjs.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/bin.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-globals/node_modules/acorn/dist/bin.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-walk/dist/walk.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-walk/dist/walk.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-walk/dist/walk.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-walk/dist/walk.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-walk/dist/walk.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-walk/dist/walk.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-walk/dist/walk.mjs` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-walk/dist/walk.mjs`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/acorn-walk/dist/walk.mjs.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/acorn-walk/dist/walk.mjs.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/agent-base/dist/src/index.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/agent-base/dist/src/index.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/agent-base/dist/src/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/agent-base/dist/src/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/agent-base/dist/src/index.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/agent-base/dist/src/index.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/cliui/build/index.cjs` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/cliui/build/index.cjs`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/cliui/build/lib/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/cliui/build/lib/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/cliui/build/lib/string-utils.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/cliui/build/lib/string-utils.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/diff/dist/diff.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/diff/dist/diff.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/escalade/dist/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/escalade/dist/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/escalade/dist/index.mjs` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/escalade/dist/index.mjs`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/esprima/dist/esprima.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/esprima/dist/esprima.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/http-proxy-agent/dist/agent.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/http-proxy-agent/dist/agent.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/http-proxy-agent/dist/agent.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/http-proxy-agent/dist/agent.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/http-proxy-agent/dist/agent.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/http-proxy-agent/dist/agent.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/http-proxy-agent/dist/index.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/http-proxy-agent/dist/index.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/http-proxy-agent/dist/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/http-proxy-agent/dist/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/https-proxy-agent/dist/agent.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/https-proxy-agent/dist/agent.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/https-proxy-agent/dist/agent.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/https-proxy-agent/dist/agent.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/https-proxy-agent/dist/agent.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/https-proxy-agent/dist/agent.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/https-proxy-agent/dist/index.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/https-proxy-agent/dist/index.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/https-proxy-agent/dist/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/https-proxy-agent/dist/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/https-proxy-agent/dist/parse-proxy-response.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/https-proxy-agent/dist/parse-proxy-response.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/https-proxy-agent/dist/parse-proxy-response.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/https-proxy-agent/dist/parse-proxy-response.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/human-signals/build/src/core.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/human-signals/build/src/core.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/human-signals/build/src/core.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/human-signals/build/src/core.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/human-signals/build/src/main.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/human-signals/build/src/main.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/human-signals/build/src/main.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/human-signals/build/src/main.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/human-signals/build/src/realtime.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/human-signals/build/src/realtime.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/human-signals/build/src/realtime.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/human-signals/build/src/realtime.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/human-signals/build/src/signals.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/human-signals/build/src/signals.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/human-signals/build/src/signals.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/human-signals/build/src/signals.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/js-yaml/dist/js-yaml.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/js-yaml/dist/js-yaml.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/js-yaml/dist/js-yaml.min.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/js-yaml/dist/js-yaml.min.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/js-yaml/dist/js-yaml.mjs` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/js-yaml/dist/js-yaml.mjs`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/lunr/build/package.json.template` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/lunr/build/package.json.template`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/lunr/build/release.sh` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/lunr/build/release.sh`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/lunr/build/wrapper_end` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/lunr/build/wrapper_end`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/make-error/dist/make-error.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/make-error/dist/make-error.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/pretty-quick/dist/createIgnorer.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/pretty-quick/dist/createIgnorer.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/pretty-quick/dist/createMatcher.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/pretty-quick/dist/createMatcher.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/pretty-quick/dist/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/pretty-quick/dist/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/pretty-quick/dist/processFiles.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/pretty-quick/dist/processFiles.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/pretty-quick/dist/scms/git.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/pretty-quick/dist/scms/git.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/pretty-quick/dist/scms/hg.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/pretty-quick/dist/scms/hg.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/pretty-quick/dist/scms/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/pretty-quick/dist/scms/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/psl/dist/psl.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/psl/dist/psl.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/psl/dist/psl.min.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/psl/dist/psl.min.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/shiki/dist/index.browser.mjs` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/shiki/dist/index.browser.mjs`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/shiki/dist/index.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/shiki/dist/index.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/shiki/dist/index.esm.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/shiki/dist/index.esm.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/shiki/dist/index.iife.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/shiki/dist/index.iife.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/shiki/dist/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/shiki/dist/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/shiki/dist/index.jsdelivr.iife.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/shiki/dist/index.jsdelivr.iife.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/shiki/dist/index.unpkg.iife.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/shiki/dist/index.unpkg.iife.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/shiki/dist/onig.wasm` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/shiki/dist/onig.wasm`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/source-map/dist/source-map.debug.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/source-map/dist/source-map.debug.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/source-map/dist/source-map.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/source-map/dist/source-map.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/source-map/dist/source-map.min.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/source-map/dist/source-map.min.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/source-map/dist/source-map.min.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/source-map/dist/source-map.min.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/terser/dist/bundle.min.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/terser/dist/bundle.min.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/bin-script-deprecated.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/bin-script-deprecated.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/bin.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/bin.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/bin.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/bin.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/bin.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/bin.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/argv-payload.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/argv-payload.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/argv-payload.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/argv-payload.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/child-entrypoint.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/child-entrypoint.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/child-entrypoint.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/child-entrypoint.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/child-loader.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/child-loader.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/child-loader.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/child-loader.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/child-require.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/child-require.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/child-require.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/child-require.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/spawn-child.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/spawn-child.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/child/spawn-child.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/child/spawn-child.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/cjs-resolve-hooks.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/cjs-resolve-hooks.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/cjs-resolve-hooks.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/cjs-resolve-hooks.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/configuration.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/configuration.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/configuration.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/configuration.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/esm.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/esm.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/esm.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/esm.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/esm.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/esm.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/file-extensions.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/file-extensions.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/file-extensions.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/file-extensions.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/index.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/index.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/index.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/index.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/module-type-classifier.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/module-type-classifier.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/module-type-classifier.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/module-type-classifier.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/node-module-type-classifier.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/node-module-type-classifier.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/node-module-type-classifier.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/node-module-type-classifier.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/repl.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/repl.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/repl.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/repl.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/repl.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/repl.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/resolver-functions.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/resolver-functions.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/resolver-functions.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/resolver-functions.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/transpilers/swc.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/transpilers/swc.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/transpilers/swc.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/transpilers/swc.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/transpilers/types.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/transpilers/types.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/transpilers/types.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/transpilers/types.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/ts-compiler-types.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/ts-compiler-types.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/ts-compiler-types.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/ts-compiler-types.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/ts-internals.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/ts-internals.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/ts-internals.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/ts-internals.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/ts-transpile-module.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/ts-transpile-module.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/ts-transpile-module.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/ts-transpile-module.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/tsconfig-schema.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/tsconfig-schema.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/tsconfigs.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/tsconfigs.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/tsconfigs.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/tsconfigs.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/util.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/util.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/dist/util.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/dist/util.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/node_modules/acorn-walk/dist/walk.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/node_modules/acorn-walk/dist/walk.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/node_modules/acorn-walk/dist/walk.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/node_modules/acorn-walk/dist/walk.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/node_modules/acorn-walk/dist/walk.mjs` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/node_modules/acorn-walk/dist/walk.mjs`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/node_modules/diff/dist/diff.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/node_modules/diff/dist/diff.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/ts-node/node_modules/diff/dist/diff.min.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/ts-node/node_modules/diff/dist/diff.min.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/index.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/index.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/application.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/application.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/application.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/application.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/context.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/context.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/context.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/context.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/convert-expression.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/convert-expression.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/converter.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/converter.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/converter.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/converter.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/comment.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/comment.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/comment.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/comment.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/index-signature.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/index-signature.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/signature.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/signature.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/signature.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/factories/signature.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/jsdoc.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/jsdoc.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/CategoryPlugin.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/CategoryPlugin.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/CategoryPlugin.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/CategoryPlugin.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/CommentPlugin.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/CommentPlugin.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/CommentPlugin.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/CommentPlugin.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/DecoratorPlugin.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/DecoratorPlugin.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/DecoratorPlugin.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/DecoratorPlugin.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/GroupPlugin.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/GroupPlugin.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/GroupPlugin.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/GroupPlugin.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/ImplementsPlugin.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/ImplementsPlugin.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/ImplementsPlugin.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/ImplementsPlugin.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/InheritDocPlugin.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/InheritDocPlugin.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/InheritDocPlugin.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/InheritDocPlugin.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/PackagePlugin.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/PackagePlugin.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/PackagePlugin.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/PackagePlugin.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/SourceLinkPlugin.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/SourceLinkPlugin.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/SourceLinkPlugin.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/SourceLinkPlugin.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/SourcePlugin.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/SourcePlugin.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/SourcePlugin.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/SourcePlugin.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/TypePlugin.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/TypePlugin.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/TypePlugin.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/TypePlugin.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/plugins/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/symbols.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/symbols.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/types.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/types.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/types.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/types.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/base-path.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/base-path.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/base-path.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/base-path.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/nodes.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/nodes.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/reflections.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/converter/utils/reflections.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/ReflectionCategory.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/ReflectionCategory.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/ReflectionCategory.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/ReflectionCategory.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/ReflectionGroup.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/ReflectionGroup.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/ReflectionGroup.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/ReflectionGroup.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/comments/comment.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/comments/comment.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/comments/comment.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/comments/comment.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/comments/tag.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/comments/tag.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/abstract.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/abstract.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/abstract.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/abstract.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/container.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/container.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/container.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/container.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/declaration.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/declaration.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/declaration.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/declaration.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/index.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/index.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/kind.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/kind.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/kind.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/kind.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/parameter.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/parameter.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/parameter.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/parameter.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/project.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/project.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/project.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/project.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/reference.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/reference.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/reference.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/reference.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/signature.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/signature.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/signature.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/signature.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/type-parameter.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/type-parameter.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/type-parameter.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/type-parameter.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/utils.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/reflections/utils.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/directory.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/directory.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/directory.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/directory.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/file.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/file.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/file.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/file.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/sources/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/types.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/types.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/types.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/models/types.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/components.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/components.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/components.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/components.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/events.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/events.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/events.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/events.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/AssetsPlugin.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/AssetsPlugin.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/AssetsPlugin.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/AssetsPlugin.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/JavascriptIndexPlugin.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/JavascriptIndexPlugin.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/JavascriptIndexPlugin.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/JavascriptIndexPlugin.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/LegendPlugin.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/LegendPlugin.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/LegendPlugin.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/LegendPlugin.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/MarkedLinksPlugin.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/MarkedLinksPlugin.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/MarkedLinksPlugin.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/MarkedLinksPlugin.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/plugins/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/renderer.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/renderer.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/renderer.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/renderer.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/theme.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/theme.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/theme.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/theme.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/MarkedPlugin.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/MarkedPlugin.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/MarkedPlugin.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/MarkedPlugin.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/DefaultTheme.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/DefaultTheme.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/DefaultTheme.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/DefaultTheme.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/DefaultThemeRenderContext.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/DefaultThemeRenderContext.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/DefaultThemeRenderContext.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/DefaultThemeRenderContext.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/layouts/default.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/layouts/default.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/analytics.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/analytics.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/anchor-icon.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/anchor-icon.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/breadcrumb.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/breadcrumb.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/comment.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/comment.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/footer.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/footer.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/header.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/header.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/hierarchy.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/hierarchy.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.declaration.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.declaration.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.getterSetter.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.getterSetter.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.reference.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.reference.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.signature.body.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.signature.body.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.signature.title.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.signature.title.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.signatures.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.signatures.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.sources.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/member.sources.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/members.group.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/members.group.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/members.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/members.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/navigation.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/navigation.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/parameter.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/parameter.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/type.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/type.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/typeAndParent.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/typeAndParent.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/typeParameters.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/partials/typeParameters.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/templates/reflection.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/default/templates/reflection.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/lib.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/lib.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/lib.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/output/themes/lib.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/components.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/components.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/components.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/components.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/events.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/events.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/events.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/events.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/index.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/index.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/schema.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/schema.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/schema.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/schema.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializer.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializer.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializer.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializer.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/comments/comment-tag.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/comments/comment-tag.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/comments/comment.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/comments/comment.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/decorator.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/decorator.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/decorator.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/decorator.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/models/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/models/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflection-category.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflection-category.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflection-category.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflection-category.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflection-group.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflection-group.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflection-group.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflection-group.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/abstract.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/abstract.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/container.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/container.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/container.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/container.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/declaration.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/declaration.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/declaration.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/declaration.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/parameter.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/parameter.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/reference.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/reference.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/reference.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/reference.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/signature.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/signature.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/type-parameter.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/reflections/type-parameter.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/sources/source-reference.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/sources/source-reference.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/sources/source-reference.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/sources/source-reference.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/abstract.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/abstract.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/array.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/array.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/conditional.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/conditional.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/index.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/index.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/indexed-access.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/indexed-access.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/inferred.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/inferred.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/intersection.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/intersection.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/intersection.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/intersection.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/intrinsic.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/intrinsic.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/intrinsic.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/intrinsic.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/literal.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/literal.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/mapped.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/mapped.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/optional.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/optional.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/optional.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/optional.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/predicate.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/predicate.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/query.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/query.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/reference.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/reference.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/reflection.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/reflection.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/rest.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/rest.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/template-literal.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/template-literal.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/tuple.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/tuple.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/tuple.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/tuple.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/type-operator.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/type-operator.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/union.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/union.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/unknown.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/unknown.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/unknown.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/serialization/serializers/types/unknown.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/array.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/array.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/array.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/array.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/component.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/component.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/component.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/component.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/entry-point.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/entry-point.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/entry-point.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/entry-point.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/enum.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/enum.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/events.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/events.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/events.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/events.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/fs.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/fs.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/fs.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/fs.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/general.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/general.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/general.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/general.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/highlighter.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/highlighter.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/hooks.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/hooks.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/hooks.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/hooks.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/index.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/index.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/jsx.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/jsx.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/jsx.elements.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/jsx.elements.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/jsx.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/jsx.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/loggers.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/loggers.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/loggers.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/loggers.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/declaration.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/declaration.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/declaration.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/declaration.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/help.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/help.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/index.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/index.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/options.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/options.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/options.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/options.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/arguments.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/arguments.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/tsconfig.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/tsconfig.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/typedoc.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/typedoc.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/typedoc.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/readers/typedoc.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/sources/typedoc.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/options/sources/typedoc.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/package-manifest.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/package-manifest.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/package-manifest.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/package-manifest.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/paths.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/paths.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/plugins.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/plugins.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/sort.d.ts` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/sort.d.ts`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/sort.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/utils/sort.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/validation/documentation.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/validation/documentation.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/typedoc/dist/lib/validation/exports.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/typedoc/dist/lib/validation/exports.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/url-parse/dist/url-parse.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/url-parse/dist/url-parse.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/url-parse/dist/url-parse.min.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/url-parse/dist/url-parse.min.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/url-parse/dist/url-parse.min.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/url-parse/dist/url-parse.min.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/workerpool/dist/worker.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/workerpool/dist/worker.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/workerpool/dist/worker.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/workerpool/dist/worker.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/workerpool/dist/workerpool.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/workerpool/dist/workerpool.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/workerpool/dist/workerpool.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/workerpool/dist/workerpool.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/workerpool/dist/workerpool.min.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/workerpool/dist/workerpool.min.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/workerpool/dist/workerpool.min.js.LICENSE.txt` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/workerpool/dist/workerpool.min.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/workerpool/dist/workerpool.min.js.map` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/workerpool/dist/workerpool.min.js.map`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/y18n/build/index.cjs` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/y18n/build/index.cjs`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/y18n/build/lib/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/y18n/build/lib/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/index.cjs` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/index.cjs`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/argsert.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/argsert.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/command.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/command.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/completion-templates.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/completion-templates.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/completion.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/completion.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/middleware.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/middleware.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/parse-command.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/parse-command.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/usage.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/usage.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/utils/apply-extends.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/utils/apply-extends.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/utils/levenshtein.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/utils/levenshtein.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/validation.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/validation.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs/build/lib/yargs-factory.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs/build/lib/yargs-factory.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs-parser/build/index.cjs` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs-parser/build/index.cjs`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs-parser/build/lib/index.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs-parser/build/lib/index.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs-parser/build/lib/string-utils.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs-parser/build/lib/string-utils.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs-parser/build/lib/tokenize-arg-string.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs-parser/build/lib/tokenize-arg-string.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/node_modules/yargs-parser/build/lib/yargs-parser.js` & `monaco_qt-0.1.8/monaco/monaco-editor/node_modules/yargs-parser/build/lib/yargs-parser.js`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco-editor/package.json` & `monaco_qt-0.1.8/monaco/monaco-editor/package.json`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/monaco/monaco_widget.py` & `monaco_qt-0.1.8/monaco/monaco_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from qtpy.QtCore import QObject, Signal, Slot, Property, QUrl
-from qtpy.QtWebEngineWidgets import * 
+from qtpy.QtWebEngineWidgets import *
 from qtpy.QtWebChannel import *
 
 from pathlib import Path
 import json
 
 
 class BaseBridge(QObject):
@@ -40,17 +40,17 @@
 class EditorBridge(BaseBridge):
     valueChanged = Signal()
     languageChanged = Signal()
     themeChanged = Signal()
 
     def __init__(self, parent=None):
         super().__init__(parent=parent)
-        self._value = ""
-        self._language = ""
-        self._theme = ""
+        self._value = ''
+        self._language = ''
+        self._theme = ''
 
     def getValue(self):
         return self._value
 
     def setValue(self, value):
         self._value = value
         self.valueChanged.emit()
@@ -66,21 +66,19 @@
         return self._theme
 
     def setTheme(self, theme):
         self._theme = theme
         self.themeChanged.emit()
 
     value = Property(str, fget=getValue, fset=setValue, notify=valueChanged)
-    language = Property(
-        str, fget=getLanguage, fset=setLanguage, notify=languageChanged
-    )
+    language = Property(str, fget=getLanguage, fset=setLanguage, notify=languageChanged)
     theme = Property(str, fget=getTheme, fset=setTheme, notify=themeChanged)
 
 
-index = Path(__file__).parent / "index.html"
+index = Path(__file__).parent / 'index.html'
 
 with open(index) as f:
     raw_html = f.read()
 
 
 class MonacoPage(QWebEnginePage):
     def javaScriptConsoleMessage(self, level, message, line, source):
@@ -96,30 +94,36 @@
 
         html = raw_html.replace('width:400px;', f'width:{self.size().width()}px;')
         html = raw_html.replace('height:400px;', f'height:{self.size().height()}px;')
 
         page = MonacoPage(parent=self)
         self.setPage(page)
 
-        filename = Path(__file__).parent / "index.html"
-        self.setHtml(html, QUrl.fromLocalFile(filename.as_posix()) )
+        filename = Path(__file__).parent / 'index.html'
+        self.setHtml(html, QUrl.fromLocalFile(filename.as_posix()))
 
         self._channel = QWebChannel(self)
         self._bridge = EditorBridge()
 
         self.page().setWebChannel(self._channel)
-        self._channel.registerObject("bridge", self._bridge)
+        self._channel.registerObject('bridge', self._bridge)
 
         self._bridge.initialized.connect(self.initialized)
         self._bridge.valueChanged.connect(lambda: self.textChanged.emit(self._bridge.value))
 
     def text(self):
         return self._bridge.value
 
     def setText(self, text):
-        self._bridge.send_to_js("value", text)
+        self._bridge.send_to_js('value', text)
 
     def language(self):
         return self._bridge.language
 
     def setLanguage(self, language):
-        self._bridge.send_to_js("language", language)
+        self._bridge.send_to_js('language', language)
+
+    def theme(self):
+        return self._bridge.theme
+
+    def setTheme(self, theme):
+        self._bridge.send_to_js('theme', theme)
```

### Comparing `monaco-qt-0.1.7/monaco_qt.egg-info/PKG-INFO` & `monaco_qt-0.1.8/monaco_qt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monaco-qt
-Version: 0.1.7
+Version: 0.1.8
 Summary: The Monaco editor as a Qt Widget
 Home-page: https://github.com/DaelonSuzuka/monaco-qt
 Author: David Kincaid
 Author-email: dlkincaid0@gmail.com
 Keywords: qtstrap,qt,pyqt,monaco,text editor
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Widget Sets
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+Requires-Dist: QtPy
 
 # monaco-qt
 
 [![license](https://img.shields.io/pypi/l/monaco-qt.svg)](./LICENSE)
 [![pypi version](https://img.shields.io/pypi/v/monaco-qt.svg)](https://pypi.org/project/monaco-qt/)
 [![PyPI status](https://img.shields.io/pypi/status/monaco-qt.svg)](https://github.com/DaelonSuzuka/monaco-qt/)
```

### Comparing `monaco-qt-0.1.7/monaco_qt.egg-info/SOURCES.txt` & `monaco_qt-0.1.8/monaco_qt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monaco-qt-0.1.7/setup.py` & `monaco_qt-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
 
 setup(
     name="monaco-qt",
-    version="0.1.7",
+    version="0.1.8",
     packages=find_packages(),
     install_requires=[
         'QtPy',
     ],
     package_data={'monaco': ['*.js', '*.html', 'monaco-editor/**']},
     include_package_data=True,
     entry_points={
```

