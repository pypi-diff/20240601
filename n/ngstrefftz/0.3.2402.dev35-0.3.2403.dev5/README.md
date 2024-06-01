# Comparing `tmp/ngstrefftz-0.3.2402.dev35.tar.gz` & `tmp/ngstrefftz-0.3.2403.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngstrefftz-0.3.2402.dev35.tar", last modified: Thu May  9 09:31:59 2024, max compression
+gzip compressed data, was "ngstrefftz-0.3.2403.dev5.tar", last modified: Sat Jun  1 14:06:08 2024, max compression
```

## Comparing `ngstrefftz-0.3.2402.dev35.tar` & `ngstrefftz-0.3.2403.dev5.tar`

### file list

```diff
@@ -1,181 +1,181 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.550742 ngstrefftz-0.3.2402.dev35/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.526741 ngstrefftz-0.3.2402.dev35/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.530741 ngstrefftz-0.3.2402.dev35/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.github/workflows/build_linux_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.github/workflows/build_pip.ps1
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.github/workflows/build_pip.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.github/workflows/build_pip_mac.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.github/workflows/fix_auditwheel_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.github/workflows/ngsolve_version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.530741 ngstrefftz-0.3.2402.dev35/.github/workflows/pyodide/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.github/workflows/pyodide/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.github/workflows/pyodide/build_in_docker.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.github/workflows/pyodide/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.github/workflows/pyodide/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-09 09:31:59.550742 ngstrefftz-0.3.2402.dev35/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.530741 ngstrefftz-0.3.2402.dev35/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.530741 ngstrefftz-0.3.2402.dev35/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/_static/breadcrumbs.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.530741 ngstrefftz-0.3.2402.dev35/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/_static/css/mytheme.css
--rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/contrib.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/docu.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/intro.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.534741 ngstrefftz-0.3.2402.dev35/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz-adv.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz-helm.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz-poi.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz-stokes.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz-wave.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/helmholtz.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/index.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/laplace.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/qtwave.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/tunfitted.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/twave.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/notebooks/twavetents.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.534741 ngstrefftz-0.3.2402.dev35/docs/paper/
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/paper/codemeta.json
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.526741 ngstrefftz-0.3.2402.dev35/external_dependencies/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.534741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.526741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.534741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/build_pip.ps1
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/build_pip.sh
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/build_pip_mac.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/fix_auditwheel_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/ngsolve_version.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.526741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.534741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/advection/
--rw-r--r--   0 runner    (1001) docker     (127)    10824 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/advection/advection2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/advection/advection2d_periodic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.534741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/burgers/
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/burgers/burgers1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/burgers/burgers2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.534741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/euler/
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/euler/euler2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.538741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/maxwell/
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/maxwell/maxwell3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.538741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.538741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/tents/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/tents/draw3dtent.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/tents/draw3dvertex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.538741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/wave/
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/wave/horn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/wave/wave2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/wave/wave3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.538741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    26966 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/BurgersMTP.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/INDEX.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    24974 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/StartPitching.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.538741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/figs/
--rw-r--r--   0 runner    (1001) docker     (127)    28475 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/figs/CausalityCond.png
--rw-r--r--   0 runner    (1001) docker     (127)    57380 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/figs/dag.png
--rw-r--r--   0 runner    (1001) docker     (127)    91865 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/figs/map.png
--rw-r--r--   0 runner    (1001) docker     (127)    70062 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/figs/subtents.png
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.538741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/py/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.542741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/py/conslaw/
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/py/conslaw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.542741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/py/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/py/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/py/utils/_drawtents.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/py/utils/_drawtents2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.542741 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/advection.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/burgers.cpp
--rw-r--r--   0 runner    (1001) docker     (127)   133375 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/concurrentqueue.h
--rw-r--r--   0 runner    (1001) docker     (127)    17133 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/conservationlaw.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    15095 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/euler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/maxwell.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/paralleldepend.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/python_conslaw.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/python_tents.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/symbolic.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    31227 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    47173 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/tents.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/tents.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/tentsolver.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/tentsolver_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/vis3d.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/vis3d.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/wave.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.546742 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/tests/test_burgers_2D.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/tests/test_causal_tents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/tests/test_conslaw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/tests/test_tent_height_2D.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-09 09:31:06.000000 ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/tests/test_tentlayers.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 09:31:59.550742 ngstrefftz-0.3.2402.dev35/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.550742 ngstrefftz-0.3.2402.dev35/src/
--rw-r--r--   0 runner    (1001) docker     (127)    10264 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/airy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/condensedg.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/condensedg.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13580 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/diffopmapped.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    26481 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/embtrefftz.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/embtrefftz.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/mesh1dtents.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/mesh1dtents.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/monomialfespace.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/monomialfespace.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.550742 ngstrefftz-0.3.2402.dev35/src/ngstrefftz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-09 09:31:59.000000 ngstrefftz-0.3.2402.dev35/src/ngstrefftz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-05-09 09:31:59.000000 ngstrefftz-0.3.2402.dev35/src/ngstrefftz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:31:59.000000 ngstrefftz-0.3.2402.dev35/src/ngstrefftz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-09 09:31:59.000000 ngstrefftz-0.3.2402.dev35/src/ngstrefftz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 09:31:59.000000 ngstrefftz-0.3.2402.dev35/src/ngstrefftz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/ngsttd.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/planewavefe.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12393 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/planewavefe.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/python_trefftz.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    46982 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/scalarmappedfe.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14965 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/scalarmappedfe.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/specialcoefficientfunction.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/specialcoefficientfunction.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    60694 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/specialintegrator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/specialintegrator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    56525 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/trefftzfespace.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/trefftzfespace.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    45126 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/twavetents.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8472 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/src/twavetents.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:31:59.550742 ngstrefftz-0.3.2402.dev35/test/
--rw-r--r--   0 runner    (1001) docker     (127)    19025 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/test/dg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/test/embt.py
--rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/test/tents.py
--rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-05-09 09:31:05.000000 ngstrefftz-0.3.2402.dev35/test/trefftz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.342658 ngstrefftz-0.3.2403.dev5/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.314658 ngstrefftz-0.3.2403.dev5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.322658 ngstrefftz-0.3.2403.dev5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/.github/workflows/build_linux_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/.github/workflows/build_pip.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/.github/workflows/build_pip.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/.github/workflows/build_pip_mac.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/.github/workflows/fix_auditwheel_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/.github/workflows/ngsolve_version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.322658 ngstrefftz-0.3.2403.dev5/.github/workflows/pyodide/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/.github/workflows/pyodide/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/.github/workflows/pyodide/build_in_docker.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/.github/workflows/pyodide/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/.github/workflows/pyodide/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-06-01 14:06:08.342658 ngstrefftz-0.3.2403.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.322658 ngstrefftz-0.3.2403.dev5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.322658 ngstrefftz-0.3.2403.dev5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/_static/breadcrumbs.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.322658 ngstrefftz-0.3.2403.dev5/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/_static/css/mytheme.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/contrib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/docu.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/intro.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.326658 ngstrefftz-0.3.2403.dev5/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/notebooks/embTrefftz-adv.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/notebooks/embTrefftz-helm.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/notebooks/embTrefftz-poi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/notebooks/embTrefftz-stokes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/notebooks/embTrefftz-wave.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/notebooks/embTrefftz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/notebooks/helmholtz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/notebooks/index.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/notebooks/laplace.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/notebooks/qtwave.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/notebooks/tunfitted.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/notebooks/twave.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/notebooks/twavetents.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.326658 ngstrefftz-0.3.2403.dev5/docs/paper/
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/paper/codemeta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.314658 ngstrefftz-0.3.2403.dev5/external_dependencies/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.326658 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.318658 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.326658 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/.github/workflows/build_pip.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/.github/workflows/build_pip.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/.github/workflows/build_pip_mac.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/.github/workflows/fix_auditwheel_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/.github/workflows/ngsolve_version.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.318658 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.326658 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/advection/
+-rw-r--r--   0 runner    (1001) docker     (127)    10824 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/advection/advection2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/advection/advection2d_periodic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.326658 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/burgers/
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/burgers/burgers1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/burgers/burgers2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.326658 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/euler/
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/euler/euler2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.326658 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/maxwell/
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/maxwell/maxwell3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.330659 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.330659 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/tents/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/tents/draw3dtent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/tents/draw3dvertex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.330659 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/wave/
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/wave/horn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/wave/wave2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/wave/wave3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.330659 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    26966 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/docs/BurgersMTP.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/docs/INDEX.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24974 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/docs/StartPitching.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.330659 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/docs/figs/
+-rw-r--r--   0 runner    (1001) docker     (127)    28475 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/docs/figs/CausalityCond.png
+-rw-r--r--   0 runner    (1001) docker     (127)    57380 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/docs/figs/dag.png
+-rw-r--r--   0 runner    (1001) docker     (127)    91865 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/docs/figs/map.png
+-rw-r--r--   0 runner    (1001) docker     (127)    70062 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/docs/figs/subtents.png
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.330659 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/py/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.334658 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/py/conslaw/
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/py/conslaw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.334658 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/py/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/py/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/py/utils/_drawtents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/py/utils/_drawtents2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.338658 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/advection.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/burgers.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)   133375 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/concurrentqueue.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17133 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/conservationlaw.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15095 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/euler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/maxwell.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/paralleldepend.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/python_conslaw.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/python_tents.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/symbolic.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    31227 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    47173 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/tents.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/tents.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/tentsolver.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/tentsolver_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/vis3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/vis3d.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/wave.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.338658 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/tests/test_burgers_2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/tests/test_causal_tents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/tests/test_conslaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/tests/test_tent_height_2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-06-01 14:04:25.000000 ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/tests/test_tentlayers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 14:06:08.342658 ngstrefftz-0.3.2403.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.342658 ngstrefftz-0.3.2403.dev5/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    10264 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/airy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/condensedg.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/condensedg.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13580 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/diffopmapped.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    26613 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/embtrefftz.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/embtrefftz.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/mesh1dtents.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/mesh1dtents.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/monomialfespace.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/monomialfespace.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.342658 ngstrefftz-0.3.2403.dev5/src/ngstrefftz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-06-01 14:06:08.000000 ngstrefftz-0.3.2403.dev5/src/ngstrefftz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-06-01 14:06:08.000000 ngstrefftz-0.3.2403.dev5/src/ngstrefftz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 14:06:08.000000 ngstrefftz-0.3.2403.dev5/src/ngstrefftz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-01 14:06:08.000000 ngstrefftz-0.3.2403.dev5/src/ngstrefftz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-01 14:06:08.000000 ngstrefftz-0.3.2403.dev5/src/ngstrefftz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/ngsttd.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/planewavefe.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12393 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/planewavefe.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/python_trefftz.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    46982 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/scalarmappedfe.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14965 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/scalarmappedfe.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/specialcoefficientfunction.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/specialcoefficientfunction.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    60694 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/specialintegrator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/specialintegrator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    60446 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/trefftzfespace.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/trefftzfespace.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    45126 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/twavetents.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8472 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/src/twavetents.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:06:08.342658 ngstrefftz-0.3.2403.dev5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    19025 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/test/dg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/test/embt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/test/tents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-06-01 14:04:24.000000 ngstrefftz-0.3.2403.dev5/test/trefftz.py
```

### Comparing `ngstrefftz-0.3.2402.dev35/.github/workflows/build.yml` & `ngstrefftz-0.3.2403.dev5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/.github/workflows/build_linux_test.sh` & `ngstrefftz-0.3.2403.dev5/.github/workflows/build_linux_test.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/.github/workflows/build_pip.ps1` & `ngstrefftz-0.3.2403.dev5/.github/workflows/build_pip.ps1`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/.github/workflows/build_pip.sh` & `ngstrefftz-0.3.2403.dev5/.github/workflows/build_pip.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/.github/workflows/build_pip_mac.sh` & `ngstrefftz-0.3.2403.dev5/.github/workflows/build_pip_mac.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/.github/workflows/fix_auditwheel_policy.py` & `ngstrefftz-0.3.2403.dev5/.github/workflows/fix_auditwheel_policy.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/.github/workflows/pyodide/Dockerfile` & `ngstrefftz-0.3.2403.dev5/.github/workflows/pyodide/Dockerfile`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/.github/workflows/pyodide/build_in_docker.sh` & `ngstrefftz-0.3.2403.dev5/.github/workflows/pyodide/build_in_docker.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/.github/workflows/pyodide/merge.py` & `ngstrefftz-0.3.2403.dev5/.github/workflows/pyodide/merge.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/.github/workflows/pyodide/requirements.txt` & `ngstrefftz-0.3.2403.dev5/.github/workflows/pyodide/requirements.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/CONTRIBUTING.md` & `ngstrefftz-0.3.2403.dev5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/LICENSE` & `ngstrefftz-0.3.2403.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/PKG-INFO` & `ngstrefftz-0.3.2403.dev5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngstrefftz
-Version: 0.3.2402.dev35
+Version: 0.3.2403.dev5
 Summary: NGSTrefftz is an add-on to NGSolve for Trefftz methods.
 Home-page: https://github.com/PaulSt/ngstrefftz
 Author: Paul Stocker
 Author-email: p.stocker@math.uni-goettingen.de
 License: LGPL2.1
 License-File: LICENSE
 Requires-Dist: ngsolve>=6.2.2402
```

### Comparing `ngstrefftz-0.3.2402.dev35/README.md` & `ngstrefftz-0.3.2403.dev5/README.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/docs/conf.py` & `ngstrefftz-0.3.2403.dev5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/docs/docu.rst` & `ngstrefftz-0.3.2403.dev5/docs/docu.rst`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/docs/index.rst` & `ngstrefftz-0.3.2403.dev5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/docs/intro.rst` & `ngstrefftz-0.3.2403.dev5/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz-adv.ipynb` & `ngstrefftz-0.3.2403.dev5/docs/notebooks/embTrefftz-adv.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz-helm.ipynb` & `ngstrefftz-0.3.2403.dev5/docs/notebooks/embTrefftz-helm.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz-poi.ipynb` & `ngstrefftz-0.3.2403.dev5/docs/notebooks/embTrefftz-poi.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz-stokes.ipynb` & `ngstrefftz-0.3.2403.dev5/docs/notebooks/embTrefftz-stokes.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz-wave.ipynb` & `ngstrefftz-0.3.2403.dev5/docs/notebooks/embTrefftz-wave.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/docs/notebooks/embTrefftz.ipynb` & `ngstrefftz-0.3.2403.dev5/docs/notebooks/embTrefftz.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/docs/notebooks/helmholtz.ipynb` & `ngstrefftz-0.3.2403.dev5/docs/notebooks/helmholtz.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/docs/notebooks/index.ipynb` & `ngstrefftz-0.3.2403.dev5/docs/notebooks/index.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/docs/notebooks/laplace.ipynb` & `ngstrefftz-0.3.2403.dev5/docs/notebooks/laplace.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/docs/notebooks/qtwave.ipynb` & `ngstrefftz-0.3.2403.dev5/docs/notebooks/qtwave.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/docs/notebooks/tunfitted.ipynb` & `ngstrefftz-0.3.2403.dev5/docs/notebooks/tunfitted.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/docs/notebooks/twave.ipynb` & `ngstrefftz-0.3.2403.dev5/docs/notebooks/twave.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/docs/notebooks/twavetents.ipynb` & `ngstrefftz-0.3.2403.dev5/docs/notebooks/twavetents.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/docs/paper/codemeta.json` & `ngstrefftz-0.3.2403.dev5/docs/paper/codemeta.json`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/docs/paper/paper.bib` & `ngstrefftz-0.3.2403.dev5/docs/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/docs/paper/paper.md` & `ngstrefftz-0.3.2403.dev5/docs/paper/paper.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/build.yml` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/build_pip.ps1` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/.github/workflows/build_pip.ps1`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/build_pip.sh` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/.github/workflows/build_pip.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/build_pip_mac.sh` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/.github/workflows/build_pip_mac.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/.github/workflows/fix_auditwheel_policy.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/.github/workflows/fix_auditwheel_policy.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/README.md` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/README.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/advection/advection2d.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/advection/advection2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/advection/advection2d_periodic.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/advection/advection2d_periodic.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/burgers/burgers1d.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/burgers/burgers1d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/burgers/burgers2d.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/burgers/burgers2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/euler/euler2d.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/euler/euler2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/maxwell/maxwell3d.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/maxwell/maxwell3d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/tents/draw3dtent.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/tents/draw3dtent.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/tents/draw3dvertex.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/tents/draw3dvertex.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/wave/horn.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/wave/horn.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/wave/wave2d.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/wave/wave2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/demo/wave/wave3d.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/demo/wave/wave3d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/BurgersMTP.ipynb` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/docs/BurgersMTP.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/INDEX.ipynb` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/docs/INDEX.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/StartPitching.ipynb` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/docs/StartPitching.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/conf.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/figs/CausalityCond.png` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/docs/figs/CausalityCond.png`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/figs/dag.png` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/docs/figs/dag.png`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/figs/map.png` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/docs/figs/map.png`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/figs/subtents.png` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/docs/figs/subtents.png`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/index.rst` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/docs/requirements.txt` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/py/conslaw/__init__.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/py/conslaw/__init__.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/py/utils/_drawtents.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/py/utils/_drawtents.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/py/utils/_drawtents2d.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/py/utils/_drawtents2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/setup.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/setup.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/CMakeLists.txt` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/advection.cpp` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/advection.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/burgers.cpp` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/burgers.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/concurrentqueue.h` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/concurrentqueue.h`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/conservationlaw.hpp` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/conservationlaw.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/euler.cpp` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/euler.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/maxwell.cpp` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/maxwell.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/paralleldepend.hpp` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/paralleldepend.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/python_conslaw.cpp` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/python_conslaw.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/python_tents.cpp` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/python_tents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/symbolic.cpp` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/symbolic.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/tents.cpp` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/tents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/tents.hpp` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/tents.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/tentsolver.hpp` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/tentsolver.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/tentsolver_impl.hpp` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/tentsolver_impl.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/vis3d.cpp` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/vis3d.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/vis3d.hpp` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/vis3d.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/src/wave.cpp` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/src/wave.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/tests/test_burgers_2D.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/tests/test_burgers_2D.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/tests/test_causal_tents.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/tests/test_causal_tents.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/tests/test_conslaw.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/tests/test_conslaw.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/tests/test_tent_height_2D.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/tests/test_tent_height_2D.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/external_dependencies/ngstents/tests/test_tentlayers.py` & `ngstrefftz-0.3.2403.dev5/external_dependencies/ngstents/tests/test_tentlayers.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/setup.py` & `ngstrefftz-0.3.2403.dev5/setup.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/src/CMakeLists.txt` & `ngstrefftz-0.3.2403.dev5/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/src/__init__.py` & `ngstrefftz-0.3.2403.dev5/src/__init__.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/src/airy.cpp` & `ngstrefftz-0.3.2403.dev5/src/airy.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/src/condensedg.cpp` & `ngstrefftz-0.3.2403.dev5/src/condensedg.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/src/condensedg.hpp` & `ngstrefftz-0.3.2403.dev5/src/condensedg.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/src/diffopmapped.hpp` & `ngstrefftz-0.3.2403.dev5/src/diffopmapped.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/src/embtrefftz.cpp` & `ngstrefftz-0.3.2403.dev5/src/embtrefftz.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,15 @@
         {
           auto &dx = icf->dx;
           lfis[dx.vb] += icf->MakeLinearFormIntegrator ();
         }
 
     vector<shared_ptr<Matrix<SCAL>>> ETmats (ne);
     auto lfvec = make_shared<VVector<SCAL>> (ndof);
+    lfvec->operator= (0.0);
 
     size_t active_elements = 0;
     size_t test_local_ndof = test_fes->GetNDof () / ne;
     Vector<SCAL> sing_val_avg;
     Vector<double> sing_val_max;
     Vector<double> sing_val_min;
 
@@ -245,22 +246,23 @@
       // either tndof is given, or try to determine local size of trefftz
       // space, must be at least dim(trefftz)>=dim(trial)-dim(test)
       int nz = 0;
       if (tndof)
         nz = tndof;
       else
         {
-          nz = dofs.Size () - test_dofs.Size ();
-          nz = max (nz, 0);
+          nz = max<size_t> (dofs.Size () - test_dofs.Size (), 0);
           for (int i = 0; i < min (elmat.Width (), elmat.Height ()); i++)
             if (abs (elmat (i, i)) < eps)
               nz++;
         }
-      if (dofs.Size () - test_dofs.Size () > nz)
-        throw Exception ("test fes not large enough for given tndof");
+      if (dofs.Size () < nz)
+        throw Exception ("tndof too large, nz: " + to_string (nz)
+                         + ", dofs:" + to_string (dofs.Size ())
+                         + ", test_dofs:" + to_string (test_dofs.Size ()));
 
       if (getrange)
         ETmats[ei.Nr ()]
             = make_shared<Matrix<SCAL>> (U.Cols (0, dofs.Size () - nz));
       else
         ETmats[ei.Nr ()] = make_shared<Matrix<SCAL>> (
             Trans (Vt.Rows (dofs.Size () - nz, dofs.Size ())));
```

### Comparing `ngstrefftz-0.3.2402.dev35/src/embtrefftz.hpp` & `ngstrefftz-0.3.2403.dev5/src/embtrefftz.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/src/mesh1dtents.cpp` & `ngstrefftz-0.3.2403.dev5/src/mesh1dtents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/src/monomialfespace.cpp` & `ngstrefftz-0.3.2403.dev5/src/monomialfespace.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -94,27 +94,42 @@
             {
               throw Exception ("illegal dim for space-time element");
               break;
             }
           case ET_QUAD:
           case ET_TRIG:
             {
+              Vec<2> scale = 1.0;
+              if (usescale == 2)
+                scale = { 1.0 / ElSize<2> (ei, { 1.0, 0 }),
+                          1.0 / ElSize<2> (ei, { 0, 1.0 }) };
+              else if (usescale != 0)
+                scale = 1.0 / ElSize<2> (ei);
               return *(new (alloc) ScalarMappedElement<2> (
                   local_ndof, order, basismat, eltype, ElCenter<2> (ei),
-                  1.0 / Adiam<2> (ei)));
+                  scale));
               break;
             }
           case ET_HEX:
           case ET_PRISM:
           case ET_PYRAMID:
           case ET_TET:
             {
+              Vec<3> scale = 1.0;
+              if (usescale == 2)
+                {
+                  double hx = ElSize<3> (ei, { 1.0, 1.0, 0 });
+                  double ht = ElSize<3> (ei, { 0, 0, 1.0 });
+                  scale = { 1.0 / hx, 1.0 / hx, 1.0 / ht };
+                }
+              else if (usescale != 0)
+                scale = 1.0 / ElSize<3> (ei);
               return *(new (alloc) ScalarMappedElement<3> (
                   local_ndof, order, basismat, eltype, ElCenter<3> (ei),
-                  1.0 / Adiam<3> (ei)));
+                  scale));
               break;
             }
           }
       }
     try
       {
         return SwitchET<ET_POINT, ET_SEGM, ET_TRIG, ET_QUAD> (
```

### Comparing `ngstrefftz-0.3.2402.dev35/src/ngstrefftz.egg-info/PKG-INFO` & `ngstrefftz-0.3.2403.dev5/src/ngstrefftz.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngstrefftz
-Version: 0.3.2402.dev35
+Version: 0.3.2403.dev5
 Summary: NGSTrefftz is an add-on to NGSolve for Trefftz methods.
 Home-page: https://github.com/PaulSt/ngstrefftz
 Author: Paul Stocker
 Author-email: p.stocker@math.uni-goettingen.de
 License: LGPL2.1
 License-File: LICENSE
 Requires-Dist: ngsolve>=6.2.2402
```

### Comparing `ngstrefftz-0.3.2402.dev35/src/ngstrefftz.egg-info/SOURCES.txt` & `ngstrefftz-0.3.2403.dev5/src/ngstrefftz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/src/planewavefe.cpp` & `ngstrefftz-0.3.2403.dev5/src/planewavefe.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/src/planewavefe.hpp` & `ngstrefftz-0.3.2403.dev5/src/planewavefe.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/src/python_trefftz.cpp` & `ngstrefftz-0.3.2403.dev5/src/python_trefftz.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/src/scalarmappedfe.cpp` & `ngstrefftz-0.3.2403.dev5/src/scalarmappedfe.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/src/scalarmappedfe.hpp` & `ngstrefftz-0.3.2403.dev5/src/scalarmappedfe.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/src/specialcoefficientfunction.cpp` & `ngstrefftz-0.3.2403.dev5/src/specialcoefficientfunction.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/src/specialcoefficientfunction.hpp` & `ngstrefftz-0.3.2403.dev5/src/specialcoefficientfunction.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/src/specialintegrator.cpp` & `ngstrefftz-0.3.2403.dev5/src/specialintegrator.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/src/specialintegrator.hpp` & `ngstrefftz-0.3.2403.dev5/src/specialintegrator.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/src/trefftzfespace.cpp` & `ngstrefftz-0.3.2403.dev5/src/trefftzfespace.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -217,35 +217,26 @@
 
   shared_ptr<GridFunction>
   TrefftzFESpace ::GetEWSolution (shared_ptr<CoefficientFunction> acoeffF)
   {
     static Timer t ("QTEll - GetEWSolution");
     RegionTimer reg (t);
     LocalHeap lh (1000 * 1000 * 1000);
-    if (eqtyp != "qtelliptic")
-      throw Exception ("TrefftzFESpace::GetEWSolution: elementwise particular "
-                       "solution not available for eqtyp");
 
     Flags flags;
     flags.SetFlag ("order", order);
-    flags.SetFlag ("usescale", 1);
+    flags.SetFlag ("usescale", this->usescale);
+    if (eqtyp == "qtheat" && usescale != 0)
+      flags.SetFlag ("usescale", 2);
     shared_ptr<FESpace> fes = make_shared<MonomialFESpace> (ma, flags);
     auto pws = CreateGridFunction (fes, "pws", flags);
     pws->Update ();
     // pws->ConnectAutoUpdate();
 
-    switch (D)
-      {
-      case 2:
-        static_cast<QTEllipticBasis<2> *> (basis)->SetRHS (acoeffF);
-        break;
-      case 3:
-        static_cast<QTEllipticBasis<3> *> (basis)->SetRHS (acoeffF);
-        break;
-      }
+    basis->SetRHS (acoeffF);
 
     // for (auto ei : ma->Elements (VOL))
     ma->IterateElements (VOL, lh, [&] (auto ei, LocalHeap &mlh) {
       HeapReset hr (mlh);
       Array<DofId> dofs;
       fes->GetDofNrs (ei, dofs, VISIBLE_DOF);
       bool hasregdof = false;
@@ -257,21 +248,35 @@
         return; // continue;
 
       FlatVector<double> elvec (dofs.Size (), mlh);
 
       switch (D)
         {
         case 2:
-          static_cast<QTEllipticBasis<2> *> (basis)->GetParticularSolution (
-              ElCenter<2> (ei), ElSize<2> (ei), elvec, mlh);
-          break;
+          {
+            Vec<2> scale = 1.0;
+            if (eqtyp == "qtheat")
+              scale
+                  = { ElSize<2> (ei, { 1.0, 0 }), ElSize<2> (ei, { 0, 1.0 }) };
+            else if (usescale != 0)
+              scale = ElSize<2> (ei);
+            basis->GetParticularSolution (ElCenter<2> (ei), scale, elvec, mlh);
+            break;
+          }
         case 3:
-          static_cast<QTEllipticBasis<3> *> (basis)->GetParticularSolution (
-              ElCenter<3> (ei), ElSize<3> (ei), elvec, mlh);
-          break;
+          {
+            Vec<3> scale = 1.0;
+            if (eqtyp == "qtheat")
+              scale = { ElSize<3> (ei, { 1.0, 1.0, 0 }), 0,
+                        ElSize<3> (ei, { 0, 0, 1.0 }) };
+            else if (usescale != 0)
+              scale = ElSize<3> (ei);
+            basis->GetParticularSolution (ElCenter<3> (ei), scale, elvec, mlh);
+            break;
+          }
         }
 
       pws->SetElementVector (dofs, elvec);
     });
 
     return pws;
   }
@@ -425,14 +430,25 @@
                 {
                   Vec<3> scale = 1.0 / sqrt (ElSize<3> (ei));
                   scale[2] = coeff_const * scale[2] * scale[2];
                   return *(new (alloc) ScalarMappedElement<3> (
                       local_ndof, order, basismat, eltype, ElCenter<3> (ei),
                       scale));
                 }
+              else if (eqtyp == "qtheat")
+                {
+                  double hx = ElSize<3> (ei, { 1.0, 1.0, 0 });
+                  double ht = ElSize<3> (ei, { 0, 0, 1.0 });
+                  Vec<3> scale ({ 1.0 / hx, 1.0 / hx, 1.0 / ht });
+                  CSR basismat = static_cast<QTHeatBasis<3> *> (basis)->Basis (
+                      ElCenter<3> (ei), hx, ht);
+                  return *(new (alloc) ScalarMappedElement<3> (
+                      local_ndof, order, basismat, eltype, ElCenter<3> (ei),
+                      scale));
+                }
               else
                 {
                   Vec<3> scale = 1.0;
                   scale[2] = coeff_const;
                   scale = 1.0 / ElSize<3> (ei, scale);
                   scale[2] *= coeff_const;
                   return *(new (alloc) ScalarMappedElement<3> (
@@ -460,14 +476,16 @@
   DocInfo TrefftzFESpace ::GetDocu ()
   {
     // auto docu = FESpace::GetDocu();
     DocInfo docu;
     docu.short_docu = "Trefftz space for different PDEs. Use kwarg 'eq' to "
                       "choose the PDE, currently implemented are:\n"
                       " - laplace - for Laplace equation\n"
+                      " - qtelliptic - for the quasi-Trefftz space for an "
+                      "elliptic problem\n"
                       " - wave - for the second order acoustic wave equation\n"
                       " - qtwave - for the quasi-Trefftz space\n"
                       " - fowave - for the first order acoustic wave "
                       "equation, returns TnT (sigv,tauw)\n"
                       " - foqtwave - for the quasi-Trefftz space \n"
                       " - helmholtz - planewaves for the helmholtz equation\n"
                       " - helmholtzconj - returns the complex conjungate of "
@@ -945,33 +963,33 @@
                     if (i2 == 0 && m == D - 1 && j == D - 1)
                       continue;
                     Vec<D, int> em = 0;
                     em[m] = 1;
                     qtbasis.Col (indexmap)
                         -= factorial (mii + ej) / factorial (mil)
                            * (AA[IndexMap2<D> (mil, order - 1)]) (j, m)
-                           / pow (elsize, vsum<D, int> (-mil))
+                           * pow (elsize, vsum<D, int> (mil))
                            * (mii[m] + ej[m] - mil[m] + 1)
                            * qtbasis.Col (PolBasis::IndexMap2<D> (
                                mii + ej - mil + em, order));
                   }
                 // vec coeff B
                 qtbasis.Col (indexmap)
                     += factorial (mii + ej) / factorial (mil)
-                       * (BB[IndexMap2<D> (mil, order - 1)]) (j)
-                       / pow (elsize, vsum<D, int> (-mil) - 1)
+                       * (BB[IndexMap2<D> (mil, order - 1)]) (j)*pow (
+                           elsize, vsum<D, int> (mil) + 1)
                        * qtbasis.Col (
                            PolBasis::IndexMap2<D> (mii + ej - mil, order));
 
                 // scal coeff C
                 if (j == 0 && mil[0] <= mii[0])
                   qtbasis.Col (indexmap)
                       += factorial (mii) / factorial (mil)
                          * CC[IndexMap2<D> (mil, order - 1)]
-                         / pow (elsize, vsum<D, int> (-mil) - 2)
+                         * pow (elsize, vsum<D, int> (mil) + 2)
                          * qtbasis.Col (
                              PolBasis::IndexMap2<D> (mii - mil, order));
               });
             }
           Vec<D, int> eD = 0;
           eD[D - 1] = 2;
           qtbasis.Col (indexmap)
@@ -991,17 +1009,18 @@
     // CSR tb;
     // MatToCSR (qtbasis, tb);
     // return tb;
   }
 
   template <int D>
   void
-  QTEllipticBasis<D>::GetParticularSolution (Vec<D> ElCenter, double elsize,
+  QTEllipticBasis<D>::GetParticularSolution (Vec<D> ElCenter, Vec<D> elsize,
                                              FlatVector<> sol, LocalHeap &lh)
   {
+    double hx = elsize[0];
     static Timer t ("QTEll - GetParticularSolution");
     RegionTimer reg (t);
     IntegrationPoint ip (ElCenter, 0);
     Mat<D, D> dummy;
     FE_ElementTransformation<D, D> et (D == 3   ? ET_TET
                                        : D == 2 ? ET_TRIG
                                                 : ET_SEGM,
@@ -1049,37 +1068,37 @@
               {
                 if (i2 == 0 && m == D - 1 && j == D - 1)
                   continue;
                 Vec<D, int> em = 0;
                 em[m] = 1;
                 sol (indexmap) -= factorial (mii + ej) / factorial (mil)
                                   * (AA[IndexMap2<D> (mil, order - 1)]) (j, m)
-                                  * pow (elsize, vsum<D, int> (mil))
+                                  * pow (hx, vsum<D, int> (mil))
                                   * (mii[m] + ej[m] - mil[m] + 1)
                                   * sol (PolBasis::IndexMap2<D> (
                                       mii + ej - mil + em, order));
               }
             // vec coeff B
             sol (indexmap)
                 += factorial (mii + ej) / factorial (mil)
                    * (BB[IndexMap2<D> (mil, order - 1)]) (j)*pow (
-                       elsize, vsum<D, int> (mil) + 1)
+                       hx, vsum<D, int> (mil) + 1)
                    * sol (PolBasis::IndexMap2<D> (mii + ej - mil, order));
 
             // scal coeff C
             if (j == 0 && mil[0] <= mii[0])
               sol (indexmap)
                   += factorial (mii) / factorial (mil)
                      * CC[IndexMap2<D> (mil, order - 1)]
-                     * pow (elsize, vsum<D, int> (mil) + 2)
+                     * pow (hx, vsum<D, int> (mil) + 2)
                      * sol (PolBasis::IndexMap2<D> (mii - mil, order));
           });
         }
       sol (indexmap) += -FF[PolBasis::IndexMap2<D> (mii, order)]
-                        * pow (elsize, vsum<D, int> (mii) + 2);
+                        * pow (hx, vsum<D, int> (mii) + 2);
       Vec<D, int> eD = 0;
       eD[D - 1] = 2;
       sol (indexmap) *= 1.0 / factorial (mii + eD) / (AA[0](D - 1, D - 1));
     });
   }
 
   template class QTEllipticBasis<1>;
@@ -1458,18 +1477,93 @@
     // str << "failed to generate trefftz basis of order " << order << endl;
     // throw Exception (str.str ());
     //}
 
     // return gtbstore[encode];
   }
 
+  template <int D>
+  void QTHeatBasis<D>::GetParticularSolution (Vec<D> ElCenter, Vec<D> elsize,
+                                              FlatVector<> sol, LocalHeap &lh)
+  {
+    double hx = elsize[0];
+    double ht = elsize[D - 1];
+    IntegrationPoint ip (ElCenter, 0);
+    Mat<D, D> dummy;
+    FE_ElementTransformation<D, D> et (D == 3 ? ET_TET : ET_TRIG, dummy);
+    MappedIntegrationPoint<D, D> mip (ip, et, 0);
+    for (int i = 0; i < D; i++)
+      mip.Point ()[i] = ElCenter[i];
+
+    int ndiffs = (BinCoeff (D + order - 1, order - 1));
+    Vector<Matrix<>> AA (ndiffs);
+    ndiffs = (BinCoeff (D + order, order));
+    FlatVector<> FF (ndiffs, lh);
+
+    TraversePol<D> (order, [&] (int i, Vec<D, int> coeff) {
+      int index = PolBasis::IndexMap2<D> (coeff, order);
+      FF[index] = FFder[index]->Evaluate (mip);
+      if (vsum<D, int> (coeff) < order)
+        {
+          index = PolBasis::IndexMap2<D> (coeff, order - 1);
+          AA[index].SetSize (D - 1, D - 1);
+          AAder[index]->Evaluate (mip, AA[index].AsVector ());
+        }
+    });
+
+    const int ndof = (BinCoeff (D - 1 + order, order)
+                      + BinCoeff (D - 1 + order - 1, order - 1));
+    const int npoly = (BinCoeff (D + order, order));
+    sol = 0;
+    // start recursion
+    TraversePol2<D> (order, [&] (int i, Vec<D, int> coeff) {
+      if (coeff[0] <= 1)
+        return;
+      int indexmap = PolBasis::IndexMap2<D> (coeff, order);
+      Vec<D, int> mii = coeff;
+      mii[0] = mii[0] - 2;
+      Vec<D, int> et = 0;
+      et[D - 1] = 1;
+      sol (indexmap) += hx * hx / ht * (mii[D - 1] + 1) / coeff[0]
+                        / (coeff[0] - 1)
+                        * sol (PolBasis::IndexMap2<D> (mii + et, order));
+      for (int j = 0; j < D - 1; j++)
+        {
+          Vec<D, int> ej = 0;
+          ej[j] = 1;
+          TraversePol<D> (mii + ej, [&] (int i2, Vec<D, int> mil) {
+            // matrix coeff A
+            for (int m = 0; m < D - 1; m++)
+              {
+                if (i2 == 0 && m == 0 && j == 0)
+                  continue;
+                Vec<D, int> em = 0;
+                em[m] = 1;
+                sol (indexmap)
+                    -= (AA[IndexMap2<D> (mil, order - 1)]) (j, m)
+                       * pow (hx, vsum<D - 1, int> (mil))
+                       * pow (ht, mil[D - 1]) * (mii[m] + ej[m] - mil[m] + 1)
+                       * (mii[j] + 1) / (mii[0] + 2) / (mii[0] + 1)
+                       / factorial (mil)
+                       * sol (PolBasis::IndexMap2<D> (mii + ej - mil + em,
+                                                      order));
+              }
+          });
+        }
+      sol (indexmap) += -FF[PolBasis::IndexMap2<D> (mii, order)]
+                        * pow (hx, vsum<D - 1, int> (coeff))
+                        * pow (ht, coeff[D - 1]) / factorial (coeff);
+      sol (indexmap) *= 1.0 / (AA[0](0, 0));
+    });
+    // cout << sol << endl;
+  }
+
   // template class QTHeatBasis<1>;
   template class QTHeatBasis<2>;
   template class QTHeatBasis<3>;
-
 }
 
 #ifdef NGS_PYTHON
 void ExportTrefftzFESpace (py::module m)
 {
   using namespace ngcomp;
 
@@ -1484,14 +1578,17 @@
           "SetCoeff",
           static_cast<void (TrefftzFESpace::*) (
               shared_ptr<CoefficientFunction>, shared_ptr<CoefficientFunction>,
               shared_ptr<CoefficientFunction>)> (&TrefftzFESpace::SetCoeff),
           R"mydelimiter(
                 Set coefficient of Trefftz space. 
 
+                For an elliptic problem, the coefficients are given by
+                - div(coeffA*grad(u)) + coeffB*grad(u) + coeffC u = 0
+
                 For the first order wave equation, the coefficients are given by
                 grad(v) + coeffB dt sigma = 0
                 div(sigma) + 1/coeffA**2 dt v = 0
 
                 For the second order wave equation, the coefficients are given by
                 - div(1/coeffB grad(u)) + 1/coeffA**2 dtt u = 0
```

### Comparing `ngstrefftz-0.3.2402.dev35/src/trefftzfespace.hpp` & `ngstrefftz-0.3.2403.dev5/src/trefftzfespace.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,34 @@
   {
   protected:
     int order;
 
   public:
     PolBasis () { ; }
     PolBasis (int aorder) : order (aorder) { ; }
+
+    virtual void SetRHS (shared_ptr<CoefficientFunction> coeffF)
+    {
+      throw Exception ("SetRHS not implemented for this basis");
+    }
+    virtual void GetParticularSolution (Vec<1> ElCenter, Vec<1> elsize,
+                                        FlatVector<> sol, LocalHeap &lh)
+    {
+      throw Exception ("GetParticularSolution not implemented for this basis");
+    }
+    virtual void GetParticularSolution (Vec<2> ElCenter, Vec<2> elsize,
+                                        FlatVector<> sol, LocalHeap &lh)
+    {
+      throw Exception ("GetParticularSolution not implemented for this basis");
+    }
+    virtual void GetParticularSolution (Vec<3> ElCenter, Vec<3> elsize,
+                                        FlatVector<> sol, LocalHeap &lh)
+    {
+      throw Exception ("GetParticularSolution not implemented for this basis");
+    }
     template <int D>
     void ComputeDerivs (int order, shared_ptr<CoefficientFunction> acoeff,
                         Vector<shared_ptr<CoefficientFunction>> &ders)
     {
       const int ndiffs = (BinCoeff (D + order, order));
       ders.SetSize (ndiffs);
 
@@ -221,20 +241,20 @@
         coeffC = make_shared<ConstantCoefficientFunction> (0);
 
       this->ComputeDerivs<D> (order - 1, coeffA, AAder);
       this->ComputeDerivs<D> (order - 1, coeffB, BBder);
       this->ComputeDerivs<D> (order - 1, coeffC, CCder);
     }
     CSR Basis (Vec<D> ElCenter, double elsize = 1.0);
-    void SetRHS (shared_ptr<CoefficientFunction> coeffF)
+    void SetRHS (shared_ptr<CoefficientFunction> coeffF) override
     {
       this->ComputeDerivs<D> (order, coeffF, FFder);
     }
-    void GetParticularSolution (Vec<D> ElCenter, double elsize,
-                                FlatVector<> sol, LocalHeap &lh);
+    void GetParticularSolution (Vec<D> ElCenter, Vec<D> elsize,
+                                FlatVector<> sol, LocalHeap &lh) override;
   };
 
   template <int D> class QTWaveBasis : public PolBasis
   {
     mutex gentrefftzbasis;
     std::map<string, CSR> gtbstore;
     Vector<shared_ptr<CoefficientFunction>> AAder;
@@ -299,25 +319,32 @@
 
   template <int D> class QTHeatBasis : public PolBasis
   {
     mutex gentrefftzbasis;
     std::map<string, CSR> gtbstore;
 
     Vector<shared_ptr<CoefficientFunction>> AAder;
+    Vector<shared_ptr<CoefficientFunction>> FFder;
 
   public:
     QTHeatBasis (int aorder, shared_ptr<CoefficientFunction> coeffA)
         : PolBasis (aorder)
     {
       if (!coeffA)
         coeffA = make_shared<ConstantCoefficientFunction> (1);
 
       this->ComputeDerivs<D> (order - 1, coeffA, AAder);
     }
     CSR Basis (Vec<D> ElCenter, double hx, double ht);
+    void SetRHS (shared_ptr<CoefficientFunction> coeffF) override
+    {
+      this->ComputeDerivs<D> (order, coeffF, FFder);
+    }
+    void GetParticularSolution (Vec<D> ElCenter, Vec<D> elsize,
+                                FlatVector<> sol, LocalHeap &lh);
   };
 }
 
 #ifdef NGS_PYTHON
 #include <python_ngstd.hpp>
 void ExportTrefftzFESpace (py::module m);
 #endif // NGS_PYTHON
```

### Comparing `ngstrefftz-0.3.2402.dev35/src/twavetents.cpp` & `ngstrefftz-0.3.2403.dev5/src/twavetents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/src/twavetents.hpp` & `ngstrefftz-0.3.2403.dev5/src/twavetents.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/test/dg.py` & `ngstrefftz-0.3.2403.dev5/test/dg.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/test/embt.py` & `ngstrefftz-0.3.2403.dev5/test/embt.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/test/tents.py` & `ngstrefftz-0.3.2403.dev5/test/tents.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev35/test/trefftz.py` & `ngstrefftz-0.3.2403.dev5/test/trefftz.py`

 * *Files identical despite different names*

