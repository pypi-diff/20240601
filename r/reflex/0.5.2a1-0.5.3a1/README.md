# Comparing `tmp/reflex-0.5.2a1.tar.gz` & `tmp/reflex-0.5.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-0.5.2a1.tar", max compression
+gzip compressed data, was "reflex-0.5.3a1.tar", max compression
```

## Comparing `reflex-0.5.2a1.tar` & `reflex-0.5.3a1.tar`

### file list

```diff
@@ -1,522 +1,536 @@
--rw-r--r--   0        0        0    11358 2023-07-20 22:42:41.698164 reflex-0.5.2a1/LICENSE
--rw-r--r--   0        0        0     9838 2024-05-23 22:07:24.004599 reflex-0.5.2a1/README.md
--rw-r--r--   0        0        0     2974 2024-05-26 21:38:07.551506 reflex-0.5.2a1/pyproject.toml
--rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.498329 reflex-0.5.2a1/reflex/.templates/apps/blank/assets/favicon.ico
--rw-r--r--   0        0        0        0 2023-11-09 03:24:59.498383 reflex-0.5.2a1/reflex/.templates/apps/blank/code/__init__.py
--rw-r--r--   0        0        0      926 2024-05-23 22:07:24.026702 reflex-0.5.2a1/reflex/.templates/apps/blank/code/blank.py
--rw-r--r--   0        0        0       32 2023-11-09 03:24:59.498951 reflex-0.5.2a1/reflex/.templates/apps/demo/.gitignore
--rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.499075 reflex-0.5.2a1/reflex/.templates/apps/demo/assets/favicon.ico
--rw-r--r--   0        0        0     1475 2023-11-09 03:24:59.499137 reflex-0.5.2a1/reflex/.templates/apps/demo/assets/github.svg
--rw-r--r--   0        0        0     1899 2023-11-09 03:24:59.499199 reflex-0.5.2a1/reflex/.templates/apps/demo/assets/icon.svg
--rw-r--r--   0        0        0     5403 2023-11-09 03:24:59.499298 reflex-0.5.2a1/reflex/.templates/apps/demo/assets/logo.svg
--rw-r--r--   0        0        0      807 2023-11-09 03:24:59.499362 reflex-0.5.2a1/reflex/.templates/apps/demo/assets/paneleft.svg
--rw-r--r--   0        0        0       32 2023-11-09 03:24:59.499458 reflex-0.5.2a1/reflex/.templates/apps/demo/code/__init__.py
--rw-r--r--   0        0        0     2927 2024-05-23 22:07:24.026869 reflex-0.5.2a1/reflex/.templates/apps/demo/code/demo.py
--rw-r--r--   0        0        0      194 2023-11-09 03:24:59.499716 reflex-0.5.2a1/reflex/.templates/apps/demo/code/pages/__init__.py
--rw-r--r--   0        0        0      706 2024-05-23 22:07:24.027050 reflex-0.5.2a1/reflex/.templates/apps/demo/code/pages/chatapp.py
--rw-r--r--   0        0        0    10906 2024-05-23 22:07:24.027242 reflex-0.5.2a1/reflex/.templates/apps/demo/code/pages/datatable.py
--rw-r--r--   0        0        0     8381 2024-05-23 22:07:24.027471 reflex-0.5.2a1/reflex/.templates/apps/demo/code/pages/forms.py
--rw-r--r--   0        0        0     8519 2024-05-23 22:07:24.027876 reflex-0.5.2a1/reflex/.templates/apps/demo/code/pages/graphing.py
--rw-r--r--   0        0        0     1822 2024-05-23 22:07:24.028048 reflex-0.5.2a1/reflex/.templates/apps/demo/code/pages/home.py
--rw-r--r--   0        0        0     4722 2024-05-23 22:07:24.028210 reflex-0.5.2a1/reflex/.templates/apps/demo/code/sidebar.py
--rw-r--r--   0        0        0      510 2023-11-09 03:24:59.500529 reflex-0.5.2a1/reflex/.templates/apps/demo/code/state.py
--rw-r--r--   0        0        0      912 2023-11-09 03:24:59.500616 reflex-0.5.2a1/reflex/.templates/apps/demo/code/states/form_state.py
--rw-r--r--   0        0        0     1189 2023-11-09 03:24:59.500682 reflex-0.5.2a1/reflex/.templates/apps/demo/code/states/pie_state.py
--rw-r--r--   0        0        0     1486 2024-05-23 22:07:24.028477 reflex-0.5.2a1/reflex/.templates/apps/demo/code/styles.py
--rw-r--r--   0        0        0        0 2023-11-09 03:24:59.500792 reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/__init__.py
--rw-r--r--   0        0        0      120 2023-11-09 03:24:59.500879 reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/components/__init__.py
--rw-r--r--   0        0        0     3584 2024-05-23 22:07:24.028657 reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/components/chat.py
--rw-r--r--   0        0        0      680 2023-11-09 03:24:59.500996 reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/components/loading_icon.py
--rw-r--r--   0        0        0     1829 2024-05-23 22:07:24.028787 reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/components/modal.py
--rw-r--r--   0        0        0     2251 2024-05-23 22:07:24.035433 reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/components/navbar.py
--rw-r--r--   0        0        0     1735 2024-05-23 22:07:24.035615 reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/components/sidebar.py
--rw-r--r--   0        0        0     4001 2023-11-09 03:24:59.501230 reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/state.py
--rw-r--r--   0        0        0     2281 2024-05-23 22:07:24.035773 reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/styles.py
--rw-r--r--   0        0        0       74 2023-10-22 18:57:13.188650 reflex-0.5.2a1/reflex/.templates/jinja/app/rxconfig.py.jinja2
--rw-r--r--   0        0        0      127 2024-05-23 22:07:24.036845 reflex-0.5.2a1/reflex/.templates/jinja/custom_components/README.md.jinja2
--rw-r--r--   0        0        0       32 2024-05-23 22:07:24.036930 reflex-0.5.2a1/reflex/.templates/jinja/custom_components/__init__.py.jinja2
--rw-r--r--   0        0        0      826 2024-05-23 22:07:24.037352 reflex-0.5.2a1/reflex/.templates/jinja/custom_components/demo_app.py.jinja2
--rw-r--r--   0        0        0      614 2024-05-23 22:07:24.037689 reflex-0.5.2a1/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2
--rw-r--r--   0        0        0     2403 2024-05-23 22:07:24.037946 reflex-0.5.2a1/reflex/.templates/jinja/custom_components/src.py.jinja2
--rw-r--r--   0        0        0      548 2023-10-22 18:57:13.188813 reflex-0.5.2a1/reflex/.templates/jinja/web/package.json.jinja2
--rw-r--r--   0        0        0      930 2024-05-23 22:07:24.038352 reflex-0.5.2a1/reflex/.templates/jinja/web/pages/_app.js.jinja2
--rw-r--r--   0        0        0      182 2023-07-20 22:42:41.708822 reflex-0.5.2a1/reflex/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      400 2024-05-23 22:07:24.038521 reflex-0.5.2a1/reflex/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0       86 2023-10-22 18:57:13.188983 reflex-0.5.2a1/reflex/.templates/jinja/web/pages/component.js.jinja2
--rw-r--r--   0        0        0      882 2023-12-01 04:51:31.091531 reflex-0.5.2a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0      343 2024-04-04 14:57:26.375114 reflex-0.5.2a1/reflex/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0      388 2024-05-23 22:07:24.038697 reflex-0.5.2a1/reflex/.templates/jinja/web/pages/stateful_component.js.jinja2
--rw-r--r--   0        0        0      101 2023-12-01 04:51:31.092250 reflex-0.5.2a1/reflex/.templates/jinja/web/pages/stateful_components.js.jinja2
--rw-r--r--   0        0        0     3883 2024-05-23 22:07:24.038822 reflex-0.5.2a1/reflex/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0      141 2023-12-06 18:41:46.628030 reflex-0.5.2a1/reflex/.templates/jinja/web/styles/styles.css.jinja2
--rw-r--r--   0        0        0      761 2024-05-23 22:07:24.039110 reflex-0.5.2a1/reflex/.templates/jinja/web/tailwind.config.js.jinja2
--rw-r--r--   0        0        0     3790 2024-05-23 22:07:24.039386 reflex-0.5.2a1/reflex/.templates/jinja/web/utils/context.js.jinja2
--rw-r--r--   0        0        0       37 2023-12-06 19:37:00.189183 reflex-0.5.2a1/reflex/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2023-07-20 22:42:41.709243 reflex-0.5.2a1/reflex/.templates/web/.gitignore
--rw-r--r--   0        0        0      595 2023-10-30 01:36:56.133208 reflex-0.5.2a1/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js
--rw-r--r--   0        0        0      645 2024-05-23 22:07:24.039706 reflex-0.5.2a1/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js
--rw-r--r--   0        0        0       97 2023-10-22 18:57:13.190257 reflex-0.5.2a1/reflex/.templates/web/jsconfig.json
--rw-r--r--   0        0        0      118 2023-11-22 05:49:24.669539 reflex-0.5.2a1/reflex/.templates/web/next.config.js
--rw-r--r--   0        0        0       82 2024-05-24 16:47:17.136778 reflex-0.5.2a1/reflex/.templates/web/postcss.config.js
--rw-r--r--   0        0        0       59 2024-05-24 16:47:17.136946 reflex-0.5.2a1/reflex/.templates/web/styles/tailwind.css
--rw-r--r--   0        0        0     1254 2023-09-16 20:27:37.277783 reflex-0.5.2a1/reflex/.templates/web/utils/client_side_routing.js
--rw-r--r--   0        0        0     1622 2024-05-23 22:07:24.039831 reflex-0.5.2a1/reflex/.templates/web/utils/helpers/dataeditor.js
--rw-r--r--   0        0        0      528 2024-05-23 22:07:24.039893 reflex-0.5.2a1/reflex/.templates/web/utils/helpers/debounce.js
--rw-r--r--   0        0        0     1152 2023-11-22 05:49:24.669991 reflex-0.5.2a1/reflex/.templates/web/utils/helpers/range.js
--rw-r--r--   0        0        0      566 2024-05-23 22:07:24.039949 reflex-0.5.2a1/reflex/.templates/web/utils/helpers/throttle.js
--rw-r--r--   0        0        0    22617 2024-05-23 22:07:24.040119 reflex-0.5.2a1/reflex/.templates/web/utils/state.js
--rw-r--r--   0        0        0     5831 2024-05-23 22:07:24.040585 reflex-0.5.2a1/reflex/__init__.py
--rw-r--r--   0        0        0     7791 2024-05-26 21:36:23.014634 reflex-0.5.2a1/reflex/__init__.pyi
--rw-r--r--   0        0        0      108 2023-08-05 17:01:44.301997 reflex-0.5.2a1/reflex/__main__.py
--rw-r--r--   0        0        0      373 2023-07-20 22:42:41.710893 reflex-0.5.2a1/reflex/admin.py
--rw-r--r--   0        0        0    48956 2024-05-24 16:47:17.137462 reflex-0.5.2a1/reflex/app.py
--rw-r--r--   0        0        0     1227 2024-05-23 22:07:24.041327 reflex-0.5.2a1/reflex/app_module_for_backend.py
--rw-r--r--   0        0        0     4274 2024-05-23 22:07:24.041585 reflex-0.5.2a1/reflex/base.py
--rw-r--r--   0        0        0       27 2023-07-20 22:42:41.711176 reflex-0.5.2a1/reflex/compiler/__init__.py
--rw-r--r--   0        0        0    17455 2024-05-23 22:07:24.041899 reflex-0.5.2a1/reflex/compiler/compiler.py
--rw-r--r--   0        0        0     4344 2024-05-23 22:07:24.042172 reflex-0.5.2a1/reflex/compiler/templates.py
--rw-r--r--   0        0        0    13274 2024-05-23 22:07:24.042547 reflex-0.5.2a1/reflex/compiler/utils.py
--rw-r--r--   0        0        0      552 2024-05-23 22:07:24.042676 reflex-0.5.2a1/reflex/components/__init__.py
--rw-r--r--   0        0        0      325 2024-05-23 22:07:24.042785 reflex-0.5.2a1/reflex/components/base/__init__.py
--rw-r--r--   0        0        0      573 2024-05-23 22:07:24.042894 reflex-0.5.2a1/reflex/components/base/app_wrap.py
--rw-r--r--   0        0        0     2890 2024-05-24 18:17:26.775810 reflex-0.5.2a1/reflex/components/base/app_wrap.pyi
--rw-r--r--   0        0        0     1234 2024-05-23 22:07:24.043424 reflex-0.5.2a1/reflex/components/base/bare.py
--rw-r--r--   0        0        0      151 2023-07-20 22:42:41.711762 reflex-0.5.2a1/reflex/components/base/body.py
--rw-r--r--   0        0        0     3206 2024-05-24 18:17:28.445017 reflex-0.5.2a1/reflex/components/base/body.pyi
--rw-r--r--   0        0        0      583 2024-05-23 22:07:24.043906 reflex-0.5.2a1/reflex/components/base/document.py
--rw-r--r--   0        0        0    14232 2024-05-24 18:17:26.993081 reflex-0.5.2a1/reflex/components/base/document.pyi
--rw-r--r--   0        0        0      312 2024-05-23 22:07:24.044107 reflex-0.5.2a1/reflex/components/base/fragment.py
--rw-r--r--   0        0        0     3218 2024-05-24 18:17:26.730059 reflex-0.5.2a1/reflex/components/base/fragment.pyi
--rw-r--r--   0        0        0      297 2024-05-23 22:07:24.044322 reflex-0.5.2a1/reflex/components/base/head.py
--rw-r--r--   0        0        0     6002 2024-05-24 18:17:27.212239 reflex-0.5.2a1/reflex/components/base/head.pyi
--rw-r--r--   0        0        0      929 2023-07-20 22:42:41.711911 reflex-0.5.2a1/reflex/components/base/link.py
--rw-r--r--   0        0        0     6990 2024-05-24 18:17:28.411498 reflex-0.5.2a1/reflex/components/base/link.pyi
--rw-r--r--   0        0        0     1438 2023-09-16 20:27:37.279391 reflex-0.5.2a1/reflex/components/base/meta.py
--rw-r--r--   0        0        0    12804 2024-05-24 18:17:27.232380 reflex-0.5.2a1/reflex/components/base/meta.pyi
--rw-r--r--   0        0        0     2298 2023-10-30 01:36:56.136333 reflex-0.5.2a1/reflex/components/base/script.py
--rw-r--r--   0        0        0     4500 2024-05-24 18:17:27.261455 reflex-0.5.2a1/reflex/components/base/script.pyi
--rw-r--r--   0        0        0     6378 2024-05-23 22:07:24.045051 reflex-0.5.2a1/reflex/components/chakra/__init__.py
--rw-r--r--   0        0        0     5242 2024-05-23 22:07:24.045134 reflex-0.5.2a1/reflex/components/chakra/base.py
--rw-r--r--   0        0        0    10917 2024-05-24 18:17:24.861757 reflex-0.5.2a1/reflex/components/chakra/base.pyi
--rw-r--r--   0        0        0      459 2024-05-23 22:07:24.045326 reflex-0.5.2a1/reflex/components/chakra/datadisplay/__init__.py
--rw-r--r--   0        0        0      352 2024-05-23 22:07:24.045398 reflex-0.5.2a1/reflex/components/chakra/datadisplay/badge.py
--rw-r--r--   0        0        0     3654 2024-05-24 18:17:23.594412 reflex-0.5.2a1/reflex/components/chakra/datadisplay/badge.pyi
--rw-r--r--   0        0        0      174 2024-05-23 22:07:24.045575 reflex-0.5.2a1/reflex/components/chakra/datadisplay/code.py
--rw-r--r--   0        0        0     3229 2024-05-24 18:17:23.555248 reflex-0.5.2a1/reflex/components/chakra/datadisplay/code.pyi
--rw-r--r--   0        0        0      657 2024-05-23 22:07:24.045714 reflex-0.5.2a1/reflex/components/chakra/datadisplay/divider.py
--rw-r--r--   0        0        0     3934 2024-05-24 18:17:23.503426 reflex-0.5.2a1/reflex/components/chakra/datadisplay/divider.pyi
--rw-r--r--   0        0        0      180 2024-05-23 22:07:24.045852 reflex-0.5.2a1/reflex/components/chakra/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     3251 2024-05-24 18:17:24.668110 reflex-0.5.2a1/reflex/components/chakra/datadisplay/keyboard_key.pyi
--rw-r--r--   0        0        0     1484 2024-05-23 22:07:24.046229 reflex-0.5.2a1/reflex/components/chakra/datadisplay/list.py
--rw-r--r--   0        0        0    12991 2024-05-24 18:17:24.625763 reflex-0.5.2a1/reflex/components/chakra/datadisplay/list.pyi
--rw-r--r--   0        0        0     2149 2024-05-23 22:07:24.046512 reflex-0.5.2a1/reflex/components/chakra/datadisplay/stat.py
--rw-r--r--   0        0        0    17461 2024-05-24 18:17:23.921677 reflex-0.5.2a1/reflex/components/chakra/datadisplay/stat.pyi
--rw-r--r--   0        0        0     9122 2024-05-23 22:07:24.046775 reflex-0.5.2a1/reflex/components/chakra/datadisplay/table.py
--rw-r--r--   0        0        0    27252 2024-05-24 18:17:24.570212 reflex-0.5.2a1/reflex/components/chakra/datadisplay/table.pyi
--rw-r--r--   0        0        0     2294 2024-05-23 22:07:24.046980 reflex-0.5.2a1/reflex/components/chakra/datadisplay/tag.py
--rw-r--r--   0        0        0    15734 2024-05-24 18:17:23.854192 reflex-0.5.2a1/reflex/components/chakra/datadisplay/tag.pyi
--rw-r--r--   0        0        0      384 2024-05-23 22:07:24.047198 reflex-0.5.2a1/reflex/components/chakra/disclosure/__init__.py
--rw-r--r--   0        0        0     3510 2024-05-23 22:07:24.047299 reflex-0.5.2a1/reflex/components/chakra/disclosure/accordion.py
--rw-r--r--   0        0        0    15803 2024-05-24 18:17:24.269813 reflex-0.5.2a1/reflex/components/chakra/disclosure/accordion.pyi
--rw-r--r--   0        0        0     3295 2024-05-23 22:07:24.047512 reflex-0.5.2a1/reflex/components/chakra/disclosure/tabs.py
--rw-r--r--   0        0        0    18525 2024-05-24 18:17:23.577560 reflex-0.5.2a1/reflex/components/chakra/disclosure/tabs.pyi
--rw-r--r--   0        0        0     1732 2024-05-23 22:07:24.047752 reflex-0.5.2a1/reflex/components/chakra/disclosure/transition.py
--rw-r--r--   0        0        0    20003 2024-05-24 18:17:23.981249 reflex-0.5.2a1/reflex/components/chakra/disclosure/transition.pyi
--rw-r--r--   0        0        0      278 2024-05-23 22:07:24.047917 reflex-0.5.2a1/reflex/components/chakra/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0     3258 2024-05-24 18:17:23.263087 reflex-0.5.2a1/reflex/components/chakra/disclosure/visuallyhidden.pyi
--rw-r--r--   0        0        0      313 2024-05-23 22:07:24.048055 reflex-0.5.2a1/reflex/components/chakra/feedback/__init__.py
--rw-r--r--   0        0        0     1623 2024-05-23 22:07:24.048128 reflex-0.5.2a1/reflex/components/chakra/feedback/alert.py
--rw-r--r--   0        0        0    12381 2024-05-24 18:17:24.114056 reflex-0.5.2a1/reflex/components/chakra/feedback/alert.pyi
--rw-r--r--   0        0        0     2006 2024-05-23 22:07:24.048304 reflex-0.5.2a1/reflex/components/chakra/feedback/circularprogress.py
--rw-r--r--   0        0        0     7637 2024-05-24 18:17:24.157731 reflex-0.5.2a1/reflex/components/chakra/feedback/circularprogress.pyi
--rw-r--r--   0        0        0      871 2024-05-23 22:07:24.048486 reflex-0.5.2a1/reflex/components/chakra/feedback/progress.py
--rw-r--r--   0        0        0     4278 2024-05-24 18:17:24.226071 reflex-0.5.2a1/reflex/components/chakra/feedback/progress.pyi
--rw-r--r--   0        0        0     1776 2024-05-23 22:07:24.048623 reflex-0.5.2a1/reflex/components/chakra/feedback/skeleton.py
--rw-r--r--   0        0        0    10690 2024-05-24 18:17:24.080524 reflex-0.5.2a1/reflex/components/chakra/feedback/skeleton.pyi
--rw-r--r--   0        0        0      704 2024-05-23 22:07:24.048760 reflex-0.5.2a1/reflex/components/chakra/feedback/spinner.py
--rw-r--r--   0        0        0     4107 2024-05-24 18:17:24.399345 reflex-0.5.2a1/reflex/components/chakra/feedback/spinner.pyi
--rw-r--r--   0        0        0     1453 2024-05-23 22:07:24.048929 reflex-0.5.2a1/reflex/components/chakra/forms/__init__.py
--rw-r--r--   0        0        0     2395 2024-05-23 22:07:24.049012 reflex-0.5.2a1/reflex/components/chakra/forms/button.py
--rw-r--r--   0        0        0    10545 2024-05-24 18:17:24.063143 reflex-0.5.2a1/reflex/components/chakra/forms/button.pyi
--rw-r--r--   0        0        0     2764 2024-05-23 22:07:24.049323 reflex-0.5.2a1/reflex/components/chakra/forms/checkbox.py
--rw-r--r--   0        0        0    10301 2024-05-24 18:17:23.972016 reflex-0.5.2a1/reflex/components/chakra/forms/checkbox.pyi
--rw-r--r--   0        0        0     2860 2024-05-23 22:07:24.049528 reflex-0.5.2a1/reflex/components/chakra/forms/colormodeswitch.py
--rw-r--r--   0        0        0    18459 2024-05-24 18:17:23.734040 reflex-0.5.2a1/reflex/components/chakra/forms/colormodeswitch.pyi
--rw-r--r--   0        0        0      246 2024-05-23 22:07:24.049762 reflex-0.5.2a1/reflex/components/chakra/forms/date_picker.py
--rw-r--r--   0        0        0     5841 2024-05-24 18:17:23.844965 reflex-0.5.2a1/reflex/components/chakra/forms/date_picker.pyi
--rw-r--r--   0        0        0      280 2024-05-23 22:07:24.049973 reflex-0.5.2a1/reflex/components/chakra/forms/date_time_picker.py
--rw-r--r--   0        0        0     5854 2024-05-24 18:17:23.355983 reflex-0.5.2a1/reflex/components/chakra/forms/date_time_picker.pyi
--rw-r--r--   0        0        0     2110 2024-05-23 22:07:24.050115 reflex-0.5.2a1/reflex/components/chakra/forms/editable.py
--rw-r--r--   0        0        0    13339 2024-05-24 18:17:24.448401 reflex-0.5.2a1/reflex/components/chakra/forms/editable.pyi
--rw-r--r--   0        0        0      246 2024-05-23 22:07:24.050281 reflex-0.5.2a1/reflex/components/chakra/forms/email.py
--rw-r--r--   0        0        0     5825 2024-05-24 18:17:23.790638 reflex-0.5.2a1/reflex/components/chakra/forms/email.pyi
--rw-r--r--   0        0        0     2579 2024-05-23 22:07:24.050478 reflex-0.5.2a1/reflex/components/chakra/forms/form.py
--rw-r--r--   0        0        0    20619 2024-05-24 18:17:23.741717 reflex-0.5.2a1/reflex/components/chakra/forms/form.pyi
--rw-r--r--   0        0        0      935 2024-05-23 22:07:24.050744 reflex-0.5.2a1/reflex/components/chakra/forms/iconbutton.py
--rw-r--r--   0        0        0     4668 2024-05-24 18:17:23.790245 reflex-0.5.2a1/reflex/components/chakra/forms/iconbutton.pyi
--rw-r--r--   0        0        0     4312 2024-05-23 22:07:24.050915 reflex-0.5.2a1/reflex/components/chakra/forms/input.py
--rw-r--r--   0        0        0    21514 2024-05-24 18:17:24.148687 reflex-0.5.2a1/reflex/components/chakra/forms/input.pyi
--rw-r--r--   0        0        0    12940 2024-05-23 22:07:24.051118 reflex-0.5.2a1/reflex/components/chakra/forms/multiselect.py
--rw-r--r--   0        0        0     4334 2024-05-23 22:07:24.051235 reflex-0.5.2a1/reflex/components/chakra/forms/numberinput.py
--rw-r--r--   0        0        0    18093 2024-05-24 18:17:24.503442 reflex-0.5.2a1/reflex/components/chakra/forms/numberinput.pyi
--rw-r--r--   0        0        0      256 2024-05-23 22:07:24.051441 reflex-0.5.2a1/reflex/components/chakra/forms/password.py
--rw-r--r--   0        0        0     5834 2024-05-24 18:17:23.849665 reflex-0.5.2a1/reflex/components/chakra/forms/password.pyi
--rw-r--r--   0        0        0     6503 2024-05-23 22:07:24.051630 reflex-0.5.2a1/reflex/components/chakra/forms/pininput.py
--rw-r--r--   0        0        0     9369 2024-05-24 18:17:23.634451 reflex-0.5.2a1/reflex/components/chakra/forms/pininput.pyi
--rw-r--r--   0        0        0     3172 2024-05-23 22:07:24.051792 reflex-0.5.2a1/reflex/components/chakra/forms/radio.py
--rw-r--r--   0        0        0     8410 2024-05-24 18:17:24.617235 reflex-0.5.2a1/reflex/components/chakra/forms/radio.pyi
--rw-r--r--   0        0        0     4543 2024-05-23 22:07:24.051994 reflex-0.5.2a1/reflex/components/chakra/forms/rangeslider.py
--rw-r--r--   0        0        0    13939 2024-05-24 18:17:23.752785 reflex-0.5.2a1/reflex/components/chakra/forms/rangeslider.pyi
--rw-r--r--   0        0        0     3624 2024-05-23 22:07:24.052210 reflex-0.5.2a1/reflex/components/chakra/forms/select.py
--rw-r--r--   0        0        0     8868 2024-05-24 18:17:23.466505 reflex-0.5.2a1/reflex/components/chakra/forms/select.pyi
--rw-r--r--   0        0        0     3532 2024-05-23 22:07:24.052410 reflex-0.5.2a1/reflex/components/chakra/forms/slider.py
--rw-r--r--   0        0        0    17461 2024-05-24 18:17:23.839820 reflex-0.5.2a1/reflex/components/chakra/forms/slider.pyi
--rw-r--r--   0        0        0     1838 2024-05-23 22:07:24.052576 reflex-0.5.2a1/reflex/components/chakra/forms/switch.py
--rw-r--r--   0        0        0     6531 2024-05-24 18:17:23.439877 reflex-0.5.2a1/reflex/components/chakra/forms/switch.pyi
--rw-r--r--   0        0        0     2474 2024-05-23 22:07:24.052732 reflex-0.5.2a1/reflex/components/chakra/forms/textarea.py
--rw-r--r--   0        0        0     5419 2024-05-24 18:17:23.406701 reflex-0.5.2a1/reflex/components/chakra/forms/textarea.pyi
--rw-r--r--   0        0        0      246 2024-05-23 22:07:24.052879 reflex-0.5.2a1/reflex/components/chakra/forms/time_picker.py
--rw-r--r--   0        0        0     5841 2024-05-24 18:17:23.338287 reflex-0.5.2a1/reflex/components/chakra/forms/time_picker.pyi
--rw-r--r--   0        0        0      487 2024-05-23 22:07:24.053058 reflex-0.5.2a1/reflex/components/chakra/layout/__init__.py
--rw-r--r--   0        0        0      315 2024-05-23 22:07:24.053146 reflex-0.5.2a1/reflex/components/chakra/layout/aspect_ratio.py
--rw-r--r--   0        0        0     3379 2024-05-24 18:17:24.134750 reflex-0.5.2a1/reflex/components/chakra/layout/aspect_ratio.pyi
--rw-r--r--   0        0        0      755 2024-05-23 22:07:24.053303 reflex-0.5.2a1/reflex/components/chakra/layout/box.py
--rw-r--r--   0        0        0     3662 2024-05-24 18:17:23.684534 reflex-0.5.2a1/reflex/components/chakra/layout/box.pyi
--rw-r--r--   0        0        0     2967 2024-05-23 22:07:24.053447 reflex-0.5.2a1/reflex/components/chakra/layout/card.py
--rw-r--r--   0        0        0    13850 2024-05-24 18:17:23.661739 reflex-0.5.2a1/reflex/components/chakra/layout/card.pyi
--rw-r--r--   0        0        0      389 2024-05-23 22:07:24.053601 reflex-0.5.2a1/reflex/components/chakra/layout/center.py
--rw-r--r--   0        0        0     8692 2024-05-24 18:17:23.861262 reflex-0.5.2a1/reflex/components/chakra/layout/center.pyi
--rw-r--r--   0        0        0      354 2024-05-23 22:07:24.053774 reflex-0.5.2a1/reflex/components/chakra/layout/container.py
--rw-r--r--   0        0        0     3431 2024-05-24 18:17:23.906150 reflex-0.5.2a1/reflex/components/chakra/layout/container.pyi
--rw-r--r--   0        0        0      715 2024-05-23 22:07:24.053931 reflex-0.5.2a1/reflex/components/chakra/layout/flex.py
--rw-r--r--   0        0        0     4138 2024-05-24 18:17:23.856235 reflex-0.5.2a1/reflex/components/chakra/layout/flex.pyi
--rw-r--r--   0        0        0     4318 2024-05-23 22:07:24.054108 reflex-0.5.2a1/reflex/components/chakra/layout/grid.py
--rw-r--r--   0        0        0    13853 2024-05-24 18:17:23.508048 reflex-0.5.2a1/reflex/components/chakra/layout/grid.pyi
--rw-r--r--   0        0        0      179 2024-05-23 22:07:24.054265 reflex-0.5.2a1/reflex/components/chakra/layout/spacer.py
--rw-r--r--   0        0        0     3230 2024-05-24 18:17:23.753119 reflex-0.5.2a1/reflex/components/chakra/layout/spacer.pyi
--rw-r--r--   0        0        0     1077 2024-05-23 22:07:24.054391 reflex-0.5.2a1/reflex/components/chakra/layout/stack.py
--rw-r--r--   0        0        0    12219 2024-05-24 18:17:23.812312 reflex-0.5.2a1/reflex/components/chakra/layout/stack.pyi
--rw-r--r--   0        0        0     1463 2024-05-23 22:07:24.054557 reflex-0.5.2a1/reflex/components/chakra/layout/wrap.py
--rw-r--r--   0        0        0     6943 2024-05-24 18:17:24.095832 reflex-0.5.2a1/reflex/components/chakra/layout/wrap.pyi
--rw-r--r--   0        0        0      190 2024-05-23 22:07:24.054738 reflex-0.5.2a1/reflex/components/chakra/media/__init__.py
--rw-r--r--   0        0        0     1668 2024-05-23 22:07:24.054834 reflex-0.5.2a1/reflex/components/chakra/media/avatar.py
--rw-r--r--   0        0        0    10445 2024-05-24 18:17:25.119256 reflex-0.5.2a1/reflex/components/chakra/media/avatar.pyi
--rw-r--r--   0        0        0     2462 2024-05-23 22:07:24.054978 reflex-0.5.2a1/reflex/components/chakra/media/icon.py
--rw-r--r--   0        0        0     6271 2024-05-24 18:17:24.970682 reflex-0.5.2a1/reflex/components/chakra/media/icon.pyi
--rw-r--r--   0        0        0     2400 2024-05-23 22:07:24.055112 reflex-0.5.2a1/reflex/components/chakra/media/image.py
--rw-r--r--   0        0        0     5423 2024-05-24 18:17:25.284214 reflex-0.5.2a1/reflex/components/chakra/media/image.pyi
--rw-r--r--   0        0        0      419 2024-05-23 22:07:24.055273 reflex-0.5.2a1/reflex/components/chakra/navigation/__init__.py
--rw-r--r--   0        0        0     2925 2024-05-23 22:07:24.055368 reflex-0.5.2a1/reflex/components/chakra/navigation/breadcrumb.py
--rw-r--r--   0        0        0    13575 2024-05-24 18:17:24.223760 reflex-0.5.2a1/reflex/components/chakra/navigation/breadcrumb.pyi
--rw-r--r--   0        0        0     1475 2024-05-23 22:07:24.055559 reflex-0.5.2a1/reflex/components/chakra/navigation/link.py
--rw-r--r--   0        0        0     3999 2024-05-24 18:17:24.135785 reflex-0.5.2a1/reflex/components/chakra/navigation/link.pyi
--rw-r--r--   0        0        0      521 2024-05-23 22:07:24.055765 reflex-0.5.2a1/reflex/components/chakra/navigation/linkoverlay.py
--rw-r--r--   0        0        0     6233 2024-05-24 18:17:24.315782 reflex-0.5.2a1/reflex/components/chakra/navigation/linkoverlay.pyi
--rw-r--r--   0        0        0     2935 2024-05-23 22:07:24.055929 reflex-0.5.2a1/reflex/components/chakra/navigation/stepper.py
--rw-r--r--   0        0        0    27922 2024-05-24 18:17:23.937771 reflex-0.5.2a1/reflex/components/chakra/navigation/stepper.pyi
--rw-r--r--   0        0        0      850 2024-05-23 22:07:24.056145 reflex-0.5.2a1/reflex/components/chakra/overlay/__init__.py
--rw-r--r--   0        0        0     5200 2024-05-23 22:07:24.056257 reflex-0.5.2a1/reflex/components/chakra/overlay/alertdialog.py
--rw-r--r--   0        0        0    23985 2024-05-24 18:17:25.493171 reflex-0.5.2a1/reflex/components/chakra/overlay/alertdialog.pyi
--rw-r--r--   0        0        0     5186 2024-05-23 22:07:24.056468 reflex-0.5.2a1/reflex/components/chakra/overlay/drawer.py
--rw-r--r--   0        0        0    25406 2024-05-24 18:17:24.311417 reflex-0.5.2a1/reflex/components/chakra/overlay/drawer.pyi
--rw-r--r--   0        0        0     6974 2024-05-23 22:07:24.056645 reflex-0.5.2a1/reflex/components/chakra/overlay/menu.py
--rw-r--r--   0        0        0    28682 2024-05-24 18:17:25.078723 reflex-0.5.2a1/reflex/components/chakra/overlay/menu.pyi
--rw-r--r--   0        0        0     5270 2024-05-23 22:07:24.056817 reflex-0.5.2a1/reflex/components/chakra/overlay/modal.py
--rw-r--r--   0        0        0    23549 2024-05-24 18:17:25.909264 reflex-0.5.2a1/reflex/components/chakra/overlay/modal.pyi
--rw-r--r--   0        0        0     5967 2024-05-23 22:07:24.057050 reflex-0.5.2a1/reflex/components/chakra/overlay/popover.py
--rw-r--r--   0        0        0    29893 2024-05-24 18:17:24.574288 reflex-0.5.2a1/reflex/components/chakra/overlay/popover.pyi
--rw-r--r--   0        0        0     2127 2024-05-23 22:07:24.057260 reflex-0.5.2a1/reflex/components/chakra/overlay/tooltip.py
--rw-r--r--   0        0        0     6060 2024-05-24 18:17:24.470002 reflex-0.5.2a1/reflex/components/chakra/overlay/tooltip.pyi
--rw-r--r--   0        0        0      271 2024-05-23 22:07:24.057423 reflex-0.5.2a1/reflex/components/chakra/typography/__init__.py
--rw-r--r--   0        0        0      379 2024-05-23 22:07:24.057495 reflex-0.5.2a1/reflex/components/chakra/typography/heading.py
--rw-r--r--   0        0        0     3706 2024-05-24 18:17:24.173439 reflex-0.5.2a1/reflex/components/chakra/typography/heading.pyi
--rw-r--r--   0        0        0      671 2024-05-23 22:07:24.057873 reflex-0.5.2a1/reflex/components/chakra/typography/highlight.py
--rw-r--r--   0        0        0     3645 2024-05-24 18:17:24.260699 reflex-0.5.2a1/reflex/components/chakra/typography/highlight.pyi
--rw-r--r--   0        0        0      328 2024-05-23 22:07:24.058053 reflex-0.5.2a1/reflex/components/chakra/typography/span.py
--rw-r--r--   0        0        0     3372 2024-05-24 18:17:24.311205 reflex-0.5.2a1/reflex/components/chakra/typography/span.pyi
--rw-r--r--   0        0        0      472 2024-05-23 22:07:24.058204 reflex-0.5.2a1/reflex/components/chakra/typography/text.py
--rw-r--r--   0        0        0     3596 2024-05-24 18:17:24.218016 reflex-0.5.2a1/reflex/components/chakra/typography/text.pyi
--rw-r--r--   0        0        0    77001 2024-05-23 22:07:24.058552 reflex-0.5.2a1/reflex/components/component.py
--rw-r--r--   0        0        0      943 2024-05-23 22:07:24.058811 reflex-0.5.2a1/reflex/components/core/__init__.py
--rw-r--r--   0        0        0     8043 2024-05-23 22:07:24.058914 reflex-0.5.2a1/reflex/components/core/banner.py
--rw-r--r--   0        0        0    22528 2024-05-24 18:17:25.155664 reflex-0.5.2a1/reflex/components/core/banner.pyi
--rw-r--r--   0        0        0     1873 2024-05-23 22:07:24.059088 reflex-0.5.2a1/reflex/components/core/client_side_routing.py
--rw-r--r--   0        0        0     6264 2024-05-24 18:17:24.651237 reflex-0.5.2a1/reflex/components/core/client_side_routing.pyi
--rw-r--r--   0        0        0      590 2024-05-23 22:07:24.059236 reflex-0.5.2a1/reflex/components/core/colors.py
--rw-r--r--   0        0        0     6163 2024-05-23 22:07:24.059313 reflex-0.5.2a1/reflex/components/core/cond.py
--rw-r--r--   0        0        0     4820 2024-05-23 22:07:24.059567 reflex-0.5.2a1/reflex/components/core/debounce.py
--rw-r--r--   0        0        0     4216 2024-05-24 18:17:24.719439 reflex-0.5.2a1/reflex/components/core/debounce.pyi
--rw-r--r--   0        0        0     4732 2024-05-23 22:07:24.060166 reflex-0.5.2a1/reflex/components/core/foreach.py
--rw-r--r--   0        0        0     1284 2024-05-23 22:07:24.060230 reflex-0.5.2a1/reflex/components/core/html.py
--rw-r--r--   0        0        0     6616 2024-05-24 18:17:24.552128 reflex-0.5.2a1/reflex/components/core/html.pyi
--rw-r--r--   0        0        0       30 2024-05-23 22:07:24.060774 reflex-0.5.2a1/reflex/components/core/layout/__init__.py
--rw-r--r--   0        0        0     9484 2024-05-23 22:07:24.060867 reflex-0.5.2a1/reflex/components/core/match.py
--rw-r--r--   0        0        0     1907 2024-05-23 22:07:24.061035 reflex-0.5.2a1/reflex/components/core/responsive.py
--rw-r--r--   0        0        0    10146 2024-05-23 22:07:24.061115 reflex-0.5.2a1/reflex/components/core/upload.py
--rw-r--r--   0        0        0    17147 2024-05-24 18:17:24.472841 reflex-0.5.2a1/reflex/components/core/upload.pyi
--rw-r--r--   0        0        0      357 2024-05-23 22:07:24.061822 reflex-0.5.2a1/reflex/components/datadisplay/__init__.py
--rw-r--r--   0        0        0    11347 2024-05-24 16:47:17.137792 reflex-0.5.2a1/reflex/components/datadisplay/code.py
--rw-r--r--   0        0        0    31197 2024-05-24 18:17:25.129041 reflex-0.5.2a1/reflex/components/datadisplay/code.pyi
--rw-r--r--   0        0        0    12632 2024-05-23 22:07:24.062397 reflex-0.5.2a1/reflex/components/datadisplay/dataeditor.py
--rw-r--r--   0        0        0    10485 2024-05-24 18:17:24.719094 reflex-0.5.2a1/reflex/components/datadisplay/dataeditor.pyi
--rw-r--r--   0        0        0     2562 2024-05-23 22:07:24.062734 reflex-0.5.2a1/reflex/components/datadisplay/logo.py
--rw-r--r--   0        0        0       73 2023-11-26 20:56:44.132351 reflex-0.5.2a1/reflex/components/el/__init__.py
--rw-r--r--   0        0        0      113 2023-11-26 20:56:44.132431 reflex-0.5.2a1/reflex/components/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-11-26 20:56:44.132596 reflex-0.5.2a1/reflex/components/el/constants/html.py
--rw-r--r--   0        0        0    15554 2023-11-26 20:56:44.132713 reflex-0.5.2a1/reflex/components/el/constants/react.py
--rw-r--r--   0        0        0     1713 2023-11-26 20:56:44.132789 reflex-0.5.2a1/reflex/components/el/constants/reflex.py
--rw-r--r--   0        0        0      494 2023-12-01 04:51:31.098496 reflex-0.5.2a1/reflex/components/el/element.py
--rw-r--r--   0        0        0     3213 2024-05-24 18:17:24.504591 reflex-0.5.2a1/reflex/components/el/element.pyi
--rw-r--r--   0        0        0     3529 2024-05-23 22:07:24.063280 reflex-0.5.2a1/reflex/components/el/elements/__init__.py
--rw-r--r--   0        0        0     1982 2024-05-23 22:07:24.063391 reflex-0.5.2a1/reflex/components/el/elements/base.py
--rw-r--r--   0        0        0     6340 2024-05-24 18:17:25.763640 reflex-0.5.2a1/reflex/components/el/elements/base.pyi
--rw-r--r--   0        0        0    20167 2024-05-23 22:07:24.063679 reflex-0.5.2a1/reflex/components/el/elements/forms.py
--rw-r--r--   0        0        0    99555 2024-05-24 18:17:29.297573 reflex-0.5.2a1/reflex/components/el/elements/forms.pyi
--rw-r--r--   0        0        0     3610 2024-05-23 22:07:24.064187 reflex-0.5.2a1/reflex/components/el/elements/inline.py
--rw-r--r--   0        0        0   164607 2024-05-24 18:17:28.121848 reflex-0.5.2a1/reflex/components/el/elements/inline.pyi
--rw-r--r--   0        0        0     8467 2024-05-23 22:07:24.064879 reflex-0.5.2a1/reflex/components/el/elements/media.py
--rw-r--r--   0        0        0    93669 2024-05-24 18:17:25.809803 reflex-0.5.2a1/reflex/components/el/elements/media.pyi
--rw-r--r--   0        0        0     1337 2023-11-26 20:56:44.134404 reflex-0.5.2a1/reflex/components/el/elements/metadata.py
--rw-r--r--   0        0        0    28031 2024-05-24 18:17:26.420859 reflex-0.5.2a1/reflex/components/el/elements/metadata.pyi
--rw-r--r--   0        0        0     1569 2023-11-26 20:56:44.134590 reflex-0.5.2a1/reflex/components/el/elements/other.py
--rw-r--r--   0        0        0    42033 2024-05-24 18:17:28.117892 reflex-0.5.2a1/reflex/components/el/elements/other.pyi
--rw-r--r--   0        0        0     1406 2024-05-23 22:07:24.065615 reflex-0.5.2a1/reflex/components/el/elements/scripts.py
--rw-r--r--   0        0        0    19615 2024-05-24 18:17:25.678066 reflex-0.5.2a1/reflex/components/el/elements/scripts.pyi
--rw-r--r--   0        0        0     1535 2024-05-23 22:07:24.065964 reflex-0.5.2a1/reflex/components/el/elements/sectioning.py
--rw-r--r--   0        0        0    87242 2024-05-24 18:17:27.638168 reflex-0.5.2a1/reflex/components/el/elements/sectioning.pyi
--rw-r--r--   0        0        0     2767 2024-05-23 22:07:24.066552 reflex-0.5.2a1/reflex/components/el/elements/tables.py
--rw-r--r--   0        0        0    61849 2024-05-24 18:17:25.354377 reflex-0.5.2a1/reflex/components/el/elements/tables.pyi
--rw-r--r--   0        0        0     2432 2024-05-23 22:07:24.067050 reflex-0.5.2a1/reflex/components/el/elements/typography.py
--rw-r--r--   0        0        0    89115 2024-05-24 18:17:25.804750 reflex-0.5.2a1/reflex/components/el/elements/typography.pyi
--rw-r--r--   0        0        0       88 2024-05-23 22:07:24.067621 reflex-0.5.2a1/reflex/components/gridjs/__init__.py
--rw-r--r--   0        0        0     4304 2024-05-23 22:07:24.067706 reflex-0.5.2a1/reflex/components/gridjs/datatable.py
--rw-r--r--   0        0        0     7053 2024-05-24 18:17:23.290206 reflex-0.5.2a1/reflex/components/gridjs/datatable.pyi
--rw-r--r--   0        0        0      501 2024-05-23 22:07:24.067888 reflex-0.5.2a1/reflex/components/literals.py
--rw-r--r--   0        0        0       73 2024-05-23 22:07:24.067968 reflex-0.5.2a1/reflex/components/lucide/__init__.py
--rw-r--r--   0        0        0    34077 2024-05-23 22:07:24.068288 reflex-0.5.2a1/reflex/components/lucide/icon.py
--rw-r--r--   0        0        0    37918 2024-05-24 18:17:27.204674 reflex-0.5.2a1/reflex/components/lucide/icon.pyi
--rw-r--r--   0        0        0       87 2024-05-23 22:07:24.068931 reflex-0.5.2a1/reflex/components/markdown/__init__.py
--rw-r--r--   0        0        0    10867 2024-05-23 22:07:24.069105 reflex-0.5.2a1/reflex/components/markdown/markdown.py
--rw-r--r--   0        0        0     5100 2024-05-24 18:17:24.542827 reflex-0.5.2a1/reflex/components/markdown/markdown.pyi
--rw-r--r--   0        0        0       44 2024-05-23 22:07:24.069399 reflex-0.5.2a1/reflex/components/media/__init__.py
--rw-r--r--   0        0        0      102 2024-05-23 22:07:24.069584 reflex-0.5.2a1/reflex/components/media/icon.py
--rw-r--r--   0        0        0       79 2024-05-23 22:07:24.069684 reflex-0.5.2a1/reflex/components/moment/__init__.py
--rw-r--r--   0        0        0     3925 2024-05-23 22:07:24.069782 reflex-0.5.2a1/reflex/components/moment/moment.py
--rw-r--r--   0        0        0     6870 2024-05-24 18:17:24.208012 reflex-0.5.2a1/reflex/components/moment/moment.pyi
--rw-r--r--   0        0        0      239 2024-05-23 22:07:24.069942 reflex-0.5.2a1/reflex/components/next/__init__.py
--rw-r--r--   0        0        0      189 2024-05-23 22:07:24.070005 reflex-0.5.2a1/reflex/components/next/base.py
--rw-r--r--   0        0        0     3233 2024-05-24 18:17:23.601458 reflex-0.5.2a1/reflex/components/next/base.pyi
--rw-r--r--   0        0        0     3831 2024-05-23 22:07:24.070176 reflex-0.5.2a1/reflex/components/next/image.py
--rw-r--r--   0        0        0     5795 2024-05-24 18:17:23.566367 reflex-0.5.2a1/reflex/components/next/image.pyi
--rw-r--r--   0        0        0      503 2024-05-23 22:07:24.070408 reflex-0.5.2a1/reflex/components/next/link.py
--rw-r--r--   0        0        0     3461 2024-05-24 18:17:23.327764 reflex-0.5.2a1/reflex/components/next/link.pyi
--rw-r--r--   0        0        0      730 2024-05-23 22:07:24.070545 reflex-0.5.2a1/reflex/components/next/video.py
--rw-r--r--   0        0        0     3429 2024-05-24 18:17:23.378778 reflex-0.5.2a1/reflex/components/next/video.pyi
--rw-r--r--   0        0        0       77 2024-05-23 22:07:24.070725 reflex-0.5.2a1/reflex/components/plotly/__init__.py
--rw-r--r--   0        0        0      964 2024-05-23 22:07:24.070795 reflex-0.5.2a1/reflex/components/plotly/plotly.py
--rw-r--r--   0        0        0     6865 2024-05-24 18:17:24.804257 reflex-0.5.2a1/reflex/components/plotly/plotly.pyi
--rw-r--r--   0        0        0      906 2024-05-23 22:07:24.071050 reflex-0.5.2a1/reflex/components/props.py
--rw-r--r--   0        0        0      112 2024-05-23 22:07:24.071248 reflex-0.5.2a1/reflex/components/radix/__init__.py
--rw-r--r--   0        0        0      214 2024-05-23 22:07:24.071337 reflex-0.5.2a1/reflex/components/radix/primitives/__init__.py
--rw-r--r--   0        0        0    15801 2024-05-24 16:47:17.138407 reflex-0.5.2a1/reflex/components/radix/primitives/accordion.py
--rw-r--r--   0        0        0    38019 2024-05-24 18:17:25.203694 reflex-0.5.2a1/reflex/components/radix/primitives/accordion.pyi
--rw-r--r--   0        0        0      869 2024-05-23 22:07:24.071818 reflex-0.5.2a1/reflex/components/radix/primitives/base.py
--rw-r--r--   0        0        0     6478 2024-05-24 18:17:25.726505 reflex-0.5.2a1/reflex/components/radix/primitives/base.pyi
--rw-r--r--   0        0        0     8660 2024-05-23 22:07:24.071992 reflex-0.5.2a1/reflex/components/radix/primitives/drawer.py
--rw-r--r--   0        0        0    34484 2024-05-24 18:17:25.412916 reflex-0.5.2a1/reflex/components/radix/primitives/drawer.pyi
--rw-r--r--   0        0        0     4941 2024-05-24 16:47:17.138863 reflex-0.5.2a1/reflex/components/radix/primitives/form.py
--rw-r--r--   0        0        0    48143 2024-05-24 18:17:26.612449 reflex-0.5.2a1/reflex/components/radix/primitives/form.pyi
--rw-r--r--   0        0        0     4022 2024-05-24 16:47:17.139254 reflex-0.5.2a1/reflex/components/radix/primitives/progress.py
--rw-r--r--   0        0        0    22866 2024-05-24 18:17:25.528909 reflex-0.5.2a1/reflex/components/radix/primitives/progress.pyi
--rw-r--r--   0        0        0     4931 2024-05-24 16:47:17.139573 reflex-0.5.2a1/reflex/components/radix/primitives/slider.py
--rw-r--r--   0        0        0    16882 2024-05-24 18:17:25.761516 reflex-0.5.2a1/reflex/components/radix/primitives/slider.pyi
--rw-r--r--   0        0        0      292 2024-05-23 22:07:24.072888 reflex-0.5.2a1/reflex/components/radix/themes/__init__.py
--rw-r--r--   0        0        0     8294 2024-05-24 16:47:17.140143 reflex-0.5.2a1/reflex/components/radix/themes/base.py
--rw-r--r--   0        0        0    26971 2024-05-24 18:17:26.902500 reflex-0.5.2a1/reflex/components/radix/themes/base.pyi
--rw-r--r--   0        0        0     5543 2024-05-23 22:07:24.073463 reflex-0.5.2a1/reflex/components/radix/themes/color_mode.py
--rw-r--r--   0        0        0    22145 2024-05-24 18:17:26.852778 reflex-0.5.2a1/reflex/components/radix/themes/color_mode.pyi
--rw-r--r--   0        0        0     2440 2024-05-23 22:07:24.073836 reflex-0.5.2a1/reflex/components/radix/themes/components/__init__.py
--rw-r--r--   0        0        0     3267 2024-05-23 22:07:24.073912 reflex-0.5.2a1/reflex/components/radix/themes/components/alert_dialog.py
--rw-r--r--   0        0        0    24434 2024-05-24 18:17:26.331761 reflex-0.5.2a1/reflex/components/radix/themes/components/alert_dialog.pyi
--rw-r--r--   0        0        0      400 2024-05-23 22:07:24.074131 reflex-0.5.2a1/reflex/components/radix/themes/components/aspect_ratio.py
--rw-r--r--   0        0        0     3640 2024-05-24 18:17:25.739485 reflex-0.5.2a1/reflex/components/radix/themes/components/aspect_ratio.pyi
--rw-r--r--   0        0        0      989 2024-05-23 22:07:24.074476 reflex-0.5.2a1/reflex/components/radix/themes/components/avatar.py
--rw-r--r--   0        0        0     6562 2024-05-24 18:17:26.067405 reflex-0.5.2a1/reflex/components/radix/themes/components/avatar.pyi
--rw-r--r--   0        0        0      821 2024-05-23 22:07:24.074712 reflex-0.5.2a1/reflex/components/radix/themes/components/badge.py
--rw-r--r--   0        0        0     9347 2024-05-24 18:17:26.688767 reflex-0.5.2a1/reflex/components/radix/themes/components/badge.pyi
--rw-r--r--   0        0        0     1125 2024-05-23 22:07:24.074970 reflex-0.5.2a1/reflex/components/radix/themes/components/button.py
--rw-r--r--   0        0        0    11939 2024-05-24 18:17:26.426242 reflex-0.5.2a1/reflex/components/radix/themes/components/button.pyi
--rw-r--r--   0        0        0     2378 2024-05-23 22:07:24.075116 reflex-0.5.2a1/reflex/components/radix/themes/components/callout.py
--rw-r--r--   0        0        0    38710 2024-05-24 18:17:27.786118 reflex-0.5.2a1/reflex/components/radix/themes/components/callout.pyi
--rw-r--r--   0        0        0      659 2024-05-23 22:07:24.075348 reflex-0.5.2a1/reflex/components/radix/themes/components/card.py
--rw-r--r--   0        0        0     7200 2024-05-24 18:17:25.927754 reflex-0.5.2a1/reflex/components/radix/themes/components/card.pyi
--rw-r--r--   0        0        0     4679 2024-05-23 22:07:24.075767 reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox.py
--rw-r--r--   0        0        0    20877 2024-05-24 18:17:26.537814 reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox.pyi
--rw-r--r--   0        0        0     1301 2024-05-23 22:07:24.075944 reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox_cards.py
--rw-r--r--   0        0        0     9591 2024-05-24 18:17:26.071013 reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox_cards.pyi
--rw-r--r--   0        0        0     1024 2024-05-23 22:07:24.076147 reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox_group.py
--rw-r--r--   0        0        0     9012 2024-05-24 18:17:26.465537 reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox_group.pyi
--rw-r--r--   0        0        0     5049 2024-05-23 22:07:24.076463 reflex-0.5.2a1/reflex/components/radix/themes/components/context_menu.py
--rw-r--r--   0        0        0    31192 2024-05-24 18:17:25.791725 reflex-0.5.2a1/reflex/components/radix/themes/components/context_menu.pyi
--rw-r--r--   0        0        0     1508 2024-05-23 22:07:24.076861 reflex-0.5.2a1/reflex/components/radix/themes/components/data_list.py
--rw-r--r--   0        0        0    15403 2024-05-24 18:17:25.949327 reflex-0.5.2a1/reflex/components/radix/themes/components/data_list.pyi
--rw-r--r--   0        0        0     2600 2024-05-23 22:07:24.077463 reflex-0.5.2a1/reflex/components/radix/themes/components/dialog.py
--rw-r--r--   0        0        0    24895 2024-05-24 18:17:26.907873 reflex-0.5.2a1/reflex/components/radix/themes/components/dialog.pyi
--rw-r--r--   0        0        0    11256 2024-05-23 22:07:24.077898 reflex-0.5.2a1/reflex/components/radix/themes/components/dropdown_menu.py
--rw-r--r--   0        0        0    37901 2024-05-24 18:17:25.758638 reflex-0.5.2a1/reflex/components/radix/themes/components/dropdown_menu.pyi
--rw-r--r--   0        0        0     2405 2024-05-23 22:07:24.078310 reflex-0.5.2a1/reflex/components/radix/themes/components/hover_card.py
--rw-r--r--   0        0        0    17744 2024-05-24 18:17:26.245730 reflex-0.5.2a1/reflex/components/radix/themes/components/hover_card.pyi
--rw-r--r--   0        0        0     2940 2024-05-23 22:07:24.078537 reflex-0.5.2a1/reflex/components/radix/themes/components/icon_button.py
--rw-r--r--   0        0        0    12126 2024-05-24 18:17:25.994520 reflex-0.5.2a1/reflex/components/radix/themes/components/icon_button.pyi
--rw-r--r--   0        0        0     1015 2024-05-23 22:07:24.078815 reflex-0.5.2a1/reflex/components/radix/themes/components/inset.py
--rw-r--r--   0        0        0     7889 2024-05-24 18:17:25.880962 reflex-0.5.2a1/reflex/components/radix/themes/components/inset.pyi
--rw-r--r--   0        0        0     3177 2024-05-23 22:07:24.078952 reflex-0.5.2a1/reflex/components/radix/themes/components/popover.py
--rw-r--r--   0        0        0    17404 2024-05-24 18:17:27.220650 reflex-0.5.2a1/reflex/components/radix/themes/components/popover.pyi
--rw-r--r--   0        0        0     1598 2024-05-23 22:07:24.079284 reflex-0.5.2a1/reflex/components/radix/themes/components/progress.py
--rw-r--r--   0        0        0     6676 2024-05-24 18:17:27.120916 reflex-0.5.2a1/reflex/components/radix/themes/components/progress.pyi
--rw-r--r--   0        0        0      762 2024-05-23 22:07:24.079594 reflex-0.5.2a1/reflex/components/radix/themes/components/radio.py
--rw-r--r--   0        0        0     5924 2024-05-24 18:17:26.105142 reflex-0.5.2a1/reflex/components/radix/themes/components/radio.pyi
--rw-r--r--   0        0        0     1250 2024-05-23 22:07:24.079896 reflex-0.5.2a1/reflex/components/radix/themes/components/radio_cards.py
--rw-r--r--   0        0        0     9561 2024-05-24 18:17:26.020173 reflex-0.5.2a1/reflex/components/radix/themes/components/radio_cards.pyi
--rw-r--r--   0        0        0     6233 2024-05-23 22:07:24.080200 reflex-0.5.2a1/reflex/components/radix/themes/components/radio_group.py
--rw-r--r--   0        0        0    24106 2024-05-24 18:17:27.243752 reflex-0.5.2a1/reflex/components/radix/themes/components/radio_group.pyi
--rw-r--r--   0        0        0      920 2024-05-23 22:07:24.080634 reflex-0.5.2a1/reflex/components/radix/themes/components/scroll_area.py
--rw-r--r--   0        0        0     4427 2024-05-24 18:17:25.967210 reflex-0.5.2a1/reflex/components/radix/themes/components/scroll_area.pyi
--rw-r--r--   0        0        0     1292 2024-05-23 22:07:24.080814 reflex-0.5.2a1/reflex/components/radix/themes/components/segmented_control.py
--rw-r--r--   0        0        0     9507 2024-05-24 18:17:27.306298 reflex-0.5.2a1/reflex/components/radix/themes/components/segmented_control.pyi
--rw-r--r--   0        0        0     8028 2024-05-23 22:07:24.081113 reflex-0.5.2a1/reflex/components/radix/themes/components/select.py
--rw-r--r--   0        0        0    45123 2024-05-24 18:17:26.898165 reflex-0.5.2a1/reflex/components/radix/themes/components/select.pyi
--rw-r--r--   0        0        0      868 2024-05-23 22:07:24.081415 reflex-0.5.2a1/reflex/components/radix/themes/components/separator.py
--rw-r--r--   0        0        0     6078 2024-05-24 18:17:25.687922 reflex-0.5.2a1/reflex/components/radix/themes/components/separator.pyi
--rw-r--r--   0        0        0      643 2024-05-23 22:07:24.081575 reflex-0.5.2a1/reflex/components/radix/themes/components/skeleton.py
--rw-r--r--   0        0        0     4289 2024-05-24 18:17:25.850463 reflex-0.5.2a1/reflex/components/radix/themes/components/skeleton.pyi
--rw-r--r--   0        0        0     3234 2024-05-23 22:07:24.081922 reflex-0.5.2a1/reflex/components/radix/themes/components/slider.py
--rw-r--r--   0        0        0     8162 2024-05-24 18:17:26.148774 reflex-0.5.2a1/reflex/components/radix/themes/components/slider.pyi
--rw-r--r--   0        0        0      431 2024-05-23 22:07:24.082079 reflex-0.5.2a1/reflex/components/radix/themes/components/spinner.py
--rw-r--r--   0        0        0     3845 2024-05-24 18:17:26.082297 reflex-0.5.2a1/reflex/components/radix/themes/components/spinner.pyi
--rw-r--r--   0        0        0     1976 2024-05-23 22:07:24.082258 reflex-0.5.2a1/reflex/components/radix/themes/components/switch.py
--rw-r--r--   0        0        0     7404 2024-05-24 18:17:26.168928 reflex-0.5.2a1/reflex/components/radix/themes/components/switch.pyi
--rw-r--r--   0        0        0     3111 2024-05-23 22:07:24.082419 reflex-0.5.2a1/reflex/components/radix/themes/components/table.py
--rw-r--r--   0        0        0    47387 2024-05-24 18:17:26.938839 reflex-0.5.2a1/reflex/components/radix/themes/components/table.pyi
--rw-r--r--   0        0        0     4150 2024-05-24 16:47:17.140632 reflex-0.5.2a1/reflex/components/radix/themes/components/tabs.py
--rw-r--r--   0        0        0    19419 2024-05-24 18:17:26.410383 reflex-0.5.2a1/reflex/components/radix/themes/components/tabs.pyi
--rw-r--r--   0        0        0     3233 2024-05-23 22:07:24.082757 reflex-0.5.2a1/reflex/components/radix/themes/components/text_area.py
--rw-r--r--   0        0        0    11711 2024-05-24 18:17:27.057578 reflex-0.5.2a1/reflex/components/radix/themes/components/text_area.pyi
--rw-r--r--   0        0        0     6527 2024-05-26 21:37:39.077690 reflex-0.5.2a1/reflex/components/radix/themes/components/text_field.py
--rw-r--r--   0        0        0    26637 2024-05-26 21:37:39.077958 reflex-0.5.2a1/reflex/components/radix/themes/components/text_field.pyi
--rw-r--r--   0        0        0     4465 2024-05-23 22:07:24.083240 reflex-0.5.2a1/reflex/components/radix/themes/components/tooltip.py
--rw-r--r--   0        0        0     8092 2024-05-24 18:17:25.698313 reflex-0.5.2a1/reflex/components/radix/themes/components/tooltip.pyi
--rw-r--r--   0        0        0      811 2024-05-23 22:07:24.083683 reflex-0.5.2a1/reflex/components/radix/themes/layout/__init__.py
--rw-r--r--   0        0        0     1211 2024-05-23 22:07:24.083755 reflex-0.5.2a1/reflex/components/radix/themes/layout/base.py
--rw-r--r--   0        0        0     7663 2024-05-24 18:17:25.624770 reflex-0.5.2a1/reflex/components/radix/themes/layout/base.pyi
--rw-r--r--   0        0        0      281 2024-05-23 22:07:24.083913 reflex-0.5.2a1/reflex/components/radix/themes/layout/box.py
--rw-r--r--   0        0        0     6462 2024-05-24 18:17:25.882224 reflex-0.5.2a1/reflex/components/radix/themes/layout/box.pyi
--rw-r--r--   0        0        0      465 2024-05-24 16:47:17.140943 reflex-0.5.2a1/reflex/components/radix/themes/layout/center.py
--rw-r--r--   0        0        0     8272 2024-05-24 18:17:25.473218 reflex-0.5.2a1/reflex/components/radix/themes/layout/center.pyi
--rw-r--r--   0        0        0     1405 2024-05-23 22:07:24.084328 reflex-0.5.2a1/reflex/components/radix/themes/layout/container.py
--rw-r--r--   0        0        0     5247 2024-05-24 18:17:25.624749 reflex-0.5.2a1/reflex/components/radix/themes/layout/container.pyi
--rw-r--r--   0        0        0     1374 2024-05-23 22:07:24.084951 reflex-0.5.2a1/reflex/components/radix/themes/layout/flex.py
--rw-r--r--   0        0        0     8501 2024-05-24 18:17:25.530022 reflex-0.5.2a1/reflex/components/radix/themes/layout/flex.pyi
--rw-r--r--   0        0        0     1498 2024-05-23 22:07:24.085255 reflex-0.5.2a1/reflex/components/radix/themes/layout/grid.py
--rw-r--r--   0        0        0     8907 2024-05-24 18:17:25.811757 reflex-0.5.2a1/reflex/components/radix/themes/layout/grid.pyi
--rw-r--r--   0        0        0     4933 2024-05-24 16:47:17.141260 reflex-0.5.2a1/reflex/components/radix/themes/layout/list.py
--rw-r--r--   0        0        0    28910 2024-05-24 18:17:25.170181 reflex-0.5.2a1/reflex/components/radix/themes/layout/list.pyi
--rw-r--r--   0        0        0      458 2024-05-23 22:07:24.085674 reflex-0.5.2a1/reflex/components/radix/themes/layout/section.py
--rw-r--r--   0        0        0     6758 2024-05-24 18:17:25.552977 reflex-0.5.2a1/reflex/components/radix/themes/layout/section.pyi
--rw-r--r--   0        0        0      448 2024-05-24 16:47:17.141536 reflex-0.5.2a1/reflex/components/radix/themes/layout/spacer.py
--rw-r--r--   0        0        0     8272 2024-05-24 18:17:25.268878 reflex-0.5.2a1/reflex/components/radix/themes/layout/spacer.pyi
--rw-r--r--   0        0        0     1522 2024-05-23 22:07:24.086073 reflex-0.5.2a1/reflex/components/radix/themes/layout/stack.py
--rw-r--r--   0        0        0    22132 2024-05-24 18:17:25.348075 reflex-0.5.2a1/reflex/components/radix/themes/layout/stack.pyi
--rw-r--r--   0        0        0      343 2024-05-23 22:07:24.086549 reflex-0.5.2a1/reflex/components/radix/themes/typography/__init__.py
--rw-r--r--   0        0        0      408 2024-05-23 22:07:24.086650 reflex-0.5.2a1/reflex/components/radix/themes/typography/base.py
--rw-r--r--   0        0        0      799 2024-05-23 22:07:24.086739 reflex-0.5.2a1/reflex/components/radix/themes/typography/blockquote.py
--rw-r--r--   0        0        0     9316 2024-05-24 18:17:27.346449 reflex-0.5.2a1/reflex/components/radix/themes/typography/blockquote.pyi
--rw-r--r--   0        0        0      909 2024-05-23 22:07:24.086897 reflex-0.5.2a1/reflex/components/radix/themes/typography/code.py
--rw-r--r--   0        0        0     9513 2024-05-24 18:17:26.430780 reflex-0.5.2a1/reflex/components/radix/themes/typography/code.pyi
--rw-r--r--   0        0        0     1324 2024-05-23 22:07:24.087027 reflex-0.5.2a1/reflex/components/radix/themes/typography/heading.py
--rw-r--r--   0        0        0    10106 2024-05-24 18:17:26.529375 reflex-0.5.2a1/reflex/components/radix/themes/typography/heading.pyi
--rw-r--r--   0        0        0     3291 2024-05-23 22:07:24.087167 reflex-0.5.2a1/reflex/components/radix/themes/typography/link.py
--rw-r--r--   0        0        0    12144 2024-05-24 18:17:26.965637 reflex-0.5.2a1/reflex/components/radix/themes/typography/link.pyi
--rw-r--r--   0        0        0     2604 2024-05-23 22:07:24.089032 reflex-0.5.2a1/reflex/components/radix/themes/typography/text.py
--rw-r--r--   0        0        0    57238 2024-05-24 18:17:27.176095 reflex-0.5.2a1/reflex/components/radix/themes/typography/text.pyi
--rw-r--r--   0        0        0      144 2024-05-23 22:07:24.089192 reflex-0.5.2a1/reflex/components/react_player/__init__.py
--rw-r--r--   0        0        0      185 2024-05-23 22:07:24.089247 reflex-0.5.2a1/reflex/components/react_player/audio.py
--rw-r--r--   0        0        0     4327 2024-05-24 18:17:24.599273 reflex-0.5.2a1/reflex/components/react_player/audio.pyi
--rw-r--r--   0        0        0     1087 2024-05-23 22:07:24.089413 reflex-0.5.2a1/reflex/components/react_player/react_player.py
--rw-r--r--   0        0        0     4354 2024-05-24 18:17:28.170716 reflex-0.5.2a1/reflex/components/react_player/react_player.pyi
--rw-r--r--   0        0        0      185 2024-05-23 22:07:24.089570 reflex-0.5.2a1/reflex/components/react_player/video.py
--rw-r--r--   0        0        0     4327 2024-05-24 18:17:24.664099 reflex-0.5.2a1/reflex/components/react_player/video.pyi
--rw-r--r--   0        0        0     2373 2024-05-23 22:07:24.089736 reflex-0.5.2a1/reflex/components/recharts/__init__.py
--rw-r--r--   0        0        0    19595 2024-05-23 22:07:24.089831 reflex-0.5.2a1/reflex/components/recharts/cartesian.py
--rw-r--r--   0        0        0    84151 2024-05-24 18:17:27.836727 reflex-0.5.2a1/reflex/components/recharts/cartesian.pyi
--rw-r--r--   0        0        0    18493 2024-05-23 22:07:24.090297 reflex-0.5.2a1/reflex/components/recharts/charts.py
--rw-r--r--   0        0        0    48757 2024-05-24 18:17:28.679664 reflex-0.5.2a1/reflex/components/recharts/charts.pyi
--rw-r--r--   0        0        0     5624 2024-05-23 22:07:24.090528 reflex-0.5.2a1/reflex/components/recharts/general.py
--rw-r--r--   0        0        0    22787 2024-05-24 18:17:28.255295 reflex-0.5.2a1/reflex/components/recharts/general.pyi
--rw-r--r--   0        0        0    10410 2024-05-23 22:07:24.090691 reflex-0.5.2a1/reflex/components/recharts/polar.py
--rw-r--r--   0        0        0    24326 2024-05-24 18:17:27.711371 reflex-0.5.2a1/reflex/components/recharts/polar.pyi
--rw-r--r--   0        0        0     2870 2024-05-23 22:07:24.090842 reflex-0.5.2a1/reflex/components/recharts/recharts.py
--rw-r--r--   0        0        0     8535 2024-05-24 18:17:27.949443 reflex-0.5.2a1/reflex/components/recharts/recharts.pyi
--rw-r--r--   0        0        0       68 2024-05-23 22:07:24.092435 reflex-0.5.2a1/reflex/components/sonner/__init__.py
--rw-r--r--   0        0        0     9822 2024-05-23 22:07:24.092539 reflex-0.5.2a1/reflex/components/sonner/toast.py
--rw-r--r--   0        0        0     8164 2024-05-24 18:17:24.719075 reflex-0.5.2a1/reflex/components/sonner/toast.pyi
--rw-r--r--   0        0        0      109 2024-05-23 22:07:24.092719 reflex-0.5.2a1/reflex/components/suneditor/__init__.py
--rw-r--r--   0        0        0     7360 2024-05-23 22:07:24.092808 reflex-0.5.2a1/reflex/components/suneditor/editor.py
--rw-r--r--   0        0        0    10330 2024-05-24 18:17:24.308668 reflex-0.5.2a1/reflex/components/suneditor/editor.pyi
--rw-r--r--   0        0        0      152 2024-05-23 22:07:24.093075 reflex-0.5.2a1/reflex/components/tags/__init__.py
--rw-r--r--   0        0        0      447 2023-07-20 22:42:41.717618 reflex-0.5.2a1/reflex/components/tags/cond_tag.py
--rw-r--r--   0        0        0     3927 2024-05-23 22:07:24.093403 reflex-0.5.2a1/reflex/components/tags/iter_tag.py
--rw-r--r--   0        0        0      387 2024-05-23 22:07:24.093478 reflex-0.5.2a1/reflex/components/tags/match_tag.py
--rw-r--r--   0        0        0     2778 2024-05-23 22:07:24.093780 reflex-0.5.2a1/reflex/components/tags/tag.py
--rw-r--r--   0        0        0      587 2023-07-20 22:42:41.717805 reflex-0.5.2a1/reflex/components/tags/tagless.py
--rw-r--r--   0        0        0    10859 2024-05-24 16:47:17.142090 reflex-0.5.2a1/reflex/config.py
--rw-r--r--   0        0        0     3402 2024-05-24 16:47:17.142369 reflex-0.5.2a1/reflex/config.pyi
--rw-r--r--   0        0        0     2036 2024-05-23 22:07:24.094524 reflex-0.5.2a1/reflex/constants/__init__.py
--rw-r--r--   0        0        0     5640 2024-05-23 22:07:24.094682 reflex-0.5.2a1/reflex/constants/base.py
--rw-r--r--   0        0        0     2980 2024-05-23 22:07:24.094912 reflex-0.5.2a1/reflex/constants/base.pyi
--rw-r--r--   0        0        0     1625 2024-05-23 22:07:24.094987 reflex-0.5.2a1/reflex/constants/colors.py
--rw-r--r--   0        0        0     4207 2024-05-23 22:07:24.095289 reflex-0.5.2a1/reflex/constants/compiler.py
--rw-r--r--   0        0        0     1331 2024-05-23 22:07:24.095442 reflex-0.5.2a1/reflex/constants/config.py
--rw-r--r--   0        0        0     1268 2024-05-23 22:07:24.095535 reflex-0.5.2a1/reflex/constants/custom_components.py
--rw-r--r--   0        0        0     2668 2024-05-23 22:07:24.095664 reflex-0.5.2a1/reflex/constants/event.py
--rw-r--r--   0        0        0     3419 2024-05-24 16:47:17.142506 reflex-0.5.2a1/reflex/constants/installer.py
--rw-r--r--   0        0        0     2144 2024-05-23 22:07:24.096361 reflex-0.5.2a1/reflex/constants/route.py
--rw-r--r--   0        0        0      636 2024-05-23 22:07:24.096532 reflex-0.5.2a1/reflex/constants/style.py
--rw-r--r--   0        0        0       36 2024-05-23 22:07:24.096625 reflex-0.5.2a1/reflex/custom_components/__init__.py
--rw-r--r--   0        0        0    33067 2024-05-24 16:47:17.143111 reflex-0.5.2a1/reflex/custom_components/custom_components.py
--rw-r--r--   0        0        0    28087 2024-05-26 21:37:48.497700 reflex-0.5.2a1/reflex/event.py
--rw-r--r--   0        0        0      778 2024-05-23 22:07:24.097229 reflex-0.5.2a1/reflex/experimental/__init__.py
--rw-r--r--   0        0        0     6597 2024-05-23 22:07:24.097324 reflex-0.5.2a1/reflex/experimental/client_state.py
--rw-r--r--   0        0        0     2196 2024-05-23 22:07:24.097529 reflex-0.5.2a1/reflex/experimental/hooks.py
--rw-r--r--   0        0        0     7267 2024-05-24 16:47:17.143287 reflex-0.5.2a1/reflex/experimental/layout.py
--rw-r--r--   0        0        0      281 2024-05-23 22:07:24.097664 reflex-0.5.2a1/reflex/experimental/misc.py
--rw-r--r--   0        0        0      111 2023-07-20 22:42:41.719277 reflex-0.5.2a1/reflex/middleware/__init__.py
--rw-r--r--   0        0        0     1484 2024-05-23 22:07:24.097791 reflex-0.5.2a1/reflex/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1169 2023-12-01 04:51:31.116521 reflex-0.5.2a1/reflex/middleware/middleware.py
--rw-r--r--   0        0        0    13227 2024-05-23 22:07:24.098145 reflex-0.5.2a1/reflex/model.py
--rw-r--r--   0        0        0     2077 2024-05-23 22:07:24.098419 reflex-0.5.2a1/reflex/page.py
--rw-r--r--   0        0        0    17826 2024-05-23 22:07:24.098559 reflex-0.5.2a1/reflex/reflex.py
--rw-r--r--   0        0        0     4198 2024-05-23 22:07:24.098696 reflex-0.5.2a1/reflex/route.py
--rw-r--r--   0        0        0   107026 2024-05-26 21:35:54.556468 reflex-0.5.2a1/reflex/state.py
--rw-r--r--   0        0        0     9542 2024-05-26 21:37:48.498428 reflex-0.5.2a1/reflex/style.py
--rw-r--r--   0        0        0    31567 2024-05-24 18:15:31.927241 reflex-0.5.2a1/reflex/testing.py
--rw-r--r--   0        0        0       24 2023-11-09 03:24:59.510665 reflex-0.5.2a1/reflex/utils/__init__.py
--rw-r--r--   0        0        0     8573 2024-05-23 22:07:24.099525 reflex-0.5.2a1/reflex/utils/build.py
--rw-r--r--   0        0        0     1255 2024-05-23 22:07:24.099853 reflex-0.5.2a1/reflex/utils/compat.py
--rw-r--r--   0        0        0     5182 2024-05-23 22:07:24.100141 reflex-0.5.2a1/reflex/utils/console.py
--rw-r--r--   0        0        0     2163 2024-05-23 22:07:24.100417 reflex-0.5.2a1/reflex/utils/exceptions.py
--rw-r--r--   0        0        0    10498 2024-05-24 16:47:17.144439 reflex-0.5.2a1/reflex/utils/exec.py
--rw-r--r--   0        0        0     2270 2024-05-23 22:07:24.100962 reflex-0.5.2a1/reflex/utils/export.py
--rw-r--r--   0        0        0    25149 2024-05-23 22:07:24.101499 reflex-0.5.2a1/reflex/utils/format.py
--rw-r--r--   0        0        0     2309 2024-05-23 22:07:24.101709 reflex-0.5.2a1/reflex/utils/imports.py
--rw-r--r--   0        0        0     4737 2024-05-23 22:07:24.101899 reflex-0.5.2a1/reflex/utils/path_ops.py
--rw-r--r--   0        0        0    52824 2024-05-23 22:07:24.102428 reflex-0.5.2a1/reflex/utils/prerequisites.py
--rw-r--r--   0        0        0    11972 2024-05-23 22:07:24.102655 reflex-0.5.2a1/reflex/utils/processes.py
--rw-r--r--   0        0        0    30637 2024-05-23 22:07:24.102877 reflex-0.5.2a1/reflex/utils/pyi_generator.py
--rw-r--r--   0        0        0     9037 2024-05-23 22:07:24.103180 reflex-0.5.2a1/reflex/utils/serializers.py
--rw-r--r--   0        0        0     5568 2024-05-24 16:47:17.144759 reflex-0.5.2a1/reflex/utils/telemetry.py
--rw-r--r--   0        0        0    15152 2024-05-23 22:07:24.103627 reflex-0.5.2a1/reflex/utils/types.py
--rw-r--r--   0        0        0     2609 2023-10-22 18:57:13.223189 reflex-0.5.2a1/reflex/utils/watch.py
--rw-r--r--   0        0        0    69637 2024-05-26 21:37:48.498752 reflex-0.5.2a1/reflex/vars.py
--rw-r--r--   0        0        0     5753 2024-05-23 22:07:24.104898 reflex-0.5.2a1/reflex/vars.pyi
--rw-r--r--   0        0        0    12085 1970-01-01 00:00:00.000000 reflex-0.5.2a1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-20 22:42:41.698164 reflex-0.5.3a1/LICENSE
+-rw-r--r--   0        0        0     9838 2024-05-23 22:07:24.004599 reflex-0.5.3a1/README.md
+-rw-r--r--   0        0        0     2996 2024-06-01 00:47:23.048934 reflex-0.5.3a1/pyproject.toml
+-rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.498329 reflex-0.5.3a1/reflex/.templates/apps/blank/assets/favicon.ico
+-rw-r--r--   0        0        0        0 2023-11-09 03:24:59.498383 reflex-0.5.3a1/reflex/.templates/apps/blank/code/__init__.py
+-rw-r--r--   0        0        0      926 2024-05-23 22:07:24.026702 reflex-0.5.3a1/reflex/.templates/apps/blank/code/blank.py
+-rw-r--r--   0        0        0       32 2023-11-09 03:24:59.498951 reflex-0.5.3a1/reflex/.templates/apps/demo/.gitignore
+-rw-r--r--   0        0        0     4286 2023-11-09 03:24:59.499075 reflex-0.5.3a1/reflex/.templates/apps/demo/assets/favicon.ico
+-rw-r--r--   0        0        0     1475 2023-11-09 03:24:59.499137 reflex-0.5.3a1/reflex/.templates/apps/demo/assets/github.svg
+-rw-r--r--   0        0        0     1899 2023-11-09 03:24:59.499199 reflex-0.5.3a1/reflex/.templates/apps/demo/assets/icon.svg
+-rw-r--r--   0        0        0     5403 2023-11-09 03:24:59.499298 reflex-0.5.3a1/reflex/.templates/apps/demo/assets/logo.svg
+-rw-r--r--   0        0        0      807 2023-11-09 03:24:59.499362 reflex-0.5.3a1/reflex/.templates/apps/demo/assets/paneleft.svg
+-rw-r--r--   0        0        0       32 2023-11-09 03:24:59.499458 reflex-0.5.3a1/reflex/.templates/apps/demo/code/__init__.py
+-rw-r--r--   0        0        0     2927 2024-05-23 22:07:24.026869 reflex-0.5.3a1/reflex/.templates/apps/demo/code/demo.py
+-rw-r--r--   0        0        0      194 2023-11-09 03:24:59.499716 reflex-0.5.3a1/reflex/.templates/apps/demo/code/pages/__init__.py
+-rw-r--r--   0        0        0      706 2024-05-23 22:07:24.027050 reflex-0.5.3a1/reflex/.templates/apps/demo/code/pages/chatapp.py
+-rw-r--r--   0        0        0    10906 2024-05-23 22:07:24.027242 reflex-0.5.3a1/reflex/.templates/apps/demo/code/pages/datatable.py
+-rw-r--r--   0        0        0     8381 2024-05-23 22:07:24.027471 reflex-0.5.3a1/reflex/.templates/apps/demo/code/pages/forms.py
+-rw-r--r--   0        0        0     8519 2024-05-23 22:07:24.027876 reflex-0.5.3a1/reflex/.templates/apps/demo/code/pages/graphing.py
+-rw-r--r--   0        0        0     1822 2024-05-23 22:07:24.028048 reflex-0.5.3a1/reflex/.templates/apps/demo/code/pages/home.py
+-rw-r--r--   0        0        0     4722 2024-05-23 22:07:24.028210 reflex-0.5.3a1/reflex/.templates/apps/demo/code/sidebar.py
+-rw-r--r--   0        0        0      510 2023-11-09 03:24:59.500529 reflex-0.5.3a1/reflex/.templates/apps/demo/code/state.py
+-rw-r--r--   0        0        0      912 2023-11-09 03:24:59.500616 reflex-0.5.3a1/reflex/.templates/apps/demo/code/states/form_state.py
+-rw-r--r--   0        0        0     1189 2023-11-09 03:24:59.500682 reflex-0.5.3a1/reflex/.templates/apps/demo/code/states/pie_state.py
+-rw-r--r--   0        0        0     1486 2024-05-23 22:07:24.028477 reflex-0.5.3a1/reflex/.templates/apps/demo/code/styles.py
+-rw-r--r--   0        0        0        0 2023-11-09 03:24:59.500792 reflex-0.5.3a1/reflex/.templates/apps/demo/code/webui/__init__.py
+-rw-r--r--   0        0        0      120 2023-11-09 03:24:59.500879 reflex-0.5.3a1/reflex/.templates/apps/demo/code/webui/components/__init__.py
+-rw-r--r--   0        0        0     3584 2024-05-23 22:07:24.028657 reflex-0.5.3a1/reflex/.templates/apps/demo/code/webui/components/chat.py
+-rw-r--r--   0        0        0      680 2023-11-09 03:24:59.500996 reflex-0.5.3a1/reflex/.templates/apps/demo/code/webui/components/loading_icon.py
+-rw-r--r--   0        0        0     1829 2024-05-23 22:07:24.028787 reflex-0.5.3a1/reflex/.templates/apps/demo/code/webui/components/modal.py
+-rw-r--r--   0        0        0     2251 2024-05-23 22:07:24.035433 reflex-0.5.3a1/reflex/.templates/apps/demo/code/webui/components/navbar.py
+-rw-r--r--   0        0        0     1735 2024-05-23 22:07:24.035615 reflex-0.5.3a1/reflex/.templates/apps/demo/code/webui/components/sidebar.py
+-rw-r--r--   0        0        0     4001 2023-11-09 03:24:59.501230 reflex-0.5.3a1/reflex/.templates/apps/demo/code/webui/state.py
+-rw-r--r--   0        0        0     2281 2024-05-23 22:07:24.035773 reflex-0.5.3a1/reflex/.templates/apps/demo/code/webui/styles.py
+-rw-r--r--   0        0        0       74 2023-10-22 18:57:13.188650 reflex-0.5.3a1/reflex/.templates/jinja/app/rxconfig.py.jinja2
+-rw-r--r--   0        0        0      127 2024-05-23 22:07:24.036845 reflex-0.5.3a1/reflex/.templates/jinja/custom_components/README.md.jinja2
+-rw-r--r--   0        0        0       32 2024-05-23 22:07:24.036930 reflex-0.5.3a1/reflex/.templates/jinja/custom_components/__init__.py.jinja2
+-rw-r--r--   0        0        0      826 2024-05-23 22:07:24.037352 reflex-0.5.3a1/reflex/.templates/jinja/custom_components/demo_app.py.jinja2
+-rw-r--r--   0        0        0      614 2024-05-23 22:07:24.037689 reflex-0.5.3a1/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2
+-rw-r--r--   0        0        0     2403 2024-05-23 22:07:24.037946 reflex-0.5.3a1/reflex/.templates/jinja/custom_components/src.py.jinja2
+-rw-r--r--   0        0        0      548 2023-10-22 18:57:13.188813 reflex-0.5.3a1/reflex/.templates/jinja/web/package.json.jinja2
+-rw-r--r--   0        0        0      930 2024-05-23 22:07:24.038352 reflex-0.5.3a1/reflex/.templates/jinja/web/pages/_app.js.jinja2
+-rw-r--r--   0        0        0      182 2023-07-20 22:42:41.708822 reflex-0.5.3a1/reflex/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      400 2024-05-23 22:07:24.038521 reflex-0.5.3a1/reflex/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0       86 2023-10-22 18:57:13.188983 reflex-0.5.3a1/reflex/.templates/jinja/web/pages/component.js.jinja2
+-rw-r--r--   0        0        0      882 2023-12-01 04:51:31.091531 reflex-0.5.3a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0      343 2024-04-04 14:57:26.375114 reflex-0.5.3a1/reflex/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0      388 2024-05-23 22:07:24.038697 reflex-0.5.3a1/reflex/.templates/jinja/web/pages/stateful_component.js.jinja2
+-rw-r--r--   0        0        0      101 2023-12-01 04:51:31.092250 reflex-0.5.3a1/reflex/.templates/jinja/web/pages/stateful_components.js.jinja2
+-rw-r--r--   0        0        0     3883 2024-05-23 22:07:24.038822 reflex-0.5.3a1/reflex/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0      141 2023-12-06 18:41:46.628030 reflex-0.5.3a1/reflex/.templates/jinja/web/styles/styles.css.jinja2
+-rw-r--r--   0        0        0      761 2024-05-23 22:07:24.039110 reflex-0.5.3a1/reflex/.templates/jinja/web/tailwind.config.js.jinja2
+-rw-r--r--   0        0        0     3790 2024-05-23 22:07:24.039386 reflex-0.5.3a1/reflex/.templates/jinja/web/utils/context.js.jinja2
+-rw-r--r--   0        0        0       37 2023-12-06 19:37:00.189183 reflex-0.5.3a1/reflex/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2023-07-20 22:42:41.709243 reflex-0.5.3a1/reflex/.templates/web/.gitignore
+-rw-r--r--   0        0        0      595 2023-10-30 01:36:56.133208 reflex-0.5.3a1/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js
+-rw-r--r--   0        0        0      645 2024-05-23 22:07:24.039706 reflex-0.5.3a1/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js
+-rw-r--r--   0        0        0       97 2023-10-22 18:57:13.190257 reflex-0.5.3a1/reflex/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0      118 2023-11-22 05:49:24.669539 reflex-0.5.3a1/reflex/.templates/web/next.config.js
+-rw-r--r--   0        0        0      108 2024-06-01 00:46:37.789133 reflex-0.5.3a1/reflex/.templates/web/postcss.config.js
+-rw-r--r--   0        0        0      112 2024-06-01 00:46:37.789413 reflex-0.5.3a1/reflex/.templates/web/styles/tailwind.css
+-rw-r--r--   0        0        0     1254 2023-09-16 20:27:37.277783 reflex-0.5.3a1/reflex/.templates/web/utils/client_side_routing.js
+-rw-r--r--   0        0        0     1622 2024-05-23 22:07:24.039831 reflex-0.5.3a1/reflex/.templates/web/utils/helpers/dataeditor.js
+-rw-r--r--   0        0        0      528 2024-05-23 22:07:24.039893 reflex-0.5.3a1/reflex/.templates/web/utils/helpers/debounce.js
+-rw-r--r--   0        0        0     1152 2023-11-22 05:49:24.669991 reflex-0.5.3a1/reflex/.templates/web/utils/helpers/range.js
+-rw-r--r--   0        0        0      566 2024-05-23 22:07:24.039949 reflex-0.5.3a1/reflex/.templates/web/utils/helpers/throttle.js
+-rw-r--r--   0        0        0    22617 2024-05-23 22:07:24.040119 reflex-0.5.3a1/reflex/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     9293 2024-06-01 00:46:37.789766 reflex-0.5.3a1/reflex/__init__.py
+-rw-r--r--   0        0        0    10367 2024-06-01 00:46:37.789991 reflex-0.5.3a1/reflex/__init__.pyi
+-rw-r--r--   0        0        0      108 2023-08-05 17:01:44.301997 reflex-0.5.3a1/reflex/__main__.py
+-rw-r--r--   0        0        0      373 2023-07-20 22:42:41.710893 reflex-0.5.3a1/reflex/admin.py
+-rw-r--r--   0        0        0    49380 2024-06-01 00:46:37.790300 reflex-0.5.3a1/reflex/app.py
+-rw-r--r--   0        0        0     1227 2024-05-23 22:07:24.041327 reflex-0.5.3a1/reflex/app_module_for_backend.py
+-rw-r--r--   0        0        0     4274 2024-05-23 22:07:24.041585 reflex-0.5.3a1/reflex/base.py
+-rw-r--r--   0        0        0       27 2023-07-20 22:42:41.711176 reflex-0.5.3a1/reflex/compiler/__init__.py
+-rw-r--r--   0        0        0    17455 2024-05-23 22:07:24.041899 reflex-0.5.3a1/reflex/compiler/compiler.py
+-rw-r--r--   0        0        0     4344 2024-05-23 22:07:24.042172 reflex-0.5.3a1/reflex/compiler/templates.py
+-rw-r--r--   0        0        0    13274 2024-05-23 22:07:24.042547 reflex-0.5.3a1/reflex/compiler/utils.py
+-rw-r--r--   0        0        0      637 2024-06-01 00:46:37.790466 reflex-0.5.3a1/reflex/components/__init__.py
+-rw-r--r--   0        0        0      930 2024-06-01 00:46:37.790544 reflex-0.5.3a1/reflex/components/__init__.pyi
+-rw-r--r--   0        0        0      647 2024-06-01 00:46:37.790857 reflex-0.5.3a1/reflex/components/base/__init__.py
+-rw-r--r--   0        0        0      973 2024-06-01 00:46:37.790954 reflex-0.5.3a1/reflex/components/base/__init__.pyi
+-rw-r--r--   0        0        0      573 2024-05-23 22:07:24.042894 reflex-0.5.3a1/reflex/components/base/app_wrap.py
+-rw-r--r--   0        0        0     2890 2024-05-24 18:17:26.775810 reflex-0.5.3a1/reflex/components/base/app_wrap.pyi
+-rw-r--r--   0        0        0     1234 2024-05-23 22:07:24.043424 reflex-0.5.3a1/reflex/components/base/bare.py
+-rw-r--r--   0        0        0      151 2023-07-20 22:42:41.711762 reflex-0.5.3a1/reflex/components/base/body.py
+-rw-r--r--   0        0        0     3206 2024-05-24 18:17:28.445017 reflex-0.5.3a1/reflex/components/base/body.pyi
+-rw-r--r--   0        0        0      583 2024-05-23 22:07:24.043906 reflex-0.5.3a1/reflex/components/base/document.py
+-rw-r--r--   0        0        0    14232 2024-05-24 18:17:26.993081 reflex-0.5.3a1/reflex/components/base/document.pyi
+-rw-r--r--   0        0        0      341 2024-06-01 00:46:37.791136 reflex-0.5.3a1/reflex/components/base/fragment.py
+-rw-r--r--   0        0        0     3246 2024-06-01 00:46:37.791322 reflex-0.5.3a1/reflex/components/base/fragment.pyi
+-rw-r--r--   0        0        0      318 2024-06-01 00:46:37.791459 reflex-0.5.3a1/reflex/components/base/head.py
+-rw-r--r--   0        0        0     6022 2024-06-01 00:46:37.791683 reflex-0.5.3a1/reflex/components/base/head.pyi
+-rw-r--r--   0        0        0      929 2023-07-20 22:42:41.711911 reflex-0.5.3a1/reflex/components/base/link.py
+-rw-r--r--   0        0        0     6990 2024-05-24 18:17:28.411498 reflex-0.5.3a1/reflex/components/base/link.pyi
+-rw-r--r--   0        0        0     1438 2023-09-16 20:27:37.279391 reflex-0.5.3a1/reflex/components/base/meta.py
+-rw-r--r--   0        0        0    12804 2024-05-24 18:17:27.232380 reflex-0.5.3a1/reflex/components/base/meta.pyi
+-rw-r--r--   0        0        0     2323 2024-06-01 00:46:37.792936 reflex-0.5.3a1/reflex/components/base/script.py
+-rw-r--r--   0        0        0     4524 2024-06-01 00:46:37.793169 reflex-0.5.3a1/reflex/components/base/script.pyi
+-rw-r--r--   0        0        0     6378 2024-05-23 22:07:24.045051 reflex-0.5.3a1/reflex/components/chakra/__init__.py
+-rw-r--r--   0        0        0     5242 2024-05-23 22:07:24.045134 reflex-0.5.3a1/reflex/components/chakra/base.py
+-rw-r--r--   0        0        0    10917 2024-05-24 18:17:24.861757 reflex-0.5.3a1/reflex/components/chakra/base.pyi
+-rw-r--r--   0        0        0      459 2024-05-23 22:07:24.045326 reflex-0.5.3a1/reflex/components/chakra/datadisplay/__init__.py
+-rw-r--r--   0        0        0      352 2024-05-23 22:07:24.045398 reflex-0.5.3a1/reflex/components/chakra/datadisplay/badge.py
+-rw-r--r--   0        0        0     3654 2024-05-24 18:17:23.594412 reflex-0.5.3a1/reflex/components/chakra/datadisplay/badge.pyi
+-rw-r--r--   0        0        0      174 2024-05-23 22:07:24.045575 reflex-0.5.3a1/reflex/components/chakra/datadisplay/code.py
+-rw-r--r--   0        0        0     3229 2024-05-24 18:17:23.555248 reflex-0.5.3a1/reflex/components/chakra/datadisplay/code.pyi
+-rw-r--r--   0        0        0      657 2024-05-23 22:07:24.045714 reflex-0.5.3a1/reflex/components/chakra/datadisplay/divider.py
+-rw-r--r--   0        0        0     3934 2024-05-24 18:17:23.503426 reflex-0.5.3a1/reflex/components/chakra/datadisplay/divider.pyi
+-rw-r--r--   0        0        0      180 2024-05-23 22:07:24.045852 reflex-0.5.3a1/reflex/components/chakra/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     3251 2024-05-24 18:17:24.668110 reflex-0.5.3a1/reflex/components/chakra/datadisplay/keyboard_key.pyi
+-rw-r--r--   0        0        0     1484 2024-05-23 22:07:24.046229 reflex-0.5.3a1/reflex/components/chakra/datadisplay/list.py
+-rw-r--r--   0        0        0    12991 2024-05-24 18:17:24.625763 reflex-0.5.3a1/reflex/components/chakra/datadisplay/list.pyi
+-rw-r--r--   0        0        0     2149 2024-05-23 22:07:24.046512 reflex-0.5.3a1/reflex/components/chakra/datadisplay/stat.py
+-rw-r--r--   0        0        0    17461 2024-05-24 18:17:23.921677 reflex-0.5.3a1/reflex/components/chakra/datadisplay/stat.pyi
+-rw-r--r--   0        0        0     9122 2024-05-23 22:07:24.046775 reflex-0.5.3a1/reflex/components/chakra/datadisplay/table.py
+-rw-r--r--   0        0        0    27252 2024-05-24 18:17:24.570212 reflex-0.5.3a1/reflex/components/chakra/datadisplay/table.pyi
+-rw-r--r--   0        0        0     2294 2024-05-23 22:07:24.046980 reflex-0.5.3a1/reflex/components/chakra/datadisplay/tag.py
+-rw-r--r--   0        0        0    15734 2024-05-24 18:17:23.854192 reflex-0.5.3a1/reflex/components/chakra/datadisplay/tag.pyi
+-rw-r--r--   0        0        0      384 2024-05-23 22:07:24.047198 reflex-0.5.3a1/reflex/components/chakra/disclosure/__init__.py
+-rw-r--r--   0        0        0     3510 2024-05-23 22:07:24.047299 reflex-0.5.3a1/reflex/components/chakra/disclosure/accordion.py
+-rw-r--r--   0        0        0    15803 2024-05-24 18:17:24.269813 reflex-0.5.3a1/reflex/components/chakra/disclosure/accordion.pyi
+-rw-r--r--   0        0        0     3295 2024-05-23 22:07:24.047512 reflex-0.5.3a1/reflex/components/chakra/disclosure/tabs.py
+-rw-r--r--   0        0        0    18525 2024-05-24 18:17:23.577560 reflex-0.5.3a1/reflex/components/chakra/disclosure/tabs.pyi
+-rw-r--r--   0        0        0     1732 2024-05-23 22:07:24.047752 reflex-0.5.3a1/reflex/components/chakra/disclosure/transition.py
+-rw-r--r--   0        0        0    20003 2024-05-24 18:17:23.981249 reflex-0.5.3a1/reflex/components/chakra/disclosure/transition.pyi
+-rw-r--r--   0        0        0      278 2024-05-23 22:07:24.047917 reflex-0.5.3a1/reflex/components/chakra/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0     3258 2024-05-24 18:17:23.263087 reflex-0.5.3a1/reflex/components/chakra/disclosure/visuallyhidden.pyi
+-rw-r--r--   0        0        0      313 2024-05-23 22:07:24.048055 reflex-0.5.3a1/reflex/components/chakra/feedback/__init__.py
+-rw-r--r--   0        0        0     1623 2024-05-23 22:07:24.048128 reflex-0.5.3a1/reflex/components/chakra/feedback/alert.py
+-rw-r--r--   0        0        0    12381 2024-05-24 18:17:24.114056 reflex-0.5.3a1/reflex/components/chakra/feedback/alert.pyi
+-rw-r--r--   0        0        0     2006 2024-05-23 22:07:24.048304 reflex-0.5.3a1/reflex/components/chakra/feedback/circularprogress.py
+-rw-r--r--   0        0        0     7637 2024-05-24 18:17:24.157731 reflex-0.5.3a1/reflex/components/chakra/feedback/circularprogress.pyi
+-rw-r--r--   0        0        0      871 2024-05-23 22:07:24.048486 reflex-0.5.3a1/reflex/components/chakra/feedback/progress.py
+-rw-r--r--   0        0        0     4278 2024-05-24 18:17:24.226071 reflex-0.5.3a1/reflex/components/chakra/feedback/progress.pyi
+-rw-r--r--   0        0        0     1776 2024-05-23 22:07:24.048623 reflex-0.5.3a1/reflex/components/chakra/feedback/skeleton.py
+-rw-r--r--   0        0        0    10690 2024-05-24 18:17:24.080524 reflex-0.5.3a1/reflex/components/chakra/feedback/skeleton.pyi
+-rw-r--r--   0        0        0      704 2024-05-23 22:07:24.048760 reflex-0.5.3a1/reflex/components/chakra/feedback/spinner.py
+-rw-r--r--   0        0        0     4107 2024-05-24 18:17:24.399345 reflex-0.5.3a1/reflex/components/chakra/feedback/spinner.pyi
+-rw-r--r--   0        0        0     1453 2024-05-23 22:07:24.048929 reflex-0.5.3a1/reflex/components/chakra/forms/__init__.py
+-rw-r--r--   0        0        0     2395 2024-05-23 22:07:24.049012 reflex-0.5.3a1/reflex/components/chakra/forms/button.py
+-rw-r--r--   0        0        0    10545 2024-05-24 18:17:24.063143 reflex-0.5.3a1/reflex/components/chakra/forms/button.pyi
+-rw-r--r--   0        0        0     2764 2024-05-23 22:07:24.049323 reflex-0.5.3a1/reflex/components/chakra/forms/checkbox.py
+-rw-r--r--   0        0        0    10301 2024-05-24 18:17:23.972016 reflex-0.5.3a1/reflex/components/chakra/forms/checkbox.pyi
+-rw-r--r--   0        0        0     2860 2024-05-23 22:07:24.049528 reflex-0.5.3a1/reflex/components/chakra/forms/colormodeswitch.py
+-rw-r--r--   0        0        0    18459 2024-05-24 18:17:23.734040 reflex-0.5.3a1/reflex/components/chakra/forms/colormodeswitch.pyi
+-rw-r--r--   0        0        0      246 2024-05-23 22:07:24.049762 reflex-0.5.3a1/reflex/components/chakra/forms/date_picker.py
+-rw-r--r--   0        0        0     5841 2024-05-24 18:17:23.844965 reflex-0.5.3a1/reflex/components/chakra/forms/date_picker.pyi
+-rw-r--r--   0        0        0      280 2024-05-23 22:07:24.049973 reflex-0.5.3a1/reflex/components/chakra/forms/date_time_picker.py
+-rw-r--r--   0        0        0     5854 2024-05-24 18:17:23.355983 reflex-0.5.3a1/reflex/components/chakra/forms/date_time_picker.pyi
+-rw-r--r--   0        0        0     2110 2024-05-23 22:07:24.050115 reflex-0.5.3a1/reflex/components/chakra/forms/editable.py
+-rw-r--r--   0        0        0    13339 2024-05-24 18:17:24.448401 reflex-0.5.3a1/reflex/components/chakra/forms/editable.pyi
+-rw-r--r--   0        0        0      246 2024-05-23 22:07:24.050281 reflex-0.5.3a1/reflex/components/chakra/forms/email.py
+-rw-r--r--   0        0        0     5825 2024-05-24 18:17:23.790638 reflex-0.5.3a1/reflex/components/chakra/forms/email.pyi
+-rw-r--r--   0        0        0     2579 2024-05-23 22:07:24.050478 reflex-0.5.3a1/reflex/components/chakra/forms/form.py
+-rw-r--r--   0        0        0    20619 2024-05-24 18:17:23.741717 reflex-0.5.3a1/reflex/components/chakra/forms/form.pyi
+-rw-r--r--   0        0        0      935 2024-05-23 22:07:24.050744 reflex-0.5.3a1/reflex/components/chakra/forms/iconbutton.py
+-rw-r--r--   0        0        0     4668 2024-05-24 18:17:23.790245 reflex-0.5.3a1/reflex/components/chakra/forms/iconbutton.pyi
+-rw-r--r--   0        0        0     4312 2024-05-23 22:07:24.050915 reflex-0.5.3a1/reflex/components/chakra/forms/input.py
+-rw-r--r--   0        0        0    21514 2024-05-24 18:17:24.148687 reflex-0.5.3a1/reflex/components/chakra/forms/input.pyi
+-rw-r--r--   0        0        0    12940 2024-05-23 22:07:24.051118 reflex-0.5.3a1/reflex/components/chakra/forms/multiselect.py
+-rw-r--r--   0        0        0     4334 2024-05-23 22:07:24.051235 reflex-0.5.3a1/reflex/components/chakra/forms/numberinput.py
+-rw-r--r--   0        0        0    18093 2024-05-24 18:17:24.503442 reflex-0.5.3a1/reflex/components/chakra/forms/numberinput.pyi
+-rw-r--r--   0        0        0      256 2024-05-23 22:07:24.051441 reflex-0.5.3a1/reflex/components/chakra/forms/password.py
+-rw-r--r--   0        0        0     5834 2024-05-24 18:17:23.849665 reflex-0.5.3a1/reflex/components/chakra/forms/password.pyi
+-rw-r--r--   0        0        0     6503 2024-05-23 22:07:24.051630 reflex-0.5.3a1/reflex/components/chakra/forms/pininput.py
+-rw-r--r--   0        0        0     9369 2024-05-24 18:17:23.634451 reflex-0.5.3a1/reflex/components/chakra/forms/pininput.pyi
+-rw-r--r--   0        0        0     3172 2024-05-23 22:07:24.051792 reflex-0.5.3a1/reflex/components/chakra/forms/radio.py
+-rw-r--r--   0        0        0     8410 2024-05-24 18:17:24.617235 reflex-0.5.3a1/reflex/components/chakra/forms/radio.pyi
+-rw-r--r--   0        0        0     4543 2024-05-23 22:07:24.051994 reflex-0.5.3a1/reflex/components/chakra/forms/rangeslider.py
+-rw-r--r--   0        0        0    13939 2024-05-24 18:17:23.752785 reflex-0.5.3a1/reflex/components/chakra/forms/rangeslider.pyi
+-rw-r--r--   0        0        0     3624 2024-05-23 22:07:24.052210 reflex-0.5.3a1/reflex/components/chakra/forms/select.py
+-rw-r--r--   0        0        0     8868 2024-05-24 18:17:23.466505 reflex-0.5.3a1/reflex/components/chakra/forms/select.pyi
+-rw-r--r--   0        0        0     3532 2024-05-23 22:07:24.052410 reflex-0.5.3a1/reflex/components/chakra/forms/slider.py
+-rw-r--r--   0        0        0    17461 2024-05-24 18:17:23.839820 reflex-0.5.3a1/reflex/components/chakra/forms/slider.pyi
+-rw-r--r--   0        0        0     1838 2024-05-23 22:07:24.052576 reflex-0.5.3a1/reflex/components/chakra/forms/switch.py
+-rw-r--r--   0        0        0     6531 2024-05-24 18:17:23.439877 reflex-0.5.3a1/reflex/components/chakra/forms/switch.pyi
+-rw-r--r--   0        0        0     2474 2024-05-23 22:07:24.052732 reflex-0.5.3a1/reflex/components/chakra/forms/textarea.py
+-rw-r--r--   0        0        0     5419 2024-05-24 18:17:23.406701 reflex-0.5.3a1/reflex/components/chakra/forms/textarea.pyi
+-rw-r--r--   0        0        0      246 2024-05-23 22:07:24.052879 reflex-0.5.3a1/reflex/components/chakra/forms/time_picker.py
+-rw-r--r--   0        0        0     5841 2024-05-24 18:17:23.338287 reflex-0.5.3a1/reflex/components/chakra/forms/time_picker.pyi
+-rw-r--r--   0        0        0      487 2024-05-23 22:07:24.053058 reflex-0.5.3a1/reflex/components/chakra/layout/__init__.py
+-rw-r--r--   0        0        0      315 2024-05-23 22:07:24.053146 reflex-0.5.3a1/reflex/components/chakra/layout/aspect_ratio.py
+-rw-r--r--   0        0        0     3379 2024-05-24 18:17:24.134750 reflex-0.5.3a1/reflex/components/chakra/layout/aspect_ratio.pyi
+-rw-r--r--   0        0        0      755 2024-05-23 22:07:24.053303 reflex-0.5.3a1/reflex/components/chakra/layout/box.py
+-rw-r--r--   0        0        0     3662 2024-05-24 18:17:23.684534 reflex-0.5.3a1/reflex/components/chakra/layout/box.pyi
+-rw-r--r--   0        0        0     2967 2024-05-23 22:07:24.053447 reflex-0.5.3a1/reflex/components/chakra/layout/card.py
+-rw-r--r--   0        0        0    13850 2024-05-24 18:17:23.661739 reflex-0.5.3a1/reflex/components/chakra/layout/card.pyi
+-rw-r--r--   0        0        0      389 2024-05-23 22:07:24.053601 reflex-0.5.3a1/reflex/components/chakra/layout/center.py
+-rw-r--r--   0        0        0     8692 2024-05-24 18:17:23.861262 reflex-0.5.3a1/reflex/components/chakra/layout/center.pyi
+-rw-r--r--   0        0        0      354 2024-05-23 22:07:24.053774 reflex-0.5.3a1/reflex/components/chakra/layout/container.py
+-rw-r--r--   0        0        0     3431 2024-05-24 18:17:23.906150 reflex-0.5.3a1/reflex/components/chakra/layout/container.pyi
+-rw-r--r--   0        0        0      715 2024-05-23 22:07:24.053931 reflex-0.5.3a1/reflex/components/chakra/layout/flex.py
+-rw-r--r--   0        0        0     4138 2024-05-24 18:17:23.856235 reflex-0.5.3a1/reflex/components/chakra/layout/flex.pyi
+-rw-r--r--   0        0        0     4318 2024-05-23 22:07:24.054108 reflex-0.5.3a1/reflex/components/chakra/layout/grid.py
+-rw-r--r--   0        0        0    13853 2024-05-24 18:17:23.508048 reflex-0.5.3a1/reflex/components/chakra/layout/grid.pyi
+-rw-r--r--   0        0        0      179 2024-05-23 22:07:24.054265 reflex-0.5.3a1/reflex/components/chakra/layout/spacer.py
+-rw-r--r--   0        0        0     3230 2024-05-24 18:17:23.753119 reflex-0.5.3a1/reflex/components/chakra/layout/spacer.pyi
+-rw-r--r--   0        0        0     1077 2024-05-23 22:07:24.054391 reflex-0.5.3a1/reflex/components/chakra/layout/stack.py
+-rw-r--r--   0        0        0    12219 2024-05-24 18:17:23.812312 reflex-0.5.3a1/reflex/components/chakra/layout/stack.pyi
+-rw-r--r--   0        0        0     1463 2024-05-23 22:07:24.054557 reflex-0.5.3a1/reflex/components/chakra/layout/wrap.py
+-rw-r--r--   0        0        0     6943 2024-05-24 18:17:24.095832 reflex-0.5.3a1/reflex/components/chakra/layout/wrap.pyi
+-rw-r--r--   0        0        0      190 2024-05-23 22:07:24.054738 reflex-0.5.3a1/reflex/components/chakra/media/__init__.py
+-rw-r--r--   0        0        0     1668 2024-05-23 22:07:24.054834 reflex-0.5.3a1/reflex/components/chakra/media/avatar.py
+-rw-r--r--   0        0        0    10445 2024-05-24 18:17:25.119256 reflex-0.5.3a1/reflex/components/chakra/media/avatar.pyi
+-rw-r--r--   0        0        0     2462 2024-05-23 22:07:24.054978 reflex-0.5.3a1/reflex/components/chakra/media/icon.py
+-rw-r--r--   0        0        0     6271 2024-05-24 18:17:24.970682 reflex-0.5.3a1/reflex/components/chakra/media/icon.pyi
+-rw-r--r--   0        0        0     2400 2024-05-23 22:07:24.055112 reflex-0.5.3a1/reflex/components/chakra/media/image.py
+-rw-r--r--   0        0        0     5423 2024-05-24 18:17:25.284214 reflex-0.5.3a1/reflex/components/chakra/media/image.pyi
+-rw-r--r--   0        0        0      419 2024-05-23 22:07:24.055273 reflex-0.5.3a1/reflex/components/chakra/navigation/__init__.py
+-rw-r--r--   0        0        0     2925 2024-05-23 22:07:24.055368 reflex-0.5.3a1/reflex/components/chakra/navigation/breadcrumb.py
+-rw-r--r--   0        0        0    13575 2024-05-24 18:17:24.223760 reflex-0.5.3a1/reflex/components/chakra/navigation/breadcrumb.pyi
+-rw-r--r--   0        0        0     1475 2024-05-23 22:07:24.055559 reflex-0.5.3a1/reflex/components/chakra/navigation/link.py
+-rw-r--r--   0        0        0     3999 2024-05-24 18:17:24.135785 reflex-0.5.3a1/reflex/components/chakra/navigation/link.pyi
+-rw-r--r--   0        0        0      521 2024-05-23 22:07:24.055765 reflex-0.5.3a1/reflex/components/chakra/navigation/linkoverlay.py
+-rw-r--r--   0        0        0     6233 2024-05-24 18:17:24.315782 reflex-0.5.3a1/reflex/components/chakra/navigation/linkoverlay.pyi
+-rw-r--r--   0        0        0     2935 2024-05-23 22:07:24.055929 reflex-0.5.3a1/reflex/components/chakra/navigation/stepper.py
+-rw-r--r--   0        0        0    27922 2024-05-24 18:17:23.937771 reflex-0.5.3a1/reflex/components/chakra/navigation/stepper.pyi
+-rw-r--r--   0        0        0      850 2024-05-23 22:07:24.056145 reflex-0.5.3a1/reflex/components/chakra/overlay/__init__.py
+-rw-r--r--   0        0        0     5200 2024-05-23 22:07:24.056257 reflex-0.5.3a1/reflex/components/chakra/overlay/alertdialog.py
+-rw-r--r--   0        0        0    23985 2024-05-24 18:17:25.493171 reflex-0.5.3a1/reflex/components/chakra/overlay/alertdialog.pyi
+-rw-r--r--   0        0        0     5186 2024-05-23 22:07:24.056468 reflex-0.5.3a1/reflex/components/chakra/overlay/drawer.py
+-rw-r--r--   0        0        0    25406 2024-05-24 18:17:24.311417 reflex-0.5.3a1/reflex/components/chakra/overlay/drawer.pyi
+-rw-r--r--   0        0        0     6974 2024-05-23 22:07:24.056645 reflex-0.5.3a1/reflex/components/chakra/overlay/menu.py
+-rw-r--r--   0        0        0    28682 2024-05-24 18:17:25.078723 reflex-0.5.3a1/reflex/components/chakra/overlay/menu.pyi
+-rw-r--r--   0        0        0     5270 2024-05-23 22:07:24.056817 reflex-0.5.3a1/reflex/components/chakra/overlay/modal.py
+-rw-r--r--   0        0        0    23549 2024-05-24 18:17:25.909264 reflex-0.5.3a1/reflex/components/chakra/overlay/modal.pyi
+-rw-r--r--   0        0        0     5967 2024-05-23 22:07:24.057050 reflex-0.5.3a1/reflex/components/chakra/overlay/popover.py
+-rw-r--r--   0        0        0    29893 2024-05-24 18:17:24.574288 reflex-0.5.3a1/reflex/components/chakra/overlay/popover.pyi
+-rw-r--r--   0        0        0     2127 2024-05-23 22:07:24.057260 reflex-0.5.3a1/reflex/components/chakra/overlay/tooltip.py
+-rw-r--r--   0        0        0     6060 2024-05-24 18:17:24.470002 reflex-0.5.3a1/reflex/components/chakra/overlay/tooltip.pyi
+-rw-r--r--   0        0        0      271 2024-05-23 22:07:24.057423 reflex-0.5.3a1/reflex/components/chakra/typography/__init__.py
+-rw-r--r--   0        0        0      379 2024-05-23 22:07:24.057495 reflex-0.5.3a1/reflex/components/chakra/typography/heading.py
+-rw-r--r--   0        0        0     3706 2024-05-24 18:17:24.173439 reflex-0.5.3a1/reflex/components/chakra/typography/heading.pyi
+-rw-r--r--   0        0        0      671 2024-05-23 22:07:24.057873 reflex-0.5.3a1/reflex/components/chakra/typography/highlight.py
+-rw-r--r--   0        0        0     3645 2024-05-24 18:17:24.260699 reflex-0.5.3a1/reflex/components/chakra/typography/highlight.pyi
+-rw-r--r--   0        0        0      328 2024-05-23 22:07:24.058053 reflex-0.5.3a1/reflex/components/chakra/typography/span.py
+-rw-r--r--   0        0        0     3372 2024-05-24 18:17:24.311205 reflex-0.5.3a1/reflex/components/chakra/typography/span.pyi
+-rw-r--r--   0        0        0      472 2024-05-23 22:07:24.058204 reflex-0.5.3a1/reflex/components/chakra/typography/text.py
+-rw-r--r--   0        0        0     3596 2024-05-24 18:17:24.218016 reflex-0.5.3a1/reflex/components/chakra/typography/text.pyi
+-rw-r--r--   0        0        0    77001 2024-05-23 22:07:24.058552 reflex-0.5.3a1/reflex/components/component.py
+-rw-r--r--   0        0        0     1184 2024-06-01 00:46:37.793372 reflex-0.5.3a1/reflex/components/core/__init__.py
+-rw-r--r--   0        0        0     1828 2024-06-01 00:46:37.793472 reflex-0.5.3a1/reflex/components/core/__init__.pyi
+-rw-r--r--   0        0        0     8226 2024-06-01 00:46:37.793607 reflex-0.5.3a1/reflex/components/core/banner.py
+-rw-r--r--   0        0        0    22710 2024-06-01 00:46:37.793735 reflex-0.5.3a1/reflex/components/core/banner.pyi
+-rw-r--r--   0        0        0     1873 2024-05-23 22:07:24.059088 reflex-0.5.3a1/reflex/components/core/client_side_routing.py
+-rw-r--r--   0        0        0     6264 2024-05-24 18:17:24.651237 reflex-0.5.3a1/reflex/components/core/client_side_routing.pyi
+-rw-r--r--   0        0        0      590 2024-05-23 22:07:24.059236 reflex-0.5.3a1/reflex/components/core/colors.py
+-rw-r--r--   0        0        0     6163 2024-05-23 22:07:24.059313 reflex-0.5.3a1/reflex/components/core/cond.py
+-rw-r--r--   0        0        0     4860 2024-06-01 00:46:37.794027 reflex-0.5.3a1/reflex/components/core/debounce.py
+-rw-r--r--   0        0        0     4255 2024-06-01 00:46:37.794211 reflex-0.5.3a1/reflex/components/core/debounce.pyi
+-rw-r--r--   0        0        0     4759 2024-06-01 00:46:37.794364 reflex-0.5.3a1/reflex/components/core/foreach.py
+-rw-r--r--   0        0        0     1305 2024-06-01 00:46:37.794490 reflex-0.5.3a1/reflex/components/core/html.py
+-rw-r--r--   0        0        0     6636 2024-06-01 00:46:37.794632 reflex-0.5.3a1/reflex/components/core/html.pyi
+-rw-r--r--   0        0        0       30 2024-05-23 22:07:24.060774 reflex-0.5.3a1/reflex/components/core/layout/__init__.py
+-rw-r--r--   0        0        0     9507 2024-06-01 00:46:37.794764 reflex-0.5.3a1/reflex/components/core/match.py
+-rw-r--r--   0        0        0     1911 2024-06-01 00:46:37.794877 reflex-0.5.3a1/reflex/components/core/responsive.py
+-rw-r--r--   0        0        0    10180 2024-06-01 00:46:37.795003 reflex-0.5.3a1/reflex/components/core/upload.py
+-rw-r--r--   0        0        0    17180 2024-06-01 00:46:37.795151 reflex-0.5.3a1/reflex/components/core/upload.pyi
+-rw-r--r--   0        0        0      470 2024-06-01 00:46:37.795296 reflex-0.5.3a1/reflex/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      690 2024-06-01 00:46:37.795373 reflex-0.5.3a1/reflex/components/datadisplay/__init__.pyi
+-rw-r--r--   0        0        0    11379 2024-06-01 00:46:37.795495 reflex-0.5.3a1/reflex/components/datadisplay/code.py
+-rw-r--r--   0        0        0    31228 2024-06-01 00:46:37.795650 reflex-0.5.3a1/reflex/components/datadisplay/code.pyi
+-rw-r--r--   0        0        0    12702 2024-06-01 00:46:37.795784 reflex-0.5.3a1/reflex/components/datadisplay/dataeditor.py
+-rw-r--r--   0        0        0    10554 2024-06-01 00:46:37.795909 reflex-0.5.3a1/reflex/components/datadisplay/dataeditor.pyi
+-rw-r--r--   0        0        0     2562 2024-05-23 22:07:24.062734 reflex-0.5.3a1/reflex/components/datadisplay/logo.py
+-rw-r--r--   0        0        0      415 2024-06-01 00:46:37.796491 reflex-0.5.3a1/reflex/components/el/__init__.py
+-rw-r--r--   0        0        0     9785 2024-06-01 00:46:37.796593 reflex-0.5.3a1/reflex/components/el/__init__.pyi
+-rw-r--r--   0        0        0      113 2023-11-26 20:56:44.132431 reflex-0.5.3a1/reflex/components/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-11-26 20:56:44.132596 reflex-0.5.3a1/reflex/components/el/constants/html.py
+-rw-r--r--   0        0        0    15554 2023-11-26 20:56:44.132713 reflex-0.5.3a1/reflex/components/el/constants/react.py
+-rw-r--r--   0        0        0     1713 2023-11-26 20:56:44.132789 reflex-0.5.3a1/reflex/components/el/constants/reflex.py
+-rw-r--r--   0        0        0      494 2023-12-01 04:51:31.098496 reflex-0.5.3a1/reflex/components/el/element.py
+-rw-r--r--   0        0        0     3213 2024-05-24 18:17:24.504591 reflex-0.5.3a1/reflex/components/el/element.pyi
+-rw-r--r--   0        0        0     2322 2024-06-01 00:46:37.796713 reflex-0.5.3a1/reflex/components/el/elements/__init__.py
+-rw-r--r--   0        0        0     9801 2024-06-01 00:46:37.796779 reflex-0.5.3a1/reflex/components/el/elements/__init__.pyi
+-rw-r--r--   0        0        0     1982 2024-05-23 22:07:24.063391 reflex-0.5.3a1/reflex/components/el/elements/base.py
+-rw-r--r--   0        0        0     6340 2024-05-24 18:17:25.763640 reflex-0.5.3a1/reflex/components/el/elements/base.pyi
+-rw-r--r--   0        0        0    20474 2024-06-01 00:46:37.797075 reflex-0.5.3a1/reflex/components/el/elements/forms.py
+-rw-r--r--   0        0        0    99861 2024-06-01 00:46:37.797289 reflex-0.5.3a1/reflex/components/el/elements/forms.pyi
+-rw-r--r--   0        0        0     4084 2024-06-01 00:46:37.797770 reflex-0.5.3a1/reflex/components/el/elements/inline.py
+-rw-r--r--   0        0        0   165080 2024-06-01 00:46:37.798006 reflex-0.5.3a1/reflex/components/el/elements/inline.pyi
+-rw-r--r--   0        0        0     8767 2024-06-01 00:46:37.798141 reflex-0.5.3a1/reflex/components/el/elements/media.py
+-rw-r--r--   0        0        0    93968 2024-06-01 00:46:37.798327 reflex-0.5.3a1/reflex/components/el/elements/media.pyi
+-rw-r--r--   0        0        0     1436 2024-06-01 00:46:37.798606 reflex-0.5.3a1/reflex/components/el/elements/metadata.py
+-rw-r--r--   0        0        0    28129 2024-06-01 00:46:37.798823 reflex-0.5.3a1/reflex/components/el/elements/metadata.pyi
+-rw-r--r--   0        0        0     1728 2024-06-01 00:46:37.798990 reflex-0.5.3a1/reflex/components/el/elements/other.py
+-rw-r--r--   0        0        0    42191 2024-06-01 00:46:37.799228 reflex-0.5.3a1/reflex/components/el/elements/other.pyi
+-rw-r--r--   0        0        0     1481 2024-06-01 00:46:37.799403 reflex-0.5.3a1/reflex/components/el/elements/scripts.py
+-rw-r--r--   0        0        0    19689 2024-06-01 00:46:37.799568 reflex-0.5.3a1/reflex/components/el/elements/scripts.pyi
+-rw-r--r--   0        0        0     1824 2024-06-01 00:46:37.799731 reflex-0.5.3a1/reflex/components/el/elements/sectioning.py
+-rw-r--r--   0        0        0    87530 2024-06-01 00:46:37.799928 reflex-0.5.3a1/reflex/components/el/elements/sectioning.pyi
+-rw-r--r--   0        0        0     2967 2024-06-01 00:46:37.800088 reflex-0.5.3a1/reflex/components/el/elements/tables.py
+-rw-r--r--   0        0        0    62048 2024-06-01 00:46:37.800263 reflex-0.5.3a1/reflex/components/el/elements/tables.pyi
+-rw-r--r--   0        0        0     2724 2024-06-01 00:46:37.800426 reflex-0.5.3a1/reflex/components/el/elements/typography.py
+-rw-r--r--   0        0        0    89365 2024-06-01 00:46:37.800602 reflex-0.5.3a1/reflex/components/el/elements/typography.pyi
+-rw-r--r--   0        0        0       88 2024-05-23 22:07:24.067621 reflex-0.5.3a1/reflex/components/gridjs/__init__.py
+-rw-r--r--   0        0        0     4304 2024-05-23 22:07:24.067706 reflex-0.5.3a1/reflex/components/gridjs/datatable.py
+-rw-r--r--   0        0        0     7053 2024-05-24 18:17:23.290206 reflex-0.5.3a1/reflex/components/gridjs/datatable.pyi
+-rw-r--r--   0        0        0      501 2024-05-23 22:07:24.067888 reflex-0.5.3a1/reflex/components/literals.py
+-rw-r--r--   0        0        0       73 2024-05-23 22:07:24.067968 reflex-0.5.3a1/reflex/components/lucide/__init__.py
+-rw-r--r--   0        0        0    34077 2024-05-23 22:07:24.068288 reflex-0.5.3a1/reflex/components/lucide/icon.py
+-rw-r--r--   0        0        0    37918 2024-05-24 18:17:27.204674 reflex-0.5.3a1/reflex/components/lucide/icon.pyi
+-rw-r--r--   0        0        0       87 2024-05-23 22:07:24.068931 reflex-0.5.3a1/reflex/components/markdown/__init__.py
+-rw-r--r--   0        0        0    10867 2024-05-23 22:07:24.069105 reflex-0.5.3a1/reflex/components/markdown/markdown.py
+-rw-r--r--   0        0        0     5100 2024-05-24 18:17:24.542827 reflex-0.5.3a1/reflex/components/markdown/markdown.pyi
+-rw-r--r--   0        0        0       44 2024-05-23 22:07:24.069399 reflex-0.5.3a1/reflex/components/media/__init__.py
+-rw-r--r--   0        0        0      102 2024-05-23 22:07:24.069584 reflex-0.5.3a1/reflex/components/media/icon.py
+-rw-r--r--   0        0        0       92 2024-06-01 00:46:37.801339 reflex-0.5.3a1/reflex/components/moment/__init__.py
+-rw-r--r--   0        0        0     3925 2024-05-23 22:07:24.069782 reflex-0.5.3a1/reflex/components/moment/moment.py
+-rw-r--r--   0        0        0     6870 2024-05-24 18:17:24.208012 reflex-0.5.3a1/reflex/components/moment/moment.pyi
+-rw-r--r--   0        0        0      239 2024-05-23 22:07:24.069942 reflex-0.5.3a1/reflex/components/next/__init__.py
+-rw-r--r--   0        0        0      189 2024-05-23 22:07:24.070005 reflex-0.5.3a1/reflex/components/next/base.py
+-rw-r--r--   0        0        0     3233 2024-05-24 18:17:23.601458 reflex-0.5.3a1/reflex/components/next/base.pyi
+-rw-r--r--   0        0        0     3831 2024-05-23 22:07:24.070176 reflex-0.5.3a1/reflex/components/next/image.py
+-rw-r--r--   0        0        0     5795 2024-05-24 18:17:23.566367 reflex-0.5.3a1/reflex/components/next/image.pyi
+-rw-r--r--   0        0        0      503 2024-05-23 22:07:24.070408 reflex-0.5.3a1/reflex/components/next/link.py
+-rw-r--r--   0        0        0     3461 2024-05-24 18:17:23.327764 reflex-0.5.3a1/reflex/components/next/link.pyi
+-rw-r--r--   0        0        0      730 2024-05-23 22:07:24.070545 reflex-0.5.3a1/reflex/components/next/video.py
+-rw-r--r--   0        0        0     3429 2024-05-24 18:17:23.378778 reflex-0.5.3a1/reflex/components/next/video.pyi
+-rw-r--r--   0        0        0       77 2024-05-23 22:07:24.070725 reflex-0.5.3a1/reflex/components/plotly/__init__.py
+-rw-r--r--   0        0        0     6201 2024-06-01 00:46:37.801747 reflex-0.5.3a1/reflex/components/plotly/plotly.py
+-rw-r--r--   0        0        0     9014 2024-06-01 00:46:37.801933 reflex-0.5.3a1/reflex/components/plotly/plotly.pyi
+-rw-r--r--   0        0        0      906 2024-05-23 22:07:24.071050 reflex-0.5.3a1/reflex/components/props.py
+-rw-r--r--   0        0        0      473 2024-06-01 00:46:37.802097 reflex-0.5.3a1/reflex/components/radix/__init__.py
+-rw-r--r--   0        0        0     4038 2024-06-01 00:46:37.802190 reflex-0.5.3a1/reflex/components/radix/__init__.pyi
+-rw-r--r--   0        0        0      442 2024-06-01 00:46:37.802509 reflex-0.5.3a1/reflex/components/radix/primitives/__init__.py
+-rw-r--r--   0        0        0      482 2024-06-01 00:46:37.802617 reflex-0.5.3a1/reflex/components/radix/primitives/__init__.pyi
+-rw-r--r--   0        0        0    15801 2024-05-24 16:47:17.138407 reflex-0.5.3a1/reflex/components/radix/primitives/accordion.py
+-rw-r--r--   0        0        0    38019 2024-05-24 18:17:25.203694 reflex-0.5.3a1/reflex/components/radix/primitives/accordion.pyi
+-rw-r--r--   0        0        0      869 2024-05-23 22:07:24.071818 reflex-0.5.3a1/reflex/components/radix/primitives/base.py
+-rw-r--r--   0        0        0     6478 2024-05-24 18:17:25.726505 reflex-0.5.3a1/reflex/components/radix/primitives/base.pyi
+-rw-r--r--   0        0        0     8660 2024-05-23 22:07:24.071992 reflex-0.5.3a1/reflex/components/radix/primitives/drawer.py
+-rw-r--r--   0        0        0    34484 2024-05-24 18:17:25.412916 reflex-0.5.3a1/reflex/components/radix/primitives/drawer.pyi
+-rw-r--r--   0        0        0     4941 2024-05-24 16:47:17.138863 reflex-0.5.3a1/reflex/components/radix/primitives/form.py
+-rw-r--r--   0        0        0    48143 2024-05-24 18:17:26.612449 reflex-0.5.3a1/reflex/components/radix/primitives/form.pyi
+-rw-r--r--   0        0        0     4022 2024-05-24 16:47:17.139254 reflex-0.5.3a1/reflex/components/radix/primitives/progress.py
+-rw-r--r--   0        0        0    22866 2024-05-24 18:17:25.528909 reflex-0.5.3a1/reflex/components/radix/primitives/progress.pyi
+-rw-r--r--   0        0        0     4931 2024-05-24 16:47:17.139573 reflex-0.5.3a1/reflex/components/radix/primitives/slider.py
+-rw-r--r--   0        0        0    16882 2024-05-24 18:17:25.761516 reflex-0.5.3a1/reflex/components/radix/primitives/slider.pyi
+-rw-r--r--   0        0        0      491 2024-06-01 00:46:37.802755 reflex-0.5.3a1/reflex/components/radix/themes/__init__.py
+-rw-r--r--   0        0        0      514 2024-06-01 00:46:37.802835 reflex-0.5.3a1/reflex/components/radix/themes/__init__.pyi
+-rw-r--r--   0        0        0     8549 2024-06-01 00:46:37.803240 reflex-0.5.3a1/reflex/components/radix/themes/base.py
+-rw-r--r--   0        0        0    27140 2024-06-01 00:46:37.803526 reflex-0.5.3a1/reflex/components/radix/themes/base.pyi
+-rw-r--r--   0        0        0     5562 2024-06-01 00:46:37.803818 reflex-0.5.3a1/reflex/components/radix/themes/color_mode.py
+-rw-r--r--   0        0        0    22164 2024-06-01 00:46:37.803942 reflex-0.5.3a1/reflex/components/radix/themes/color_mode.pyi
+-rw-r--r--   0        0        0      422 2024-06-01 00:46:37.804206 reflex-0.5.3a1/reflex/components/radix/themes/components/__init__.py
+-rw-r--r--   0        0        0     1991 2024-06-01 00:46:37.804280 reflex-0.5.3a1/reflex/components/radix/themes/components/__init__.pyi
+-rw-r--r--   0        0        0     3293 2024-06-01 00:46:37.804525 reflex-0.5.3a1/reflex/components/radix/themes/components/alert_dialog.py
+-rw-r--r--   0        0        0    24460 2024-06-01 00:46:37.804648 reflex-0.5.3a1/reflex/components/radix/themes/components/alert_dialog.pyi
+-rw-r--r--   0        0        0      400 2024-05-23 22:07:24.074131 reflex-0.5.3a1/reflex/components/radix/themes/components/aspect_ratio.py
+-rw-r--r--   0        0        0     3640 2024-05-24 18:17:25.739485 reflex-0.5.3a1/reflex/components/radix/themes/components/aspect_ratio.pyi
+-rw-r--r--   0        0        0      989 2024-05-23 22:07:24.074476 reflex-0.5.3a1/reflex/components/radix/themes/components/avatar.py
+-rw-r--r--   0        0        0     6562 2024-05-24 18:17:26.067405 reflex-0.5.3a1/reflex/components/radix/themes/components/avatar.pyi
+-rw-r--r--   0        0        0      847 2024-06-01 00:46:37.804761 reflex-0.5.3a1/reflex/components/radix/themes/components/badge.py
+-rw-r--r--   0        0        0     9373 2024-06-01 00:46:37.804883 reflex-0.5.3a1/reflex/components/radix/themes/components/badge.pyi
+-rw-r--r--   0        0        0     1151 2024-06-01 00:46:37.805000 reflex-0.5.3a1/reflex/components/radix/themes/components/button.py
+-rw-r--r--   0        0        0    11965 2024-06-01 00:46:37.805212 reflex-0.5.3a1/reflex/components/radix/themes/components/button.pyi
+-rw-r--r--   0        0        0     2416 2024-06-01 00:46:37.805337 reflex-0.5.3a1/reflex/components/radix/themes/components/callout.py
+-rw-r--r--   0        0        0    38748 2024-06-01 00:46:37.805450 reflex-0.5.3a1/reflex/components/radix/themes/components/callout.pyi
+-rw-r--r--   0        0        0      685 2024-06-01 00:46:37.805568 reflex-0.5.3a1/reflex/components/radix/themes/components/card.py
+-rw-r--r--   0        0        0     7226 2024-06-01 00:46:37.805687 reflex-0.5.3a1/reflex/components/radix/themes/components/card.pyi
+-rw-r--r--   0        0        0     4679 2024-05-23 22:07:24.075767 reflex-0.5.3a1/reflex/components/radix/themes/components/checkbox.py
+-rw-r--r--   0        0        0    20877 2024-05-24 18:17:26.537814 reflex-0.5.3a1/reflex/components/radix/themes/components/checkbox.pyi
+-rw-r--r--   0        0        0     1301 2024-05-23 22:07:24.075944 reflex-0.5.3a1/reflex/components/radix/themes/components/checkbox_cards.py
+-rw-r--r--   0        0        0     9591 2024-05-24 18:17:26.071013 reflex-0.5.3a1/reflex/components/radix/themes/components/checkbox_cards.pyi
+-rw-r--r--   0        0        0     1024 2024-05-23 22:07:24.076147 reflex-0.5.3a1/reflex/components/radix/themes/components/checkbox_group.py
+-rw-r--r--   0        0        0     9012 2024-05-24 18:17:26.465537 reflex-0.5.3a1/reflex/components/radix/themes/components/checkbox_group.pyi
+-rw-r--r--   0        0        0     5049 2024-05-23 22:07:24.076463 reflex-0.5.3a1/reflex/components/radix/themes/components/context_menu.py
+-rw-r--r--   0        0        0    31192 2024-05-24 18:17:25.791725 reflex-0.5.3a1/reflex/components/radix/themes/components/context_menu.pyi
+-rw-r--r--   0        0        0     1508 2024-05-23 22:07:24.076861 reflex-0.5.3a1/reflex/components/radix/themes/components/data_list.py
+-rw-r--r--   0        0        0    15403 2024-05-24 18:17:25.949327 reflex-0.5.3a1/reflex/components/radix/themes/components/data_list.pyi
+-rw-r--r--   0        0        0     2626 2024-06-01 00:46:37.805808 reflex-0.5.3a1/reflex/components/radix/themes/components/dialog.py
+-rw-r--r--   0        0        0    24921 2024-06-01 00:46:37.805945 reflex-0.5.3a1/reflex/components/radix/themes/components/dialog.pyi
+-rw-r--r--   0        0        0    11256 2024-05-23 22:07:24.077898 reflex-0.5.3a1/reflex/components/radix/themes/components/dropdown_menu.py
+-rw-r--r--   0        0        0    37901 2024-05-24 18:17:25.758638 reflex-0.5.3a1/reflex/components/radix/themes/components/dropdown_menu.pyi
+-rw-r--r--   0        0        0     2431 2024-06-01 00:46:37.806083 reflex-0.5.3a1/reflex/components/radix/themes/components/hover_card.py
+-rw-r--r--   0        0        0    17770 2024-06-01 00:46:37.806219 reflex-0.5.3a1/reflex/components/radix/themes/components/hover_card.pyi
+-rw-r--r--   0        0        0     2966 2024-06-01 00:46:37.806354 reflex-0.5.3a1/reflex/components/radix/themes/components/icon_button.py
+-rw-r--r--   0        0        0    12152 2024-06-01 00:46:37.806486 reflex-0.5.3a1/reflex/components/radix/themes/components/icon_button.pyi
+-rw-r--r--   0        0        0     1041 2024-06-01 00:46:37.806640 reflex-0.5.3a1/reflex/components/radix/themes/components/inset.py
+-rw-r--r--   0        0        0     7915 2024-06-01 00:46:37.806783 reflex-0.5.3a1/reflex/components/radix/themes/components/inset.pyi
+-rw-r--r--   0        0        0     3203 2024-06-01 00:46:37.806906 reflex-0.5.3a1/reflex/components/radix/themes/components/popover.py
+-rw-r--r--   0        0        0    17430 2024-06-01 00:46:37.807021 reflex-0.5.3a1/reflex/components/radix/themes/components/popover.pyi
+-rw-r--r--   0        0        0     1598 2024-05-23 22:07:24.079284 reflex-0.5.3a1/reflex/components/radix/themes/components/progress.py
+-rw-r--r--   0        0        0     6676 2024-05-24 18:17:27.120916 reflex-0.5.3a1/reflex/components/radix/themes/components/progress.pyi
+-rw-r--r--   0        0        0      762 2024-05-23 22:07:24.079594 reflex-0.5.3a1/reflex/components/radix/themes/components/radio.py
+-rw-r--r--   0        0        0     5924 2024-05-24 18:17:26.105142 reflex-0.5.3a1/reflex/components/radix/themes/components/radio.pyi
+-rw-r--r--   0        0        0     1250 2024-05-23 22:07:24.079896 reflex-0.5.3a1/reflex/components/radix/themes/components/radio_cards.py
+-rw-r--r--   0        0        0     9561 2024-05-24 18:17:26.020173 reflex-0.5.3a1/reflex/components/radix/themes/components/radio_cards.pyi
+-rw-r--r--   0        0        0     6233 2024-05-23 22:07:24.080200 reflex-0.5.3a1/reflex/components/radix/themes/components/radio_group.py
+-rw-r--r--   0        0        0    24106 2024-05-24 18:17:27.243752 reflex-0.5.3a1/reflex/components/radix/themes/components/radio_group.pyi
+-rw-r--r--   0        0        0      920 2024-05-23 22:07:24.080634 reflex-0.5.3a1/reflex/components/radix/themes/components/scroll_area.py
+-rw-r--r--   0        0        0     4427 2024-05-24 18:17:25.967210 reflex-0.5.3a1/reflex/components/radix/themes/components/scroll_area.pyi
+-rw-r--r--   0        0        0     1292 2024-05-23 22:07:24.080814 reflex-0.5.3a1/reflex/components/radix/themes/components/segmented_control.py
+-rw-r--r--   0        0        0     9507 2024-05-24 18:17:27.306298 reflex-0.5.3a1/reflex/components/radix/themes/components/segmented_control.pyi
+-rw-r--r--   0        0        0     8028 2024-05-23 22:07:24.081113 reflex-0.5.3a1/reflex/components/radix/themes/components/select.py
+-rw-r--r--   0        0        0    45123 2024-05-24 18:17:26.898165 reflex-0.5.3a1/reflex/components/radix/themes/components/select.pyi
+-rw-r--r--   0        0        0      868 2024-05-23 22:07:24.081415 reflex-0.5.3a1/reflex/components/radix/themes/components/separator.py
+-rw-r--r--   0        0        0     6078 2024-05-24 18:17:25.687922 reflex-0.5.3a1/reflex/components/radix/themes/components/separator.pyi
+-rw-r--r--   0        0        0      643 2024-05-23 22:07:24.081575 reflex-0.5.3a1/reflex/components/radix/themes/components/skeleton.py
+-rw-r--r--   0        0        0     4289 2024-05-24 18:17:25.850463 reflex-0.5.3a1/reflex/components/radix/themes/components/skeleton.pyi
+-rw-r--r--   0        0        0     3234 2024-05-23 22:07:24.081922 reflex-0.5.3a1/reflex/components/radix/themes/components/slider.py
+-rw-r--r--   0        0        0     8162 2024-05-24 18:17:26.148774 reflex-0.5.3a1/reflex/components/radix/themes/components/slider.pyi
+-rw-r--r--   0        0        0      431 2024-05-23 22:07:24.082079 reflex-0.5.3a1/reflex/components/radix/themes/components/spinner.py
+-rw-r--r--   0        0        0     3845 2024-05-24 18:17:26.082297 reflex-0.5.3a1/reflex/components/radix/themes/components/spinner.pyi
+-rw-r--r--   0        0        0     1976 2024-05-23 22:07:24.082258 reflex-0.5.3a1/reflex/components/radix/themes/components/switch.py
+-rw-r--r--   0        0        0     7404 2024-05-24 18:17:26.168928 reflex-0.5.3a1/reflex/components/radix/themes/components/switch.pyi
+-rw-r--r--   0        0        0     3173 2024-06-01 00:46:37.807165 reflex-0.5.3a1/reflex/components/radix/themes/components/table.py
+-rw-r--r--   0        0        0    47449 2024-06-01 00:46:37.807380 reflex-0.5.3a1/reflex/components/radix/themes/components/table.pyi
+-rw-r--r--   0        0        0     4150 2024-05-24 16:47:17.140632 reflex-0.5.3a1/reflex/components/radix/themes/components/tabs.py
+-rw-r--r--   0        0        0    19419 2024-05-24 18:17:26.410383 reflex-0.5.3a1/reflex/components/radix/themes/components/tabs.pyi
+-rw-r--r--   0        0        0     3595 2024-06-01 00:46:37.807542 reflex-0.5.3a1/reflex/components/radix/themes/components/text_area.py
+-rw-r--r--   0        0        0    12460 2024-06-01 00:46:37.807845 reflex-0.5.3a1/reflex/components/radix/themes/components/text_area.pyi
+-rw-r--r--   0        0        0     6550 2024-06-01 00:46:37.807981 reflex-0.5.3a1/reflex/components/radix/themes/components/text_field.py
+-rw-r--r--   0        0        0    26660 2024-06-01 00:46:37.808102 reflex-0.5.3a1/reflex/components/radix/themes/components/text_field.pyi
+-rw-r--r--   0        0        0     4465 2024-05-23 22:07:24.083240 reflex-0.5.3a1/reflex/components/radix/themes/components/tooltip.py
+-rw-r--r--   0        0        0     8092 2024-05-24 18:17:25.698313 reflex-0.5.3a1/reflex/components/radix/themes/components/tooltip.pyi
+-rw-r--r--   0        0        0      405 2024-06-01 00:46:37.808237 reflex-0.5.3a1/reflex/components/radix/themes/layout/__init__.py
+-rw-r--r--   0        0        0      860 2024-06-01 00:46:37.808318 reflex-0.5.3a1/reflex/components/radix/themes/layout/__init__.pyi
+-rw-r--r--   0        0        0     1211 2024-05-23 22:07:24.083755 reflex-0.5.3a1/reflex/components/radix/themes/layout/base.py
+-rw-r--r--   0        0        0     7663 2024-05-24 18:17:25.624770 reflex-0.5.3a1/reflex/components/radix/themes/layout/base.pyi
+-rw-r--r--   0        0        0      326 2024-06-01 00:46:37.808434 reflex-0.5.3a1/reflex/components/radix/themes/layout/box.py
+-rw-r--r--   0        0        0     6506 2024-06-01 00:46:37.808576 reflex-0.5.3a1/reflex/components/radix/themes/layout/box.pyi
+-rw-r--r--   0        0        0      490 2024-06-01 00:46:37.808745 reflex-0.5.3a1/reflex/components/radix/themes/layout/center.py
+-rw-r--r--   0        0        0     8296 2024-06-01 00:46:37.808933 reflex-0.5.3a1/reflex/components/radix/themes/layout/center.pyi
+-rw-r--r--   0        0        0     1462 2024-06-01 00:46:37.809066 reflex-0.5.3a1/reflex/components/radix/themes/layout/container.py
+-rw-r--r--   0        0        0     5303 2024-06-01 00:46:37.809188 reflex-0.5.3a1/reflex/components/radix/themes/layout/container.pyi
+-rw-r--r--   0        0        0     1421 2024-06-01 00:46:37.809301 reflex-0.5.3a1/reflex/components/radix/themes/layout/flex.py
+-rw-r--r--   0        0        0     8547 2024-06-01 00:46:37.809826 reflex-0.5.3a1/reflex/components/radix/themes/layout/flex.pyi
+-rw-r--r--   0        0        0     1545 2024-06-01 00:46:37.810055 reflex-0.5.3a1/reflex/components/radix/themes/layout/grid.py
+-rw-r--r--   0        0        0     8953 2024-06-01 00:46:37.810175 reflex-0.5.3a1/reflex/components/radix/themes/layout/grid.pyi
+-rw-r--r--   0        0        0     5343 2024-06-01 00:46:37.810355 reflex-0.5.3a1/reflex/components/radix/themes/layout/list.py
+-rw-r--r--   0        0        0    29001 2024-06-01 00:46:37.810503 reflex-0.5.3a1/reflex/components/radix/themes/layout/list.pyi
+-rw-r--r--   0        0        0      534 2024-06-01 00:46:37.810747 reflex-0.5.3a1/reflex/components/radix/themes/layout/section.py
+-rw-r--r--   0        0        0     6810 2024-06-01 00:46:37.810877 reflex-0.5.3a1/reflex/components/radix/themes/layout/section.pyi
+-rw-r--r--   0        0        0      473 2024-06-01 00:46:37.810990 reflex-0.5.3a1/reflex/components/radix/themes/layout/spacer.py
+-rw-r--r--   0        0        0     8296 2024-06-01 00:46:37.811109 reflex-0.5.3a1/reflex/components/radix/themes/layout/spacer.pyi
+-rw-r--r--   0        0        0     1591 2024-06-01 00:46:37.811290 reflex-0.5.3a1/reflex/components/radix/themes/layout/stack.py
+-rw-r--r--   0        0        0    22200 2024-06-01 00:46:37.811406 reflex-0.5.3a1/reflex/components/radix/themes/layout/stack.pyi
+-rw-r--r--   0        0        0      421 2024-06-01 00:46:37.811710 reflex-0.5.3a1/reflex/components/radix/themes/typography/__init__.py
+-rw-r--r--   0        0        0      521 2024-06-01 00:46:37.811776 reflex-0.5.3a1/reflex/components/radix/themes/typography/__init__.pyi
+-rw-r--r--   0        0        0      408 2024-05-23 22:07:24.086650 reflex-0.5.3a1/reflex/components/radix/themes/typography/base.py
+-rw-r--r--   0        0        0      858 2024-06-01 00:46:37.811908 reflex-0.5.3a1/reflex/components/radix/themes/typography/blockquote.py
+-rw-r--r--   0        0        0     9374 2024-06-01 00:46:37.812018 reflex-0.5.3a1/reflex/components/radix/themes/typography/blockquote.pyi
+-rw-r--r--   0        0        0      956 2024-06-01 00:46:37.812123 reflex-0.5.3a1/reflex/components/radix/themes/typography/code.py
+-rw-r--r--   0        0        0     9559 2024-06-01 00:46:37.812769 reflex-0.5.3a1/reflex/components/radix/themes/typography/code.pyi
+-rw-r--r--   0        0        0     1377 2024-06-01 00:46:37.812890 reflex-0.5.3a1/reflex/components/radix/themes/typography/heading.py
+-rw-r--r--   0        0        0    10158 2024-06-01 00:46:37.813010 reflex-0.5.3a1/reflex/components/radix/themes/typography/heading.pyi
+-rw-r--r--   0        0        0     3312 2024-06-01 00:46:37.813127 reflex-0.5.3a1/reflex/components/radix/themes/typography/link.py
+-rw-r--r--   0        0        0    12164 2024-06-01 00:46:37.813240 reflex-0.5.3a1/reflex/components/radix/themes/typography/link.pyi
+-rw-r--r--   0        0        0     2654 2024-06-01 00:46:37.813356 reflex-0.5.3a1/reflex/components/radix/themes/typography/text.py
+-rw-r--r--   0        0        0    57288 2024-06-01 00:46:37.813486 reflex-0.5.3a1/reflex/components/radix/themes/typography/text.pyi
+-rw-r--r--   0        0        0      144 2024-05-23 22:07:24.089192 reflex-0.5.3a1/reflex/components/react_player/__init__.py
+-rw-r--r--   0        0        0      185 2024-05-23 22:07:24.089247 reflex-0.5.3a1/reflex/components/react_player/audio.py
+-rw-r--r--   0        0        0     4327 2024-05-24 18:17:24.599273 reflex-0.5.3a1/reflex/components/react_player/audio.pyi
+-rw-r--r--   0        0        0     1087 2024-05-23 22:07:24.089413 reflex-0.5.3a1/reflex/components/react_player/react_player.py
+-rw-r--r--   0        0        0     4354 2024-05-24 18:17:28.170716 reflex-0.5.3a1/reflex/components/react_player/react_player.pyi
+-rw-r--r--   0        0        0      185 2024-05-23 22:07:24.089570 reflex-0.5.3a1/reflex/components/react_player/video.py
+-rw-r--r--   0        0        0     4327 2024-05-24 18:17:24.664099 reflex-0.5.3a1/reflex/components/react_player/video.pyi
+-rw-r--r--   0        0        0     2643 2024-06-01 00:46:37.813794 reflex-0.5.3a1/reflex/components/recharts/__init__.py
+-rw-r--r--   0        0        0     5113 2024-06-01 00:46:37.813988 reflex-0.5.3a1/reflex/components/recharts/__init__.pyi
+-rw-r--r--   0        0        0    20003 2024-06-01 00:46:37.814159 reflex-0.5.3a1/reflex/components/recharts/cartesian.py
+-rw-r--r--   0        0        0    84558 2024-06-01 00:46:37.814343 reflex-0.5.3a1/reflex/components/recharts/cartesian.pyi
+-rw-r--r--   0        0        0    18817 2024-06-01 00:46:37.814493 reflex-0.5.3a1/reflex/components/recharts/charts.py
+-rw-r--r--   0        0        0    49080 2024-06-01 00:46:37.814627 reflex-0.5.3a1/reflex/components/recharts/charts.pyi
+-rw-r--r--   0        0        0     5792 2024-06-01 00:46:37.814776 reflex-0.5.3a1/reflex/components/recharts/general.py
+-rw-r--r--   0        0        0    22954 2024-06-01 00:46:37.814898 reflex-0.5.3a1/reflex/components/recharts/general.pyi
+-rw-r--r--   0        0        0    10714 2024-06-01 00:46:37.815045 reflex-0.5.3a1/reflex/components/recharts/polar.py
+-rw-r--r--   0        0        0    24653 2024-06-01 00:46:37.815196 reflex-0.5.3a1/reflex/components/recharts/polar.pyi
+-rw-r--r--   0        0        0     2870 2024-05-23 22:07:24.090842 reflex-0.5.3a1/reflex/components/recharts/recharts.py
+-rw-r--r--   0        0        0     8535 2024-05-24 18:17:27.949443 reflex-0.5.3a1/reflex/components/recharts/recharts.pyi
+-rw-r--r--   0        0        0       68 2024-05-23 22:07:24.092435 reflex-0.5.3a1/reflex/components/sonner/__init__.py
+-rw-r--r--   0        0        0     9822 2024-05-23 22:07:24.092539 reflex-0.5.3a1/reflex/components/sonner/toast.py
+-rw-r--r--   0        0        0     8164 2024-05-24 18:17:24.719075 reflex-0.5.3a1/reflex/components/sonner/toast.pyi
+-rw-r--r--   0        0        0      109 2024-05-23 22:07:24.092719 reflex-0.5.3a1/reflex/components/suneditor/__init__.py
+-rw-r--r--   0        0        0     7360 2024-05-23 22:07:24.092808 reflex-0.5.3a1/reflex/components/suneditor/editor.py
+-rw-r--r--   0        0        0    10330 2024-05-24 18:17:24.308668 reflex-0.5.3a1/reflex/components/suneditor/editor.pyi
+-rw-r--r--   0        0        0      152 2024-05-23 22:07:24.093075 reflex-0.5.3a1/reflex/components/tags/__init__.py
+-rw-r--r--   0        0        0      447 2023-07-20 22:42:41.717618 reflex-0.5.3a1/reflex/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     3927 2024-05-23 22:07:24.093403 reflex-0.5.3a1/reflex/components/tags/iter_tag.py
+-rw-r--r--   0        0        0      387 2024-05-23 22:07:24.093478 reflex-0.5.3a1/reflex/components/tags/match_tag.py
+-rw-r--r--   0        0        0     2778 2024-05-23 22:07:24.093780 reflex-0.5.3a1/reflex/components/tags/tag.py
+-rw-r--r--   0        0        0      587 2023-07-20 22:42:41.717805 reflex-0.5.3a1/reflex/components/tags/tagless.py
+-rw-r--r--   0        0        0    10944 2024-06-01 00:46:37.815355 reflex-0.5.3a1/reflex/config.py
+-rw-r--r--   0        0        0     1980 2024-06-01 00:46:37.815944 reflex-0.5.3a1/reflex/constants/__init__.py
+-rw-r--r--   0        0        0     5768 2024-06-01 00:46:37.816129 reflex-0.5.3a1/reflex/constants/base.py
+-rw-r--r--   0        0        0     3120 2024-06-01 00:46:37.816267 reflex-0.5.3a1/reflex/constants/base.pyi
+-rw-r--r--   0        0        0     1625 2024-05-23 22:07:24.094987 reflex-0.5.3a1/reflex/constants/colors.py
+-rw-r--r--   0        0        0     4207 2024-05-23 22:07:24.095289 reflex-0.5.3a1/reflex/constants/compiler.py
+-rw-r--r--   0        0        0     1331 2024-05-23 22:07:24.095442 reflex-0.5.3a1/reflex/constants/config.py
+-rw-r--r--   0        0        0     1268 2024-05-23 22:07:24.095535 reflex-0.5.3a1/reflex/constants/custom_components.py
+-rw-r--r--   0        0        0     2668 2024-05-23 22:07:24.095664 reflex-0.5.3a1/reflex/constants/event.py
+-rw-r--r--   0        0        0     3456 2024-06-01 00:46:37.816402 reflex-0.5.3a1/reflex/constants/installer.py
+-rw-r--r--   0        0        0     2144 2024-05-23 22:07:24.096361 reflex-0.5.3a1/reflex/constants/route.py
+-rw-r--r--   0        0        0      636 2024-05-23 22:07:24.096532 reflex-0.5.3a1/reflex/constants/style.py
+-rw-r--r--   0        0        0       36 2024-05-23 22:07:24.096625 reflex-0.5.3a1/reflex/custom_components/__init__.py
+-rw-r--r--   0        0        0    33067 2024-05-24 16:47:17.143111 reflex-0.5.3a1/reflex/custom_components/custom_components.py
+-rw-r--r--   0        0        0    28087 2024-05-26 21:37:48.497700 reflex-0.5.3a1/reflex/event.py
+-rw-r--r--   0        0        0      830 2024-06-01 00:46:37.816777 reflex-0.5.3a1/reflex/experimental/__init__.py
+-rw-r--r--   0        0        0     1757 2024-06-01 00:46:37.816884 reflex-0.5.3a1/reflex/experimental/assets.py
+-rw-r--r--   0        0        0     6623 2024-06-01 00:46:37.817052 reflex-0.5.3a1/reflex/experimental/client_state.py
+-rw-r--r--   0        0        0     2256 2024-06-01 00:46:37.817184 reflex-0.5.3a1/reflex/experimental/hooks.py
+-rw-r--r--   0        0        0     7385 2024-06-01 00:46:37.817344 reflex-0.5.3a1/reflex/experimental/layout.py
+-rw-r--r--   0        0        0      281 2024-05-23 22:07:24.097664 reflex-0.5.3a1/reflex/experimental/misc.py
+-rw-r--r--   0        0        0      111 2023-07-20 22:42:41.719277 reflex-0.5.3a1/reflex/middleware/__init__.py
+-rw-r--r--   0        0        0     1484 2024-05-23 22:07:24.097791 reflex-0.5.3a1/reflex/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1169 2023-12-01 04:51:31.116521 reflex-0.5.3a1/reflex/middleware/middleware.py
+-rw-r--r--   0        0        0    13227 2024-05-23 22:07:24.098145 reflex-0.5.3a1/reflex/model.py
+-rw-r--r--   0        0        0     2077 2024-05-23 22:07:24.098419 reflex-0.5.3a1/reflex/page.py
+-rw-r--r--   0        0        0    17826 2024-05-23 22:07:24.098559 reflex-0.5.3a1/reflex/reflex.py
+-rw-r--r--   0        0        0     4198 2024-05-23 22:07:24.098696 reflex-0.5.3a1/reflex/route.py
+-rw-r--r--   0        0        0   108928 2024-06-01 00:46:37.817959 reflex-0.5.3a1/reflex/state.py
+-rw-r--r--   0        0        0     9542 2024-05-26 21:37:48.498428 reflex-0.5.3a1/reflex/style.py
+-rw-r--r--   0        0        0    31567 2024-05-24 18:15:31.927241 reflex-0.5.3a1/reflex/testing.py
+-rw-r--r--   0        0        0       24 2023-11-09 03:24:59.510665 reflex-0.5.3a1/reflex/utils/__init__.py
+-rw-r--r--   0        0        0     8573 2024-05-23 22:07:24.099525 reflex-0.5.3a1/reflex/utils/build.py
+-rw-r--r--   0        0        0     1255 2024-05-23 22:07:24.099853 reflex-0.5.3a1/reflex/utils/compat.py
+-rw-r--r--   0        0        0     5182 2024-05-23 22:07:24.100141 reflex-0.5.3a1/reflex/utils/console.py
+-rw-r--r--   0        0        0     2163 2024-05-23 22:07:24.100417 reflex-0.5.3a1/reflex/utils/exceptions.py
+-rw-r--r--   0        0        0    10961 2024-06-01 00:46:37.821149 reflex-0.5.3a1/reflex/utils/exec.py
+-rw-r--r--   0        0        0     2270 2024-05-23 22:07:24.100962 reflex-0.5.3a1/reflex/utils/export.py
+-rw-r--r--   0        0        0    25149 2024-05-23 22:07:24.101499 reflex-0.5.3a1/reflex/utils/format.py
+-rw-r--r--   0        0        0     2309 2024-05-23 22:07:24.101709 reflex-0.5.3a1/reflex/utils/imports.py
+-rw-r--r--   0        0        0     1281 2024-06-01 00:46:37.821241 reflex-0.5.3a1/reflex/utils/lazy_loader.py
+-rw-r--r--   0        0        0     4737 2024-05-23 22:07:24.101899 reflex-0.5.3a1/reflex/utils/path_ops.py
+-rw-r--r--   0        0        0    52552 2024-06-01 00:46:37.821755 reflex-0.5.3a1/reflex/utils/prerequisites.py
+-rw-r--r--   0        0        0    11972 2024-05-23 22:07:24.102655 reflex-0.5.3a1/reflex/utils/processes.py
+-rw-r--r--   0        0        0    32709 2024-06-01 00:46:37.821935 reflex-0.5.3a1/reflex/utils/pyi_generator.py
+-rw-r--r--   0        0        0     9028 2024-06-01 00:46:37.828158 reflex-0.5.3a1/reflex/utils/serializers.py
+-rw-r--r--   0        0        0     5568 2024-05-24 16:47:17.144759 reflex-0.5.3a1/reflex/utils/telemetry.py
+-rw-r--r--   0        0        0    15152 2024-05-23 22:07:24.103627 reflex-0.5.3a1/reflex/utils/types.py
+-rw-r--r--   0        0        0     2609 2023-10-22 18:57:13.223189 reflex-0.5.3a1/reflex/utils/watch.py
+-rw-r--r--   0        0        0    72774 2024-06-01 00:46:37.828798 reflex-0.5.3a1/reflex/vars.py
+-rw-r--r--   0        0        0     6322 2024-06-01 00:46:37.828962 reflex-0.5.3a1/reflex/vars.pyi
+-rw-r--r--   0        0        0    12120 1970-01-01 00:00:00.000000 reflex-0.5.3a1/PKG-INFO
```

### Comparing `reflex-0.5.2a1/LICENSE` & `reflex-0.5.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/README.md` & `reflex-0.5.3a1/README.md`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/pyproject.toml` & `reflex-0.5.3a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reflex"
-version = "0.5.2a1"
+version = "0.5.3a1"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@reflex.dev>",
     "Alek Petuskey <alek@reflex.dev>",
     "Masen Furer <masen@reflex.dev>",
     "Elijah Ahianyo <elijah@reflex.dev>",
@@ -59,14 +59,15 @@
 charset-normalizer = ">=3.3.2,<4.0"
 wheel = ">=0.42.0,<1.0"
 build = ">=1.0.3,<2.0"
 setuptools = ">=69.1.1,<70.0"
 httpx = ">=0.25.1,<1.0"
 twine = ">=4.0.0,<6.0"
 tomlkit = ">=0.12.4,<1.0"
+lazy_loader = ">=0.4"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.1.2,<8.0"
 pytest-mock = ">=3.10.0,<4.0"
 pyright = ">=1.1.229,<1.1.335"
 darglint = ">=1.8.1,<2.0"
 toml = ">=0.10.2,<1.0"
```

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/blank/assets/favicon.ico` & `reflex-0.5.3a1/reflex/.templates/apps/blank/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/blank/code/blank.py` & `reflex-0.5.3a1/reflex/.templates/apps/blank/code/blank.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/demo/assets/favicon.ico` & `reflex-0.5.3a1/reflex/.templates/apps/demo/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/demo/assets/github.svg` & `reflex-0.5.3a1/reflex/.templates/apps/demo/assets/github.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/demo/assets/icon.svg` & `reflex-0.5.3a1/reflex/.templates/apps/demo/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/demo/assets/logo.svg` & `reflex-0.5.3a1/reflex/.templates/apps/demo/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/demo/assets/paneleft.svg` & `reflex-0.5.3a1/reflex/.templates/apps/demo/assets/paneleft.svg`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/demo/code/demo.py` & `reflex-0.5.3a1/reflex/.templates/apps/demo/code/demo.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/demo/code/pages/chatapp.py` & `reflex-0.5.3a1/reflex/.templates/apps/demo/code/pages/chatapp.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/demo/code/pages/datatable.py` & `reflex-0.5.3a1/reflex/.templates/apps/demo/code/pages/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/demo/code/pages/forms.py` & `reflex-0.5.3a1/reflex/.templates/apps/demo/code/pages/forms.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/demo/code/pages/graphing.py` & `reflex-0.5.3a1/reflex/.templates/apps/demo/code/pages/graphing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/demo/code/pages/home.py` & `reflex-0.5.3a1/reflex/.templates/apps/demo/code/pages/home.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/demo/code/sidebar.py` & `reflex-0.5.3a1/reflex/.templates/apps/demo/code/sidebar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/demo/code/states/form_state.py` & `reflex-0.5.3a1/reflex/.templates/apps/demo/code/states/form_state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/demo/code/states/pie_state.py` & `reflex-0.5.3a1/reflex/.templates/apps/demo/code/states/pie_state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/demo/code/styles.py` & `reflex-0.5.3a1/reflex/.templates/apps/demo/code/styles.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/components/chat.py` & `reflex-0.5.3a1/reflex/.templates/apps/demo/code/webui/components/chat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/components/loading_icon.py` & `reflex-0.5.3a1/reflex/.templates/apps/demo/code/webui/components/loading_icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/components/modal.py` & `reflex-0.5.3a1/reflex/.templates/apps/demo/code/webui/components/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/components/navbar.py` & `reflex-0.5.3a1/reflex/.templates/apps/demo/code/webui/components/navbar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/components/sidebar.py` & `reflex-0.5.3a1/reflex/.templates/apps/demo/code/webui/components/sidebar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/state.py` & `reflex-0.5.3a1/reflex/.templates/apps/demo/code/webui/state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/apps/demo/code/webui/styles.py` & `reflex-0.5.3a1/reflex/.templates/apps/demo/code/webui/styles.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/jinja/custom_components/demo_app.py.jinja2` & `reflex-0.5.3a1/reflex/.templates/jinja/custom_components/demo_app.py.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2` & `reflex-0.5.3a1/reflex/.templates/jinja/custom_components/pyproject.toml.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/jinja/custom_components/src.py.jinja2` & `reflex-0.5.3a1/reflex/.templates/jinja/custom_components/src.py.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/jinja/web/package.json.jinja2` & `reflex-0.5.3a1/reflex/.templates/jinja/web/package.json.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/jinja/web/pages/_app.js.jinja2` & `reflex-0.5.3a1/reflex/.templates/jinja/web/pages/_app.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2` & `reflex-0.5.3a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/jinja/web/pages/utils.js.jinja2` & `reflex-0.5.3a1/reflex/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/jinja/web/tailwind.config.js.jinja2` & `reflex-0.5.3a1/reflex/.templates/jinja/web/tailwind.config.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/jinja/web/utils/context.js.jinja2` & `reflex-0.5.3a1/reflex/.templates/jinja/web/utils/context.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js` & `reflex-0.5.3a1/reflex/.templates/web/components/reflex/chakra_color_mode_provider.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js` & `reflex-0.5.3a1/reflex/.templates/web/components/reflex/radix_themes_color_mode_provider.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/web/utils/client_side_routing.js` & `reflex-0.5.3a1/reflex/.templates/web/utils/client_side_routing.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/web/utils/helpers/dataeditor.js` & `reflex-0.5.3a1/reflex/.templates/web/utils/helpers/dataeditor.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/web/utils/helpers/debounce.js` & `reflex-0.5.3a1/reflex/.templates/web/utils/helpers/debounce.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/web/utils/helpers/range.js` & `reflex-0.5.3a1/reflex/.templates/web/utils/helpers/range.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/web/utils/helpers/throttle.js` & `reflex-0.5.3a1/reflex/.templates/web/utils/helpers/throttle.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/.templates/web/utils/state.js` & `reflex-0.5.3a1/reflex/.templates/web/utils/state.js`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/app.py` & `reflex-0.5.3a1/reflex/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 from reflex.components.base.app_wrap import AppWrap
 from reflex.components.base.fragment import Fragment
 from reflex.components.component import (
     Component,
     ComponentStyle,
     evaluate_style_namespaces,
 )
-from reflex.components.core import connection_pulser, connection_toaster
+from reflex.components.core.banner import connection_pulser, connection_toaster
 from reflex.components.core.client_side_routing import (
     Default404Page,
     wait_for_client_redirect,
 )
 from reflex.components.core.upload import Upload, get_upload_dir
 from reflex.components.radix import themes
 from reflex.config import get_config
@@ -1298,14 +1298,20 @@
 
 class EventNamespace(AsyncNamespace):
     """The event namespace."""
 
     # The application object.
     app: App
 
+    # Keep a mapping between socket ID and client token.
+    token_to_sid: dict[str, str] = {}
+
+    # Keep a mapping between client token and socket ID.
+    sid_to_token: dict[str, str] = {}
+
     def __init__(self, namespace: str, app: App):
         """Initialize the event namespace.
 
         Args:
             namespace: The namespace.
             app: The application object.
         """
@@ -1323,15 +1329,17 @@
 
     def on_disconnect(self, sid):
         """Event for when the websocket disconnects.
 
         Args:
             sid: The Socket.IO session id.
         """
-        pass
+        disconnect_token = self.sid_to_token.pop(sid, None)
+        if disconnect_token:
+            self.token_to_sid.pop(disconnect_token, None)
 
     async def emit_update(self, update: StateUpdate, sid: str) -> None:
         """Emit an update to the client.
 
         Args:
             update: The state update to send.
             sid: The Socket.IO session id.
@@ -1347,14 +1355,17 @@
         Args:
             sid: The Socket.IO session id.
             data: The event data.
         """
         # Get the event.
         event = Event.parse_raw(data)
 
+        self.token_to_sid[event.token] = sid
+        self.sid_to_token[sid] = event.token
+
         # Get the event environment.
         assert self.app.sio is not None
         environ = self.app.sio.get_environ(sid, self.namespace)
         assert environ is not None
 
         # Get the client headers.
         headers = {
```

### Comparing `reflex-0.5.2a1/reflex/app_module_for_backend.py` & `reflex-0.5.3a1/reflex/app_module_for_backend.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/base.py` & `reflex-0.5.3a1/reflex/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/compiler/compiler.py` & `reflex-0.5.3a1/reflex/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/compiler/templates.py` & `reflex-0.5.3a1/reflex/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/compiler/utils.py` & `reflex-0.5.3a1/reflex/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/base/app_wrap.py` & `reflex-0.5.3a1/reflex/components/base/app_wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/base/app_wrap.pyi` & `reflex-0.5.3a1/reflex/components/base/app_wrap.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/base/bare.py` & `reflex-0.5.3a1/reflex/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/base/body.pyi` & `reflex-0.5.3a1/reflex/components/base/body.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/base/document.py` & `reflex-0.5.3a1/reflex/components/base/document.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/base/document.pyi` & `reflex-0.5.3a1/reflex/components/base/document.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/base/fragment.pyi` & `reflex-0.5.3a1/reflex/components/base/fragment.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -80,7 +80,9 @@
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
         """
         ...
+
+fragment = Fragment.create
```

### Comparing `reflex-0.5.2a1/reflex/components/base/head.pyi` & `reflex-0.5.3a1/reflex/components/base/head.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -156,7 +156,9 @@
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The memoization leaf
         """
         ...
+
+head = Head.create
```

### Comparing `reflex-0.5.2a1/reflex/components/base/link.py` & `reflex-0.5.3a1/reflex/components/base/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/base/link.pyi` & `reflex-0.5.3a1/reflex/components/base/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/base/meta.py` & `reflex-0.5.3a1/reflex/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/base/meta.pyi` & `reflex-0.5.3a1/reflex/components/base/meta.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/base/script.py` & `reflex-0.5.3a1/reflex/components/base/script.py`

 * *Files 9% similar despite different names*

```diff
@@ -66,7 +66,10 @@
         """
         return {
             **super().get_event_triggers(),
             "on_load": lambda: [],
             "on_ready": lambda: [],
             "on_error": lambda: [],
         }
+
+
+script = Script.create
```

### Comparing `reflex-0.5.2a1/reflex/components/base/script.pyi` & `reflex-0.5.3a1/reflex/components/base/script.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -109,7 +109,9 @@
             The component.
 
         Raises:
             ValueError: when neither children nor `src` are specified.
         """
         ...
     def get_event_triggers(self) -> dict[str, Union[Var, Any]]: ...
+
+script = Script.create
```

### Comparing `reflex-0.5.2a1/reflex/components/chakra/__init__.py` & `reflex-0.5.3a1/reflex/components/chakra/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/base.py` & `reflex-0.5.3a1/reflex/components/chakra/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/base.pyi` & `reflex-0.5.3a1/reflex/components/chakra/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/datadisplay/badge.pyi` & `reflex-0.5.3a1/reflex/components/chakra/datadisplay/badge.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/datadisplay/code.pyi` & `reflex-0.5.3a1/reflex/components/chakra/datadisplay/code.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/datadisplay/divider.py` & `reflex-0.5.3a1/reflex/components/chakra/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/datadisplay/divider.pyi` & `reflex-0.5.3a1/reflex/components/chakra/datadisplay/divider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/datadisplay/keyboard_key.pyi` & `reflex-0.5.3a1/reflex/components/chakra/datadisplay/keyboard_key.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/datadisplay/list.py` & `reflex-0.5.3a1/reflex/components/chakra/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/datadisplay/list.pyi` & `reflex-0.5.3a1/reflex/components/chakra/datadisplay/list.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/datadisplay/stat.py` & `reflex-0.5.3a1/reflex/components/chakra/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/datadisplay/stat.pyi` & `reflex-0.5.3a1/reflex/components/chakra/datadisplay/stat.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/datadisplay/table.py` & `reflex-0.5.3a1/reflex/components/chakra/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/datadisplay/table.pyi` & `reflex-0.5.3a1/reflex/components/chakra/datadisplay/table.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/datadisplay/tag.py` & `reflex-0.5.3a1/reflex/components/chakra/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/datadisplay/tag.pyi` & `reflex-0.5.3a1/reflex/components/chakra/datadisplay/tag.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/disclosure/accordion.py` & `reflex-0.5.3a1/reflex/components/chakra/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/disclosure/accordion.pyi` & `reflex-0.5.3a1/reflex/components/chakra/disclosure/accordion.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/disclosure/tabs.py` & `reflex-0.5.3a1/reflex/components/chakra/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/disclosure/tabs.pyi` & `reflex-0.5.3a1/reflex/components/chakra/disclosure/tabs.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/disclosure/transition.py` & `reflex-0.5.3a1/reflex/components/chakra/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/disclosure/transition.pyi` & `reflex-0.5.3a1/reflex/components/chakra/disclosure/transition.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/disclosure/visuallyhidden.pyi` & `reflex-0.5.3a1/reflex/components/chakra/disclosure/visuallyhidden.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/feedback/alert.py` & `reflex-0.5.3a1/reflex/components/chakra/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/feedback/alert.pyi` & `reflex-0.5.3a1/reflex/components/chakra/feedback/alert.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/feedback/circularprogress.py` & `reflex-0.5.3a1/reflex/components/chakra/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/feedback/circularprogress.pyi` & `reflex-0.5.3a1/reflex/components/chakra/feedback/circularprogress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/feedback/progress.py` & `reflex-0.5.3a1/reflex/components/chakra/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/feedback/progress.pyi` & `reflex-0.5.3a1/reflex/components/chakra/feedback/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/feedback/skeleton.py` & `reflex-0.5.3a1/reflex/components/chakra/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/feedback/skeleton.pyi` & `reflex-0.5.3a1/reflex/components/chakra/feedback/skeleton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/feedback/spinner.py` & `reflex-0.5.3a1/reflex/components/chakra/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/feedback/spinner.pyi` & `reflex-0.5.3a1/reflex/components/chakra/feedback/spinner.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/__init__.py` & `reflex-0.5.3a1/reflex/components/chakra/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/button.py` & `reflex-0.5.3a1/reflex/components/chakra/forms/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/button.pyi` & `reflex-0.5.3a1/reflex/components/chakra/forms/button.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/checkbox.py` & `reflex-0.5.3a1/reflex/components/chakra/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/checkbox.pyi` & `reflex-0.5.3a1/reflex/components/chakra/forms/checkbox.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/colormodeswitch.py` & `reflex-0.5.3a1/reflex/components/chakra/forms/colormodeswitch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/colormodeswitch.pyi` & `reflex-0.5.3a1/reflex/components/chakra/forms/colormodeswitch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/date_picker.pyi` & `reflex-0.5.3a1/reflex/components/chakra/forms/date_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/date_time_picker.pyi` & `reflex-0.5.3a1/reflex/components/chakra/forms/date_time_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/editable.py` & `reflex-0.5.3a1/reflex/components/chakra/forms/editable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/editable.pyi` & `reflex-0.5.3a1/reflex/components/chakra/forms/editable.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/email.pyi` & `reflex-0.5.3a1/reflex/components/chakra/forms/email.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/form.py` & `reflex-0.5.3a1/reflex/components/chakra/forms/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/form.pyi` & `reflex-0.5.3a1/reflex/components/chakra/forms/form.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/iconbutton.py` & `reflex-0.5.3a1/reflex/components/chakra/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/iconbutton.pyi` & `reflex-0.5.3a1/reflex/components/chakra/forms/iconbutton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/input.py` & `reflex-0.5.3a1/reflex/components/chakra/forms/input.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/input.pyi` & `reflex-0.5.3a1/reflex/components/chakra/forms/input.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/multiselect.py` & `reflex-0.5.3a1/reflex/components/chakra/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/numberinput.py` & `reflex-0.5.3a1/reflex/components/chakra/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/numberinput.pyi` & `reflex-0.5.3a1/reflex/components/chakra/forms/numberinput.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/password.pyi` & `reflex-0.5.3a1/reflex/components/chakra/forms/password.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/pininput.py` & `reflex-0.5.3a1/reflex/components/chakra/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/pininput.pyi` & `reflex-0.5.3a1/reflex/components/chakra/forms/pininput.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/radio.py` & `reflex-0.5.3a1/reflex/components/chakra/forms/radio.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/radio.pyi` & `reflex-0.5.3a1/reflex/components/chakra/forms/radio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/rangeslider.py` & `reflex-0.5.3a1/reflex/components/chakra/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/rangeslider.pyi` & `reflex-0.5.3a1/reflex/components/chakra/forms/rangeslider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/select.py` & `reflex-0.5.3a1/reflex/components/chakra/forms/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/select.pyi` & `reflex-0.5.3a1/reflex/components/chakra/forms/select.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/slider.py` & `reflex-0.5.3a1/reflex/components/chakra/forms/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/slider.pyi` & `reflex-0.5.3a1/reflex/components/chakra/forms/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/switch.py` & `reflex-0.5.3a1/reflex/components/chakra/forms/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/switch.pyi` & `reflex-0.5.3a1/reflex/components/chakra/forms/switch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/textarea.py` & `reflex-0.5.3a1/reflex/components/chakra/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/textarea.pyi` & `reflex-0.5.3a1/reflex/components/chakra/forms/textarea.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/forms/time_picker.pyi` & `reflex-0.5.3a1/reflex/components/chakra/forms/time_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/layout/aspect_ratio.pyi` & `reflex-0.5.3a1/reflex/components/chakra/layout/aspect_ratio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/layout/box.py` & `reflex-0.5.3a1/reflex/components/chakra/layout/box.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/layout/box.pyi` & `reflex-0.5.3a1/reflex/components/chakra/layout/box.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/layout/card.py` & `reflex-0.5.3a1/reflex/components/chakra/layout/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/layout/card.pyi` & `reflex-0.5.3a1/reflex/components/chakra/layout/card.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/layout/center.pyi` & `reflex-0.5.3a1/reflex/components/chakra/layout/center.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/layout/container.pyi` & `reflex-0.5.3a1/reflex/components/chakra/layout/container.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/layout/flex.py` & `reflex-0.5.3a1/reflex/components/chakra/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/layout/flex.pyi` & `reflex-0.5.3a1/reflex/components/chakra/layout/flex.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/layout/grid.py` & `reflex-0.5.3a1/reflex/components/chakra/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/layout/grid.pyi` & `reflex-0.5.3a1/reflex/components/chakra/layout/grid.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/layout/spacer.pyi` & `reflex-0.5.3a1/reflex/components/chakra/layout/spacer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/layout/stack.py` & `reflex-0.5.3a1/reflex/components/chakra/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/layout/stack.pyi` & `reflex-0.5.3a1/reflex/components/chakra/layout/stack.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/layout/wrap.py` & `reflex-0.5.3a1/reflex/components/chakra/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/layout/wrap.pyi` & `reflex-0.5.3a1/reflex/components/chakra/layout/wrap.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/media/avatar.py` & `reflex-0.5.3a1/reflex/components/chakra/media/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/media/avatar.pyi` & `reflex-0.5.3a1/reflex/components/chakra/media/avatar.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/media/icon.py` & `reflex-0.5.3a1/reflex/components/chakra/media/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/media/icon.pyi` & `reflex-0.5.3a1/reflex/components/chakra/media/icon.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/media/image.py` & `reflex-0.5.3a1/reflex/components/chakra/media/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/media/image.pyi` & `reflex-0.5.3a1/reflex/components/chakra/media/image.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/navigation/breadcrumb.py` & `reflex-0.5.3a1/reflex/components/chakra/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/navigation/breadcrumb.pyi` & `reflex-0.5.3a1/reflex/components/chakra/navigation/breadcrumb.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/navigation/link.py` & `reflex-0.5.3a1/reflex/components/chakra/navigation/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/navigation/link.pyi` & `reflex-0.5.3a1/reflex/components/chakra/navigation/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/navigation/linkoverlay.py` & `reflex-0.5.3a1/reflex/components/chakra/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/navigation/linkoverlay.pyi` & `reflex-0.5.3a1/reflex/components/chakra/navigation/linkoverlay.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/navigation/stepper.py` & `reflex-0.5.3a1/reflex/components/chakra/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/navigation/stepper.pyi` & `reflex-0.5.3a1/reflex/components/chakra/navigation/stepper.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/overlay/__init__.py` & `reflex-0.5.3a1/reflex/components/chakra/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/overlay/alertdialog.py` & `reflex-0.5.3a1/reflex/components/chakra/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/overlay/alertdialog.pyi` & `reflex-0.5.3a1/reflex/components/chakra/overlay/alertdialog.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/overlay/drawer.py` & `reflex-0.5.3a1/reflex/components/chakra/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/overlay/drawer.pyi` & `reflex-0.5.3a1/reflex/components/chakra/overlay/drawer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/overlay/menu.py` & `reflex-0.5.3a1/reflex/components/chakra/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/overlay/menu.pyi` & `reflex-0.5.3a1/reflex/components/chakra/overlay/menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/overlay/modal.py` & `reflex-0.5.3a1/reflex/components/chakra/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/overlay/modal.pyi` & `reflex-0.5.3a1/reflex/components/chakra/overlay/modal.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/overlay/popover.py` & `reflex-0.5.3a1/reflex/components/chakra/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/overlay/popover.pyi` & `reflex-0.5.3a1/reflex/components/chakra/overlay/popover.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/overlay/tooltip.py` & `reflex-0.5.3a1/reflex/components/chakra/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/overlay/tooltip.pyi` & `reflex-0.5.3a1/reflex/components/chakra/overlay/tooltip.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/typography/heading.pyi` & `reflex-0.5.3a1/reflex/components/chakra/typography/heading.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/typography/highlight.py` & `reflex-0.5.3a1/reflex/components/chakra/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/typography/highlight.pyi` & `reflex-0.5.3a1/reflex/components/chakra/typography/highlight.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/typography/span.pyi` & `reflex-0.5.3a1/reflex/components/chakra/typography/span.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/chakra/typography/text.pyi` & `reflex-0.5.3a1/reflex/components/chakra/typography/text.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/component.py` & `reflex-0.5.3a1/reflex/components/component.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/core/banner.py` & `reflex-0.5.3a1/reflex/components/core/banner.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from reflex.components.el.elements.typography import Div
 from reflex.components.lucide.icon import Icon
 from reflex.components.radix.themes.components.dialog import (
     DialogContent,
     DialogRoot,
     DialogTitle,
 )
-from reflex.components.radix.themes.layout import Flex
+from reflex.components.radix.themes.layout.flex import Flex
 from reflex.components.radix.themes.typography.text import Text
 from reflex.components.sonner.toast import Toaster, ToastProps
 from reflex.constants import Dirs, Hooks, Imports
 from reflex.constants.compiler import CompileVars
 from reflex.utils import imports
 from reflex.utils.serializers import serialize
 from reflex.vars import Var, VarData
@@ -274,7 +274,13 @@
                 WifiOffPulse.create(**props),
             ),
             title=f"Connection Error: {connection_error}",
             position="fixed",
             width="100vw",
             height="0",
         )
+
+
+connection_banner = ConnectionBanner.create
+connection_modal = ConnectionModal.create
+connection_toaster = ConnectionToaster.create
+connection_pulser = ConnectionPulser.create
```

### Comparing `reflex-0.5.2a1/reflex/components/core/banner.pyi` & `reflex-0.5.3a1/reflex/components/core/banner.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from reflex.components.el.elements.typography import Div
 from reflex.components.lucide.icon import Icon
 from reflex.components.radix.themes.components.dialog import (
     DialogContent,
     DialogRoot,
     DialogTitle,
 )
-from reflex.components.radix.themes.layout import Flex
+from reflex.components.radix.themes.layout.flex import Flex
 from reflex.components.radix.themes.typography.text import Text
 from reflex.components.sonner.toast import Toaster, ToastProps
 from reflex.constants import Dirs, Hooks, Imports
 from reflex.constants.compiler import CompileVars
 from reflex.utils import imports
 from reflex.utils.serializers import serialize
 from reflex.vars import Var, VarData
@@ -570,7 +570,12 @@
             custom_attrs: custom attribute
             **props: The properties of the component.
 
         Returns:
             The connection pulser component.
         """
         ...
+
+connection_banner = ConnectionBanner.create
+connection_modal = ConnectionModal.create
+connection_toaster = ConnectionToaster.create
+connection_pulser = ConnectionPulser.create
```

### Comparing `reflex-0.5.2a1/reflex/components/core/client_side_routing.py` & `reflex-0.5.3a1/reflex/components/core/client_side_routing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/core/client_side_routing.pyi` & `reflex-0.5.3a1/reflex/components/core/client_side_routing.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/core/colors.py` & `reflex-0.5.3a1/reflex/components/core/colors.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/core/cond.py` & `reflex-0.5.3a1/reflex/components/core/cond.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/core/debounce.py` & `reflex-0.5.3a1/reflex/components/core/debounce.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,7 +132,10 @@
         return {
             **super().get_event_triggers(),
             EventTriggers.ON_CHANGE: lambda e0: [e0.value],
         }
 
     def _render(self):
         return super()._render().remove_props("ref")
+
+
+debounce_input = DebounceInput.create
```

### Comparing `reflex-0.5.2a1/reflex/components/core/debounce.pyi` & `reflex-0.5.3a1/reflex/components/core/debounce.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -102,7 +102,9 @@
 
         Raises:
             RuntimeError: unless exactly one child element is provided.
             ValueError: if the child element does not have an on_change handler.
         """
         ...
     def get_event_triggers(self) -> dict[str, Any]: ...
+
+debounce_input = DebounceInput.create
```

### Comparing `reflex-0.5.2a1/reflex/components/core/foreach.py` & `reflex-0.5.3a1/reflex/components/core/foreach.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,7 +135,10 @@
         return dict(
             tag,
             iterable_state=tag.iterable._var_full_name,
             arg_name=tag.arg_var_name,
             arg_index=tag.get_index_var_arg(),
             iterable_type=tag.iterable._var_type.mro()[0].__name__,
         )
+
+
+foreach = Foreach.create
```

### Comparing `reflex-0.5.2a1/reflex/components/core/html.py` & `reflex-0.5.3a1/reflex/components/core/html.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,7 +39,10 @@
         given_class_name = props.pop("class_name", [])
         if isinstance(given_class_name, str):
             given_class_name = [given_class_name]
         props["class_name"] = ["rx-Html", *given_class_name]
 
         # Create the component.
         return super().create(**props)
+
+
+html = Html.create
```

### Comparing `reflex-0.5.2a1/reflex/components/core/html.pyi` & `reflex-0.5.3a1/reflex/components/core/html.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -145,7 +145,9 @@
         Returns:
             The html component.
 
         Raises:
             ValueError: If children are not provided or more than one child is provided.
         """
         ...
+
+html = Html.create
```

### Comparing `reflex-0.5.2a1/reflex/components/core/match.py` & `reflex-0.5.3a1/reflex/components/core/match.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,7 +269,10 @@
         return dict(tag)
 
     def _get_imports(self) -> imports.ImportDict:
         return imports.merge_imports(
             super()._get_imports(),
             getattr(self.cond._var_data, "imports", {}),
         )
+
+
+match = Match.create
```

### Comparing `reflex-0.5.2a1/reflex/components/core/responsive.py` & `reflex-0.5.3a1/reflex/components/core/responsive.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Responsive components."""
 
-from reflex.components.radix.themes.layout import Box
+from reflex.components.radix.themes.layout.box import Box
 
 
 # Add responsive styles shortcuts.
 def mobile_only(*children, **props):
     """Create a component that is only visible on mobile.
 
     Args:
```

### Comparing `reflex-0.5.2a1/reflex/components/core/upload.py` & `reflex-0.5.3a1/reflex/components/core/upload.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from __future__ import annotations
 
 import os
 from pathlib import Path
 from typing import Any, Callable, ClassVar, Dict, List, Optional, Union
 
 from reflex import constants
-from reflex.components.chakra.forms.input import Input
-from reflex.components.chakra.layout.box import Box
 from reflex.components.component import Component, ComponentNamespace, MemoizationLeaf
+from reflex.components.el.elements.forms import Input
+from reflex.components.radix.themes.layout.box import Box
 from reflex.constants import Dirs
 from reflex.event import (
     CallableEventSpec,
     EventChain,
     EventSpec,
     call_event_fn,
     call_script,
@@ -335,7 +335,10 @@
 
 
 class UploadNamespace(ComponentNamespace):
     """Upload component namespace."""
 
     root = Upload.create
     __call__ = StyledUpload.create
+
+
+upload = UploadNamespace()
```

### Comparing `reflex-0.5.2a1/reflex/components/core/upload.pyi` & `reflex-0.5.3a1/reflex/components/core/upload.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 import os
 from pathlib import Path
 from typing import Any, Callable, ClassVar, Dict, List, Optional, Union
 from reflex import constants
-from reflex.components.chakra.forms.input import Input
-from reflex.components.chakra.layout.box import Box
 from reflex.components.component import Component, ComponentNamespace, MemoizationLeaf
+from reflex.components.el.elements.forms import Input
+from reflex.components.radix.themes.layout.box import Box
 from reflex.constants import Dirs
 from reflex.event import (
     CallableEventSpec,
     EventChain,
     EventSpec,
     call_event_fn,
     call_script,
@@ -413,7 +413,9 @@
             custom_attrs: custom attribute
             **props: The properties of the component.
 
         Returns:
             The styled upload component.
         """
         ...
+
+upload = UploadNamespace()
```

### Comparing `reflex-0.5.2a1/reflex/components/datadisplay/code.py` & `reflex-0.5.3a1/reflex/components/datadisplay/code.py`

 * *Files 1% similar despite different names*

```diff
@@ -519,7 +519,10 @@
 
         Returns:
             The right theme name.
         """
         if theme in ["light", "dark"]:
             return f"one-{theme}"
         return theme
+
+
+code_block = CodeBlock.create
```

### Comparing `reflex-0.5.2a1/reflex/components/datadisplay/code.pyi` & `reflex-0.5.3a1/reflex/components/datadisplay/code.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1110,7 +1110,9 @@
         Returns:
             The text component.
         """
         ...
     def add_style(self): ...
     @staticmethod
     def convert_theme_name(theme) -> str: ...
+
+code_block = CodeBlock.create
```

### Comparing `reflex-0.5.2a1/reflex/components/datadisplay/dataeditor.py` & `reflex-0.5.3a1/reflex/components/datadisplay/dataeditor.py`

 * *Files 2% similar despite different names*

```diff
@@ -406,7 +406,11 @@
 
     Returns:
         The serialized theme.
     """
     return format.json_dumps(
         {format.to_camel_case(k): v for k, v in theme.__dict__.items() if v is not None}
     )
+
+
+data_editor = DataEditor.create
+data_editor_theme = DataEditorTheme
```

### Comparing `reflex-0.5.2a1/reflex/components/datadisplay/dataeditor.pyi` & `reflex-0.5.3a1/reflex/components/datadisplay/dataeditor.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -232,7 +232,10 @@
         Returns:
             The DataEditor component.&
         """
         ...
 
 @serializer
 def serialize_dataeditortheme(theme: DataEditorTheme): ...
+
+data_editor = DataEditor.create
+data_editor_theme = DataEditorTheme
```

### Comparing `reflex-0.5.2a1/reflex/components/datadisplay/logo.py` & `reflex-0.5.3a1/reflex/components/datadisplay/logo.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/el/constants/html.py` & `reflex-0.5.3a1/reflex/components/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/el/constants/react.py` & `reflex-0.5.3a1/reflex/components/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/el/constants/reflex.py` & `reflex-0.5.3a1/reflex/components/el/constants/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/el/element.pyi` & `reflex-0.5.3a1/reflex/components/el/element.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/el/elements/base.py` & `reflex-0.5.3a1/reflex/components/el/elements/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/el/elements/base.pyi` & `reflex-0.5.3a1/reflex/components/el/elements/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/el/elements/forms.py` & `reflex-0.5.3a1/reflex/components/el/elements/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -646,7 +646,22 @@
             **super().get_event_triggers(),
             EventTriggers.ON_CHANGE: lambda e0: [e0.target.value],
             EventTriggers.ON_FOCUS: lambda e0: [e0.target.value],
             EventTriggers.ON_BLUR: lambda e0: [e0.target.value],
             EventTriggers.ON_KEY_DOWN: lambda e0: [e0.key],
             EventTriggers.ON_KEY_UP: lambda e0: [e0.key],
         }
+
+
+button = Button.create
+fieldset = Fieldset.create
+form = Form.create
+input = Input.create
+label = Label.create
+legend = Legend.create
+meter = Meter.create
+optgroup = Optgroup.create
+option = Option.create
+output = Output.create
+progress = Progress.create
+select = Select.create
+textarea = Textarea.create
```

### Comparing `reflex-0.5.2a1/reflex/components/el/elements/forms.pyi` & `reflex-0.5.3a1/reflex/components/el/elements/forms.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2176,7 +2176,21 @@
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
         """
         ...
+
+button = Button.create
+fieldset = Fieldset.create
+form = Form.create
+input = Input.create
+label = Label.create
+legend = Legend.create
+meter = Meter.create
+optgroup = Optgroup.create
+option = Option.create
+output = Output.create
+progress = Progress.create
+select = Select.create
+textarea = Textarea.create
```

### Comparing `reflex-0.5.2a1/reflex/components/el/elements/inline.py` & `reflex-0.5.3a1/reflex/components/el/elements/inline.py`

 * *Files 17% similar despite different names*

```diff
@@ -204,7 +204,37 @@
     tag = "u"
 
 
 class Wbr(BaseHTML):
     """Display the wbr element."""
 
     tag = "wbr"
+
+
+a = A.create
+abbr = Abbr.create
+b = B.create
+bdi = Bdi.create
+bdo = Bdo.create
+br = Br.create
+cite = Cite.create
+code = Code.create
+data = Data.create
+dfn = Dfn.create
+em = Em.create
+i = I.create
+kbd = Kbd.create
+mark = Mark.create
+q = Q.create
+rp = Rp.create
+rt = Rt.create
+ruby = Ruby.create
+s = S.create
+samp = Samp.create
+small = Small.create
+span = Span.create
+strong = Strong.create
+sub = Sub.create
+sup = Sup.create
+time = Time.create
+u = U.create
+wbr = Wbr.create
```

### Comparing `reflex-0.5.2a1/reflex/components/el/elements/inline.pyi` & `reflex-0.5.3a1/reflex/components/el/elements/inline.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -3742,7 +3742,36 @@
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
         """
         ...
+
+a = A.create
+abbr = Abbr.create
+b = B.create
+bdi = Bdi.create
+bdo = Bdo.create
+br = Br.create
+cite = Cite.create
+code = Code.create
+data = Data.create
+dfn = Dfn.create
+em = Em.create
+i = I.create
+kbd = Kbd.create
+mark = Mark.create
+q = Q.create
+rp = Rp.create
+rt = Rt.create
+ruby = Ruby.create
+s = S.create
+samp = Samp.create
+small = Small.create
+span = Span.create
+strong = Strong.create
+sub = Sub.create
+sup = Sup.create
+time = Time.create
+u = U.create
+wbr = Wbr.create
```

### Comparing `reflex-0.5.2a1/reflex/components/el/elements/media.py` & `reflex-0.5.3a1/reflex/components/el/elements/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,7 +312,23 @@
 class Path(BaseHTML):
     """Display the path element."""
 
     tag = "path"
 
     # Defines the shape of the path
     d: Var[Union[str, int, bool]]
+
+
+area = Area.create
+audio = Audio.create
+image = img = Img.create
+map = Map.create
+track = Track.create
+video = Video.create
+embed = Embed.create
+iframe = Iframe.create
+object = Object.create
+picture = Picture.create
+portal = Portal.create
+source = Source.create
+svg = Svg.create
+path = Path.create
```

### Comparing `reflex-0.5.2a1/reflex/components/el/elements/media.pyi` & `reflex-0.5.3a1/reflex/components/el/elements/media.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2082,7 +2082,22 @@
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
         """
         ...
+
+area = Area.create
+audio = Audio.create
+image = img = Img.create
+map = Map.create
+track = Track.create
+video = Video.create
+embed = Embed.create
+iframe = Iframe.create
+object = Object.create
+picture = Picture.create
+portal = Portal.create
+source = Source.create
+svg = Svg.create
+path = Path.create
```

### Comparing `reflex-0.5.2a1/reflex/components/el/elements/metadata.py` & `reflex-0.5.3a1/reflex/components/el/elements/metadata.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,7 +49,14 @@
     name: Var[Union[str, int, bool]]
 
 
 class Title(Element):  # noqa: E742
     """Display the title element."""
 
     tag = "title"
+
+
+base = Base.create
+head = Head.create
+link = Link.create
+meta = Meta.create
+title = Title.create
```

### Comparing `reflex-0.5.2a1/reflex/components/el/elements/metadata.pyi` & `reflex-0.5.3a1/reflex/components/el/elements/metadata.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -646,7 +646,13 @@
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
         """
         ...
+
+base = Base.create
+head = Head.create
+link = Link.create
+meta = Meta.create
+title = Title.create
```

### Comparing `reflex-0.5.2a1/reflex/components/el/elements/other.py` & `reflex-0.5.3a1/reflex/components/el/elements/other.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,7 +55,16 @@
 class Html(BaseHTML):
     """Display the html element."""
 
     tag = "html"
 
     # Specifies the URL of the document's cache manifest (obsolete in HTML5)
     manifest: Var[Union[str, int, bool]]
+
+
+details = Details.create
+dialog = Dialog.create
+summary = Summary.create
+slot = Slot.create
+template = Template.create
+math = Math.create
+html = Html.create
```

### Comparing `reflex-0.5.2a1/reflex/components/el/elements/other.pyi` & `reflex-0.5.3a1/reflex/components/el/elements/other.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -938,7 +938,15 @@
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
         """
         ...
+
+details = Details.create
+dialog = Dialog.create
+summary = Summary.create
+slot = Slot.create
+template = Template.create
+math = Math.create
+html = Html.create
```

### Comparing `reflex-0.5.2a1/reflex/components/el/elements/scripts.py` & `reflex-0.5.3a1/reflex/components/el/elements/scripts.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,7 +46,12 @@
     referrer_policy: Var[Union[str, int, bool]]
 
     # URL of an external script
     src: Var[Union[str, int, bool]]
 
     # Specifies the MIME type of the script
     type: Var[Union[str, int, bool]]
+
+
+canvas = Canvas.create
+noscript = Noscript.create
+script = Script.create
```

### Comparing `reflex-0.5.2a1/reflex/components/el/elements/scripts.pyi` & `reflex-0.5.3a1/reflex/components/el/elements/scripts.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -434,7 +434,11 @@
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
         """
         ...
+
+canvas = Canvas.create
+noscript = Noscript.create
+script = Script.create
```

### Comparing `reflex-0.5.2a1/reflex/components/el/elements/sectioning.py` & `reflex-0.5.3a1/reflex/components/el/elements/sectioning.py`

 * *Files 17% similar despite different names*

```diff
@@ -89,7 +89,24 @@
     tag = "nav"
 
 
 class Section(BaseHTML):  # noqa: E742
     """Display the section element."""
 
     tag = "section"
+
+
+address = Address.create
+article = Article.create
+aside = Aside.create
+body = Body.create
+header = Header.create
+footer = Footer.create
+h1 = H1.create
+h2 = H2.create
+h3 = H3.create
+h4 = H4.create
+h5 = H5.create
+h6 = H6.create
+main = Main.create
+nav = Nav.create
+section = Section.create
```

### Comparing `reflex-0.5.2a1/reflex/components/el/elements/sectioning.pyi` & `reflex-0.5.3a1/reflex/components/el/elements/sectioning.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1985,7 +1985,23 @@
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
         """
         ...
+
+address = Address.create
+article = Article.create
+aside = Aside.create
+body = Body.create
+header = Header.create
+footer = Footer.create
+h1 = H1.create
+h2 = H2.create
+h3 = H3.create
+h4 = H4.create
+h5 = H5.create
+h6 = H6.create
+main = Main.create
+nav = Nav.create
+section = Section.create
```

### Comparing `reflex-0.5.2a1/reflex/components/el/elements/tables.py` & `reflex-0.5.3a1/reflex/components/el/elements/tables.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,7 +120,19 @@
 class Tr(BaseHTML):
     """Display the tr element."""
 
     tag = "tr"
 
     # Alignment of the content within the table row
     align: Var[Union[str, int, bool]]
+
+
+caption = Caption.create
+col = Col.create
+colgroup = Colgroup.create
+table = Table.create
+tbody = Tbody.create
+td = Td.create
+tfoot = Tfoot.create
+th = Th.create
+thead = Thead.create
+tr = Tr.create
```

### Comparing `reflex-0.5.2a1/reflex/components/el/elements/tables.pyi` & `reflex-0.5.3a1/reflex/components/el/elements/tables.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1402,7 +1402,18 @@
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
         """
         ...
+
+caption = Caption.create
+col = Col.create
+colgroup = Colgroup.create
+table = Table.create
+tbody = Tbody.create
+td = Td.create
+tfoot = Tfoot.create
+th = Th.create
+thead = Thead.create
+tr = Tr.create
```

### Comparing `reflex-0.5.2a1/reflex/components/el/elements/typography.py` & `reflex-0.5.3a1/reflex/components/el/elements/typography.py`

 * *Files 9% similar despite different names*

```diff
@@ -120,7 +120,23 @@
     tag = "del"
 
     # Specifies the URL of the document that explains the reason why the text was deleted.
     cite: Var[Union[str, int, bool]]
 
     # Specifies the date and time of when the text was deleted.
     date_time: Var[Union[str, int, bool]]
+
+
+blockquote = Blockquote.create
+dd = Dd.create
+div = Div.create
+dl = Dl.create
+dt = Dt.create
+figcaption = Figcaption.create
+hr = Hr.create
+li = Li.create
+ol = Ol.create
+p = P.create
+pre = Pre.create
+ul = Ul.create
+ins = Ins.create
+del_ = Del.create  # 'del' is a reserved keyword in Python
```

### Comparing `reflex-0.5.2a1/reflex/components/el/elements/typography.pyi` & `reflex-0.5.3a1/reflex/components/el/elements/typography.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2016,7 +2016,22 @@
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
         """
         ...
+
+blockquote = Blockquote.create
+dd = Dd.create
+div = Div.create
+dl = Dl.create
+dt = Dt.create
+figcaption = Figcaption.create
+hr = Hr.create
+li = Li.create
+ol = Ol.create
+p = P.create
+pre = Pre.create
+ul = Ul.create
+ins = Ins.create
+del_ = Del.create
```

### Comparing `reflex-0.5.2a1/reflex/components/gridjs/datatable.py` & `reflex-0.5.3a1/reflex/components/gridjs/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/gridjs/datatable.pyi` & `reflex-0.5.3a1/reflex/components/gridjs/datatable.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/lucide/icon.py` & `reflex-0.5.3a1/reflex/components/lucide/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/lucide/icon.pyi` & `reflex-0.5.3a1/reflex/components/lucide/icon.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/markdown/markdown.py` & `reflex-0.5.3a1/reflex/components/markdown/markdown.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/markdown/markdown.pyi` & `reflex-0.5.3a1/reflex/components/markdown/markdown.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/moment/moment.py` & `reflex-0.5.3a1/reflex/components/moment/moment.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/moment/moment.pyi` & `reflex-0.5.3a1/reflex/components/moment/moment.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/next/base.pyi` & `reflex-0.5.3a1/reflex/components/next/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/next/image.py` & `reflex-0.5.3a1/reflex/components/next/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/next/image.pyi` & `reflex-0.5.3a1/reflex/components/next/image.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/next/link.pyi` & `reflex-0.5.3a1/reflex/components/next/link.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/next/video.py` & `reflex-0.5.3a1/reflex/components/next/video.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/next/video.pyi` & `reflex-0.5.3a1/reflex/components/next/video.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/plotly/plotly.pyi` & `reflex-0.5.3a1/reflex/components/radix/primitives/base.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-"""Stub file for reflex/components/plotly/plotly.py"""
+"""Stub file for reflex/components/radix/primitives/base.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Any, Dict, List
-from reflex.components.component import NoSSRComponent
+from typing import List
+from reflex.components.component import Component
+from reflex.components.tags.tag import Tag
+from reflex.utils import format
 from reflex.vars import Var
 
-try:
-    from plotly.graph_objects import Figure  # type: ignore
-except ImportError:
-    Figure = Any  # type: ignore
-
-class PlotlyLib(NoSSRComponent):
+class RadixPrimitiveComponent(Component):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
+        as_child: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -70,44 +68,40 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "PlotlyLib":
+    ) -> "RadixPrimitiveComponent":
         """Create the component.
 
         Args:
             *children: The children of the component.
+            as_child: Change the default rendered element for the one passed as a child.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
         """
         ...
 
-class Plotly(PlotlyLib):
+class RadixPrimitiveComponentWithClassName(RadixPrimitiveComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        data: Optional[Union[Var[Figure], Figure]] = None,  # type: ignore
-        layout: Optional[Union[Var[Dict], Dict]] = None,
-        config: Optional[Union[Var[Dict], Dict]] = None,
-        width: Optional[Union[Var[str], str]] = None,
-        height: Optional[Union[Var[str], str]] = None,
-        use_resize_handler: Optional[Union[Var[bool], bool]] = None,
+        as_child: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -152,25 +146,20 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Plotly":
+    ) -> "RadixPrimitiveComponentWithClassName":
         """Create the component.
 
         Args:
             *children: The children of the component.
-            data: The figure to display. This can be a plotly figure or a plotly data json.
-            layout: The layout of the graph.
-            config: The config of the graph.
-            width: The width of the graph.
-            height: The height of the graph.
-            use_resize_handler: If true, the graph will resize when the window is resized.
+            as_child: Change the default rendered element for the one passed as a child.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
```

### Comparing `reflex-0.5.2a1/reflex/components/props.py` & `reflex-0.5.3a1/reflex/components/props.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/primitives/accordion.py` & `reflex-0.5.3a1/reflex/components/radix/primitives/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/primitives/accordion.pyi` & `reflex-0.5.3a1/reflex/components/radix/primitives/accordion.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/primitives/base.py` & `reflex-0.5.3a1/reflex/components/radix/primitives/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/primitives/base.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/card.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,107 +1,79 @@
-"""Stub file for reflex/components/radix/primitives/base.py"""
+"""Stub file for reflex/components/radix/themes/components/card.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import List
-from reflex.components.component import Component
-from reflex.components.tags.tag import Tag
-from reflex.utils import format
+from typing import Literal
+from reflex.components.el import elements
 from reflex.vars import Var
+from ..base import RadixThemesComponent
 
-class RadixPrimitiveComponent(Component):
+class Card(elements.Div, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         as_child: Optional[Union[Var[bool], bool]] = None,
-        style: Optional[Style] = None,
-        key: Optional[Any] = None,
-        id: Optional[Any] = None,
-        class_name: Optional[Any] = None,
-        autofocus: Optional[bool] = None,
-        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
-        on_blur: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        size: Optional[
+            Union[
+                Var[Literal["1", "2", "3", "4", "5"]], Literal["1", "2", "3", "4", "5"]
+            ]
         ] = None,
-        on_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        variant: Optional[
+            Union[
+                Var[Literal["surface", "classic", "ghost"]],
+                Literal["surface", "classic", "ghost"],
+            ]
         ] = None,
-        on_context_menu: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        access_key: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_double_click: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        auto_capitalize: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_focus: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        content_editable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        context_menu: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_down: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        draggable: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_enter: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        enter_key_hint: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_leave: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        hidden: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_move: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        input_mode: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_out: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        item_prop: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_over: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
+        spell_check: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_mouse_up: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
-        ] = None,
-        on_scroll: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        tab_index: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        on_unmount: Optional[
-            Union[EventHandler, EventSpec, list, function, BaseVar]
+        title: Optional[
+            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
-        **props
-    ) -> "RadixPrimitiveComponent":
-        """Create the component.
-
-        Args:
-            *children: The children of the component.
-            as_child: Change the default rendered element for the one passed as a child.
-            style: The style of the component.
-            key: A unique key for the component.
-            id: The id for the component.
-            class_name: The class name for the component.
-            autofocus: Whether the component should take the focus once the page is loaded
-            custom_attrs: custom attribute
-            **props: The props of the component.
-
-        Returns:
-            The component.
-        """
-        ...
-
-class RadixPrimitiveComponentWithClassName(RadixPrimitiveComponent):
-    @overload
-    @classmethod
-    def create(  # type: ignore
-        cls,
-        *children,
-        as_child: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_blur: Optional[
@@ -146,25 +118,48 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "RadixPrimitiveComponentWithClassName":
-        """Create the component.
+    ) -> "Card":
+        """Create a new component instance.
+
+        Will prepend "RadixThemes" to the component tag to avoid conflicts with
+        other UI libraries for common names, like Text and Button.
 
         Args:
-            *children: The children of the component.
-            as_child: Change the default rendered element for the one passed as a child.
+            *children: Child components.
+            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior.
+            size: Card size: "1" - "5"
+            variant: Variant of Card: "solid" | "soft" | "outline" | "ghost"
+            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
+            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
+            content_editable: Indicates whether the element's content is editable.
+            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
+            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
+            draggable: Defines whether the element can be dragged.
+            enter_key_hint: Hints what media types the media element is able to play.
+            hidden: Defines whether the element is hidden.
+            input_mode: Defines the type of the element.
+            item_prop: Defines the name of the element for metadata purposes.
+            lang: Defines the language used in the element.
+            role: Defines the role of the element.
+            slot: Assigns a slot in a shadow DOM shadow tree to an element.
+            spell_check: Defines whether the element may be checked for spelling errors.
+            tab_index: Defines the position of the current element in the tabbing order.
+            title: Defines a tooltip for the element.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: The props of the component.
+            **props: Component properties.
 
         Returns:
-            The component.
+            A new component instance.
         """
         ...
+
+card = Card.create
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/primitives/drawer.py` & `reflex-0.5.3a1/reflex/components/radix/primitives/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/primitives/drawer.pyi` & `reflex-0.5.3a1/reflex/components/radix/primitives/drawer.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/primitives/form.py` & `reflex-0.5.3a1/reflex/components/radix/primitives/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/primitives/form.pyi` & `reflex-0.5.3a1/reflex/components/radix/primitives/form.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/primitives/progress.py` & `reflex-0.5.3a1/reflex/components/radix/primitives/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/primitives/progress.pyi` & `reflex-0.5.3a1/reflex/components/radix/primitives/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/primitives/slider.py` & `reflex-0.5.3a1/reflex/components/radix/primitives/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/primitives/slider.pyi` & `reflex-0.5.3a1/reflex/components/radix/primitives/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/base.py` & `reflex-0.5.3a1/reflex/components/radix/themes/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from __future__ import annotations
 
 from typing import Any, Dict, Literal
 
 from reflex.components import Component
 from reflex.components.tags import Tag
-from reflex.utils import imports
+from reflex.config import get_config
+from reflex.utils.imports import ImportVar
 from reflex.vars import Var
 
 LiteralAlign = Literal["start", "center", "end", "baseline", "stretch"]
 LiteralJustify = Literal["start", "center", "end", "between"]
 LiteralSpacing = Literal["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"]
 LiteralVariant = Literal["classic", "solid", "soft", "surface", "outline", "ghost"]
 LiteralAppearance = Literal["inherit", "light", "dark"]
@@ -204,26 +205,31 @@
         """
         if color_mode is not None:
             props["appearance"] = color_mode
         if theme_panel:
             children = [ThemePanel.create(), *children]
         return super().create(*children, **props)
 
-    def _get_imports(self) -> imports.ImportDict:
-        return imports.merge_imports(
-            super()._get_imports(),
-            {
-                "": [
-                    imports.ImportVar(tag="@radix-ui/themes/styles.css", install=False)
-                ],
-                "/utils/theme.js": [
-                    imports.ImportVar(tag="theme", is_default=True),
-                ],
-            },
-        )
+    def add_imports(self) -> dict[str, list[ImportVar] | ImportVar]:
+        """Add imports for the Theme component.
+
+        Returns:
+            The import dict.
+        """
+        _imports: dict[str, list[ImportVar] | ImportVar] = {
+            "/utils/theme.js": [ImportVar(tag="theme", is_default=True)],
+        }
+        if get_config().tailwind is None:
+            # When tailwind is disabled, import the radix-ui styles directly because they will
+            # not be included in the tailwind.css file.
+            _imports[""] = ImportVar(
+                tag="@radix-ui/themes/styles.css",
+                install=False,
+            )
+        return _imports
 
     def _render(self, props: dict[str, Any] | None = None) -> Tag:
         tag = super()._render(props)
         tag.add_props(
             css=Var.create(
                 "{{...theme.styles.global[':root'], ...theme.styles.global.body}}",
                 _var_is_local=False,
@@ -239,21 +245,21 @@
     """
 
     tag = "ThemePanel"
 
     # Whether the panel is open. Defaults to False.
     default_open: Var[bool]
 
-    def _get_imports(self) -> dict[str, list[imports.ImportVar]]:
-        return imports.merge_imports(
-            super()._get_imports(),
-            {
-                "react": [imports.ImportVar(tag="useEffect")],
-            },
-        )
+    def add_imports(self) -> dict[str, str]:
+        """Add imports for the ThemePanel component.
+
+        Returns:
+            The import dict.
+        """
+        return {"react": "useEffect"}
 
     def _get_hooks(self) -> str | None:
         # The panel freezes the tab if the user color preference differs from the
         # theme "appearance", so clear it out when theme panel is used.
         return """
             useEffect(() => {
                 if (typeof window !== 'undefined') {
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/base.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/base.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Any, Dict, Literal
 from reflex.components import Component
 from reflex.components.tags import Tag
-from reflex.utils import imports
+from reflex.config import get_config
+from reflex.utils.imports import ImportVar
 from reflex.vars import Var
 
 LiteralAlign = Literal["start", "center", "end", "baseline", "stretch"]
 LiteralJustify = Literal["start", "center", "end", "between"]
 LiteralSpacing = Literal["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"]
 LiteralVariant = Literal["classic", "solid", "soft", "surface", "outline", "ghost"]
 LiteralAppearance = Literal["inherit", "light", "dark"]
@@ -575,16 +576,18 @@
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
+    def add_imports(self) -> dict[str, list[ImportVar] | ImportVar]: ...
 
 class ThemePanel(RadixThemesComponent):
+    def add_imports(self) -> dict[str, str]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         default_open: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/color_mode.py` & `reflex-0.5.3a1/reflex/components/radix/themes/color_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,8 +170,10 @@
     """Namespace for color mode components."""
 
     icon = staticmethod(ColorModeIcon.create)
     button = staticmethod(ColorModeIconButton.create)
     switch = staticmethod(ColorModeSwitch.create)
 
 
-color_mode_var_and_namespace = ColorModeNamespace(**dataclasses.asdict(color_mode))
+color_mode = color_mode_var_and_namespace = ColorModeNamespace(
+    **dataclasses.asdict(color_mode)
+)
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/color_mode.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/color_mode.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -539,8 +539,10 @@
         ...
 
 class ColorModeNamespace(BaseVar):
     icon = staticmethod(ColorModeIcon.create)
     button = staticmethod(ColorModeIconButton.create)
     switch = staticmethod(ColorModeSwitch.create)
 
-color_mode_var_and_namespace = ColorModeNamespace(**dataclasses.asdict(color_mode))
+color_mode = color_mode_var_and_namespace = ColorModeNamespace(
+    **dataclasses.asdict(color_mode)
+)
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/__init__.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/__init__.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,44 @@
-"""Radix themes components."""
+"""Stub file for reflex/components/radix/themes/components/__init__.py"""
+# ------------------- DO NOT EDIT ----------------------
+# This file was generated by `reflex/utils/pyi_generator.py`!
+# ------------------------------------------------------
 
 from .alert_dialog import alert_dialog as alert_dialog
 from .aspect_ratio import aspect_ratio as aspect_ratio
 from .avatar import avatar as avatar
 from .badge import badge as badge
 from .button import button as button
 from .callout import callout as callout
 from .card import card as card
 from .checkbox import checkbox as checkbox
-from .checkbox_cards import checkbox_cards as checkbox_cards
-from .checkbox_group import checkbox_group as checkbox_group
 from .context_menu import context_menu as context_menu
 from .data_list import data_list as data_list
 from .dialog import dialog as dialog
-from .dropdown_menu import dropdown_menu as dropdown_menu
-from .dropdown_menu import menu as menu
 from .hover_card import hover_card as hover_card
 from .icon_button import icon_button as icon_button
+from .text_field import input as input
 from .inset import inset as inset
 from .popover import popover as popover
-from .progress import progress as progress
-from .radio_cards import radio_cards as radio_cards
-from .radio_group import radio as radio
-from .radio_group import radio_group as radio_group
 from .scroll_area import scroll_area as scroll_area
-from .segmented_control import segmented_control as segmented_control
 from .select import select as select
-from .separator import divider as divider
-from .separator import separator as separator
 from .skeleton import skeleton as skeleton
 from .slider import slider as slider
 from .spinner import spinner as spinner
 from .switch import switch as switch
 from .table import table as table
 from .tabs import tabs as tabs
 from .text_area import text_area as text_area
-from .text_field import text_field as text_field
 from .tooltip import tooltip as tooltip
-
-input = text_field
-
-__all__ = [
-    "alert_dialog",
-    "aspect_ratio",
-    "avatar",
-    "badge",
-    "button",
-    "callout",
-    "card",
-    "checkbox",
-    "checkbox_cards",
-    "checkbox_group",
-    "context_menu",
-    "data_list",
-    "dialog",
-    "divider",
-    "dropdown_menu",
-    "hover_card",
-    "icon_button",
-    "input",
-    "inset",
-    "menu",
-    "popover",
-    # progress is in experimental namespace until https://github.com/radix-ui/themes/pull/492
-    # "progress",
-    "radio",
-    "radio_cards",
-    "radio_group",
-    "scroll_area",
-    "segmented_control",
-    "select",
-    "separator",
-    "skeleton",
-    "slider",
-    "spinner",
-    "switch",
-    "table",
-    "tabs",
-    "text_area",
-    "text_field",
-    "tooltip",
-]
+from .segmented_control import segmented_control as segmented_control
+from .radio_cards import radio_cards as radio_cards
+from .checkbox_cards import checkbox_cards as checkbox_cards
+from .checkbox_group import checkbox_group as checkbox_group
+from .text_field import text_field as text_field
+from .radio_group import radio as radio
+from .radio_group import radio_group as radio_group
+from .dropdown_menu import menu as menu
+from .dropdown_menu import dropdown_menu as dropdown_menu
+from .separator import divider as divider
+from .separator import separator as separator
+from reflex import RADIX_THEMES_COMPONENTS_MAPPING
+from reflex.utils import lazy_loader
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/alert_dialog.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/alert_dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Interactive components provided by @radix-ui/themes."""
 from typing import Any, Dict, Literal
 
-from reflex import el
 from reflex.components.component import ComponentNamespace
+from reflex.components.el import elements
 from reflex.constants import EventTriggers
 from reflex.vars import Var
 
 from ..base import RadixThemesComponent, RadixThemesTriggerComponent
 
 LiteralContentSize = Literal["1", "2", "3", "4"]
 
@@ -33,15 +33,15 @@
 
 class AlertDialogTrigger(RadixThemesTriggerComponent):
     """Wraps the control that will open the dialog."""
 
     tag = "AlertDialog.Trigger"
 
 
-class AlertDialogContent(el.Div, RadixThemesComponent):
+class AlertDialogContent(elements.Div, RadixThemesComponent):
     """Contains the content of the dialog. This component is based on the div element."""
 
     tag = "AlertDialog.Content"
 
     # The size of the content.
     size: Var[LiteralContentSize]
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/alert_dialog.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/alert_dialog.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Any, Dict, Literal
-from reflex import el
 from reflex.components.component import ComponentNamespace
+from reflex.components.el import elements
 from reflex.constants import EventTriggers
 from reflex.vars import Var
 from ..base import RadixThemesComponent, RadixThemesTriggerComponent
 
 LiteralContentSize = Literal["1", "2", "3", "4"]
 
 class AlertDialogRoot(RadixThemesComponent):
@@ -167,15 +167,15 @@
             props: The properties of the component.
 
         Returns:
             The new RadixThemesTriggerComponent instance.
         """
         ...
 
-class AlertDialogContent(el.Div, RadixThemesComponent):
+class AlertDialogContent(elements.Div, RadixThemesComponent):
     def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         size: Optional[
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/aspect_ratio.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/aspect_ratio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/avatar.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/avatar.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/avatar.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/badge.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/badge.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Interactive components provided by @radix-ui/themes."""
 
 from typing import Literal
 
-from reflex import el
+from reflex.components.el import elements
 from reflex.vars import Var
 
 from ..base import (
     LiteralAccentColor,
     LiteralRadius,
     RadixThemesComponent,
 )
 
 
-class Badge(el.Span, RadixThemesComponent):
+class Badge(elements.Span, RadixThemesComponent):
     """A stylized badge element."""
 
     tag = "Badge"
 
     # The variant of the badge
     variant: Var[Literal["solid", "soft", "surface", "outline"]]
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/badge.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/badge.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Literal
-from reflex import el
+from reflex.components.el import elements
 from reflex.vars import Var
 from ..base import LiteralAccentColor, LiteralRadius, RadixThemesComponent
 
-class Badge(el.Span, RadixThemesComponent):
+class Badge(elements.Span, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         variant: Optional[
             Union[
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/button.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/button.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Interactive components provided by @radix-ui/themes."""
 
 from typing import Literal
 
-from reflex import el
+from reflex.components.el import elements
 from reflex.vars import Var
 
 from ..base import (
     LiteralAccentColor,
     LiteralRadius,
     LiteralVariant,
     RadixLoadingProp,
     RadixThemesComponent,
 )
 
 LiteralButtonSize = Literal["1", "2", "3", "4"]
 
 
-class Button(el.Button, RadixLoadingProp, RadixThemesComponent):
+class Button(elements.Button, RadixLoadingProp, RadixThemesComponent):
     """Trigger an action or event, such as submitting a form or displaying a dialog."""
 
     tag = "Button"
 
     # Change the default rendered element for the one passed as a child, merging their props and behavior.
     as_child: Var[bool]
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/button.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/button.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Literal
-from reflex import el
+from reflex.components.el import elements
 from reflex.vars import Var
 from ..base import (
     LiteralAccentColor,
     LiteralRadius,
     LiteralVariant,
     RadixLoadingProp,
     RadixThemesComponent,
 )
 
 LiteralButtonSize = Literal["1", "2", "3", "4"]
 
-class Button(el.Button, RadixLoadingProp, RadixThemesComponent):
+class Button(elements.Button, RadixLoadingProp, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         as_child: Optional[Union[Var[bool], bool]] = None,
         size: Optional[
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/callout.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/callout.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Interactive components provided by @radix-ui/themes."""
 
 from typing import Literal, Union
 
 import reflex as rx
-from reflex import el
 from reflex.components.component import Component, ComponentNamespace
+from reflex.components.el import elements
 from reflex.components.lucide.icon import Icon
 from reflex.vars import Var
 
 from ..base import (
     LiteralAccentColor,
     RadixThemesComponent,
 )
 
 CalloutVariant = Literal["soft", "surface", "outline"]
 
 
-class CalloutRoot(el.Div, RadixThemesComponent):
+class CalloutRoot(elements.Div, RadixThemesComponent):
     """Groups Icon and Text parts of a Callout."""
 
     tag = "Callout.Root"
 
     # Change the default rendered element for the one passed as a child, merging their props and behavior.
     as_child: Var[bool]
 
@@ -33,21 +33,21 @@
     # Override theme color for button
     color_scheme: Var[LiteralAccentColor]
 
     # Whether to render the button with higher contrast color against background
     high_contrast: Var[bool]
 
 
-class CalloutIcon(el.Div, RadixThemesComponent):
+class CalloutIcon(elements.Div, RadixThemesComponent):
     """Provides width and height for the icon associated with the callout."""
 
     tag = "Callout.Icon"
 
 
-class CalloutText(el.P, RadixThemesComponent):
+class CalloutText(elements.P, RadixThemesComponent):
     """Renders the callout text. This component is based on the p element."""
 
     tag = "Callout.Text"
 
 
 class Callout(CalloutRoot):
     """A short message to attract user's attention."""
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/callout.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/callout.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Literal, Union
 import reflex as rx
-from reflex import el
 from reflex.components.component import Component, ComponentNamespace
+from reflex.components.el import elements
 from reflex.components.lucide.icon import Icon
 from reflex.vars import Var
 from ..base import LiteralAccentColor, RadixThemesComponent
 
 CalloutVariant = Literal["soft", "surface", "outline"]
 
-class CalloutRoot(el.Div, RadixThemesComponent):
+class CalloutRoot(elements.Div, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         as_child: Optional[Union[Var[bool], bool]] = None,
         size: Optional[
@@ -226,15 +226,15 @@
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class CalloutIcon(el.Div, RadixThemesComponent):
+class CalloutIcon(elements.Div, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         access_key: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
@@ -361,15 +361,15 @@
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class CalloutText(el.P, RadixThemesComponent):
+class CalloutText(elements.P, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         access_key: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/card.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/card.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Interactive components provided by @radix-ui/themes."""
 from typing import Literal
 
-from reflex import el
+from reflex.components.el import elements
 from reflex.vars import Var
 
 from ..base import (
     RadixThemesComponent,
 )
 
 
-class Card(el.Div, RadixThemesComponent):
+class Card(elements.Div, RadixThemesComponent):
     """Container that groups related content and actions."""
 
     tag = "Card"
 
     # Change the default rendered element for the one passed as a child, merging their props and behavior.
     as_child: Var[bool]
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/card.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/layout/section.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,31 @@
-"""Stub file for reflex/components/radix/themes/components/card.py"""
+"""Stub file for reflex/components/radix/themes/layout/section.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Literal
-from reflex import el
+from reflex.components.el import elements
 from reflex.vars import Var
 from ..base import RadixThemesComponent
 
-class Card(el.Div, RadixThemesComponent):
+LiteralSectionSize = Literal["1", "2", "3"]
+
+class Section(elements.Section, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        as_child: Optional[Union[Var[bool], bool]] = None,
         size: Optional[
-            Union[
-                Var[Literal["1", "2", "3", "4", "5"]], Literal["1", "2", "3", "4", "5"]
-            ]
-        ] = None,
-        variant: Optional[
-            Union[
-                Var[Literal["surface", "classic", "ghost"]],
-                Literal["surface", "classic", "ghost"],
-            ]
+            Union[Var[Literal["1", "2", "3"]], Literal["1", "2", "3"]]
         ] = None,
         access_key: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
         auto_capitalize: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
         ] = None,
@@ -118,25 +111,23 @@
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Card":
+    ) -> "Section":
         """Create a new component instance.
 
         Will prepend "RadixThemes" to the component tag to avoid conflicts with
         other UI libraries for common names, like Text and Button.
 
         Args:
             *children: Child components.
-            as_child: Change the default rendered element for the one passed as a child, merging their props and behavior.
-            size: Card size: "1" - "5"
-            variant: Variant of Card: "solid" | "soft" | "outline" | "ghost"
+            size: The size of the section: "1" - "3" (default "2")
             access_key:  Provides a hint for generating a keyboard shortcut for the current element.
             auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
             content_editable: Indicates whether the element's content is editable.
             context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
             dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
             draggable: Defines whether the element can be dragged.
             enter_key_hint: Hints what media types the media element is able to play.
@@ -158,8 +149,8 @@
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-card = Card.create
+section = Section.create
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/checkbox.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox_cards.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/checkbox_cards.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox_cards.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/checkbox_cards.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox_group.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/checkbox_group.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/checkbox_group.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/checkbox_group.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/context_menu.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/context_menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/context_menu.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/context_menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/data_list.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/data_list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/data_list.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/data_list.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/dialog.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Interactive components provided by @radix-ui/themes."""
 
 from typing import Any, Dict, Literal
 
-from reflex import el
 from reflex.components.component import ComponentNamespace
+from reflex.components.el import elements
 from reflex.constants import EventTriggers
 from reflex.vars import Var
 
 from ..base import (
     RadixThemesComponent,
     RadixThemesTriggerComponent,
 )
@@ -41,15 +41,15 @@
 
 class DialogTitle(RadixThemesComponent):
     """Title component to display inside a Dialog modal."""
 
     tag = "Dialog.Title"
 
 
-class DialogContent(el.Div, RadixThemesComponent):
+class DialogContent(elements.Div, RadixThemesComponent):
     """Content component to display inside a Dialog modal."""
 
     tag = "Dialog.Content"
 
     # DialogContent size "1" - "4"
     size: Var[Literal["1", "2", "3", "4"]]
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/dialog.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/dialog.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Any, Dict, Literal
-from reflex import el
 from reflex.components.component import ComponentNamespace
+from reflex.components.el import elements
 from reflex.constants import EventTriggers
 from reflex.vars import Var
 from ..base import RadixThemesComponent, RadixThemesTriggerComponent
 
 class DialogRoot(RadixThemesComponent):
     def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
@@ -244,15 +244,15 @@
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class DialogContent(el.Div, RadixThemesComponent):
+class DialogContent(elements.Div, RadixThemesComponent):
     def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         size: Optional[
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/dropdown_menu.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/dropdown_menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/dropdown_menu.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/dropdown_menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/hover_card.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/hover_card.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Interactive components provided by @radix-ui/themes."""
 from typing import Any, Dict, Literal
 
-from reflex import el
 from reflex.components.component import ComponentNamespace
+from reflex.components.el import elements
 from reflex.constants import EventTriggers
 from reflex.vars import Var
 
 from ..base import (
     RadixThemesComponent,
     RadixThemesTriggerComponent,
 )
@@ -43,15 +43,15 @@
 
 class HoverCardTrigger(RadixThemesTriggerComponent):
     """Wraps the link that will open the hover card."""
 
     tag = "HoverCard.Trigger"
 
 
-class HoverCardContent(el.Div, RadixThemesComponent):
+class HoverCardContent(elements.Div, RadixThemesComponent):
     """Contains the content of the open hover card."""
 
     tag = "HoverCard.Content"
 
     # The preferred side of the trigger to render against when open. Will be reversed when collisions occur and avoidCollisions is enabled.
     side: Var[Literal["top", "right", "bottom", "left"]]
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/hover_card.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/hover_card.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Any, Dict, Literal
-from reflex import el
 from reflex.components.component import ComponentNamespace
+from reflex.components.el import elements
 from reflex.constants import EventTriggers
 from reflex.vars import Var
 from ..base import RadixThemesComponent, RadixThemesTriggerComponent
 
 class HoverCardRoot(RadixThemesComponent):
     def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
@@ -171,15 +171,15 @@
             props: The properties of the component.
 
         Returns:
             The new RadixThemesTriggerComponent instance.
         """
         ...
 
-class HoverCardContent(el.Div, RadixThemesComponent):
+class HoverCardContent(elements.Div, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         side: Optional[
             Union[
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/icon_button.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/icon_button.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Interactive components provided by @radix-ui/themes."""
 from __future__ import annotations
 
 from typing import Literal
 
-from reflex import el
 from reflex.components.component import Component
 from reflex.components.core.match import Match
+from reflex.components.el import elements
 from reflex.components.lucide import Icon
 from reflex.style import Style
 from reflex.vars import Var
 
 from ..base import (
     LiteralAccentColor,
     LiteralRadius,
@@ -17,15 +17,15 @@
     RadixLoadingProp,
     RadixThemesComponent,
 )
 
 LiteralButtonSize = Literal["1", "2", "3", "4"]
 
 
-class IconButton(el.Button, RadixLoadingProp, RadixThemesComponent):
+class IconButton(elements.Button, RadixLoadingProp, RadixThemesComponent):
     """A button designed specifically for usage with a single icon."""
 
     tag = "IconButton"
 
     # Change the default rendered element for the one passed as a child, merging their props and behavior.
     as_child: Var[bool]
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/icon_button.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/icon_button.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Literal
-from reflex import el
 from reflex.components.component import Component
 from reflex.components.core.match import Match
+from reflex.components.el import elements
 from reflex.components.lucide import Icon
 from reflex.style import Style
 from reflex.vars import Var
 from ..base import (
     LiteralAccentColor,
     LiteralRadius,
     LiteralVariant,
     RadixLoadingProp,
     RadixThemesComponent,
 )
 
 LiteralButtonSize = Literal["1", "2", "3", "4"]
 
-class IconButton(el.Button, RadixLoadingProp, RadixThemesComponent):
+class IconButton(elements.Button, RadixLoadingProp, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         as_child: Optional[Union[Var[bool], bool]] = None,
         size: Optional[
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/inset.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/inset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Interactive components provided by @radix-ui/themes."""
 from typing import Literal, Union
 
-from reflex import el
+from reflex.components.el import elements
 from reflex.vars import Var
 
 from ..base import (
     RadixThemesComponent,
 )
 
 LiteralButtonSize = Literal["1", "2", "3", "4"]
 
 
-class Inset(el.Div, RadixThemesComponent):
+class Inset(elements.Div, RadixThemesComponent):
     """Applies a negative margin to allow content to bleed into the surrounding container."""
 
     tag = "Inset"
 
     # The side
     side: Var[Literal["x", "y", "top", "bottom", "right", "left"]]
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/inset.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/inset.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Literal, Union
-from reflex import el
+from reflex.components.el import elements
 from reflex.vars import Var
 from ..base import RadixThemesComponent
 
 LiteralButtonSize = Literal["1", "2", "3", "4"]
 
-class Inset(el.Div, RadixThemesComponent):
+class Inset(elements.Div, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         side: Optional[
             Union[
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/popover.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/popover.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Interactive components provided by @radix-ui/themes."""
 from typing import Any, Dict, Literal
 
-from reflex import el
 from reflex.components.component import ComponentNamespace
+from reflex.components.el import elements
 from reflex.constants import EventTriggers
 from reflex.vars import Var
 
 from ..base import (
     RadixThemesComponent,
     RadixThemesTriggerComponent,
 )
@@ -37,15 +37,15 @@
 
 class PopoverTrigger(RadixThemesTriggerComponent):
     """Wraps the control that will open the popover."""
 
     tag = "Popover.Trigger"
 
 
-class PopoverContent(el.Div, RadixThemesComponent):
+class PopoverContent(elements.Div, RadixThemesComponent):
     """Contains content to be rendered in the open popover."""
 
     tag = "Popover.Content"
 
     # Size of the button: "1" | "2" | "3" | "4"
     size: Var[Literal["1", "2", "3", "4"]]
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/popover.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/popover.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Any, Dict, Literal
-from reflex import el
 from reflex.components.component import ComponentNamespace
+from reflex.components.el import elements
 from reflex.constants import EventTriggers
 from reflex.vars import Var
 from ..base import RadixThemesComponent, RadixThemesTriggerComponent
 
 class PopoverRoot(RadixThemesComponent):
     def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
@@ -167,15 +167,15 @@
             props: The properties of the component.
 
         Returns:
             The new RadixThemesTriggerComponent instance.
         """
         ...
 
-class PopoverContent(el.Div, RadixThemesComponent):
+class PopoverContent(elements.Div, RadixThemesComponent):
     def get_event_triggers(self) -> Dict[str, Any]: ...
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         size: Optional[
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/progress.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/progress.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/radio.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/radio.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/radio.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/radio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/radio_cards.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/radio_cards.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/radio_cards.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/radio_cards.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/radio_group.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/radio_group.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/radio_group.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/radio_group.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/scroll_area.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/scroll_area.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/scroll_area.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/scroll_area.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/segmented_control.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/segmented_control.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/segmented_control.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/segmented_control.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/select.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/select.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/select.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/separator.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/separator.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/separator.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/separator.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/skeleton.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/skeleton.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/skeleton.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/slider.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/slider.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/spinner.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/spinner.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/switch.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/switch.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/switch.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/table.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 """Interactive components provided by @radix-ui/themes."""
 from typing import List, Literal
 
-from reflex import el
 from reflex.components.component import ComponentNamespace
+from reflex.components.el import elements
 from reflex.vars import Var
 
 from ..base import (
     RadixThemesComponent,
 )
 
 
-class TableRoot(el.Table, RadixThemesComponent):
+class TableRoot(elements.Table, RadixThemesComponent):
     """A semantic table for presenting tabular data."""
 
     tag = "Table.Root"
 
     # The size of the table: "1" | "2" | "3"
     size: Var[Literal["1", "2", "3"]]
 
     # The variant of the table
     variant: Var[Literal["surface", "ghost"]]
 
 
-class TableHeader(el.Thead, RadixThemesComponent):
+class TableHeader(elements.Thead, RadixThemesComponent):
     """The header of the table defines column names and other non-data elements."""
 
     tag = "Table.Header"
 
     _invalid_children: List[str] = ["TableBody"]
 
     _valid_parents: List[str] = ["TableRoot"]
 
 
-class TableRow(el.Tr, RadixThemesComponent):
+class TableRow(elements.Tr, RadixThemesComponent):
     """A row containing table cells."""
 
     tag = "Table.Row"
 
     # The alignment of the row
     align: Var[Literal["start", "center", "end", "baseline"]]
 
     _invalid_children: List[str] = ["TableBody", "TableHeader", "TableRow"]
 
 
-class TableColumnHeaderCell(el.Th, RadixThemesComponent):
+class TableColumnHeaderCell(elements.Th, RadixThemesComponent):
     """A table cell that is semantically treated as a column header."""
 
     tag = "Table.ColumnHeaderCell"
 
     # The justification of the column
     justify: Var[Literal["start", "center", "end"]]
 
@@ -57,30 +57,30 @@
         "TableRow",
         "TableCell",
         "TableColumnHeaderCell",
         "TableRowHeaderCell",
     ]
 
 
-class TableBody(el.Tbody, RadixThemesComponent):
+class TableBody(elements.Tbody, RadixThemesComponent):
     """The body of the table contains the data rows."""
 
     tag = "Table.Body"
 
     _invalid_children: List[str] = [
         "TableHeader",
         "TableRowHeaderCell",
         "TableColumnHeaderCell",
         "TableCell",
     ]
 
     _valid_parents: List[str] = ["TableRoot"]
 
 
-class TableCell(el.Td, RadixThemesComponent):
+class TableCell(elements.Td, RadixThemesComponent):
     """A cell containing data."""
 
     tag = "Table.Cell"
 
     # The justification of the column
     justify: Var[Literal["start", "center", "end"]]
 
@@ -89,15 +89,15 @@
         "TableHeader",
         "TableRowHeaderCell",
         "TableColumnHeaderCell",
         "TableCell",
     ]
 
 
-class TableRowHeaderCell(el.Th, RadixThemesComponent):
+class TableRowHeaderCell(elements.Th, RadixThemesComponent):
     """A table cell that is semantically treated as a row header."""
 
     tag = "Table.RowHeaderCell"
 
     # The justification of the column
     justify: Var[Literal["start", "center", "end"]]
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/table.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/table.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import List, Literal
-from reflex import el
 from reflex.components.component import ComponentNamespace
+from reflex.components.el import elements
 from reflex.vars import Var
 from ..base import RadixThemesComponent
 
-class TableRoot(el.Table, RadixThemesComponent):
+class TableRoot(elements.Table, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         size: Optional[
             Union[Var[Literal["1", "2", "3"]], Literal["1", "2", "3"]]
@@ -160,15 +160,15 @@
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class TableHeader(el.Thead, RadixThemesComponent):
+class TableHeader(elements.Thead, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         align: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
@@ -299,15 +299,15 @@
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class TableRow(el.Tr, RadixThemesComponent):
+class TableRow(elements.Tr, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         align: Optional[
             Union[
@@ -441,15 +441,15 @@
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class TableColumnHeaderCell(el.Th, RadixThemesComponent):
+class TableColumnHeaderCell(elements.Th, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         justify: Optional[
             Union[
@@ -603,15 +603,15 @@
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class TableBody(el.Tbody, RadixThemesComponent):
+class TableBody(elements.Tbody, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         align: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
@@ -742,15 +742,15 @@
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class TableCell(el.Td, RadixThemesComponent):
+class TableCell(elements.Td, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         justify: Optional[
             Union[
@@ -900,15 +900,15 @@
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class TableRowHeaderCell(el.Th, RadixThemesComponent):
+class TableRowHeaderCell(elements.Th, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         justify: Optional[
             Union[
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/tabs.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/tabs.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/tabs.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/text_area.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/text_area.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 """Interactive components provided by @radix-ui/themes."""
 from typing import Any, Dict, Literal, Union
 
-from reflex import el
 from reflex.components.component import Component
 from reflex.components.core.debounce import DebounceInput
+from reflex.components.el import elements
 from reflex.constants import EventTriggers
 from reflex.vars import Var
 
 from ..base import (
     LiteralAccentColor,
+    LiteralRadius,
     RadixThemesComponent,
 )
 
 LiteralTextAreaSize = Literal["1", "2", "3"]
 
+LiteralTextAreaResize = Literal["none", "vertical", "horizontal", "both"]
 
-class TextArea(RadixThemesComponent, el.Textarea):
+
+class TextArea(RadixThemesComponent, elements.Textarea):
     """The input part of a TextArea, may be used by itself."""
 
     tag = "TextArea"
 
     # The size of the text area: "1" | "2" | "3"
     size: Var[LiteralTextAreaSize]
 
     # The variant of the text area
     variant: Var[Literal["classic", "surface", "soft"]]
 
+    # The resize behavior of the text area: "none" | "vertical" | "horizontal" | "both"
+    resize: Var[LiteralTextAreaResize]
+
     # The color of the text area
     color_scheme: Var[LiteralAccentColor]
 
+    # The radius of the text area: "none" | "small" | "medium" | "large" | "full"
+    radius: Var[LiteralRadius]
+
     # Whether the form control should have autocomplete enabled
     auto_complete: Var[bool]
 
     # Automatically focuses the textarea when the page loads
     auto_focus: Var[bool]
 
     # Name part of the textarea to submit in 'dir' and 'name' pair when form is submitted
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/text_area.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/text_area.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,38 +4,45 @@
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Any, Dict, Literal, Union
-from reflex import el
 from reflex.components.component import Component
 from reflex.components.core.debounce import DebounceInput
+from reflex.components.el import elements
 from reflex.constants import EventTriggers
 from reflex.vars import Var
-from ..base import LiteralAccentColor, RadixThemesComponent
+from ..base import LiteralAccentColor, LiteralRadius, RadixThemesComponent
 
 LiteralTextAreaSize = Literal["1", "2", "3"]
+LiteralTextAreaResize = Literal["none", "vertical", "horizontal", "both"]
 
-class TextArea(RadixThemesComponent, el.Textarea):
+class TextArea(RadixThemesComponent, elements.Textarea):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         size: Optional[
             Union[Var[Literal["1", "2", "3"]], Literal["1", "2", "3"]]
         ] = None,
         variant: Optional[
             Union[
                 Var[Literal["classic", "surface", "soft"]],
                 Literal["classic", "surface", "soft"],
             ]
         ] = None,
+        resize: Optional[
+            Union[
+                Var[Literal["none", "vertical", "horizontal", "both"]],
+                Literal["none", "vertical", "horizontal", "both"],
+            ]
+        ] = None,
         color_scheme: Optional[
             Union[
                 Var[
                     Literal[
                         "tomato",
                         "red",
                         "ruby",
@@ -90,14 +97,20 @@
                     "amber",
                     "gold",
                     "bronze",
                     "gray",
                 ],
             ]
         ] = None,
+        radius: Optional[
+            Union[
+                Var[Literal["none", "small", "medium", "large", "full"]],
+                Literal["none", "small", "medium", "large", "full"],
+            ]
+        ] = None,
         auto_complete: Optional[Union[Var[bool], bool]] = None,
         auto_focus: Optional[Union[Var[bool], bool]] = None,
         dirname: Optional[Union[Var[str], str]] = None,
         disabled: Optional[Union[Var[bool], bool]] = None,
         form: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
         max_length: Optional[Union[Var[int], int]] = None,
         min_length: Optional[Union[Var[int], int]] = None,
@@ -215,15 +228,17 @@
     ) -> "TextArea":
         """Create an Input component.
 
         Args:
             *children: The children of the component.
             size: The size of the text area: "1" | "2" | "3"
             variant: The variant of the text area
+            resize: The resize behavior of the text area: "none" | "vertical" | "horizontal" | "both"
             color_scheme: The color of the text area
+            radius: The radius of the text area: "none" | "small" | "medium" | "large" | "full"
             auto_complete: Whether the form control should have autocomplete enabled
             auto_focus: Automatically focuses the textarea when the page loads
             dirname: Name part of the textarea to submit in 'dir' and 'name' pair when form is submitted
             disabled: Disables the textarea
             form: Associates the textarea with a form (by id)
             max_length: Maximum number of characters allowed in the textarea
             min_length: Minimum number of characters required in the textarea
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/text_field.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/text_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Interactive components provided by @radix-ui/themes."""
 from __future__ import annotations
 
 from typing import Any, Dict, Literal, Union
 
-from reflex.components import el
 from reflex.components.base.fragment import Fragment
 from reflex.components.component import Component, ComponentNamespace
 from reflex.components.core.debounce import DebounceInput
+from reflex.components.el import elements
 from reflex.constants import EventTriggers
 from reflex.style import Style, format_as_emotion
 from reflex.utils import console
 from reflex.vars import Var
 
 from ..base import (
     LiteralAccentColor,
@@ -18,15 +18,15 @@
     RadixThemesComponent,
 )
 
 LiteralTextFieldSize = Literal["1", "2", "3"]
 LiteralTextFieldVariant = Literal["classic", "surface", "soft"]
 
 
-class TextFieldRoot(el.Div, RadixThemesComponent):
+class TextFieldRoot(elements.Div, RadixThemesComponent):
     """Captures user input with an optional slot for buttons and icons."""
 
     tag = "TextField.Root"
 
     # Text field size "1" - "3"
     size: Var[LiteralTextFieldSize]
 
@@ -193,8 +193,8 @@
 
     root = staticmethod(TextFieldRoot.create_root_deprecated)
     input = staticmethod(TextFieldRoot.create_input_deprecated)
     slot = staticmethod(TextFieldSlot.create)
     __call__ = staticmethod(TextFieldRoot.create)
 
 
-text_field = TextField()
+input = text_field = TextField()
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/text_field.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/text_field.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Any, Dict, Literal, Union
-from reflex.components import el
 from reflex.components.base.fragment import Fragment
 from reflex.components.component import Component, ComponentNamespace
 from reflex.components.core.debounce import DebounceInput
+from reflex.components.el import elements
 from reflex.constants import EventTriggers
 from reflex.style import Style, format_as_emotion
 from reflex.utils import console
 from reflex.vars import Var
 from ..base import LiteralAccentColor, LiteralRadius, RadixThemesComponent
 
 LiteralTextFieldSize = Literal["1", "2", "3"]
 LiteralTextFieldVariant = Literal["classic", "surface", "soft"]
 
-class TextFieldRoot(el.Div, RadixThemesComponent):
+class TextFieldRoot(elements.Div, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         size: Optional[
             Union[Var[Literal["1", "2", "3"]], Literal["1", "2", "3"]]
@@ -658,8 +658,8 @@
             **props: The properties of the component.
 
         Returns:
             The component.
         """
         ...
 
-text_field = TextField()
+input = text_field = TextField()
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/tooltip.py` & `reflex-0.5.3a1/reflex/components/radix/themes/components/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/components/tooltip.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/components/tooltip.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/layout/base.py` & `reflex-0.5.3a1/reflex/components/radix/themes/layout/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/layout/base.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/layout/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/layout/box.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/layout/box.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from reflex import el
+from reflex.components.el import elements
 from ..base import RadixThemesComponent
 
-class Box(el.Div, RadixThemesComponent):
+class Box(elements.Div, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         access_key: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
@@ -140,7 +140,9 @@
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
+
+box = Box.create
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/layout/center.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/layout/center.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -178,7 +178,9 @@
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
+
+center = Center.create
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/layout/container.py` & `reflex-0.5.3a1/reflex/components/radix/themes/layout/container.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Declarative layout and common spacing props."""
 from __future__ import annotations
 
 from typing import Literal
 
-from reflex import el
+from reflex.components.el import elements
 from reflex.style import STACK_CHILDREN_FULL_WIDTH
 from reflex.vars import Var
 
 from ..base import RadixThemesComponent
 
 LiteralContainerSize = Literal["1", "2", "3", "4"]
 
 
-class Container(el.Div, RadixThemesComponent):
+class Container(elements.Div, RadixThemesComponent):
     """Constrains the maximum width of page content.
 
     See https://www.radix-ui.com/themes/docs/components/container
     """
 
     tag = "Container"
 
@@ -45,7 +45,10 @@
         if stack_children_full_width:
             props["style"] = {**STACK_CHILDREN_FULL_WIDTH, **props.pop("style", {})}
         return super().create(
             *children,
             padding=padding,
             **props,
         )
+
+
+container = Container.create
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/layout/container.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/layout/container.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Literal
-from reflex import el
+from reflex.components.el import elements
 from reflex.style import STACK_CHILDREN_FULL_WIDTH
 from reflex.vars import Var
 from ..base import RadixThemesComponent
 
 LiteralContainerSize = Literal["1", "2", "3", "4"]
 
-class Container(el.Div, RadixThemesComponent):
+class Container(elements.Div, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         padding: Optional[str] = "16px",
         stack_children_full_width: Optional[bool] = False,
@@ -127,7 +127,9 @@
             stack_children_full_width: If True, any vstack/hstack children will have 100% width.
             props: The properties of the container.
 
         Returns:
             The container component.
         """
         ...
+
+container = Container.create
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/layout/flex.py` & `reflex-0.5.3a1/reflex/components/radix/themes/layout/flex.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Declarative layout and common spacing props."""
 
 from __future__ import annotations
 
 from typing import Dict, Literal
 
-from reflex import el
+from reflex.components.el import elements
 from reflex.vars import Var
 
 from ..base import (
     LiteralAlign,
     LiteralJustify,
     LiteralSpacing,
     RadixThemesComponent,
 )
 
 LiteralFlexDirection = Literal["row", "column", "row-reverse", "column-reverse"]
 LiteralFlexWrap = Literal["nowrap", "wrap", "wrap-reverse"]
 
 
-class Flex(el.Div, RadixThemesComponent):
+class Flex(elements.Div, RadixThemesComponent):
     """Component for creating flex layouts."""
 
     tag = "Flex"
 
     # Change the default rendered element for the one passed as a child, merging their props and behavior.
     as_child: Var[bool]
 
@@ -39,7 +39,10 @@
     wrap: Var[LiteralFlexWrap]
 
     # Gap between children: "0" - "9"
     spacing: Var[LiteralSpacing]
 
     # Reflex maps the "spacing" prop to "gap" prop.
     _rename_props: Dict[str, str] = {"spacing": "gap"}
+
+
+flex = Flex.create
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/layout/flex.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/layout/flex.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Dict, Literal
-from reflex import el
+from reflex.components.el import elements
 from reflex.vars import Var
 from ..base import LiteralAlign, LiteralJustify, LiteralSpacing, RadixThemesComponent
 
 LiteralFlexDirection = Literal["row", "column", "row-reverse", "column-reverse"]
 LiteralFlexWrap = Literal["nowrap", "wrap", "wrap-reverse"]
 
-class Flex(el.Div, RadixThemesComponent):
+class Flex(elements.Div, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         as_child: Optional[Union[Var[bool], bool]] = None,
         direction: Optional[
@@ -182,7 +182,9 @@
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
+
+flex = Flex.create
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/layout/grid.py` & `reflex-0.5.3a1/reflex/components/radix/themes/layout/grid.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Declarative layout and common spacing props."""
 
 from __future__ import annotations
 
 from typing import Dict, Literal
 
-from reflex import el
+from reflex.components.el import elements
 from reflex.vars import Var
 
 from ..base import (
     LiteralAlign,
     LiteralJustify,
     LiteralSpacing,
     RadixThemesComponent,
 )
 
 LiteralGridFlow = Literal["row", "column", "dense", "row-dense", "column-dense"]
 
 
-class Grid(el.Div, RadixThemesComponent):
+class Grid(elements.Div, RadixThemesComponent):
     """Component for creating grid layouts."""
 
     tag = "Grid"
 
     # Change the default rendered element for the one passed as a child, merging their props and behavior.
     as_child: Var[bool]
 
@@ -51,7 +51,10 @@
 
     # Reflex maps the "spacing" prop to "gap" prop.
     _rename_props: Dict[str, str] = {
         "spacing": "gap",
         "spacing_x": "gap_x",
         "spacing_y": "gap_y",
     }
+
+
+grid = Grid.create
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/layout/grid.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/layout/grid.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Dict, Literal
-from reflex import el
+from reflex.components.el import elements
 from reflex.vars import Var
 from ..base import LiteralAlign, LiteralJustify, LiteralSpacing, RadixThemesComponent
 
 LiteralGridFlow = Literal["row", "column", "dense", "row-dense", "column-dense"]
 
-class Grid(el.Div, RadixThemesComponent):
+class Grid(elements.Div, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         as_child: Optional[Union[Var[bool], bool]] = None,
         columns: Optional[Union[Var[str], str]] = None,
@@ -192,7 +192,9 @@
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
+
+grid = Grid.create
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/layout/list.py` & `reflex-0.5.3a1/reflex/components/radix/themes/layout/list.py`

 * *Files 5% similar despite different names*

```diff
@@ -180,7 +180,21 @@
     item = staticmethod(ListItem.create)
     ordered = staticmethod(OrderedList.create)
     unordered = staticmethod(UnorderedList.create)
     __call__ = staticmethod(BaseList.create)
 
 
 list_ns = List()
+list_item = list_ns.item
+ordered_list = list_ns.ordered
+unordered_list = list_ns.unordered
+
+
+def __getattr__(name):
+    # special case for when accessing list to avoid shadowing
+    # python's built in list object.
+    if name == "list":
+        return list_ns
+    try:
+        return globals()[name]
+    except KeyError:
+        raise AttributeError(f"module '{__name__} has no attribute '{name}'") from None
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/layout/list.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/layout/list.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -698,7 +698,10 @@
         Returns:
             The list component.
 
         """
         ...
 
 list_ns = List()
+list_item = list_ns.item
+ordered_list = list_ns.ordered
+unordered_list = list_ns.unordered
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/layout/section.pyi` & `reflex-0.5.3a1/reflex/components/plotly/plotly.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,167 @@
-"""Stub file for reflex/components/radix/themes/layout/section.py"""
+"""Stub file for reflex/components/plotly/plotly.py"""
 # ------------------- DO NOT EDIT ----------------------
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from typing import Literal
-from reflex import el
+from typing import Any, Dict, List
+from reflex.base import Base
+from reflex.components.component import NoSSRComponent
+from reflex.event import EventHandler
 from reflex.vars import Var
-from ..base import RadixThemesComponent
 
-LiteralSectionSize = Literal["1", "2", "3"]
+try:
+    from plotly.graph_objects import Figure  # type: ignore
+except ImportError:
+    Figure = Any  # type: ignore
+
+class _ButtonClickData(Base):
+    menu: Any
+    button: Any
+    active: Any
 
-class Section(el.Section, RadixThemesComponent):
+class PlotlyLib(NoSSRComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
-        size: Optional[
-            Union[Var[Literal["1", "2", "3"]], Literal["1", "2", "3"]]
+        style: Optional[Style] = None,
+        key: Optional[Any] = None,
+        id: Optional[Any] = None,
+        class_name: Optional[Any] = None,
+        autofocus: Optional[bool] = None,
+        custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_blur: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        access_key: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        auto_capitalize: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_context_menu: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        content_editable: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_double_click: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        context_menu: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_focus: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        dir: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        draggable: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        enter_key_hint: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_down: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        hidden: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_enter: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        input_mode: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_leave: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        item_prop: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_move: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_mouse_out: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        lang: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        role: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        slot: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
-        spell_check: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_over: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        tab_index: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_mouse_up: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
-        title: Optional[
-            Union[Var[Union[str, int, bool]], Union[str, int, bool]]
+        on_scroll: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_unmount: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        **props
+    ) -> "PlotlyLib":
+        """Create the component.
+
+        Args:
+            *children: The children of the component.
+            style: The style of the component.
+            key: A unique key for the component.
+            id: The id for the component.
+            class_name: The class name for the component.
+            autofocus: Whether the component should take the focus once the page is loaded
+            custom_attrs: custom attribute
+            **props: The props of the component.
+
+        Returns:
+            The component.
+        """
+        ...
+
+class Plotly(PlotlyLib):
+    def add_custom_code(self) -> list[str]: ...
+    @overload
+    @classmethod
+    def create(  # type: ignore
+        cls,
+        *children,
+        data: Optional[Union[Var[Figure], Figure]] = None,  # type: ignore
+        layout: Optional[Union[Var[Dict], Dict]] = None,
+        config: Optional[Union[Var[Dict], Dict]] = None,
+        use_resize_handler: Optional[Union[Var[bool], bool]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
+        on_after_plot: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_animated: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_animating_frame: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_animation_interrupted: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_autosize: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_before_hover: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_blur: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_button_clicked: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_context_menu: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_deselect: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_double_click: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_focus: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_hover: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_mount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_down: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_enter: Optional[
@@ -104,51 +178,62 @@
         ] = None,
         on_mouse_over: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         on_mouse_up: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_redraw: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_relayout: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_relayouting: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_restyle: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_scroll: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
+        on_selected: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_selecting: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_transition_interrupted: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_transitioning: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
+        on_unhover: Optional[
+            Union[EventHandler, EventSpec, list, function, BaseVar]
+        ] = None,
         on_unmount: Optional[
             Union[EventHandler, EventSpec, list, function, BaseVar]
         ] = None,
         **props
-    ) -> "Section":
-        """Create a new component instance.
-
-        Will prepend "RadixThemes" to the component tag to avoid conflicts with
-        other UI libraries for common names, like Text and Button.
+    ) -> "Plotly":
+        """Create the component.
 
         Args:
-            *children: Child components.
-            size: The size of the section: "1" - "3" (default "3")
-            access_key:  Provides a hint for generating a keyboard shortcut for the current element.
-            auto_capitalize: Controls whether and how text input is automatically capitalized as it is entered/edited by the user.
-            content_editable: Indicates whether the element's content is editable.
-            context_menu: Defines the ID of a <menu> element which will serve as the element's context menu.
-            dir: Defines the text direction. Allowed values are ltr (Left-To-Right) or rtl (Right-To-Left)
-            draggable: Defines whether the element can be dragged.
-            enter_key_hint: Hints what media types the media element is able to play.
-            hidden: Defines whether the element is hidden.
-            input_mode: Defines the type of the element.
-            item_prop: Defines the name of the element for metadata purposes.
-            lang: Defines the language used in the element.
-            role: Defines the role of the element.
-            slot: Assigns a slot in a shadow DOM shadow tree to an element.
-            spell_check: Defines whether the element may be checked for spelling errors.
-            tab_index: Defines the position of the current element in the tabbing order.
-            title: Defines a tooltip for the element.
+            *children: The children of the component.
+            data: The figure to display. This can be a plotly figure or a plotly data json.
+            layout: The layout of the graph.
+            config: The config of the graph.
+            use_resize_handler: If true, the graph will resize when the window is resized.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
-            **props: Component properties.
+            **props: The props of the component.
 
         Returns:
-            A new component instance.
+            The component.
         """
         ...
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/layout/spacer.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/layout/spacer.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -178,7 +178,9 @@
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
+
+spacer = Spacer.create
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/layout/stack.py` & `reflex-0.5.3a1/reflex/components/radix/themes/layout/stack.py`

 * *Files 14% similar despite different names*

```diff
@@ -53,7 +53,12 @@
 
 
 class HStack(Stack):
     """A horizontal stack component."""
 
     # The direction of the stack.
     direction: Var[LiteralFlexDirection] = "row"  # type: ignore
+
+
+stack = Stack.create
+hstack = HStack.create
+vstack = VStack.create
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/layout/stack.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/layout/stack.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -484,7 +484,11 @@
             custom_attrs: custom attribute
             **props: The properties of the stack.
 
         Returns:
             The stack component.
         """
         ...
+
+stack = Stack.create
+hstack = HStack.create
+vstack = VStack.create
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/typography/blockquote.py` & `reflex-0.5.3a1/reflex/components/radix/themes/typography/blockquote.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Components for rendering heading.
 
 https://www.radix-ui.com/themes/docs/theme/typography
 """
 from __future__ import annotations
 
-from reflex import el
+from reflex.components.el import elements
 from reflex.vars import Var
 
 from ..base import (
     LiteralAccentColor,
     RadixThemesComponent,
 )
 from .base import (
     LiteralTextSize,
     LiteralTextWeight,
 )
 
 
-class Blockquote(el.Blockquote, RadixThemesComponent):
+class Blockquote(elements.Blockquote, RadixThemesComponent):
     """A block level extended quotation."""
 
     tag = "Blockquote"
 
     # Text size: "1" - "9"
     size: Var[LiteralTextSize]
 
@@ -29,7 +29,10 @@
     weight: Var[LiteralTextWeight]
 
     # Overrides the accent color inherited from the Theme.
     color_scheme: Var[LiteralAccentColor]
 
     # Whether to render the text with higher contrast color
     high_contrast: Var[bool]
+
+
+blockquote = Blockquote.create
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/typography/blockquote.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/typography/blockquote.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from reflex import el
+from reflex.components.el import elements
 from reflex.vars import Var
 from ..base import LiteralAccentColor, RadixThemesComponent
 from .base import LiteralTextSize, LiteralTextWeight
 
-class Blockquote(el.Blockquote, RadixThemesComponent):
+class Blockquote(elements.Blockquote, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         size: Optional[
             Union[
@@ -223,7 +223,9 @@
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
+
+blockquote = Blockquote.create
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/typography/code.py` & `reflex-0.5.3a1/reflex/components/radix/themes/typography/code.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Components for rendering heading.
 
 https://www.radix-ui.com/themes/docs/theme/typography
 """
 from __future__ import annotations
 
-from reflex import el
+from reflex.components.el import elements
 from reflex.vars import Var
 
 from ..base import (
     LiteralAccentColor,
     LiteralVariant,
     RadixThemesComponent,
 )
 from .base import (
     LiteralTextSize,
     LiteralTextWeight,
 )
 
 
-class Code(el.Code, RadixThemesComponent):
+class Code(elements.Code, RadixThemesComponent):
     """A block level extended quotation."""
 
     tag = "Code"
 
     # The visual variant to apply: "solid" | "soft" | "outline" | "ghost"
     variant: Var[LiteralVariant]
 
@@ -33,7 +33,10 @@
     weight: Var[LiteralTextWeight]
 
     # Overrides the accent color inherited from the Theme.
     color_scheme: Var[LiteralAccentColor]
 
     # Whether to render the text with higher contrast color
     high_contrast: Var[bool]
+
+
+code = Code.create
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/typography/code.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/typography/code.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from reflex import el
+from reflex.components.el import elements
 from reflex.vars import Var
 from ..base import LiteralAccentColor, LiteralVariant, RadixThemesComponent
 from .base import LiteralTextSize, LiteralTextWeight
 
-class Code(el.Code, RadixThemesComponent):
+class Code(elements.Code, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         variant: Optional[
             Union[
@@ -228,7 +228,9 @@
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
+
+code = Code.create
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/typography/heading.py` & `reflex-0.5.3a1/reflex/components/radix/themes/typography/heading.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """Components for rendering heading.
 
 https://www.radix-ui.com/themes/docs/theme/typography
 """
 from __future__ import annotations
 
-from reflex import el
+from reflex.components.el import elements
 from reflex.vars import Var
 
 from ..base import (
     LiteralAccentColor,
     RadixThemesComponent,
 )
 from .base import (
     LiteralTextAlign,
     LiteralTextSize,
     LiteralTextTrim,
     LiteralTextWeight,
 )
 
 
-class Heading(el.H1, RadixThemesComponent):
+class Heading(elements.H1, RadixThemesComponent):
     """A foundational text primitive based on the <span> element."""
 
     tag = "Heading"
 
     # Change the default rendered element for the one passed as a child, merging their props and behavior.
     as_child: Var[bool]
 
@@ -43,7 +43,10 @@
     trim: Var[LiteralTextTrim]
 
     # Overrides the accent color inherited from the Theme.
     color_scheme: Var[LiteralAccentColor]
 
     # Whether to render the text with higher contrast color
     high_contrast: Var[bool]
+
+
+heading = Heading.create
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/typography/heading.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/typography/heading.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 # This file was generated by `reflex/utils/pyi_generator.py`!
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
-from reflex import el
+from reflex.components.el import elements
 from reflex.vars import Var
 from ..base import LiteralAccentColor, RadixThemesComponent
 from .base import LiteralTextAlign, LiteralTextSize, LiteralTextTrim, LiteralTextWeight
 
-class Heading(el.H1, RadixThemesComponent):
+class Heading(elements.H1, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         as_child: Optional[Union[Var[bool], bool]] = None,
         as_: Optional[Union[Var[str], str]] = None,
@@ -239,7 +239,9 @@
             custom_attrs: custom attribute
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
+
+heading = Heading.create
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/typography/link.py` & `reflex-0.5.3a1/reflex/components/radix/themes/typography/link.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,7 +98,10 @@
                 # If user does not use `as_child`, by default we render using next_link to avoid page refresh during internal navigation
                 return super().create(
                     NextLink.create(*children, **next_link_props),
                     as_child=True,
                     **props,
                 )
         return super().create(*children, **props)
+
+
+link = Link.create
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/typography/link.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/typography/link.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -278,7 +278,9 @@
         Raises:
             ValueError: in case of missing children
 
         Returns:
             Component: The link component
         """
         ...
+
+link = Link.create
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/typography/text.py` & `reflex-0.5.3a1/reflex/components/radix/themes/typography/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 https://www.radix-ui.com/themes/docs/theme/typography
 """
 
 from __future__ import annotations
 
 from typing import Literal
 
-from reflex import el
 from reflex.components.component import ComponentNamespace
+from reflex.components.el import elements
 from reflex.vars import Var
 
 from ..base import (
     LiteralAccentColor,
     RadixThemesComponent,
 )
 from .base import (
@@ -40,15 +40,15 @@
     "s",
     "samp",
     "sub",
     "sup",
 ]
 
 
-class Text(el.Span, RadixThemesComponent):
+class Text(elements.Span, RadixThemesComponent):
     """A foundational text primitive based on the <span> element."""
 
     tag = "Text"
 
     # Change the default rendered element for the one passed as a child, merging their props and behavior.
     as_child: Var[bool]
 
@@ -76,36 +76,36 @@
 
 class Span(Text):
     """A variant of text rendering as <span> element."""
 
     as_: Var[LiteralType] = "span"  # type: ignore
 
 
-class Em(el.Em, RadixThemesComponent):
+class Em(elements.Em, RadixThemesComponent):
     """Marks text to stress emphasis."""
 
     tag = "Em"
 
 
-class Kbd(el.Kbd, RadixThemesComponent):
+class Kbd(elements.Kbd, RadixThemesComponent):
     """Represents keyboard input or a hotkey."""
 
     tag = "Kbd"
 
     # Text size: "1" - "9"
     size: Var[LiteralTextSize]
 
 
-class Quote(el.Q, RadixThemesComponent):
+class Quote(elements.Q, RadixThemesComponent):
     """A short inline quotation."""
 
     tag = "Quote"
 
 
-class Strong(el.Strong, RadixThemesComponent):
+class Strong(elements.Strong, RadixThemesComponent):
     """Marks text to signify strong importance."""
 
     tag = "Strong"
 
 
 class TextNamespace(ComponentNamespace):
     """Checkbox components namespace."""
```

### Comparing `reflex-0.5.2a1/reflex/components/radix/themes/typography/text.pyi` & `reflex-0.5.3a1/reflex/components/radix/themes/typography/text.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # ------------------------------------------------------
 
 from typing import Any, Dict, Literal, Optional, Union, overload
 from reflex.vars import Var, BaseVar, ComputedVar
 from reflex.event import EventChain, EventHandler, EventSpec
 from reflex.style import Style
 from typing import Literal
-from reflex import el
 from reflex.components.component import ComponentNamespace
+from reflex.components.el import elements
 from reflex.vars import Var
 from ..base import LiteralAccentColor, RadixThemesComponent
 from .base import LiteralTextAlign, LiteralTextSize, LiteralTextTrim, LiteralTextWeight
 
 LiteralType = Literal[
     "p",
     "label",
@@ -31,15 +31,15 @@
     "mark",
     "s",
     "samp",
     "sub",
     "sup",
 ]
 
-class Text(el.Span, RadixThemesComponent):
+class Text(elements.Span, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         as_child: Optional[Union[Var[bool], bool]] = None,
         as_: Optional[
@@ -585,15 +585,15 @@
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class Em(el.Em, RadixThemesComponent):
+class Em(elements.Em, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         access_key: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
@@ -720,15 +720,15 @@
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class Kbd(el.Kbd, RadixThemesComponent):
+class Kbd(elements.Kbd, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         size: Optional[
             Union[
@@ -862,15 +862,15 @@
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class Quote(el.Q, RadixThemesComponent):
+class Quote(elements.Q, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         cite: Optional[Union[Var[Union[str, int, bool]], Union[str, int, bool]]] = None,
         access_key: Optional[
@@ -999,15 +999,15 @@
             **props: Component properties.
 
         Returns:
             A new component instance.
         """
         ...
 
-class Strong(el.Strong, RadixThemesComponent):
+class Strong(elements.Strong, RadixThemesComponent):
     @overload
     @classmethod
     def create(  # type: ignore
         cls,
         *children,
         access_key: Optional[
             Union[Var[Union[str, int, bool]], Union[str, int, bool]]
```

### Comparing `reflex-0.5.2a1/reflex/components/react_player/audio.pyi` & `reflex-0.5.3a1/reflex/components/react_player/audio.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/react_player/react_player.py` & `reflex-0.5.3a1/reflex/components/react_player/react_player.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/react_player/react_player.pyi` & `reflex-0.5.3a1/reflex/components/react_player/react_player.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/react_player/video.pyi` & `reflex-0.5.3a1/reflex/components/react_player/video.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/recharts/cartesian.py` & `reflex-0.5.3a1/reflex/components/recharts/cartesian.py`

 * *Files 2% similar despite different names*

```diff
@@ -568,7 +568,24 @@
     label: Var[str]
 
     # If set true, flips ticks around the axis line, displaying the labels inside the chart instead of outside.
     mirror: Var[bool]
 
     # The margin between tick line and tick.
     tick_margin: Var[int]
+
+
+area = Area.create
+bar = Bar.create
+line = Line.create
+scatter = Scatter.create
+x_axis = XAxis.create
+y_axis = YAxis.create
+z_axis = ZAxis.create
+brush = Brush.create
+cartesian_axis = CartesianAxis.create
+cartesian_grid = CartesianGrid.create
+reference_line = ReferenceLine.create
+reference_dot = ReferenceDot.create
+reference_area = ReferenceArea.create
+error_bar = ErrorBar.create
+funnel = Funnel.create
```

### Comparing `reflex-0.5.2a1/reflex/components/recharts/cartesian.pyi` & `reflex-0.5.3a1/reflex/components/recharts/cartesian.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1845,7 +1845,23 @@
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
         """
         ...
+
+area = Area.create
+bar = Bar.create
+line = Line.create
+scatter = Scatter.create
+x_axis = XAxis.create
+y_axis = YAxis.create
+z_axis = ZAxis.create
+brush = Brush.create
+cartesian_axis = CartesianAxis.create
+cartesian_grid = CartesianGrid.create
+reference_line = ReferenceLine.create
+reference_dot = ReferenceDot.create
+reference_area = ReferenceArea.create
+error_bar = ErrorBar.create
+funnel = Funnel.create
```

### Comparing `reflex-0.5.2a1/reflex/components/recharts/charts.py` & `reflex-0.5.3a1/reflex/components/recharts/charts.py`

 * *Files 1% similar despite different names*

```diff
@@ -517,7 +517,19 @@
             The Treemap component wrapped in a responsive container.
         """
         return ResponsiveContainer.create(
             super().create(*children, **props),
             width=props.pop("width", "100%"),
             height=props.pop("height", "100%"),
         )
+
+
+area_chart = AreaChart.create
+bar_chart = BarChart.create
+line_chart = LineChart.create
+composed_chart = ComposedChart.create
+pie_chart = PieChart.create
+radar_chart = RadarChart.create
+radial_bar_chart = RadialBarChart.create
+scatter_chart = ScatterChart.create
+funnel_chart = FunnelChart.create
+treemap = Treemap.create
```

### Comparing `reflex-0.5.2a1/reflex/components/recharts/charts.pyi` & `reflex-0.5.3a1/reflex/components/recharts/charts.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -889,7 +889,18 @@
             custom_attrs: custom attribute
             **props: The properties of the chart component.
 
         Returns:
             The Treemap component wrapped in a responsive container.
         """
         ...
+
+area_chart = AreaChart.create
+bar_chart = BarChart.create
+line_chart = LineChart.create
+composed_chart = ComposedChart.create
+pie_chart = PieChart.create
+radar_chart = RadarChart.create
+radial_bar_chart = RadialBarChart.create
+scatter_chart = ScatterChart.create
+funnel_chart = FunnelChart.create
+treemap = Treemap.create
```

### Comparing `reflex-0.5.2a1/reflex/components/recharts/general.py` & `reflex-0.5.3a1/reflex/components/recharts/general.py`

 * *Files 3% similar despite different names*

```diff
@@ -178,7 +178,14 @@
     offset: Var[int]
 
     # Color of the fill
     fill: Var[str]
 
     # Color of the stroke
     stroke: Var[str]
+
+
+responsive_container = ResponsiveContainer.create
+legend = Legend.create
+graphing_tooltip = GraphingTooltip.create
+label = Label.create
+label_list = LabelList.create
```

### Comparing `reflex-0.5.2a1/reflex/components/recharts/general.pyi` & `reflex-0.5.3a1/reflex/components/recharts/general.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -569,7 +569,13 @@
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
         """
         ...
+
+responsive_container = ResponsiveContainer.create
+legend = Legend.create
+graphing_tooltip = GraphingTooltip.create
+label = Label.create
+label_list = LabelList.create
```

### Comparing `reflex-0.5.2a1/reflex/components/recharts/polar.py` & `reflex-0.5.3a1/reflex/components/recharts/polar.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,21 +304,32 @@
 
     # If 'auto' set, the scale funtion is linear scale. 'auto' | 'linear' | 'pow' | 'sqrt' | 'log' | 'identity' | 'time' | 'band' | 'point' | 'ordinal' | 'quantile' | 'quantize' | 'utc' | 'sequential' | 'threshold'
     scale: Var[LiteralScale]
 
     # Valid children components
     _valid_children: List[str] = ["Label"]
 
+    # The domain of the polar radius axis, specifying the minimum and maximum values.
+    domain: List[int] = [0, 250]
+
     def get_event_triggers(self) -> dict[str, Union[Var, Any]]:
         """Get the event triggers that pass the component's value to the handler.
 
         Returns:
             A dict mapping the event trigger to the var that is passed to the handler.
         """
         return {
             EventTriggers.ON_CLICK: lambda: [],
             EventTriggers.ON_MOUSE_MOVE: lambda: [],
             EventTriggers.ON_MOUSE_OVER: lambda: [],
             EventTriggers.ON_MOUSE_OUT: lambda: [],
             EventTriggers.ON_MOUSE_ENTER: lambda: [],
             EventTriggers.ON_MOUSE_LEAVE: lambda: [],
         }
+
+
+pie = Pie.create
+radar = Radar.create
+radial_bar = RadialBar.create
+polar_angle_axis = PolarAngleAxis.create
+polar_grid = PolarGrid.create
+polar_radius_axis = PolarRadiusAxis.create
```

### Comparing `reflex-0.5.2a1/reflex/components/recharts/polar.pyi` & `reflex-0.5.3a1/reflex/components/recharts/polar.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -488,14 +488,15 @@
                     "quantize",
                     "utc",
                     "sequential",
                     "threshold",
                 ],
             ]
         ] = None,
+        domain: Optional[List[int]] = None,
         style: Optional[Style] = None,
         key: Optional[Any] = None,
         id: Optional[Any] = None,
         class_name: Optional[Any] = None,
         autofocus: Optional[bool] = None,
         custom_attrs: Optional[Dict[str, Union[Var, str]]] = None,
         on_click: Optional[
@@ -529,19 +530,27 @@
             cy: The y-coordinate of center.
             reversed: If set to true, the ticks of this axis are reversed.
             orientation: The orientation of axis text.
             axis_line: If false set, axis line will not be drawn. If true set, axis line will be drawn which have the props calculated internally. If object set, axis line will be drawn which have the props mergered by the internal calculated props and the option.
             tick: The width or height of tick.
             tick_count: The count of ticks.
             scale: If 'auto' set, the scale funtion is linear scale. 'auto' | 'linear' | 'pow' | 'sqrt' | 'log' | 'identity' | 'time' | 'band' | 'point' | 'ordinal' | 'quantile' | 'quantize' | 'utc' | 'sequential' | 'threshold'
+            domain: The domain of the polar radius axis, specifying the minimum and maximum values.
             style: The style of the component.
             key: A unique key for the component.
             id: The id for the component.
             class_name: The class name for the component.
             autofocus: Whether the component should take the focus once the page is loaded
             custom_attrs: custom attribute
             **props: The props of the component.
 
         Returns:
             The component.
         """
         ...
+
+pie = Pie.create
+radar = Radar.create
+radial_bar = RadialBar.create
+polar_angle_axis = PolarAngleAxis.create
+polar_grid = PolarGrid.create
+polar_radius_axis = PolarRadiusAxis.create
```

### Comparing `reflex-0.5.2a1/reflex/components/recharts/recharts.py` & `reflex-0.5.3a1/reflex/components/recharts/recharts.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/recharts/recharts.pyi` & `reflex-0.5.3a1/reflex/components/recharts/recharts.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/sonner/toast.py` & `reflex-0.5.3a1/reflex/components/sonner/toast.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/sonner/toast.pyi` & `reflex-0.5.3a1/reflex/components/sonner/toast.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/suneditor/editor.py` & `reflex-0.5.3a1/reflex/components/suneditor/editor.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/suneditor/editor.pyi` & `reflex-0.5.3a1/reflex/components/suneditor/editor.pyi`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/tags/iter_tag.py` & `reflex-0.5.3a1/reflex/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/tags/tag.py` & `reflex-0.5.3a1/reflex/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/components/tags/tagless.py` & `reflex-0.5.3a1/reflex/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/config.py` & `reflex-0.5.3a1/reflex/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,14 +198,17 @@
 
     # Timeout when launching the gunicorn server. TODO(rename this to backend_timeout?)
     timeout: int = 120
 
     # Whether to enable or disable nextJS gzip compression.
     next_compression: bool = True
 
+    # Whether to use React strict mode in nextJS
+    react_strict_mode: bool = True
+
     # Additional frontend packages to install.
     frontend_packages: List[str] = []
 
     # The hosting service backend URL.
     cp_backend_url: str = Hosting.CP_BACKEND_URL
     # The hosting service frontend URL.
     cp_web_url: str = Hosting.CP_WEB_URL
```

### Comparing `reflex-0.5.2a1/reflex/constants/__init__.py` & `reflex-0.5.3a1/reflex/constants/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     Imports,
     MemoizationDisposition,
     MemoizationMode,
     PageNames,
 )
 from .config import (
     ALEMBIC_CONFIG,
-    PRODUCTION_BACKEND_URL,
     Config,
     Expiration,
     GitIgnore,
     RequirementsTxt,
 )
 from .custom_components import (
     CustomComponents,
@@ -95,15 +94,14 @@
     NOCOMPILE_FILE,
     PackageJson,
     PageNames,
     Page404,
     Ping,
     POLLING_MAX_HTTP_BUFFER_SIZE,
     PYTEST_CURRENT_TEST,
-    PRODUCTION_BACKEND_URL,
     Reflex,
     RELOAD_CONFIG,
     RequirementsTxt,
     RouteArgType,
     RouteRegex,
     RouteVar,
     ROUTER,
```

### Comparing `reflex-0.5.2a1/reflex/constants/base.py` & `reflex-0.5.3a1/reflex/constants/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     """Various directories/paths used by Reflex."""
 
     # The frontend directories in a project.
     # The web folder where the NextJS app is compiled to.
     WEB = ".web"
     # The name of the assets directory.
     APP_ASSETS = "assets"
+    # The name of the assets directory for external ressource (a subfolder of APP_ASSETS).
+    EXTERNAL_APP_ASSETS = "external"
     # The name of the utils file.
     UTILS = "utils"
     # The name of the output static directory.
     STATIC = "_static"
     # The name of the state file.
     STATE_PATH = "/".join([UTILS, "state"])
     # The name of the components file.
```

### Comparing `reflex-0.5.2a1/reflex/constants/base.pyi` & `reflex-0.5.3a1/reflex/constants/base.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -11,18 +11,23 @@
 import platform
 from enum import Enum
 from importlib import metadata
 from types import SimpleNamespace
 from platformdirs import PlatformDirs
 
 IS_WINDOWS = platform.system() == "Windows"
+IS_WINDOWS_BUN_SUPPORTED_MACHINE = IS_WINDOWS and platform.machine() in [
+    "AMD64",
+    "x86_64",
+]
 
 class Dirs(SimpleNamespace):
     WEB = ".web"
     APP_ASSETS = "assets"
+    EXTERNAL_APP_ASSETS = "external"
     UTILS = "utils"
     STATIC = "_static"
     STATE_PATH = "/".join([UTILS, "state"])
     COMPONENTS_PATH = "/".join([UTILS, "components"])
     CONTEXTS_PATH = "/".join([UTILS, "context"])
     WEB_PAGES = os.path.join(WEB, "pages")
     WEB_STATIC = os.path.join(WEB, STATIC)
```

### Comparing `reflex-0.5.2a1/reflex/constants/colors.py` & `reflex-0.5.3a1/reflex/constants/colors.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/constants/compiler.py` & `reflex-0.5.3a1/reflex/constants/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/constants/config.py` & `reflex-0.5.3a1/reflex/constants/config.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/constants/custom_components.py` & `reflex-0.5.3a1/reflex/constants/custom_components.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/constants/event.py` & `reflex-0.5.3a1/reflex/constants/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/constants/installer.py` & `reflex-0.5.3a1/reflex/constants/installer.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 # Bun config.
 class Bun(SimpleNamespace):
     """Bun constants."""
 
     # The Bun version.
-    VERSION = "1.1.8"
+    VERSION = "1.1.10"
     # Min Bun Version
     MIN_VERSION = "0.7.0"
     # The directory to store the bun.
     ROOT_PATH = os.path.join(Reflex.DIR, "bun")
     # Default bun path.
     DEFAULT_PATH = os.path.join(
         ROOT_PATH, "bin", "bun" if not IS_WINDOWS else "bun.exe"
@@ -119,8 +119,9 @@
         "react-focus-lock": "2.11.3",
         "socket.io-client": "4.6.1",
         "universal-cookie": "4.0.4",
     }
     DEV_DEPENDENCIES = {
         "autoprefixer": "10.4.14",
         "postcss": "8.4.31",
+        "postcss-import": "16.1.0",
     }
```

### Comparing `reflex-0.5.2a1/reflex/constants/route.py` & `reflex-0.5.3a1/reflex/constants/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/constants/style.py` & `reflex-0.5.3a1/reflex/constants/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/custom_components/custom_components.py` & `reflex-0.5.3a1/reflex/custom_components/custom_components.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/event.py` & `reflex-0.5.3a1/reflex/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/experimental/__init__.py` & `reflex-0.5.3a1/reflex/experimental/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 
 from reflex.components.props import PropsBase
 from reflex.components.radix.themes.components.progress import progress as progress
 from reflex.components.sonner.toast import toast as toast
 
 from ..utils.console import warn
 from . import hooks as hooks
+from .assets import asset as asset
 from .client_state import ClientStateVar as ClientStateVar
 from .layout import layout as layout
 from .misc import run_in_thread as run_in_thread
 
 warn(
     "`rx._x` contains experimental features and might be removed at any time in the future .",
 )
 
 _x = SimpleNamespace(
+    asset=asset,
     client_state=ClientStateVar.create,
     hooks=hooks,
     layout=layout,
     progress=progress,
     PropsBase=PropsBase,
     run_in_thread=run_in_thread,
     toast=toast,
```

### Comparing `reflex-0.5.2a1/reflex/experimental/client_state.py` & `reflex-0.5.3a1/reflex/experimental/client_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Handle client side state with `useState`."""
 
 import dataclasses
 import sys
-from typing import Any, Callable, Optional, Type
+from typing import Any, Callable, Optional, Type, Union
 
 from reflex import constants
 from reflex.event import EventChain, EventHandler, EventSpec, call_script
 from reflex.utils.imports import ImportVar
 from reflex.vars import Var, VarData
 
 
@@ -167,15 +167,17 @@
                     imports={
                         f"/{constants.Dirs.STATE_PATH}": [ImportVar(tag="refs")],
                     }
                 )
             )
         )
 
-    def retrieve(self, callback: EventHandler | Callable | None = None) -> EventSpec:
+    def retrieve(
+        self, callback: Union[EventHandler, Callable, None] = None
+    ) -> EventSpec:
         """Pass the value of the client state variable to a backend EventHandler.
 
         The event handler must `yield` or `return` the EventSpec to trigger the event.
 
         Args:
             callback: The callback to pass the value to.
```

### Comparing `reflex-0.5.2a1/reflex/experimental/hooks.py` & `reflex-0.5.3a1/reflex/experimental/hooks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 """Add standard Hooks wrapper for React."""
 
+from typing import Optional, Union
+
 from reflex.utils.imports import ImportVar
 from reflex.vars import Var, VarData
 
 
-def _add_react_import(v: Var | None, tags: str | list):
+def _add_react_import(v: Optional[Var], tags: Union[str, list]):
     if v is None:
         return
 
     if isinstance(tags, str):
         tags = [tags]
 
     v._var_data = VarData(  # type: ignore
         imports={"react": [ImportVar(tag=tag, install=False) for tag in tags]},
     )
 
 
-def const(name, value) -> Var | None:
+def const(name, value) -> Optional[Var]:
     """Create a constant Var.
 
     Args:
         name: The name of the constant.
         value: The value of the constant.
 
     Returns:
         The constant Var.
     """
     if isinstance(name, list):
         return Var.create(f"const [{', '.join(name)}] = {value}")
     return Var.create(f"const {name} = {value}")
 
 
-def useCallback(func, deps) -> Var | None:
+def useCallback(func, deps) -> Optional[Var]:
     """Create a useCallback hook with a function and dependencies.
 
     Args:
         func: The function to wrap.
         deps: The dependencies of the function.
 
     Returns:
@@ -45,43 +47,43 @@
         v = Var.create(f"useCallback({func}, {deps})")
     else:
         v = Var.create(f"useCallback({func})")
     _add_react_import(v, "useCallback")
     return v
 
 
-def useContext(context) -> Var | None:
+def useContext(context) -> Optional[Var]:
     """Create a useContext hook with a context.
 
     Args:
         context: The context to use.
 
     Returns:
         The useContext hook.
     """
     v = Var.create(f"useContext({context})")
     _add_react_import(v, "useContext")
     return v
 
 
-def useRef(default) -> Var | None:
+def useRef(default) -> Optional[Var]:
     """Create a useRef hook with a default value.
 
     Args:
         default: The default value of the ref.
 
     Returns:
         The useRef hook.
     """
     v = Var.create(f"useRef({default})")
     _add_react_import(v, "useRef")
     return v
 
 
-def useState(var_name, default=None) -> Var | None:
+def useState(var_name, default=None) -> Optional[Var]:
     """Create a useState hook with a variable name and setter name.
 
     Args:
         var_name: The name of the variable.
         default: The default value of the variable.
 
     Returns:
```

### Comparing `reflex-0.5.2a1/reflex/experimental/layout.py` & `reflex-0.5.3a1/reflex/experimental/layout.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from typing import Any
 
 from reflex import color, cond
 from reflex.components.base.fragment import Fragment
 from reflex.components.component import Component, ComponentNamespace, MemoizationLeaf
 from reflex.components.radix.primitives.drawer import DrawerRoot, drawer
 from reflex.components.radix.themes.components.icon_button import IconButton
-from reflex.components.radix.themes.layout import Box, Container, HStack
+from reflex.components.radix.themes.layout.box import Box
+from reflex.components.radix.themes.layout.container import Container
+from reflex.components.radix.themes.layout.stack import HStack
 from reflex.event import call_script
 from reflex.experimental import hooks
 from reflex.state import ComponentState
 from reflex.style import Style
 from reflex.vars import Var
```

### Comparing `reflex-0.5.2a1/reflex/middleware/hydrate_middleware.py` & `reflex-0.5.3a1/reflex/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/middleware/middleware.py` & `reflex-0.5.3a1/reflex/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/model.py` & `reflex-0.5.3a1/reflex/model.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/page.py` & `reflex-0.5.3a1/reflex/page.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/reflex.py` & `reflex-0.5.3a1/reflex/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/route.py` & `reflex-0.5.3a1/reflex/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/state.py` & `reflex-0.5.3a1/reflex/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 
 import asyncio
 import contextlib
 import copy
 import functools
 import inspect
+import os
 import traceback
 import uuid
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from types import FunctionType, MethodType
 from typing import (
     TYPE_CHECKING,
@@ -31,14 +32,15 @@
 try:
     import pydantic.v1 as pydantic
 except ModuleNotFoundError:
     import pydantic
 
 import wrapt
 from redis.asyncio import Redis
+from redis.exceptions import ResponseError
 
 from reflex import constants
 from reflex.base import Base
 from reflex.event import (
     BACKGROUND_TASK_MARKER,
     Event,
     EventHandler,
@@ -1532,14 +1534,26 @@
             for cvar in self._dirty_computed_vars(from_vars=calc_vars):
                 self.dirty_vars.add(cvar)
                 dirty_vars.add(cvar)
                 actual_var = self.computed_vars.get(cvar)
                 if actual_var is not None:
                     actual_var.mark_dirty(instance=self)
 
+    def _expired_computed_vars(self) -> set[str]:
+        """Determine ComputedVars that need to be recalculated based on the expiration time.
+
+        Returns:
+            Set of computed vars to include in the delta.
+        """
+        return set(
+            cvar
+            for cvar in self.computed_vars
+            if self.computed_vars[cvar].needs_update(instance=self)
+        )
+
     def _dirty_computed_vars(self, from_vars: set[str] | None = None) -> set[str]:
         """Determine ComputedVars that need to be recalculated based on the given vars.
 
         Args:
             from_vars: find ComputedVar that depend on this set of vars. If unspecified, will use the dirty_vars.
 
         Returns:
@@ -1584,14 +1598,15 @@
         self.dirty_vars.update(self._always_dirty_computed_vars)
         self._mark_dirty()
 
         # Return the dirty vars for this instance, any cached/dependent computed vars,
         # and always dirty computed vars (cache=False)
         delta_vars = (
             self.dirty_vars.intersection(self.base_vars)
+            .union(self.dirty_vars.intersection(self.computed_vars))
             .union(self._dirty_computed_vars())
             .union(self._always_dirty_computed_vars)
         )
 
         subdelta = {
             prop: getattr(self, prop)
             for prop in delta_vars
@@ -1617,14 +1632,17 @@
         if (
             self.parent_state is not None
             and state_name not in self.parent_state.dirty_substates
         ):
             self.parent_state.dirty_substates.add(self.get_name())
             self.parent_state._mark_dirty()
 
+        # Append expired computed vars to dirty_vars to trigger recalculation
+        self.dirty_vars.update(self._expired_computed_vars())
+
         # have to mark computed vars dirty to allow access to newly computed
         # values within the same ComputedVar function
         self._mark_dirty_computed_vars()
         self._mark_dirty_substates()
 
     def _mark_dirty_substates(self):
         """Propagate dirty var / computed var status into substates."""
@@ -2618,21 +2636,34 @@
         """Wait for a redis lock to be released via pubsub.
 
         Coroutine will not return until the lock is obtained.
 
         Args:
             lock_key: The redis key for the lock.
             lock_id: The ID of the lock.
+
+        Raises:
+            ResponseError: when the keyspace config cannot be set.
         """
         state_is_locked = False
         lock_key_channel = f"__keyspace@0__:{lock_key.decode()}"
         # Enable keyspace notifications for the lock key, so we know when it is available.
-        await self.redis.config_set(
-            "notify-keyspace-events", self._redis_notify_keyspace_events
-        )
+        try:
+            await self.redis.config_set(
+                "notify-keyspace-events",
+                self._redis_notify_keyspace_events,
+            )
+        except ResponseError:
+            # Some redis servers only allow out-of-band configuration, so ignore errors here.
+            ignore_config_error = os.environ.get(
+                "REFLEX_IGNORE_REDIS_CONFIG_ERROR",
+                None,
+            )
+            if not ignore_config_error:
+                raise
         async with self.redis.pubsub() as pubsub:
             await pubsub.psubscribe(lock_key_channel)
             while not state_is_locked:
                 # wait for the lock to be released
                 while True:
                     if not await self.redis.exists(lock_key):
                         break  # key was removed, try to get the lock again
@@ -2832,14 +2863,19 @@
     __wrap_mutable_attrs__ = set(
         [
             "get",
             "setdefault",
         ]
     )
 
+    # These internal attributes on rx.Base should NOT be wrapped in a MutableProxy.
+    __never_wrap_base_attrs__ = set(Base.__dict__) - {"set"} | set(
+        pydantic.BaseModel.__dict__
+    )
+
     __mutable_types__ = (list, dict, set, Base)
 
     def __init__(self, wrapped: Any, state: BaseState, field_name: str):
         """Create a proxy for a mutable object that tracks changes.
 
         Args:
             wrapped: The object to proxy.
@@ -2881,15 +2917,18 @@
 
         Args:
             value: The value to wrap.
 
         Returns:
             The wrapped value.
         """
-        if isinstance(value, self.__mutable_types__):
+        # Recursively wrap mutable types, but do not re-wrap MutableProxy instances.
+        if isinstance(value, self.__mutable_types__) and not isinstance(
+            value, MutableProxy
+        ):
             return type(self)(
                 wrapped=value,
                 state=self._self_state,
                 field_name=self._self_field_name,
             )
         return value
 
@@ -2928,14 +2967,25 @@
             if __name in self.__wrap_mutable_attrs__:
                 # Wrap methods that may return mutable objects tied to the state.
                 value = wrapt.FunctionWrapper(
                     value,
                     self._wrap_recursive_decorator,
                 )
 
+            if (
+                isinstance(self.__wrapped__, Base)
+                and __name not in self.__never_wrap_base_attrs__
+                and hasattr(value, "__func__")
+            ):
+                # Wrap methods called on Base subclasses, which might do _anything_
+                return wrapt.FunctionWrapper(
+                    functools.partial(value.__func__, self),
+                    self._wrap_recursive_decorator,
+                )
+
         if isinstance(value, self.__mutable_types__) and __name not in (
             "__wrapped__",
             "_self_state",
         ):
             # Recursively wrap mutable attribute values retrieved through this proxy.
             return self._wrap_recursive(value)
```

### Comparing `reflex-0.5.2a1/reflex/style.py` & `reflex-0.5.3a1/reflex/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/testing.py` & `reflex-0.5.3a1/reflex/testing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/utils/build.py` & `reflex-0.5.3a1/reflex/utils/build.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/utils/compat.py` & `reflex-0.5.3a1/reflex/utils/compat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/utils/console.py` & `reflex-0.5.3a1/reflex/utils/console.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/utils/exceptions.py` & `reflex-0.5.3a1/reflex/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/utils/exec.py` & `reflex-0.5.3a1/reflex/utils/exec.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,14 +109,22 @@
                         if get_config().frontend_path != "":
                             url = urljoin(url, get_config().frontend_path)
                         console.print(f"App running at: [bold green]{url}")
                         first_run = False
                     else:
                         console.print("New packages detected: Updating app...")
                 else:
+                    if any(
+                        [x in line for x in ("bin executable does not exist on disk",)]
+                    ):
+                        console.error(
+                            "Try setting `REFLEX_USE_NPM=1` and re-running `reflex init` and `reflex run` to use npm instead of bun:\n"
+                            "`REFLEX_USE_NPM=1 reflex init`\n"
+                            "`REFLEX_USE_NPM=1 reflex run`"
+                        )
                     new_hash = detect_package_change(json_file_path)
                     if new_hash != last_hash:
                         last_hash = new_hash
                         kill(process.pid)
                         process = None
                         break  # for line in process.stdout
         if process is not None:
```

### Comparing `reflex-0.5.2a1/reflex/utils/export.py` & `reflex-0.5.3a1/reflex/utils/export.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/utils/format.py` & `reflex-0.5.3a1/reflex/utils/format.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/utils/imports.py` & `reflex-0.5.3a1/reflex/utils/imports.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/utils/path_ops.py` & `reflex-0.5.3a1/reflex/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/utils/prerequisites.py` & `reflex-0.5.3a1/reflex/utils/prerequisites.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,27 +328,14 @@
     redis_url, has_port, redis_port = config.redis_url.partition(":")
     if not has_port:
         redis_port = 6379
     console.info(f"Using redis at {config.redis_url}")
     return dict(host=redis_url, port=int(redis_port), db=0)
 
 
-def get_production_backend_url() -> str:
-    """Get the production backend URL.
-
-    Returns:
-        The production backend URL.
-    """
-    config = get_config()
-    return constants.PRODUCTION_BACKEND_URL.format(
-        username=config.username,
-        app_name=config.app_name,
-    )
-
-
 def validate_app_name(app_name: str | None = None) -> str:
     """Validate the app name.
 
     The default app name is the name of the current directory.
 
     Args:
         app_name: the name passed by user during reflex init
@@ -621,15 +608,15 @@
 
 def _update_next_config(
     config: Config, export: bool = False, transpile_packages: Optional[List[str]] = None
 ):
     next_config = {
         "basePath": config.frontend_path or "",
         "compress": config.next_compression,
-        "reactStrictMode": True,
+        "reactStrictMode": config.react_strict_mode,
         "trailingSlash": True,
     }
     if transpile_packages:
         next_config["transpilePackages"] = list(
             set((format_library_name(p) for p in transpile_packages))
         )
     if export:
```

### Comparing `reflex-0.5.2a1/reflex/utils/processes.py` & `reflex-0.5.3a1/reflex/utils/processes.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/utils/pyi_generator.py` & `reflex-0.5.3a1/reflex/utils/pyi_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,19 +25,17 @@
 
 from reflex.components.component import Component
 from reflex.utils import types as rx_types
 from reflex.vars import Var
 
 logger = logging.getLogger("pyi_generator")
 
-INIT_FILE = Path("reflex/__init__.pyi").resolve()
 PWD = Path(".").resolve()
 
 EXCLUDED_FILES = [
-    "__init__.py",
     # "app.py",
     "component.py",
     "bare.py",
     "foreach.py",
     "cond.py",
     "match.py",
     "multiselect.py",
@@ -318,21 +316,23 @@
     Returns:
         The list of props as ast arg nodes
     """
     spec = getfullargspec(func)
     all_props = []
     kwargs = []
     for target_class in clzs:
+        event_triggers = target_class().get_event_triggers()
         # Import from the target class to ensure type hints are resolvable.
         exec(f"from {target_class.__module__} import *", type_hint_globals)
         for name, value in target_class.__annotations__.items():
             if (
                 name in spec.kwonlyargs
                 or name in EXCLUDED_PROPS
                 or name in all_props
+                or name in event_triggers
                 or (isinstance(value, str) and "ClassVar" in value)
             ):
                 continue
             all_props.append(name)
 
             default = None
             if extract_real_default:
@@ -771,14 +771,21 @@
         ):
             return node
 
         if self._current_class_is_component():
             # Remove annotated assignments in Component classes (props)
             return None
 
+        # remove dunder method assignments for lazy_loader.attach
+        for target in node.targets:
+            if isinstance(target, ast.Tuple):
+                for name in target.elts:
+                    if isinstance(name, ast.Name) and name.id.startswith("_"):
+                        return
+
         return node
 
     def visit_AnnAssign(self, node: ast.AnnAssign) -> ast.AnnAssign | None:
         """Visit an AnnAssign node (Annotated assignment).
 
         Remove private target and remove the assignment value in the stub.
 
@@ -801,14 +808,31 @@
             # Remove annotated assignments in Component classes (props)
             return None
         # Blank out assignments in type stubs.
         node.value = None
         return node
 
 
+class InitStubGenerator(StubGenerator):
+    """A node transformer that will generate the stubs for a given init file."""
+
+    def visit_Import(
+        self, node: ast.Import | ast.ImportFrom
+    ) -> ast.Import | ast.ImportFrom | list[ast.Import | ast.ImportFrom]:
+        """Collect import statements from the init module.
+
+        Args:
+            node: The import node to visit.
+
+        Returns:
+                The modified import node(s).
+        """
+        return [node]
+
+
 class PyiGenerator:
     """A .pyi file generator that will scan all defined Component in Reflex and
     generate the approriate stub.
     """
 
     modules: list = []
     root: str = ""
@@ -838,14 +862,45 @@
         else:
             pyi_content = source.splitlines()
 
         pyi_path = module_path.with_suffix(".pyi")
         pyi_path.write_text("\n".join(pyi_content))
         logger.info(f"Wrote {relpath}")
 
+    def _get_init_lazy_imports(self, mod, new_tree):
+        # retrieve the _SUBMODULES and _SUBMOD_ATTRS from an init file if present.
+        sub_mods = getattr(mod, "_SUBMODULES", None)
+        sub_mod_attrs = getattr(mod, "_SUBMOD_ATTRS", None)
+
+        if not sub_mods and not sub_mod_attrs:
+            return
+        sub_mods_imports = []
+        sub_mod_attrs_imports = []
+
+        if sub_mods:
+            sub_mods_imports = [
+                f"from . import {mod} as {mod}" for mod in sorted(sub_mods)
+            ]
+            sub_mods_imports.append("")
+
+        if sub_mod_attrs:
+            sub_mod_attrs = {
+                attr: mod for mod, attrs in sub_mod_attrs.items() for attr in attrs
+            }
+            # construct the import statement and handle special cases for aliases
+            sub_mod_attrs_imports = [
+                f"from .{path} import {mod if not isinstance(mod, tuple) else mod[0]} as {mod if not isinstance(mod, tuple) else mod[1]}"
+                for mod, path in sub_mod_attrs.items()
+            ]
+            sub_mod_attrs_imports.append("")
+
+        text = "\n" + "\n".join([*sub_mods_imports, *sub_mod_attrs_imports])
+        text += ast.unparse(new_tree) + "\n"
+        return text
+
     def _scan_file(self, module_path: Path):
         module_import = (
             _relative_to_pwd(module_path)
             .with_suffix("")
             .as_posix()
             .replace("/", ".")
             .replace("\\", ".")
@@ -856,21 +911,30 @@
             name: obj
             for name, obj in vars(module).items()
             if inspect.isclass(obj)
             and (issubclass(obj, Component) or issubclass(obj, SimpleNamespace))
             and obj != Component
             and inspect.getmodule(obj) == module
         }
-        if not class_names:
+        is_init_file = _relative_to_pwd(module_path).name == "__init__.py"
+        if not class_names and not is_init_file:
             return
 
-        new_tree = StubGenerator(module, class_names).visit(
-            ast.parse(inspect.getsource(module))
-        )
-        self._write_pyi_file(module_path, ast.unparse(new_tree))
+        if is_init_file:
+            new_tree = InitStubGenerator(module, class_names).visit(
+                ast.parse(inspect.getsource(module))
+            )
+            init_imports = self._get_init_lazy_imports(module, new_tree)
+            if init_imports:
+                self._write_pyi_file(module_path, init_imports)
+        else:
+            new_tree = StubGenerator(module, class_names).visit(
+                ast.parse(inspect.getsource(module))
+            )
+            self._write_pyi_file(module_path, ast.unparse(new_tree))
 
     def _scan_files_multiprocess(self, files: list[Path]):
         with Pool(processes=cpu_count()) as pool:
             pool.map(self._scan_file, files)
 
     def _scan_files(self, files: list[Path]):
         for file in files:
@@ -918,20 +982,7 @@
                     continue
                 subprocess.run(["git", "checkout", changed_file])
 
         if cpu_count() == 1 or len(file_targets) < 5:
             self._scan_files(file_targets)
         else:
             self._scan_files_multiprocess(file_targets)
-
-
-def generate_init():
-    """Generate a pyi file for the main __init__.py."""
-    from reflex import _MAPPING  # type: ignore
-
-    imports = [
-        f"from {path if mod != path.rsplit('.')[-1] or mod == 'page' else '.'.join(path.rsplit('.')[:-1])} import {mod} as {mod}"
-        for mod, path in _MAPPING.items()
-    ]
-    imports.append("")
-    with contextlib.suppress(Exception):
-        INIT_FILE.write_text("\n".join(imports))
```

### Comparing `reflex-0.5.2a1/reflex/utils/serializers.py` & `reflex-0.5.3a1/reflex/utils/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,15 @@
 def serialize_enum(en: Enum) -> str:
     """Serialize a enum to a JSON string.
 
     Args:
         en: The enum to serialize.
 
     Returns:
-         The serialized enum.
+        The serialized enum.
     """
     return en.value
 
 
 @serializer
 def serialize_color(color: Color) -> str:
     """Serialize a color.
@@ -309,24 +309,24 @@
     pass
 
 try:
     from plotly.graph_objects import Figure
     from plotly.io import to_json
 
     @serializer
-    def serialize_figure(figure: Figure) -> list:
+    def serialize_figure(figure: Figure) -> dict:
         """Serialize a plotly figure.
 
         Args:
             figure: The figure to serialize.
 
         Returns:
             The serialized figure.
         """
-        return json.loads(str(to_json(figure)))["data"]
+        return json.loads(str(to_json(figure)))
 
 except ImportError:
     pass
 
 
 try:
     import base64
```

### Comparing `reflex-0.5.2a1/reflex/utils/telemetry.py` & `reflex-0.5.3a1/reflex/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/utils/types.py` & `reflex-0.5.3a1/reflex/utils/types.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/utils/watch.py` & `reflex-0.5.3a1/reflex/utils/watch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.5.2a1/reflex/vars.py` & `reflex-0.5.3a1/reflex/vars.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Define a state var."""
 
 from __future__ import annotations
 
 import contextlib
 import dataclasses
+import datetime
 import dis
 import functools
 import inspect
 import json
 import random
 import re
 import string
@@ -1869,33 +1870,58 @@
 @dataclasses.dataclass(init=False, eq=False)
 class ComputedVar(Var, property):
     """A field with computed getters."""
 
     # Whether to track dependencies and cache computed values
     _cache: bool = dataclasses.field(default=False)
 
-    _initial_value: Any | types.Unset = dataclasses.field(default_factory=types.Unset)
+    # The initial value of the computed var
+    _initial_value: Any | types.Unset = dataclasses.field(default=types.Unset())
+
+    # Explicit var dependencies to track
+    _static_deps: set[str] = dataclasses.field(default_factory=set)
+
+    # Whether var dependencies should be auto-determined
+    _auto_deps: bool = dataclasses.field(default=True)
+
+    # Interval at which the computed var should be updated
+    _update_interval: Optional[datetime.timedelta] = dataclasses.field(default=None)
 
     def __init__(
         self,
         fget: Callable[[BaseState], Any],
         initial_value: Any | types.Unset = types.Unset(),
         cache: bool = False,
+        deps: Optional[List[Union[str, Var]]] = None,
+        auto_deps: bool = True,
+        interval: Optional[Union[int, datetime.timedelta]] = None,
         **kwargs,
     ):
         """Initialize a ComputedVar.
 
         Args:
             fget: The getter function.
             initial_value: The initial value of the computed var.
             cache: Whether to cache the computed value.
+            deps: Explicit var dependencies to track.
+            auto_deps: Whether var dependencies should be auto-determined.
+            interval: Interval at which the computed var should be updated.
             **kwargs: additional attributes to set on the instance
         """
         self._initial_value = initial_value
         self._cache = cache
+        if isinstance(interval, int):
+            interval = datetime.timedelta(seconds=interval)
+        self._update_interval = interval
+        if deps is None:
+            deps = []
+        self._static_deps = {
+            dep._var_name if isinstance(dep, Var) else dep for dep in deps
+        }
+        self._auto_deps = auto_deps
         property.__init__(self, fget)
         kwargs["_var_name"] = kwargs.pop("_var_name", fget.__name__)
         kwargs["_var_type"] = kwargs.pop("_var_type", self._determine_var_type())
         BaseVar.__init__(self, **kwargs)  # type: ignore
 
     @override
     def _replace(self, merge_var_data=None, **kwargs: Any) -> ComputedVar:
@@ -1908,14 +1934,17 @@
         Returns:
             The new ComputedVar instance.
         """
         return ComputedVar(
             fget=kwargs.get("fget", self.fget),
             initial_value=kwargs.get("initial_value", self._initial_value),
             cache=kwargs.get("cache", self._cache),
+            deps=kwargs.get("deps", self._static_deps),
+            auto_deps=kwargs.get("auto_deps", self._auto_deps),
+            interval=kwargs.get("interval", self._update_interval),
             _var_name=kwargs.get("_var_name", self._var_name),
             _var_type=kwargs.get("_var_type", self._var_type),
             _var_is_local=kwargs.get("_var_is_local", self._var_is_local),
             _var_is_string=kwargs.get("_var_is_string", self._var_is_string),
             _var_full_name_needs_state_prefix=kwargs.get(
                 "_var_full_name_needs_state_prefix",
                 self._var_full_name_needs_state_prefix,
@@ -1928,15 +1957,40 @@
         """Get the attribute used to cache the value on the instance.
 
         Returns:
             An attribute name.
         """
         return f"__cached_{self._var_name}"
 
-    def __get__(self, instance, owner):
+    @property
+    def _last_updated_attr(self) -> str:
+        """Get the attribute used to store the last updated timestamp.
+
+        Returns:
+            An attribute name.
+        """
+        return f"__last_updated_{self._var_name}"
+
+    def needs_update(self, instance: BaseState) -> bool:
+        """Check if the computed var needs to be updated.
+
+        Args:
+            instance: The state instance that the computed var is attached to.
+
+        Returns:
+            True if the computed var needs to be updated, False otherwise.
+        """
+        if self._update_interval is None:
+            return False
+        last_updated = getattr(instance, self._last_updated_attr, None)
+        if last_updated is None:
+            return True
+        return datetime.datetime.now() - last_updated > self._update_interval
+
+    def __get__(self, instance: BaseState | None, owner):
         """Get the ComputedVar value.
 
         If the value is already cached on the instance, return the cached value.
 
         Args:
             instance: the instance of the class accessing this computed var.
             owner: the class that this descriptor is attached to.
@@ -1944,18 +1998,21 @@
         Returns:
             The value of the var for the given instance.
         """
         if instance is None or not self._cache:
             return super().__get__(instance, owner)
 
         # handle caching
-        if not hasattr(instance, self._cache_attr):
+        if not hasattr(instance, self._cache_attr) or self.needs_update(instance):
+            # Set cache attr on state instance.
             setattr(instance, self._cache_attr, super().__get__(instance, owner))
             # Ensure the computed var gets serialized to redis.
             instance._was_touched = True
+            # Set the last updated timestamp on the state instance.
+            setattr(instance, self._last_updated_attr, datetime.datetime.now())
         return getattr(instance, self._cache_attr)
 
     def _deps(
         self,
         objclass: Type,
         obj: FunctionType | CodeType | None = None,
         self_name: Optional[str] = None,
@@ -1974,15 +2031,17 @@
         Returns:
             A set of variable names accessed by the given obj.
 
         Raises:
             VarValueError: if the function references the get_state, parent_state, or substates attributes
                 (cannot track deps in a related state, only implicitly via parent state).
         """
-        d = set()
+        if not self._auto_deps:
+            return self._static_deps
+        d = self._static_deps.copy()
         if obj is None:
             fget = property.__getattribute__(self, "fget")
             if fget is not None:
                 obj = cast(FunctionType, fget)
             else:
                 return set()
         with contextlib.suppress(AttributeError):
@@ -2072,35 +2131,50 @@
         return Any
 
 
 def computed_var(
     fget: Callable[[BaseState], Any] | None = None,
     initial_value: Any | None = None,
     cache: bool = False,
+    deps: Optional[List[Union[str, Var]]] = None,
+    auto_deps: bool = True,
+    interval: Optional[Union[datetime.timedelta, int]] = None,
     **kwargs,
 ) -> ComputedVar | Callable[[Callable[[BaseState], Any]], ComputedVar]:
     """A ComputedVar decorator with or without kwargs.
 
     Args:
         fget: The getter function.
         initial_value: The initial value of the computed var.
         cache: Whether to cache the computed value.
+        deps: Explicit var dependencies to track.
+        auto_deps: Whether var dependencies should be auto-determined.
+        interval: Interval at which the computed var should be updated.
         **kwargs: additional attributes to set on the instance
 
     Returns:
         A ComputedVar instance.
+
+    Raises:
+        ValueError: If caching is disabled and an update interval is set.
     """
+    if cache is False and interval is not None:
+        raise ValueError("Cannot set update interval without caching.")
+
     if fget is not None:
         return ComputedVar(fget=fget, cache=cache)
 
-    def wrapper(fget):
+    def wrapper(fget: Callable[[BaseState], Any]) -> ComputedVar:
         return ComputedVar(
             fget=fget,
             initial_value=initial_value,
             cache=cache,
+            deps=deps,
+            auto_deps=auto_deps,
+            interval=interval,
             **kwargs,
         )
 
     return wrapper
 
 
 # Partial function of computed_var with cache=True
```

### Comparing `reflex-0.5.2a1/reflex/vars.pyi` & `reflex-0.5.3a1/reflex/vars.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ Generated with stubgen from mypy, then manually edited, do not regen."""
 
 from __future__ import annotations
 
+import datetime
 from dataclasses import dataclass
 from _typeshed import Incomplete
 from reflex import constants as constants
 from reflex.base import Base as Base
 from reflex.state import State as State
 from reflex.state import BaseState as BaseState
 from reflex.utils import console as console, format as format, types as types
@@ -137,32 +138,47 @@
     fget: FunctionType
     @property
     def _cache_attr(self) -> str: ...
     def __get__(self, instance, owner): ...
     def _deps(self, objclass: Type, obj: Optional[FunctionType] = ...) -> Set[str]: ...
     def _replace(self, merge_var_data=None, **kwargs: Any) -> ComputedVar: ...
     def mark_dirty(self, instance) -> None: ...
+    def needs_update(self, instance) -> bool: ...
     def _determine_var_type(self) -> Type: ...
     @overload
     def __init__(
         self,
         fget: Callable[[BaseState], Any],
         **kwargs,
     ) -> None: ...
     @overload
     def __init__(self, func) -> None: ...
 
 @overload
 def computed_var(
     fget: Callable[[BaseState], Any] | None = None,
     initial_value: Any | None = None,
+    cache: bool = False,
+    deps: Optional[List[Union[str, Var]]] = None,
+    auto_deps: bool = True,
+    interval: Optional[Union[datetime.timedelta, int]] = None,
     **kwargs,
 ) -> Callable[[Callable[[Any], Any]], ComputedVar]: ...
 @overload
 def computed_var(fget: Callable[[Any], Any]) -> ComputedVar: ...
+@overload
+def cached_var(
+    fget: Callable[[BaseState], Any] | None = None,
+    initial_value: Any | None = None,
+    deps: Optional[List[Union[str, Var]]] = None,
+    auto_deps: bool = True,
+    interval: Optional[Union[datetime.timedelta, int]] = None,
+    **kwargs,
+) -> Callable[[Callable[[Any], Any]], ComputedVar]: ...
+@overload
 def cached_var(fget: Callable[[Any], Any]) -> ComputedVar: ...
 
 class CallableVar(BaseVar):
     def __init__(self, fn: Callable[..., BaseVar]): ...
     def __call__(self, *args, **kwargs) -> BaseVar: ...
 
 def get_uuid_string_var() -> Var: ...
```

### Comparing `reflex-0.5.2a1/PKG-INFO` & `reflex-0.5.3a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex
-Version: 0.5.2a1
+Version: 0.5.3a1
 Summary: Web apps in pure Python.
 Home-page: https://reflex.dev
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@reflex.dev
 Requires-Python: >=3.8,<4.0
@@ -21,14 +21,15 @@
 Requires-Dist: charset-normalizer (>=3.3.2,<4.0)
 Requires-Dist: dill (>=0.3.8,<0.4)
 Requires-Dist: distro (>=1.8.0,<2.0) ; sys_platform == "linux"
 Requires-Dist: fastapi (>=0.96.0,<1.0)
 Requires-Dist: gunicorn (>=20.1.0,<23.0)
 Requires-Dist: httpx (>=0.25.1,<1.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0)
+Requires-Dist: lazy_loader (>=0.4)
 Requires-Dist: packaging (>=23.1,<25.0)
 Requires-Dist: platformdirs (>=3.10.0,<5.0)
 Requires-Dist: psutil (>=5.9.4,<6.0)
 Requires-Dist: pydantic (>=1.10.2,<3.0)
 Requires-Dist: python-engineio (!=4.6.0)
 Requires-Dist: python-multipart (>=0.0.5,<0.1)
 Requires-Dist: python-socketio (>=5.7.0,<6.0)
```

