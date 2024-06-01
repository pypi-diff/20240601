# Comparing `tmp/tikhub-1.10.1.tar.gz` & `tmp/tikhub-1.10.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tikhub-1.10.1.tar", last modified: Thu May 30 12:40:52 2024, max compression
+gzip compressed data, was "tikhub-1.10.2.tar", last modified: Sat Jun  1 00:50:28 2024, max compression
```

## Comparing `tikhub-1.10.1.tar` & `tikhub-1.10.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.878707 tikhub-1.10.1/
--rw-rw-rw-   0        0        0    11558 2024-05-21 08:59:32.000000 tikhub-1.10.1/LICENSE
--rw-rw-rw-   0        0        0       36 2024-05-30 11:25:11.000000 tikhub-1.10.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3235 2024-05-30 12:40:52.877707 tikhub-1.10.1/PKG-INFO
--rw-rw-rw-   0        0        0     2709 2024-05-30 11:39:24.000000 tikhub-1.10.1/README.md
--rw-rw-rw-   0        0        0       93 2024-05-30 11:27:47.000000 tikhub-1.10.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-30 12:40:52.878707 tikhub-1.10.1/setup.cfg
--rw-rw-rw-   0        0        0      976 2024-05-30 12:40:51.000000 tikhub-1.10.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.845054 tikhub-1.10.1/tikhub/
--rw-rw-rw-   0        0        0       59 2024-05-30 12:40:12.000000 tikhub-1.10.1/tikhub/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.848867 tikhub-1.10.1/tikhub/api/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.10.1/tikhub/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.849866 tikhub-1.10.1/tikhub/api/v1/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.10.1/tikhub/api/v1/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.849866 tikhub-1.10.1/tikhub/api/v1/endpoints/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:06:51.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.850867 tikhub-1.10.1/tikhub/api/v1/endpoints/captcha/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:16:46.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/captcha/__init__.py
--rw-rw-rw-   0        0        0      478 2024-05-30 12:14:39.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/captcha/captcha_solver.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.852371 tikhub-1.10.1/tikhub/api/v1/endpoints/douyin/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/douyin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.855375 tikhub-1.10.1/tikhub/api/v1/endpoints/douyin/app/
--rw-rw-rw-   0        0        0        0 2024-05-21 11:57:03.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/douyin/app/__init__.py
--rw-rw-rw-   0        0        0    14139 2024-05-30 12:14:39.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/douyin/app/douyin_app_v1.py
--rw-rw-rw-   0        0        0    15959 2024-05-30 12:14:39.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/douyin/app/douyin_app_v2.py
--rw-rw-rw-   0        0        0    12565 2024-05-30 12:14:39.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/douyin/app/douyin_app_v3.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.856375 tikhub-1.10.1/tikhub/api/v1/endpoints/douyin/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/douyin/web/__init__.py
--rw-rw-rw-   0        0        0    31217 2024-05-30 12:14:39.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/douyin/web/douyin_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.857375 tikhub-1.10.1/tikhub/api/v1/endpoints/instagram/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:14:52.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/instagram/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.858376 tikhub-1.10.1/tikhub/api/v1/endpoints/instagram/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:14:52.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/instagram/web/__init__.py
--rw-rw-rw-   0        0        0      961 2024-05-30 12:14:39.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/instagram/web/instagram_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.860375 tikhub-1.10.1/tikhub/api/v1/endpoints/tikhub/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:07.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/tikhub/__init__.py
--rw-rw-rw-   0        0        0     3246 2024-05-30 12:14:39.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/tikhub/tikhub_user.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.860375 tikhub-1.10.1/tikhub/api/v1/endpoints/tiktok/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:32.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/tiktok/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.862878 tikhub-1.10.1/tikhub/api/v1/endpoints/tiktok/app/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:32.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/tiktok/app/__init__.py
--rw-rw-rw-   0        0        0    13951 2024-05-30 12:14:39.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v2.py
--rw-rw-rw-   0        0        0    22972 2024-05-30 12:14:39.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v3.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.863882 tikhub-1.10.1/tikhub/api/v1/endpoints/tiktok/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:37.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/tiktok/web/__init__.py
--rw-rw-rw-   0        0        0    13858 2024-05-30 12:14:39.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/tiktok/web/tiktok_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.864882 tikhub-1.10.1/tikhub/api/v1/endpoints/weibo/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:58.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/weibo/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.865882 tikhub-1.10.1/tikhub/api/v1/endpoints/weibo/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:58.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/weibo/web/__init__.py
--rw-rw-rw-   0        0        0     1834 2024-05-30 12:14:39.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/weibo/web/weibo_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.866883 tikhub-1.10.1/tikhub/api/v1/endpoints/xiaohongshu/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:16:23.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/xiaohongshu/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.867883 tikhub-1.10.1/tikhub/api/v1/endpoints/xiaohongshu/app/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:16:23.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/xiaohongshu/app/__init__.py
--rw-rw-rw-   0        0        0      664 2024-05-04 23:05:56.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/xiaohongshu/app/xiaohongshu_app.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.868882 tikhub-1.10.1/tikhub/api/v1/endpoints/xiaohongshu/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:16:27.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/xiaohongshu/web/__init__.py
--rw-rw-rw-   0        0        0      662 2024-05-04 23:05:56.000000 tikhub-1.10.1/tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.870882 tikhub-1.10.1/tikhub/api/v1/models/
--rw-rw-rw-   0        0        0     2508 2024-05-20 09:37:37.000000 tikhub-1.10.1/tikhub/api/v1/models/APIResponseModel.py
--rw-rw-rw-   0        0        0        0 2024-05-21 09:06:51.000000 tikhub-1.10.1/tikhub/api/v1/models/__init__.py
--rw-rw-rw-   0        0        0     1930 2024-04-04 10:53:44.000000 tikhub-1.10.1/tikhub/api/v1/models/douyin_web_models.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.872385 tikhub-1.10.1/tikhub/client/
--rw-rw-rw-   0        0        0        0 2024-05-30 12:34:35.000000 tikhub-1.10.1/tikhub/client/__init__.py
--rw-rw-rw-   0        0        0     2428 2024-05-30 12:19:09.000000 tikhub-1.10.1/tikhub/client/client.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.875703 tikhub-1.10.1/tikhub/http_client/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.10.1/tikhub/http_client/__init__.py
--rw-rw-rw-   0        0        0    11320 2024-05-30 12:14:39.000000 tikhub-1.10.1/tikhub/http_client/api_client.py
--rw-rw-rw-   0        0        0     2819 2024-05-21 09:17:26.000000 tikhub-1.10.1/tikhub/http_client/api_exceptions.py
--rw-rw-rw-   0        0        0     2978 2024-05-30 11:44:11.000000 tikhub-1.10.1/tikhub/http_client/api_logger.py
--rw-rw-rw-   0        0        0      438 2024-05-21 13:15:30.000000 tikhub-1.10.1/tikhub/http_client/deprecated.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.876708 tikhub-1.10.1/tikhub/test/
--rw-rw-rw-   0        0        0        0 2024-05-30 12:29:47.000000 tikhub-1.10.1/tikhub/test/__init__.py
--rw-rw-rw-   0        0        0     1279 2024-05-30 12:16:42.000000 tikhub-1.10.1/tikhub/test/test.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:40:52.847862 tikhub-1.10.1/tikhub.egg-info/
--rw-rw-rw-   0        0        0     3235 2024-05-30 12:40:52.000000 tikhub-1.10.1/tikhub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2054 2024-05-30 12:40:52.000000 tikhub-1.10.1/tikhub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 12:40:52.000000 tikhub-1.10.1/tikhub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-30 12:40:52.000000 tikhub-1.10.1/tikhub.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-30 12:40:52.000000 tikhub-1.10.1/tikhub.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.693317 tikhub-1.10.2/
+-rw-rw-rw-   0        0        0    11558 2024-05-21 08:59:32.000000 tikhub-1.10.2/LICENSE
+-rw-rw-rw-   0        0        0       36 2024-05-30 11:25:11.000000 tikhub-1.10.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1868 2024-06-01 00:50:28.692317 tikhub-1.10.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1342 2024-05-31 09:52:07.000000 tikhub-1.10.2/README.md
+-rw-rw-rw-   0        0        0       93 2024-05-30 11:27:47.000000 tikhub-1.10.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-01 00:50:28.693317 tikhub-1.10.2/setup.cfg
+-rw-rw-rw-   0        0        0      976 2024-06-01 00:50:21.000000 tikhub-1.10.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.652317 tikhub-1.10.2/tikhub/
+-rw-rw-rw-   0        0        0       59 2024-05-30 12:40:12.000000 tikhub-1.10.2/tikhub/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.656318 tikhub-1.10.2/tikhub/api/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.10.2/tikhub/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.657317 tikhub-1.10.2/tikhub/api/v1/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.10.2/tikhub/api/v1/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.657317 tikhub-1.10.2/tikhub/api/v1/endpoints/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:06:51.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.658316 tikhub-1.10.2/tikhub/api/v1/endpoints/captcha/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:46.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/captcha/__init__.py
+-rw-rw-rw-   0        0        0      478 2024-05-30 12:14:39.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/captcha/captcha_solver.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.659316 tikhub-1.10.2/tikhub/api/v1/endpoints/douyin/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/douyin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.662318 tikhub-1.10.2/tikhub/api/v1/endpoints/douyin/app/
+-rw-rw-rw-   0        0        0        0 2024-05-21 11:57:03.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/douyin/app/__init__.py
+-rw-rw-rw-   0        0        0    14139 2024-05-30 12:14:39.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/douyin/app/douyin_app_v1.py
+-rw-rw-rw-   0        0        0    15959 2024-05-30 12:14:39.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/douyin/app/douyin_app_v2.py
+-rw-rw-rw-   0        0        0    12565 2024-05-30 12:14:39.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/douyin/app/douyin_app_v3.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.663320 tikhub-1.10.2/tikhub/api/v1/endpoints/douyin/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/douyin/web/__init__.py
+-rw-rw-rw-   0        0        0    31217 2024-05-30 12:14:39.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/douyin/web/douyin_web.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.664317 tikhub-1.10.2/tikhub/api/v1/endpoints/instagram/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:14:52.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/instagram/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.665317 tikhub-1.10.2/tikhub/api/v1/endpoints/instagram/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:14:52.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/instagram/web/__init__.py
+-rw-rw-rw-   0        0        0      961 2024-05-30 12:14:39.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/instagram/web/instagram_web.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.667317 tikhub-1.10.2/tikhub/api/v1/endpoints/tikhub/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:07.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/tikhub/__init__.py
+-rw-rw-rw-   0        0        0     3246 2024-05-30 12:14:39.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/tikhub/tikhub_user.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.667317 tikhub-1.10.2/tikhub/api/v1/endpoints/tiktok/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:32.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/tiktok/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.671316 tikhub-1.10.2/tikhub/api/v1/endpoints/tiktok/app/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:32.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/tiktok/app/__init__.py
+-rw-rw-rw-   0        0        0    13951 2024-05-30 12:14:39.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v2.py
+-rw-rw-rw-   0        0        0    22972 2024-05-30 12:14:39.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v3.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.675317 tikhub-1.10.2/tikhub/api/v1/endpoints/tiktok/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:37.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/tiktok/web/__init__.py
+-rw-rw-rw-   0        0        0    14425 2024-06-01 00:50:03.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/tiktok/web/tiktok_web.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.675317 tikhub-1.10.2/tikhub/api/v1/endpoints/weibo/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:58.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/weibo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.677317 tikhub-1.10.2/tikhub/api/v1/endpoints/weibo/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:58.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/weibo/web/__init__.py
+-rw-rw-rw-   0        0        0     1834 2024-05-30 12:14:39.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/weibo/web/weibo_web.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.678318 tikhub-1.10.2/tikhub/api/v1/endpoints/xiaohongshu/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:23.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/xiaohongshu/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.679317 tikhub-1.10.2/tikhub/api/v1/endpoints/xiaohongshu/app/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:23.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/xiaohongshu/app/__init__.py
+-rw-rw-rw-   0        0        0      664 2024-05-04 23:05:56.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/xiaohongshu/app/xiaohongshu_app.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.680318 tikhub-1.10.2/tikhub/api/v1/endpoints/xiaohongshu/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:27.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/xiaohongshu/web/__init__.py
+-rw-rw-rw-   0        0        0      662 2024-05-04 23:05:56.000000 tikhub-1.10.2/tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.683317 tikhub-1.10.2/tikhub/api/v1/models/
+-rw-rw-rw-   0        0        0     2508 2024-05-20 09:37:37.000000 tikhub-1.10.2/tikhub/api/v1/models/APIResponseModel.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:06:51.000000 tikhub-1.10.2/tikhub/api/v1/models/__init__.py
+-rw-rw-rw-   0        0        0     1930 2024-04-04 10:53:44.000000 tikhub-1.10.2/tikhub/api/v1/models/douyin_web_models.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.684317 tikhub-1.10.2/tikhub/client/
+-rw-rw-rw-   0        0        0        0 2024-05-30 12:34:35.000000 tikhub-1.10.2/tikhub/client/__init__.py
+-rw-rw-rw-   0        0        0     2428 2024-05-30 12:19:09.000000 tikhub-1.10.2/tikhub/client/client.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.689318 tikhub-1.10.2/tikhub/http_client/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.10.2/tikhub/http_client/__init__.py
+-rw-rw-rw-   0        0        0    11320 2024-05-30 12:14:39.000000 tikhub-1.10.2/tikhub/http_client/api_client.py
+-rw-rw-rw-   0        0        0     2819 2024-05-21 09:17:26.000000 tikhub-1.10.2/tikhub/http_client/api_exceptions.py
+-rw-rw-rw-   0        0        0     2978 2024-05-30 11:44:11.000000 tikhub-1.10.2/tikhub/http_client/api_logger.py
+-rw-rw-rw-   0        0        0      438 2024-05-21 13:15:30.000000 tikhub-1.10.2/tikhub/http_client/deprecated.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.691317 tikhub-1.10.2/tikhub/test/
+-rw-rw-rw-   0        0        0        0 2024-05-30 12:29:47.000000 tikhub-1.10.2/tikhub/test/__init__.py
+-rw-rw-rw-   0        0        0     1279 2024-05-30 12:16:42.000000 tikhub-1.10.2/tikhub/test/test.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:50:28.655317 tikhub-1.10.2/tikhub.egg-info/
+-rw-rw-rw-   0        0        0     1868 2024-06-01 00:50:28.000000 tikhub-1.10.2/tikhub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2054 2024-06-01 00:50:28.000000 tikhub-1.10.2/tikhub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 00:50:28.000000 tikhub-1.10.2/tikhub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-06-01 00:50:28.000000 tikhub-1.10.2/tikhub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-06-01 00:50:28.000000 tikhub-1.10.2/tikhub.egg-info/top_level.txt
```

### Comparing `tikhub-1.10.1/LICENSE` & `tikhub-1.10.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tikhub-1.10.1/setup.py` & `tikhub-1.10.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setup(
     name="tikhub",
-    version="1.10.1",
+    version="1.10.2",
     author="TikHub.io",
     author_email="tikhub.io@proton.me",
     description="A Python SDK for TikHub RESTful API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TikHubIO/TikHub-API-SDK-Python",
     packages=find_packages(),
```

### Comparing `tikhub-1.10.1/tikhub/api/v1/endpoints/douyin/app/douyin_app_v1.py` & `tikhub-1.10.2/tikhub/api/v1/endpoints/douyin/app/douyin_app_v1.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.10.1/tikhub/api/v1/endpoints/douyin/app/douyin_app_v2.py` & `tikhub-1.10.2/tikhub/api/v1/endpoints/douyin/app/douyin_app_v2.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.10.1/tikhub/api/v1/endpoints/douyin/app/douyin_app_v3.py` & `tikhub-1.10.2/tikhub/api/v1/endpoints/douyin/app/douyin_app_v3.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.10.1/tikhub/api/v1/endpoints/douyin/web/douyin_web.py` & `tikhub-1.10.2/tikhub/api/v1/endpoints/douyin/web/douyin_web.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.10.1/tikhub/api/v1/endpoints/instagram/web/instagram_web.py` & `tikhub-1.10.2/tikhub/api/v1/endpoints/instagram/web/instagram_web.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.10.1/tikhub/api/v1/endpoints/tikhub/tikhub_user.py` & `tikhub-1.10.2/tikhub/api/v1/endpoints/tikhub/tikhub_user.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.10.1/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v2.py` & `tikhub-1.10.2/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v2.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.10.1/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v3.py` & `tikhub-1.10.2/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v3.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.10.1/tikhub/api/v1/endpoints/tiktok/web/tiktok_web.py` & `tikhub-1.10.2/tikhub/api/v1/endpoints/tiktok/web/tiktok_web.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,14 +102,26 @@
 
     # 搜索直播 | Search live
     async def fetch_search_live(self, keyword: str, count: int, offset: int):
         endpoint = "/api/v1/tiktok/web/fetch_search_live"
         data = await self.client.fetch_get_json(f"{endpoint}?keyword={keyword}&count={count}&offset={offset}")
         return data
 
+    # Tag详情 | Tag detail
+    async def fetch_tag_detail(self, tag_name: str):
+        endpoint = "/api/v1/tiktok/web/fetch_tag_detail"
+        data = await self.client.fetch_get_json(f"{endpoint}?tag_name={tag_name}")
+        return data
+
+    # Tag作品列表 | Tag post list
+    async def fetch_tag_post(self, challengeID: str, cursor: int, count: int):
+        endpoint = "/api/v1/tiktok/web/fetch_tag_post"
+        data = await self.client.fetch_get_json(f"{endpoint}?challengeID={challengeID}&cursor={cursor}&count={count}")
+        return data
+
     # 生成真实msToken | Generate real msToken
     async def fetch_real_msToken(self):
         endpoint = "/api/v1/tiktok/web/generate_real_msToken"
         data = await self.client.fetch_get_json(endpoint)
         return data
 
     # 生成ttwid | Generate ttwid
```

### Comparing `tikhub-1.10.1/tikhub/api/v1/endpoints/weibo/web/weibo_web.py` & `tikhub-1.10.2/tikhub/api/v1/endpoints/weibo/web/weibo_web.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.10.1/tikhub/api/v1/endpoints/xiaohongshu/app/xiaohongshu_app.py` & `tikhub-1.10.2/tikhub/api/v1/endpoints/xiaohongshu/app/xiaohongshu_app.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.10.1/tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py` & `tikhub-1.10.2/tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.10.1/tikhub/api/v1/models/APIResponseModel.py` & `tikhub-1.10.2/tikhub/api/v1/models/APIResponseModel.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.10.1/tikhub/api/v1/models/douyin_web_models.py` & `tikhub-1.10.2/tikhub/api/v1/models/douyin_web_models.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.10.1/tikhub/client/client.py` & `tikhub-1.10.2/tikhub/client/client.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.10.1/tikhub/http_client/api_client.py` & `tikhub-1.10.2/tikhub/http_client/api_client.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.10.1/tikhub/http_client/api_exceptions.py` & `tikhub-1.10.2/tikhub/http_client/api_exceptions.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.10.1/tikhub/http_client/api_logger.py` & `tikhub-1.10.2/tikhub/http_client/api_logger.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.10.1/tikhub/test/test.py` & `tikhub-1.10.2/tikhub/test/test.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.10.1/tikhub.egg-info/SOURCES.txt` & `tikhub-1.10.2/tikhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

