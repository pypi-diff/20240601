# Comparing `tmp/gitlab_projects_issues-1.0.0.tar.gz` & `tmp/gitlab_projects_issues-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_projects_issues-1.0.0.tar", last modified: Sat Jun  1 19:49:44 2024, max compression
+gzip compressed data, was "gitlab_projects_issues-1.0.1.tar", last modified: Sat Jun  1 21:42:09 2024, max compression
```

## Comparing `gitlab_projects_issues-1.0.0.tar` & `gitlab_projects_issues-1.0.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 19:49:44.352258 gitlab_projects_issues-1.0.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 19:49:44.344258 gitlab_projects_issues-1.0.0/.chglog/
--rwxrwxrwx   0 root         (0) root         (0)      649 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/.chglog/CHANGELOG.tpl.md
--rw-rw-rw-   0 root         (0) root         (0)      759 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/.chglog/changelog.sh
--rwxrwxrwx   0 root         (0) root         (0)      701 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/.chglog/config.yml
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)    13581 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/.markdownlint.json
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/.style.yapf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 19:49:44.344258 gitlab_projects_issues-1.0.0/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/.vscode/extensions.json
--rw-rw-rw-   0 root         (0) root         (0)     1252 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/.vscode/settings.json
--rw-rw-rw-   0 root         (0) root         (0)     6055 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6485 2024-06-01 19:49:44.352258 gitlab_projects_issues-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4828 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 19:49:44.352258 gitlab_projects_issues-1.0.0/gitlab_projects_issues.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6485 2024-06-01 19:49:44.000000 gitlab_projects_issues-1.0.0/gitlab_projects_issues.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1046 2024-06-01 19:49:44.000000 gitlab_projects_issues-1.0.0/gitlab_projects_issues.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 19:49:44.000000 gitlab_projects_issues-1.0.0/gitlab_projects_issues.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2024-06-01 19:49:44.000000 gitlab_projects_issues-1.0.0/gitlab_projects_issues.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-06-01 19:49:44.000000 gitlab_projects_issues-1.0.0/gitlab_projects_issues.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-06-01 19:49:44.000000 gitlab_projects_issues-1.0.0/gitlab_projects_issues.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 19:49:44.347258 gitlab_projects_issues-1.0.0/requirements/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/requirements/build.txt
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/requirements/deploy.txt
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/requirements/quality.txt
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/requirements/runtime.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-06-01 19:49:44.352258 gitlab_projects_issues-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2886 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 19:49:44.347258 gitlab_projects_issues-1.0.0/src/
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/src/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 19:49:44.348258 gitlab_projects_issues-1.0.0/src/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/src/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9193 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/src/cli/entrypoint.py
--rwxrwxrwx   0 root         (0) root         (0)     6171 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/src/cli/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 19:49:44.348258 gitlab_projects_issues-1.0.0/src/features/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/src/features/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      597 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/src/features/gitlab.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 19:49:44.349258 gitlab_projects_issues-1.0.0/src/package/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/src/package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      761 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/src/package/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)     3810 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/src/package/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     6845 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/src/package/updates.py
--rw-rw-rw-   0 root         (0) root         (0)     1607 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/src/package/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 19:49:44.350258 gitlab_projects_issues-1.0.0/src/prints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/src/prints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2549 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/src/prints/boxes.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/src/prints/colors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 19:49:44.351258 gitlab_projects_issues-1.0.0/src/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/src/system/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1788 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/src/system/platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 19:49:44.351258 gitlab_projects_issues-1.0.0/src/types/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/src/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1898 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/src/types/milestones.py
--rw-rw-rw-   0 root         (0) root         (0)     3449 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/src/types/statistics.py
--rw-rw-rw-   0 root         (0) root         (0)     3849 2024-06-01 19:49:40.000000 gitlab_projects_issues-1.0.0/src/types/strings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.760916 gitlab_projects_issues-1.0.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.752916 gitlab_projects_issues-1.0.1/.chglog/
+-rwxrwxrwx   0 root         (0) root         (0)      649 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/.chglog/CHANGELOG.tpl.md
+-rw-rw-rw-   0 root         (0) root         (0)      759 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/.chglog/changelog.sh
+-rwxrwxrwx   0 root         (0) root         (0)      714 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/.chglog/config.yml
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)    13599 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/.markdownlint.json
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/.style.yapf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.752916 gitlab_projects_issues-1.0.1/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/.vscode/extensions.json
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7306 2024-06-01 21:42:09.760916 gitlab_projects_issues-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5649 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.760916 gitlab_projects_issues-1.0.1/gitlab_projects_issues.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7306 2024-06-01 21:42:09.000000 gitlab_projects_issues-1.0.1/gitlab_projects_issues.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1046 2024-06-01 21:42:09.000000 gitlab_projects_issues-1.0.1/gitlab_projects_issues.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 21:42:09.000000 gitlab_projects_issues-1.0.1/gitlab_projects_issues.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2024-06-01 21:42:09.000000 gitlab_projects_issues-1.0.1/gitlab_projects_issues.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2024-06-01 21:42:09.000000 gitlab_projects_issues-1.0.1/gitlab_projects_issues.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-06-01 21:42:09.000000 gitlab_projects_issues-1.0.1/gitlab_projects_issues.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.754916 gitlab_projects_issues-1.0.1/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/requirements/build.txt
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/requirements/deploy.txt
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/requirements/quality.txt
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/requirements/runtime.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-01 21:42:09.760916 gitlab_projects_issues-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2886 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.755916 gitlab_projects_issues-1.0.1/src/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.756916 gitlab_projects_issues-1.0.1/src/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9193 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/cli/entrypoint.py
+-rwxrwxrwx   0 root         (0) root         (0)     6171 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/cli/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.756916 gitlab_projects_issues-1.0.1/src/features/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/features/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      597 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/features/gitlab.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.757916 gitlab_projects_issues-1.0.1/src/package/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      761 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/package/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)     3810 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/package/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     6845 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/package/updates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/package/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.758916 gitlab_projects_issues-1.0.1/src/prints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/prints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2549 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/prints/boxes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/prints/colors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.758916 gitlab_projects_issues-1.0.1/src/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/system/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1788 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/system/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:42:09.759916 gitlab_projects_issues-1.0.1/src/types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1898 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/types/milestones.py
+-rw-rw-rw-   0 root         (0) root         (0)     3449 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/types/statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2024-06-01 21:42:06.000000 gitlab_projects_issues-1.0.1/src/types/strings.py
```

### Comparing `gitlab_projects_issues-1.0.0/.chglog/CHANGELOG.tpl.md` & `gitlab_projects_issues-1.0.1/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.0/.chglog/changelog.sh` & `gitlab_projects_issues-1.0.1/.chglog/changelog.sh`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.0/.chglog/config.yml` & `gitlab_projects_issues-1.0.1/.chglog/config.yml`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
       #   - fix
       #   - perf
       #   - refactor
       #   - test
   commit_groups:
     title_maps:
       chore: Cleanups
+      ci: CI
       docs: Documentation
       feat: Features
       fix: Bug Fixes
       perf: Performance Improvements
       refactor: Code Refactoring
       test: Test
   header:
```

### Comparing `gitlab_projects_issues-1.0.0/.gitlab-ci.yml` & `gitlab_projects_issues-1.0.1/.gitlab-ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -38,25 +38,25 @@
         chmod +x ./.tmp/git-chglog
       fi
     - 'echo -n " > Current commit : "'
     - git describe --always
     - echo ''
     - 'read -p " > Release tag : " -r tag'
     - echo ''
-    - git tag -f -m '' "${tag}"
+    - git tag -f -m "${tag}" "${tag}"
     - ./.tmp/git-chglog -o ./CHANGELOG.md
     - sed -i "s#raw/[^/]*/docs#raw/${tag}/docs#g" ./README.md
     - git add -v ./CHANGELOG.md ./README.md
     - 'git commit -m "docs(changelog): regenerate release tag changes history" -s'
-    - git tag -f -m '' "${tag}"
+    - git tag -f -m "${tag}" "${tag}"
     - ./.tmp/git-chglog -o ./CHANGELOG.md
     - sh ./.chglog/changelog.sh --clean
     - git add -v ./CHANGELOG.md
     - git commit --amend --no-edit
-    - git tag -f -m '' "${tag}"
+    - git tag -f -m "${tag}" "${tag}"
   rules:
     - if: $CI_LOCAL
 
 images:
   stage: development
   image: local:silent
   script:
```

### Comparing `gitlab_projects_issues-1.0.0/.style.yapf` & `gitlab_projects_issues-1.0.1/.style.yapf`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.0/.vscode/extensions.json` & `gitlab_projects_issues-1.0.1/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.0/.vscode/settings.json` & `gitlab_projects_issues-1.0.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.0/LICENSE` & `gitlab_projects_issues-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.0/PKG-INFO` & `gitlab_projects_issues-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-issues
-Version: 1.0.0
+Version: 1.0.1
 Summary: Generate GitLab project issues and milestones statistics automatically
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-issues
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-issues/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-issues/blob/main/CHANGELOG.md
@@ -35,48 +35,64 @@
 
 # gitlab-projects-issues
 
 <!-- markdownlint-disable no-inline-html -->
 
 [![Build](https://gitlab.com/AdrianDC/gitlab-projects-issues/badges/main/pipeline.svg)](https://gitlab.com/AdrianDC/gitlab-projects-issues/-/commits/main/)
 
-Configure GitLab groups and projects settings automatically
+Generate GitLab project issues and milestones statistics automatically
 
 ---
 
 ## Purpose
 
-This tool can automatically configure and update the GitLab settings  
-of groups, subgroups and projects, using multiple available options.
+This tool can automatically generate issues and milestones statistics,  
+by analyzing project's issues, detecting milestones and assignees.
 
-Repetitive tasks can be performed accross multiple projects at once,  
-for example protecting tags and branches, or setting a new avatar recursively.
+If issues without time estimations are found, `~?` will be shown before time outputs.
+
+Milestone statistics will automatically be injected in the milestone description,  
+with a markdown table of assignees, timings, progress and issues total.
 
 The following step is required before using the tool:
 
 - The GitLab user tokens must be created with an `api` scope (a short expiration date is recommended)
 
 ---
 
+## Outputs
+
+### Milestone statistics - NAME
+
+| Assignees | Issues | Estimated | Spent | Remaining | Progress |
+|-----------|--------|-----------|-------|-----------|----------|
+| **Without assignee** | 10 | 18d | 18d | / | ██████████ 100.00% |
+| **USER ONE** | 22 | 42d | 5d | 37d | █▂▁▁▁▁▁▁▁▁ 11.90% |
+| **USER TWO** | 29 | 50d 2h | 20d 6h | 29d 4h | ████▂▁▁▁▁▁ 41.29% |
+| **USER THREE** | 7 | 9d 2h | 3d 4h | 5d 6h | ███▅▁▁▁▁▁▁ 37.84% |
+| **USER FOUR** | 6 | 21d | / | 21d | ▁▁▁▁▁▁▁▁▁▁ 0.00% |
+| _**Total**_ | _74_ | _135d 4h_ | _47d 2h_ | 93d 2h | _███▄▁▁▁▁▁▁ 34.87%_ |
+
+_Last update using gitlab-projects-issues : 2024-06-01 19:38:48 UTC_
+
+---
+
 ## Examples
 
 <!-- prettier-ignore-start -->
 
 ```bash
 # Show the helper menu
 gitlab-projects-issues
 
-# Protect all projects' tags under a group
-gitlab-projects-issues --protect-tags -- 'https://gitlab.com' 'group'
-
-# Update all avatars and descriptions under a group
-gitlab-projects-issues --set-avatar ./avatar.png --update-description 'https://gitlab.com' 'group'
+# Inject milestones statistics into milestones' description
+gitlab-projects-issues --milestones-statistics 'https://gitlab.com' 'group/project'
 
-# Automatically detect and reset features of projects based on usage
-gitlab-projects-issues --reset-features 'https://gitlab.com' 'group/project'
+# Inject milestones statistics into milestones' description (with default 20h time per unestimated issues)
+gitlab-projects-issues --milestones-statistics --default-estimate '20' 'https://gitlab.com' 'group/project'
 ```
 
 <!-- prettier-ignore-end -->
 
 ---
 
 ## Usage
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gitlab_projects_issues-1.0.0/README.md` & `gitlab_projects_issues-1.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,63 @@
 # gitlab-projects-issues
 
 <!-- markdownlint-disable no-inline-html -->
 
 [![Build](https://gitlab.com/AdrianDC/gitlab-projects-issues/badges/main/pipeline.svg)](https://gitlab.com/AdrianDC/gitlab-projects-issues/-/commits/main/)
 
-Configure GitLab groups and projects settings automatically
+Generate GitLab project issues and milestones statistics automatically
 
 ---
 
 ## Purpose
 
-This tool can automatically configure and update the GitLab settings  
-of groups, subgroups and projects, using multiple available options.
+This tool can automatically generate issues and milestones statistics,  
+by analyzing project's issues, detecting milestones and assignees.
 
-Repetitive tasks can be performed accross multiple projects at once,  
-for example protecting tags and branches, or setting a new avatar recursively.
+If issues without time estimations are found, `~?` will be shown before time outputs.
+
+Milestone statistics will automatically be injected in the milestone description,  
+with a markdown table of assignees, timings, progress and issues total.
 
 The following step is required before using the tool:
 
 - The GitLab user tokens must be created with an `api` scope (a short expiration date is recommended)
 
 ---
 
+## Outputs
+
+### Milestone statistics - NAME
+
+| Assignees | Issues | Estimated | Spent | Remaining | Progress |
+|-----------|--------|-----------|-------|-----------|----------|
+| **Without assignee** | 10 | 18d | 18d | / | ██████████ 100.00% |
+| **USER ONE** | 22 | 42d | 5d | 37d | █▂▁▁▁▁▁▁▁▁ 11.90% |
+| **USER TWO** | 29 | 50d 2h | 20d 6h | 29d 4h | ████▂▁▁▁▁▁ 41.29% |
+| **USER THREE** | 7 | 9d 2h | 3d 4h | 5d 6h | ███▅▁▁▁▁▁▁ 37.84% |
+| **USER FOUR** | 6 | 21d | / | 21d | ▁▁▁▁▁▁▁▁▁▁ 0.00% |
+| _**Total**_ | _74_ | _135d 4h_ | _47d 2h_ | 93d 2h | _███▄▁▁▁▁▁▁ 34.87%_ |
+
+_Last update using gitlab-projects-issues : 2024-06-01 19:38:48 UTC_
+
+---
+
 ## Examples
 
 <!-- prettier-ignore-start -->
 
 ```bash
 # Show the helper menu
 gitlab-projects-issues
 
-# Protect all projects' tags under a group
-gitlab-projects-issues --protect-tags -- 'https://gitlab.com' 'group'
-
-# Update all avatars and descriptions under a group
-gitlab-projects-issues --set-avatar ./avatar.png --update-description 'https://gitlab.com' 'group'
+# Inject milestones statistics into milestones' description
+gitlab-projects-issues --milestones-statistics 'https://gitlab.com' 'group/project'
 
-# Automatically detect and reset features of projects based on usage
-gitlab-projects-issues --reset-features 'https://gitlab.com' 'group/project'
+# Inject milestones statistics into milestones' description (with default 20h time per unestimated issues)
+gitlab-projects-issues --milestones-statistics --default-estimate '20' 'https://gitlab.com' 'group/project'
 ```
 
 <!-- prettier-ignore-end -->
 
 ---
 
 ## Usage
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gitlab_projects_issues-1.0.0/gitlab_projects_issues.egg-info/PKG-INFO` & `gitlab_projects_issues-1.0.1/gitlab_projects_issues.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-projects-issues
-Version: 1.0.0
+Version: 1.0.1
 Summary: Generate GitLab project issues and milestones statistics automatically
 Home-page: https://gitlab.com/AdrianDC/gitlab-projects-issues
 Author: Adrian DC
 Author-email: radian.dc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://gitlab.com/AdrianDC/gitlab-projects-issues/-/issues
 Project-URL: Changelog, https://gitlab.com/AdrianDC/gitlab-projects-issues/blob/main/CHANGELOG.md
@@ -35,48 +35,64 @@
 
 # gitlab-projects-issues
 
 <!-- markdownlint-disable no-inline-html -->
 
 [![Build](https://gitlab.com/AdrianDC/gitlab-projects-issues/badges/main/pipeline.svg)](https://gitlab.com/AdrianDC/gitlab-projects-issues/-/commits/main/)
 
-Configure GitLab groups and projects settings automatically
+Generate GitLab project issues and milestones statistics automatically
 
 ---
 
 ## Purpose
 
-This tool can automatically configure and update the GitLab settings  
-of groups, subgroups and projects, using multiple available options.
+This tool can automatically generate issues and milestones statistics,  
+by analyzing project's issues, detecting milestones and assignees.
 
-Repetitive tasks can be performed accross multiple projects at once,  
-for example protecting tags and branches, or setting a new avatar recursively.
+If issues without time estimations are found, `~?` will be shown before time outputs.
+
+Milestone statistics will automatically be injected in the milestone description,  
+with a markdown table of assignees, timings, progress and issues total.
 
 The following step is required before using the tool:
 
 - The GitLab user tokens must be created with an `api` scope (a short expiration date is recommended)
 
 ---
 
+## Outputs
+
+### Milestone statistics - NAME
+
+| Assignees | Issues | Estimated | Spent | Remaining | Progress |
+|-----------|--------|-----------|-------|-----------|----------|
+| **Without assignee** | 10 | 18d | 18d | / | ██████████ 100.00% |
+| **USER ONE** | 22 | 42d | 5d | 37d | █▂▁▁▁▁▁▁▁▁ 11.90% |
+| **USER TWO** | 29 | 50d 2h | 20d 6h | 29d 4h | ████▂▁▁▁▁▁ 41.29% |
+| **USER THREE** | 7 | 9d 2h | 3d 4h | 5d 6h | ███▅▁▁▁▁▁▁ 37.84% |
+| **USER FOUR** | 6 | 21d | / | 21d | ▁▁▁▁▁▁▁▁▁▁ 0.00% |
+| _**Total**_ | _74_ | _135d 4h_ | _47d 2h_ | 93d 2h | _███▄▁▁▁▁▁▁ 34.87%_ |
+
+_Last update using gitlab-projects-issues : 2024-06-01 19:38:48 UTC_
+
+---
+
 ## Examples
 
 <!-- prettier-ignore-start -->
 
 ```bash
 # Show the helper menu
 gitlab-projects-issues
 
-# Protect all projects' tags under a group
-gitlab-projects-issues --protect-tags -- 'https://gitlab.com' 'group'
-
-# Update all avatars and descriptions under a group
-gitlab-projects-issues --set-avatar ./avatar.png --update-description 'https://gitlab.com' 'group'
+# Inject milestones statistics into milestones' description
+gitlab-projects-issues --milestones-statistics 'https://gitlab.com' 'group/project'
 
-# Automatically detect and reset features of projects based on usage
-gitlab-projects-issues --reset-features 'https://gitlab.com' 'group/project'
+# Inject milestones statistics into milestones' description (with default 20h time per unestimated issues)
+gitlab-projects-issues --milestones-statistics --default-estimate '20' 'https://gitlab.com' 'group/project'
 ```
 
 <!-- prettier-ignore-end -->
 
 ---
 
 ## Usage
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gitlab_projects_issues-1.0.0/gitlab_projects_issues.egg-info/SOURCES.txt` & `gitlab_projects_issues-1.0.1/gitlab_projects_issues.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.0/setup.py` & `gitlab_projects_issues-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.0/src/cli/entrypoint.py` & `gitlab_projects_issues-1.0.1/src/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.0/src/cli/main.py` & `gitlab_projects_issues-1.0.1/src/cli/main.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.0/src/features/gitlab.py` & `gitlab_projects_issues-1.0.1/src/features/gitlab.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.0/src/package/bundle.py` & `gitlab_projects_issues-1.0.1/src/package/bundle.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.0/src/package/settings.py` & `gitlab_projects_issues-1.0.1/src/package/settings.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.0/src/package/updates.py` & `gitlab_projects_issues-1.0.1/src/package/updates.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.0/src/package/version.py` & `gitlab_projects_issues-1.0.1/src/package/version.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.0/src/prints/boxes.py` & `gitlab_projects_issues-1.0.1/src/prints/boxes.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.0/src/prints/colors.py` & `gitlab_projects_issues-1.0.1/src/prints/colors.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.0/src/system/platform.py` & `gitlab_projects_issues-1.0.1/src/system/platform.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.0/src/types/milestones.py` & `gitlab_projects_issues-1.0.1/src/types/milestones.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.0/src/types/statistics.py` & `gitlab_projects_issues-1.0.1/src/types/statistics.py`

 * *Files identical despite different names*

### Comparing `gitlab_projects_issues-1.0.0/src/types/strings.py` & `gitlab_projects_issues-1.0.1/src/types/strings.py`

 * *Files identical despite different names*

