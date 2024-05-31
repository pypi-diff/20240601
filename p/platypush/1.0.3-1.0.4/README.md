# Comparing `tmp/platypush-1.0.3.tar.gz` & `tmp/platypush-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platypush-1.0.3.tar", last modified: Fri May 31 01:06:36 2024, max compression
+gzip compressed data, was "platypush-1.0.4.tar", last modified: Fri May 31 18:06:00 2024, max compression
```

## Comparing `platypush-1.0.3.tar` & `platypush-1.0.4.tar`

### file list

```diff
@@ -1,2225 +1,2225 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.504654 platypush-1.0.3/
--rw-r--r--   0 root         (0) root         (0)     1081 2024-05-31 01:03:24.000000 platypush-1.0.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      280 2024-05-31 01:03:24.000000 platypush-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    56629 2024-05-31 01:06:36.504654 platypush-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    45388 2024-05-31 01:03:24.000000 platypush-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.194643 platypush-1.0.3/platypush/
--rw-r--r--   0 root         (0) root         (0)      930 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/__init__.py
--rw-r--r--   0 root         (0) root         (0)       42 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.194643 platypush-1.0.3/platypush/app/
--rw-r--r--   0 root         (0) root         (0)       84 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/app/__init__.py
--rw-r--r--   0 root         (0) root         (0)       66 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/app/__main__.py
--rw-r--r--   0 root         (0) root         (0)    17899 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/app/_app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.194643 platypush-1.0.3/platypush/backend/
--rw-r--r--   0 root         (0) root         (0)    16878 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.194643 platypush-1.0.3/platypush/backend/http/
--rw-r--r--   0 root         (0) root         (0)    18042 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.194643 platypush-1.0.3/platypush/backend/http/app/
--rw-r--r--   0 root         (0) root         (0)      945 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.194643 platypush-1.0.3/platypush/backend/http/app/mixins/
--rw-r--r--   0 root         (0) root         (0)     5021 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/mixins/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.197976 platypush-1.0.3/platypush/backend/http/app/routes/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/routes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1980 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/routes/auth.py
--rw-r--r--   0 root         (0) root         (0)      611 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/routes/dashboard.py
--rw-r--r--   0 root         (0) root         (0)     1083 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/routes/execute.py
--rw-r--r--   0 root         (0) root         (0)     2868 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/routes/hook.py
--rw-r--r--   0 root         (0) root         (0)      501 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/routes/index.py
--rw-r--r--   0 root         (0) root         (0)     1820 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/routes/login.py
--rw-r--r--   0 root         (0) root         (0)     5412 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/routes/logo.py
--rw-r--r--   0 root         (0) root         (0)      990 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/routes/logout.py
--rw-r--r--   0 root         (0) root         (0)      570 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/routes/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.197976 platypush-1.0.3/platypush/backend/http/app/routes/plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/routes/plugins/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.197976 platypush-1.0.3/platypush/backend/http/app/routes/plugins/camera/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/routes/plugins/camera/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1536 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/routes/plugins/camera/pi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.197976 platypush-1.0.3/platypush/backend/http/app/routes/plugins/qrcode/
--rw-r--r--   0 root         (0) root         (0)      854 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/routes/plugins/qrcode/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1057 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/routes/plugins/spotify.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.197976 platypush-1.0.3/platypush/backend/http/app/routes/plugins/tts/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/routes/plugins/tts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3776 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/routes/pwa.py
--rw-r--r--   0 root         (0) root         (0)     2346 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/routes/register.py
--rw-r--r--   0 root         (0) root         (0)     2520 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/routes/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.197976 platypush-1.0.3/platypush/backend/http/app/streaming/
--rw-r--r--   0 root         (0) root         (0)       64 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/streaming/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4457 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/streaming/_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.197976 platypush-1.0.3/platypush/backend/http/app/streaming/plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/streaming/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4223 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/streaming/plugins/camera.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.201310 platypush-1.0.3/platypush/backend/http/app/streaming/plugins/media/
--rw-r--r--   0 root         (0) root         (0)      138 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/streaming/plugins/media/__init__.py
--rw-r--r--   0 root         (0) root         (0)      472 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/streaming/plugins/media/_constants.py
--rw-r--r--   0 root         (0) root         (0)     1318 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/streaming/plugins/media/_register.py
--rw-r--r--   0 root         (0) root         (0)     1097 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/streaming/plugins/media/_registry.py
--rw-r--r--   0 root         (0) root         (0)     4429 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/streaming/plugins/media/_stream.py
--rw-r--r--   0 root         (0) root         (0)     4168 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/streaming/plugins/media/_subtitles.py
--rw-r--r--   0 root         (0) root         (0)      821 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/streaming/plugins/media/_unregister.py
--rw-r--r--   0 root         (0) root         (0)     2997 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/streaming/plugins/sound.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.201310 platypush-1.0.3/platypush/backend/http/app/utils/
--rw-r--r--   0 root         (0) root         (0)      763 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.201310 platypush-1.0.3/platypush/backend/http/app/utils/auth/
--rw-r--r--   0 root         (0) root         (0)     5346 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/utils/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      478 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/utils/auth/status.py
--rw-r--r--   0 root         (0) root         (0)     1977 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/utils/bus.py
--rw-r--r--   0 root         (0) root         (0)      801 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     1662 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/utils/routes.py
--rw-r--r--   0 root         (0) root         (0)     1114 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/utils/streaming.py
--rw-r--r--   0 root         (0) root         (0)     1013 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/utils/ws.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.201310 platypush-1.0.3/platypush/backend/http/app/ws/
--rw-r--r--   0 root         (0) root         (0)       68 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/ws/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2168 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/ws/_base.py
--rw-r--r--   0 root         (0) root         (0)     1786 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/ws/cmd.py
--rw-r--r--   0 root         (0) root         (0)     1350 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/ws/events.py
--rw-r--r--   0 root         (0) root         (0)     1464 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/app/ws/requests.py
--rw-r--r--   0 root         (0) root         (0)      144 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.201310 platypush-1.0.3/platypush/backend/http/media/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/media/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.201310 platypush-1.0.3/platypush/backend/http/media/handlers/
--rw-r--r--   0 root         (0) root         (0)     3364 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/media/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1710 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/media/handlers/file.py
--rw-r--r--   0 root         (0) root         (0)     4014 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.167976 platypush-1.0.3/platypush/backend/http/webapp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.204643 platypush-1.0.3/platypush/backend/http/webapp/dist/
--rw-r--r--   0 root         (0) root         (0)    16958 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.204643 platypush-1.0.3/platypush/backend/http/webapp/dist/fonts/
--rw-r--r--   0 root         (0) root         (0)   154584 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/fonts/Poppins.ttf
--rw-r--r--   0 root         (0) root         (0)      151 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/fonts/poppins.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.204643 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/
--rw-r--r--   0 root         (0) root         (0)     1120 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/jellyfin.svg
--rw-r--r--   0 root         (0) root         (0)     1370 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/kodi.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.167976 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.207977 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/
--rw-r--r--   0 root         (0) root         (0)     1029 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/01d.png
--rw-r--r--   0 root         (0) root         (0)     4338 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/01n.png
--rw-r--r--   0 root         (0) root         (0)     1624 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/02d.png
--rw-r--r--   0 root         (0) root         (0)     4297 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/02n.png
--rw-r--r--   0 root         (0) root         (0)     1571 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/03d.png
--rw-r--r--   0 root         (0) root         (0)     3887 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/03n.png
--rw-r--r--   0 root         (0) root         (0)     1032 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/04d.png
--rw-r--r--   0 root         (0) root         (0)     1032 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/04n.png
--rw-r--r--   0 root         (0) root         (0)     1612 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/09d.png
--rw-r--r--   0 root         (0) root         (0)     1612 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/09n.png
--rw-r--r--   0 root         (0) root         (0)     1700 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/10d.png
--rw-r--r--   0 root         (0) root         (0)     1700 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/10n.png
--rw-r--r--   0 root         (0) root         (0)     1994 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/11d.png
--rw-r--r--   0 root         (0) root         (0)     1994 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/11n.png
--rw-r--r--   0 root         (0) root         (0)     1191 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/13d.png
--rw-r--r--   0 root         (0) root         (0)     1191 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/13n.png
--rw-r--r--   0 root         (0) root         (0)     1041 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/50d.png
--rw-r--r--   0 root         (0) root         (0)     1041 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/50n.png
--rw-r--r--   0 root         (0) root         (0)     1195 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/unknown.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.211310 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/
--rw-r--r--   0 root         (0) root         (0)     1029 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/01d.png
--rw-r--r--   0 root         (0) root         (0)     4338 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/01n.png
--rw-r--r--   0 root         (0) root         (0)     1624 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/02d.png
--rw-r--r--   0 root         (0) root         (0)     4297 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/02n.png
--rw-r--r--   0 root         (0) root         (0)     1571 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/03d.png
--rw-r--r--   0 root         (0) root         (0)     3887 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/03n.png
--rw-r--r--   0 root         (0) root         (0)     1032 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/04d.png
--rw-r--r--   0 root         (0) root         (0)     1032 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/04n.png
--rw-r--r--   0 root         (0) root         (0)     1612 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/09d.png
--rw-r--r--   0 root         (0) root         (0)     1612 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/09n.png
--rw-r--r--   0 root         (0) root         (0)     1700 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/10d.png
--rw-r--r--   0 root         (0) root         (0)     1700 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/10n.png
--rw-r--r--   0 root         (0) root         (0)     1994 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/11d.png
--rw-r--r--   0 root         (0) root         (0)     1994 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/11n.png
--rw-r--r--   0 root         (0) root         (0)     1191 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/13d.png
--rw-r--r--   0 root         (0) root         (0)     1191 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/13n.png
--rw-r--r--   0 root         (0) root         (0)     1041 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/50d.png
--rw-r--r--   0 root         (0) root         (0)     1041 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/50n.png
--rw-r--r--   0 root         (0) root         (0)     1195 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/unknown.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.214644 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/
--rw-r--r--   0 root         (0) root         (0)     1333 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/01d.png
--rw-r--r--   0 root         (0) root         (0)     2489 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/01n.png
--rw-r--r--   0 root         (0) root         (0)     1871 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/02d.png
--rw-r--r--   0 root         (0) root         (0)     3888 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/02n.png
--rw-r--r--   0 root         (0) root         (0)     1762 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/03d.png
--rw-r--r--   0 root         (0) root         (0)     3363 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/03n.png
--rw-r--r--   0 root         (0) root         (0)     1203 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/04d.png
--rw-r--r--   0 root         (0) root         (0)     1203 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/04n.png
--rw-r--r--   0 root         (0) root         (0)     1826 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/09d.png
--rw-r--r--   0 root         (0) root         (0)     1826 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/09n.png
--rw-r--r--   0 root         (0) root         (0)     1890 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/10d.png
--rw-r--r--   0 root         (0) root         (0)     1890 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/10n.png
--rw-r--r--   0 root         (0) root         (0)     2178 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/11d.png
--rw-r--r--   0 root         (0) root         (0)     2178 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/11n.png
--rw-r--r--   0 root         (0) root         (0)     1502 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/13d.png
--rw-r--r--   0 root         (0) root         (0)     1502 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/13n.png
--rw-r--r--   0 root         (0) root         (0)     1211 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/50d.png
--rw-r--r--   0 root         (0) root         (0)     1211 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/50n.png
--rw-r--r--   0 root         (0) root         (0)     1396 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/unknown.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.214644 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/
--rw-r--r--   0 root         (0) root         (0)     1333 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/01d.png
--rw-r--r--   0 root         (0) root         (0)     2489 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/01n.png
--rw-r--r--   0 root         (0) root         (0)     1871 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/02d.png
--rw-r--r--   0 root         (0) root         (0)     3888 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/02n.png
--rw-r--r--   0 root         (0) root         (0)     1762 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/03d.png
--rw-r--r--   0 root         (0) root         (0)     3363 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/03n.png
--rw-r--r--   0 root         (0) root         (0)     1203 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/04d.png
--rw-r--r--   0 root         (0) root         (0)     1203 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/04n.png
--rw-r--r--   0 root         (0) root         (0)     1826 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/09d.png
--rw-r--r--   0 root         (0) root         (0)     1826 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/09n.png
--rw-r--r--   0 root         (0) root         (0)     1890 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/10d.png
--rw-r--r--   0 root         (0) root         (0)     1890 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/10n.png
--rw-r--r--   0 root         (0) root         (0)     2178 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/11d.png
--rw-r--r--   0 root         (0) root         (0)     2178 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/11n.png
--rw-r--r--   0 root         (0) root         (0)     1502 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/13d.png
--rw-r--r--   0 root         (0) root         (0)     1502 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/13n.png
--rw-r--r--   0 root         (0) root         (0)     1211 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/50d.png
--rw-r--r--   0 root         (0) root         (0)     1211 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/50n.png
--rw-r--r--   0 root         (0) root         (0)     1396 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/unknown.png
--rw-r--r--   0 root         (0) root         (0)      191 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/plex.svg
--rw-r--r--   0 root         (0) root         (0)     4057 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/smartthings.png
--rw-r--r--   0 root         (0) root         (0)     4034 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/z-wave.png
--rw-r--r--   0 root         (0) root         (0)      632 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/icons/zigbee.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.214644 platypush-1.0.3/platypush/backend/http/webapp/dist/img/
--rw-r--r--   0 root         (0) root         (0)    11833 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/img/dashboard-bg-light.jpg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.217977 platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/
--rw-r--r--   0 root         (0) root         (0)    12675 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/android-chrome-192x192.png
--rw-r--r--   0 root         (0) root         (0)    48520 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/android-chrome-512x512.png
--rw-r--r--   0 root         (0) root         (0)    12675 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/android-chrome-maskable-192x192.png
--rw-r--r--   0 root         (0) root         (0)    48520 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/android-chrome-maskable-512x512.png
--rw-r--r--   0 root         (0) root         (0)     7644 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon-120x120.png
--rw-r--r--   0 root         (0) root         (0)     9796 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon-152x152.png
--rw-r--r--   0 root         (0) root         (0)    11988 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon-180x180.png
--rw-r--r--   0 root         (0) root         (0)     3744 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon-60x60.png
--rw-r--r--   0 root         (0) root         (0)     4786 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon-76x76.png
--rw-r--r--   0 root         (0) root         (0)    11988 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon.png
--rw-r--r--   0 root         (0) root         (0)     4675 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/favicon-16x16.png
--rw-r--r--   0 root         (0) root         (0)     1694 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/favicon-32x32.png
--rw-r--r--   0 root         (0) root         (0)     4677 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/favicon.svg
--rw-r--r--   0 root         (0) root         (0)    20814 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/logo-256x256.png
--rw-r--r--   0 root         (0) root         (0)     9248 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/msapplication-icon-144x144.png
--rw-r--r--   0 root         (0) root         (0)     9654 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/mstile-150x150.png
--rw-r--r--   0 root         (0) root         (0)     4675 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/safari-pinned-tab.svg
--rw-r--r--   0 root         (0) root         (0)    20925 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/img/logo.png
--rw-r--r--   0 root         (0) root         (0)    32701 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/img/spinner.gif
--rw-r--r--   0 root         (0) root         (0)     1573 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/index.html
--rw-r--r--   0 root         (0) root         (0)      551 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/manifest.json
--rw-r--r--   0 root         (0) root         (0)    43705 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/service-worker.js
--rw-r--r--   0 root         (0) root         (0)    91952 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/service-worker.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.167976 platypush-1.0.3/platypush/backend/http/webapp/dist/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.234644 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/
--rw-r--r--   0 root         (0) root         (0)   106570 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/1259.ad51b86e.css
--rw-r--r--   0 root         (0) root         (0)    29794 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/1391.8fb65128.css
--rw-r--r--   0 root         (0) root         (0)   149888 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/1449.bf964828.css
--rw-r--r--   0 root         (0) root         (0)   154136 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/1587.f52aafce.css
--rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/169.9ec6abc1.css
--rw-r--r--   0 root         (0) root         (0)    35140 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/1706.c1e22194.css
--rw-r--r--   0 root         (0) root         (0)   205770 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/1807.333a022f.css
--rw-r--r--   0 root         (0) root         (0)    30556 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/1949.d8d63590.css
--rw-r--r--   0 root         (0) root         (0)    53589 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/2140.08e216c1.css
--rw-r--r--   0 root         (0) root         (0)    30675 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/2154.20cf0934.css
--rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/2217.da1b8fd6.css
--rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/2460.83acd505.css
--rw-r--r--   0 root         (0) root         (0)    31886 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/2461.1fc0b5b4.css
--rw-r--r--   0 root         (0) root         (0)   371529 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/2509.77a756c6.css
--rw-r--r--   0 root         (0) root         (0)    31962 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/2844.23273db2.css
--rw-r--r--   0 root         (0) root         (0)    29745 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/2892.3a7569e7.css
--rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/2893.21a9931c.css
--rw-r--r--   0 root         (0) root         (0)    29790 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/2976.bafd7cea.css
--rw-r--r--   0 root         (0) root         (0)    30412 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/2992.f8bddaf0.css
--rw-r--r--   0 root         (0) root         (0)    35106 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/3368.467cedc6.css
--rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/3369.69c504e7.css
--rw-r--r--   0 root         (0) root         (0)    30629 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/3390.481c441e.css
--rw-r--r--   0 root         (0) root         (0)   251755 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/3553.6d93b4b8.css
--rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/3559.5665c422.css
--rw-r--r--   0 root         (0) root         (0)    30173 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/3661.c12867e9.css
--rw-r--r--   0 root         (0) root         (0)    30854 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/3671.e6547429.css
--rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/3826.53d49948.css
--rw-r--r--   0 root         (0) root         (0)    34817 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/3835.91d8befb.css
--rw-r--r--   0 root         (0) root         (0)    33195 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/3924.e7e714bc.css
--rw-r--r--   0 root         (0) root         (0)    34753 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/4221.76c11dc1.css
--rw-r--r--   0 root         (0) root         (0)    30121 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/446.e0a96773.css
--rw-r--r--   0 root         (0) root         (0)    31611 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/4589.d7fd389b.css
--rw-r--r--   0 root         (0) root         (0)    37383 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/472.20f2f41f.css
--rw-r--r--   0 root         (0) root         (0)    29820 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/4790.3ef3568e.css
--rw-r--r--   0 root         (0) root         (0)    29745 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/5059.e5cd6fe3.css
--rw-r--r--   0 root         (0) root         (0)    22679 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/5207.e1e8949a.css
--rw-r--r--   0 root         (0) root         (0)   182984 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/5285.2250c5c9.css
--rw-r--r--   0 root         (0) root         (0)    34710 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/5329.2f2c6a0e.css
--rw-r--r--   0 root         (0) root         (0)    30285 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/5638.05ee3a45.css
--rw-r--r--   0 root         (0) root         (0)    65509 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/5795.3b193db6.css
--rw-r--r--   0 root         (0) root         (0)    29749 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/5833.e1e503a2.css
--rw-r--r--   0 root         (0) root         (0)    34872 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/5906.52ba6beb.css
--rw-r--r--   0 root         (0) root         (0)    30308 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/5931.e6c8f94d.css
--rw-r--r--   0 root         (0) root         (0)   161995 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/6062.b6571ed4.css
--rw-r--r--   0 root         (0) root         (0)    32679 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/6079.f88a21ae.css
--rw-r--r--   0 root         (0) root         (0)    35248 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/6324.bb3e2171.css
--rw-r--r--   0 root         (0) root         (0)    26608 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/65.cb15a9a6.css
--rw-r--r--   0 root         (0) root         (0)    30129 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/6523.d6576265.css
--rw-r--r--   0 root         (0) root         (0)    49371 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/6561.77bbcd33.css
--rw-r--r--   0 root         (0) root         (0)    30152 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/6579.04ad63dc.css
--rw-r--r--   0 root         (0) root         (0)    35642 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/669.73188f7e.css
--rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/729.16b20067.css
--rw-r--r--   0 root         (0) root         (0)    29885 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/746.18c59228.css
--rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/7590.b45a8e92.css
--rw-r--r--   0 root         (0) root         (0)    32924 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/7651.9b63654f.css
--rw-r--r--   0 root         (0) root         (0)    32383 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/7841.2a1ced53.css
--rw-r--r--   0 root         (0) root         (0)    35431 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/7878.e3469993.css
--rw-r--r--   0 root         (0) root         (0)   181061 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/7880.4f4a202a.css
--rw-r--r--   0 root         (0) root         (0)    60270 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/7968.29db26b1.css
--rw-r--r--   0 root         (0) root         (0)    24683 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/8039.e77a760e.css
--rw-r--r--   0 root         (0) root         (0)    30722 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/8069.111183af.css
--rw-r--r--   0 root         (0) root         (0)    29809 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/8179.b5fb83f9.css
--rw-r--r--   0 root         (0) root         (0)    34712 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/8391.b5dd11a9.css
--rw-r--r--   0 root         (0) root         (0)    35341 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/8498.3676728c.css
--rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/8621.5db86eb0.css
--rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/8769.fda642fb.css
--rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/8825.f608e2c2.css
--rw-r--r--   0 root         (0) root         (0)    34997 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/8989.63c7ae13.css
--rw-r--r--   0 root         (0) root         (0)    30070 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/906.80f1f8a3.css
--rw-r--r--   0 root         (0) root         (0)    30034 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/9211.b8dcc633.css
--rw-r--r--   0 root         (0) root         (0)   189438 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/9381.ade341db.css
--rw-r--r--   0 root         (0) root         (0)    35171 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/9461.79136fbe.css
--rw-r--r--   0 root         (0) root         (0)   207104 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/9751.0631f530.css
--rw-r--r--   0 root         (0) root         (0)    35151 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/980.b4628099.css
--rw-r--r--   0 root         (0) root         (0)    34712 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/984.0c88349b.css
--rw-r--r--   0 root         (0) root         (0)    59998 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/9962.eb89f1f6.css
--rw-r--r--   0 root         (0) root         (0)  1037999 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/app.200dd9cf.css
--rw-r--r--   0 root         (0) root         (0)    27965 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/chunk-vendors.a2412607.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.237978 platypush-1.0.3/platypush/backend/http/webapp/dist/static/fonts/
--rw-r--r--   0 root         (0) root         (0)   209128 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/fonts/fa-brands-400.5d18d427.ttf
--rw-r--r--   0 root         (0) root         (0)   117852 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/fonts/fa-brands-400.87587a68.woff2
--rw-r--r--   0 root         (0) root         (0)    25392 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/fonts/fa-regular-400.3ccdbd3d.woff2
--rw-r--r--   0 root         (0) root         (0)    67860 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/fonts/fa-regular-400.81482cd4.ttf
--rw-r--r--   0 root         (0) root         (0)   156400 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/fonts/fa-solid-900.0b0cc8a6.woff2
--rw-r--r--   0 root         (0) root         (0)   420332 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/fonts/fa-solid-900.69d3141a.ttf
--rw-r--r--   0 root         (0) root         (0)   325936 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/fonts/lato-medium-italic.1996cc15.woff
--rw-r--r--   0 root         (0) root         (0)   194608 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/fonts/lato-medium-italic.1e312dd9.woff2
--rw-r--r--   0 root         (0) root         (0)   182144 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/fonts/lato-medium.13fcde4c.woff2
--rw-r--r--   0 root         (0) root         (0)   305920 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/fonts/lato-medium.b41c3821.woff
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.321314 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/
--rw-r--r--   0 root         (0) root         (0)    32679 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ad.cb33f69a.svg
--rw-r--r--   0 root         (0) root         (0)    33893 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ad.fa8477e6.svg
--rw-r--r--   0 root         (0) root         (0)      254 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ae.a3f5e295.svg
--rw-r--r--   0 root         (0) root         (0)      262 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ae.f06e0095.svg
--rw-r--r--   0 root         (0) root         (0)    21257 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/af.89591ab0.svg
--rw-r--r--   0 root         (0) root         (0)    21123 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/af.8ca96393.svg
--rw-r--r--   0 root         (0) root         (0)      743 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ag.4c37bc2e.svg
--rw-r--r--   0 root         (0) root         (0)      761 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ag.56074d55.svg
--rw-r--r--   0 root         (0) root         (0)    47971 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ai.70eefdc0.svg
--rw-r--r--   0 root         (0) root         (0)    42204 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ai.893d1179.svg
--rw-r--r--   0 root         (0) root         (0)     3220 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/al.b16acdb2.svg
--rw-r--r--   0 root         (0) root         (0)     3218 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/al.e0864b5d.svg
--rw-r--r--   0 root         (0) root         (0)      223 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/am.00f0fec4.svg
--rw-r--r--   0 root         (0) root         (0)      231 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/am.a566904f.svg
--rw-r--r--   0 root         (0) root         (0)     1601 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ao.3df23f21.svg
--rw-r--r--   0 root         (0) root         (0)     1601 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ao.c0c32201.svg
--rw-r--r--   0 root         (0) root         (0)     3180 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/aq.1b8c45a6.svg
--rw-r--r--   0 root         (0) root         (0)     2969 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/aq.aa242c4a.svg
--rw-r--r--   0 root         (0) root         (0)     3500 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ar.22a3116e.svg
--rw-r--r--   0 root         (0) root         (0)     3427 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ar.d3238270.svg
--rw-r--r--   0 root         (0) root         (0)     8082 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/as.10ed1a23.svg
--rw-r--r--   0 root         (0) root         (0)     7838 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/as.4a330654.svg
--rw-r--r--   0 root         (0) root         (0)      240 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/at.02a64279.svg
--rw-r--r--   0 root         (0) root         (0)      242 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/at.94cde74c.svg
--rw-r--r--   0 root         (0) root         (0)     1330 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/au.cc65fc07.svg
--rw-r--r--   0 root         (0) root         (0)     1317 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/au.dbcdef2c.svg
--rw-r--r--   0 root         (0) root         (0)     9945 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/aw.abbad4ac.svg
--rw-r--r--   0 root         (0) root         (0)    12084 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/aw.be4540eb.svg
--rw-r--r--   0 root         (0) root         (0)      541 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ax.371c7af2.svg
--rw-r--r--   0 root         (0) root         (0)      553 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ax.91eea523.svg
--rw-r--r--   0 root         (0) root         (0)      512 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/az.0e2f1d1a.svg
--rw-r--r--   0 root         (0) root         (0)      498 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/az.f399f1c8.svg
--rw-r--r--   0 root         (0) root         (0)     1304 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ba.032070d4.svg
--rw-r--r--   0 root         (0) root         (0)     1242 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ba.e167b08f.svg
--rw-r--r--   0 root         (0) root         (0)      610 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bb.23a15e67.svg
--rw-r--r--   0 root         (0) root         (0)      613 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bb.b800513b.svg
--rw-r--r--   0 root         (0) root         (0)      192 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bd.c1abcb00.svg
--rw-r--r--   0 root         (0) root         (0)      190 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bd.c4a5f0e2.svg
--rw-r--r--   0 root         (0) root         (0)      290 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/be.29774a37.svg
--rw-r--r--   0 root         (0) root         (0)      290 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/be.3eb14701.svg
--rw-r--r--   0 root         (0) root         (0)      383 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bf.2334e919.svg
--rw-r--r--   0 root         (0) root         (0)      357 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bf.4ffd5dc6.svg
--rw-r--r--   0 root         (0) root         (0)      286 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bg.700f100c.svg
--rw-r--r--   0 root         (0) root         (0)      294 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bg.d0a49130.svg
--rw-r--r--   0 root         (0) root         (0)      543 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bh.2a884f6c.svg
--rw-r--r--   0 root         (0) root         (0)      569 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bh.3968dfe0.svg
--rw-r--r--   0 root         (0) root         (0)     1045 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bi.211d0f9e.svg
--rw-r--r--   0 root         (0) root         (0)     1071 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bi.ae3bb248.svg
--rw-r--r--   0 root         (0) root         (0)      499 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bj.2cdc8a62.svg
--rw-r--r--   0 root         (0) root         (0)      496 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bj.aba95ad2.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bl.04966866.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bl.3e69e968.svg
--rw-r--r--   0 root         (0) root         (0)    22617 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bm.e6903c8e.svg
--rw-r--r--   0 root         (0) root         (0)    22304 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bm.e69e40c4.svg
--rw-r--r--   0 root         (0) root         (0)    14506 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bn.07911e0c.svg
--rw-r--r--   0 root         (0) root         (0)    14367 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bn.4d91734a.svg
--rw-r--r--   0 root         (0) root         (0)   117922 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bo.03595499.svg
--rw-r--r--   0 root         (0) root         (0)   119582 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bo.9c1d9ef8.svg
--rw-r--r--   0 root         (0) root         (0)      224 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bq.747d8177.svg
--rw-r--r--   0 root         (0) root         (0)      228 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bq.b9355bec.svg
--rw-r--r--   0 root         (0) root         (0)     7816 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/br.058a5086.svg
--rw-r--r--   0 root         (0) root         (0)     8231 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/br.fe030c1c.svg
--rw-r--r--   0 root         (0) root         (0)      568 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bs.d228cbb2.svg
--rw-r--r--   0 root         (0) root         (0)      546 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bs.ef0a29ed.svg
--rw-r--r--   0 root         (0) root         (0)    25138 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bt.3f8ecb9b.svg
--rw-r--r--   0 root         (0) root         (0)    25318 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bt.fc241981.svg
--rw-r--r--   0 root         (0) root         (0)      582 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bv.5503f03a.svg
--rw-r--r--   0 root         (0) root         (0)      579 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bv.7f7cd26f.svg
--rw-r--r--   0 root         (0) root         (0)      254 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bw.494aae64.svg
--rw-r--r--   0 root         (0) root         (0)      252 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bw.b767df8c.svg
--rw-r--r--   0 root         (0) root         (0)     6086 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/by.78d2c3c9.svg
--rw-r--r--   0 root         (0) root         (0)     5956 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/by.fba98c48.svg
--rw-r--r--   0 root         (0) root         (0)    47095 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bz.14c3376a.svg
--rw-r--r--   0 root         (0) root         (0)    46832 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bz.5e0ef548.svg
--rw-r--r--   0 root         (0) root         (0)      705 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ca.163ac200.svg
--rw-r--r--   0 root         (0) root         (0)      725 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ca.a2ab234d.svg
--rw-r--r--   0 root         (0) root         (0)     3089 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cc.51960f85.svg
--rw-r--r--   0 root         (0) root         (0)     3135 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cc.813adff8.svg
--rw-r--r--   0 root         (0) root         (0)      349 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cd.39186ec2.svg
--rw-r--r--   0 root         (0) root         (0)      507 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cd.b4bd46ee.svg
--rw-r--r--   0 root         (0) root         (0)      685 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cf.b5702729.svg
--rw-r--r--   0 root         (0) root         (0)      632 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cf.fe1120e9.svg
--rw-r--r--   0 root         (0) root         (0)      469 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cg.00603842.svg
--rw-r--r--   0 root         (0) root         (0)      481 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cg.12414c99.svg
--rw-r--r--   0 root         (0) root         (0)      295 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ch.7376c9c3.svg
--rw-r--r--   0 root         (0) root         (0)      297 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ch.a558d859.svg
--rw-r--r--   0 root         (0) root         (0)      280 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ci.1251a8e3.svg
--rw-r--r--   0 root         (0) root         (0)      283 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ci.425a24c2.svg
--rw-r--r--   0 root         (0) root         (0)     1843 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ck.4e83dd3e.svg
--rw-r--r--   0 root         (0) root         (0)     1884 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ck.6303aa5b.svg
--rw-r--r--   0 root         (0) root         (0)      574 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cl.0917a91e.svg
--rw-r--r--   0 root         (0) root         (0)      557 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cl.b5974a35.svg
--rw-r--r--   0 root         (0) root         (0)      824 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cm.253adb39.svg
--rw-r--r--   0 root         (0) root         (0)      824 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cm.853e2843.svg
--rw-r--r--   0 root         (0) root         (0)      743 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cn.38f63e1e.svg
--rw-r--r--   0 root         (0) root         (0)      801 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cn.e1b166eb.svg
--rw-r--r--   0 root         (0) root         (0)      289 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/co.33e249d8.svg
--rw-r--r--   0 root         (0) root         (0)      289 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/co.b5cbc817.svg
--rw-r--r--   0 root         (0) root         (0)      293 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cr.2e572846.svg
--rw-r--r--   0 root         (0) root         (0)      293 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cr.336eb7d3.svg
--rw-r--r--   0 root         (0) root         (0)      573 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cu.c2a6f0ed.svg
--rw-r--r--   0 root         (0) root         (0)      616 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cu.d6e33f19.svg
--rw-r--r--   0 root         (0) root         (0)     1409 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cv.5ea64968.svg
--rw-r--r--   0 root         (0) root         (0)     1357 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cv.b3ab83f5.svg
--rw-r--r--   0 root         (0) root         (0)      675 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cw.0e14b0b7.svg
--rw-r--r--   0 root         (0) root         (0)      682 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cw.9b9b7ed5.svg
--rw-r--r--   0 root         (0) root         (0)     2505 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cx.da5de6d2.svg
--rw-r--r--   0 root         (0) root         (0)     2466 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cx.e04e07e8.svg
--rw-r--r--   0 root         (0) root         (0)     6024 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cy.834e6240.svg
--rw-r--r--   0 root         (0) root         (0)     5930 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cy.bfcfd736.svg
--rw-r--r--   0 root         (0) root         (0)      480 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cz.aa114964.svg
--rw-r--r--   0 root         (0) root         (0)      478 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cz.b5f98a6b.svg
--rw-r--r--   0 root         (0) root         (0)    11833 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/dashboard-bg-light.06da6eab.jpg
--rw-r--r--   0 root         (0) root         (0)      213 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/de.8e159e6e.svg
--rw-r--r--   0 root         (0) root         (0)      221 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/de.b827ac51.svg
--rw-r--r--   0 root         (0) root         (0)      585 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/dj.4197a18a.svg
--rw-r--r--   0 root         (0) root         (0)      585 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/dj.925748d5.svg
--rw-r--r--   0 root         (0) root         (0)      239 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/dk.3ca1caed.svg
--rw-r--r--   0 root         (0) root         (0)      235 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/dk.a867eeef.svg
--rw-r--r--   0 root         (0) root         (0)    16480 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/dm.7ddb00ac.svg
--rw-r--r--   0 root         (0) root         (0)    15992 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/dm.bca6d70c.svg
--rw-r--r--   0 root         (0) root         (0)   391693 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/do.81097daa.svg
--rw-r--r--   0 root         (0) root         (0)   394127 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/do.954f0f3e.svg
--rw-r--r--   0 root         (0) root         (0)      309 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/dz.76d47b01.svg
--rw-r--r--   0 root         (0) root         (0)      298 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/dz.b7e2fbce.svg
--rw-r--r--   0 root         (0) root         (0)    29916 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ec.0029f514.svg
--rw-r--r--   0 root         (0) root         (0)    29359 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ec.5f387e2f.svg
--rw-r--r--   0 root         (0) root         (0)      321 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ee.1b4839e0.svg
--rw-r--r--   0 root         (0) root         (0)      352 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ee.828384a8.svg
--rw-r--r--   0 root         (0) root         (0)     9964 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/eg.38443fa6.svg
--rw-r--r--   0 root         (0) root         (0)     9978 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/eg.5756a758.svg
--rw-r--r--   0 root         (0) root         (0)      823 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/eh.82bd1c7b.svg
--rw-r--r--   0 root         (0) root         (0)      873 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/eh.f8d7b64f.svg
--rw-r--r--   0 root         (0) root         (0)     3202 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/er.bf5b134b.svg
--rw-r--r--   0 root         (0) root         (0)     3388 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/er.e932abe1.svg
--rw-r--r--   0 root         (0) root         (0)      258 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/es-ct.64a68954.svg
--rw-r--r--   0 root         (0) root         (0)      257 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/es-ct.69469f50.svg
--rw-r--r--   0 root         (0) root         (0)    93922 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/es.7dd46df0.svg
--rw-r--r--   0 root         (0) root         (0)    92061 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/es.de5915e5.svg
--rw-r--r--   0 root         (0) root         (0)     1239 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/et.82e8eb21.svg
--rw-r--r--   0 root         (0) root         (0)     1240 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/et.a998a1b2.svg
--rw-r--r--   0 root         (0) root         (0)     1249 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/eu.4c6e130f.svg
--rw-r--r--   0 root         (0) root         (0)     1250 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/eu.aba724b1.svg
--rw-r--r--   0 root         (0) root         (0)      240 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/fi.0cd85b78.svg
--rw-r--r--   0 root         (0) root         (0)      237 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/fi.3be6b378.svg
--rw-r--r--   0 root         (0) root         (0)    27208 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/fj.ac9c916f.svg
--rw-r--r--   0 root         (0) root         (0)    27355 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/fj.e8d3e00b.svg
--rw-r--r--   0 root         (0) root         (0)    30431 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/fk.af0350f8.svg
--rw-r--r--   0 root         (0) root         (0)    30626 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/fk.db55fa14.svg
--rw-r--r--   0 root         (0) root         (0)      759 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/fm.3491efc7.svg
--rw-r--r--   0 root         (0) root         (0)      770 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/fm.78d44caa.svg
--rw-r--r--   0 root         (0) root         (0)      534 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/fo.1da81e3a.svg
--rw-r--r--   0 root         (0) root         (0)      564 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/fo.72949ad1.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/fr.3565b8f4.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/fr.9cb70285.svg
--rw-r--r--   0 root         (0) root         (0)      278 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ga.3e474381.svg
--rw-r--r--   0 root         (0) root         (0)      274 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ga.59f7d865.svg
--rw-r--r--   0 root         (0) root         (0)      232 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gb-eng.0fac6e79.svg
--rw-r--r--   0 root         (0) root         (0)      242 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gb-eng.513dcf1b.svg
--rw-r--r--   0 root         (0) root         (0)    26859 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gb-nir.2b7d2c3a.svg
--rw-r--r--   0 root         (0) root         (0)    25348 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gb-nir.f59817d6.svg
--rw-r--r--   0 root         (0) root         (0)      239 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gb-sct.f5001e5d.svg
--rw-r--r--   0 root         (0) root         (0)      231 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gb-sct.fee55173.svg
--rw-r--r--   0 root         (0) root         (0)     9183 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gb-wls.13481560.svg
--rw-r--r--   0 root         (0) root         (0)     9076 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gb-wls.95b2cfab.svg
--rw-r--r--   0 root         (0) root         (0)      795 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gb.2aafb374.svg
--rw-r--r--   0 root         (0) root         (0)      837 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gb.7a456bb2.svg
--rw-r--r--   0 root         (0) root         (0)     1831 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gd.04ea09b7.svg
--rw-r--r--   0 root         (0) root         (0)     1687 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gd.60b96978.svg
--rw-r--r--   0 root         (0) root         (0)     1397 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ge.b7b65b55.svg
--rw-r--r--   0 root         (0) root         (0)     1541 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ge.c7190912.svg
--rw-r--r--   0 root         (0) root         (0)      261 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gf.531f9e07.svg
--rw-r--r--   0 root         (0) root         (0)      258 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gf.90f438a3.svg
--rw-r--r--   0 root         (0) root         (0)      595 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gg.3aebc3ce.svg
--rw-r--r--   0 root         (0) root         (0)      625 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gg.65174039.svg
--rw-r--r--   0 root         (0) root         (0)      296 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gh.af443995.svg
--rw-r--r--   0 root         (0) root         (0)      281 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gh.f2b6baac.svg
--rw-r--r--   0 root         (0) root         (0)     2949 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gi.302c2506.svg
--rw-r--r--   0 root         (0) root         (0)     2957 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gi.7beea6ed.svg
--rw-r--r--   0 root         (0) root         (0)      226 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gl.551d0783.svg
--rw-r--r--   0 root         (0) root         (0)      240 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gl.6a5c17b0.svg
--rw-r--r--   0 root         (0) root         (0)      540 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gm.0e00e9d4.svg
--rw-r--r--   0 root         (0) root         (0)      382 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gm.1724dc37.svg
--rw-r--r--   0 root         (0) root         (0)      295 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gn.54a75b28.svg
--rw-r--r--   0 root         (0) root         (0)      295 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gn.7c96520b.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gp.4327060f.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gp.f8adbf5c.svg
--rw-r--r--   0 root         (0) root         (0)     5277 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gq.b1679302.svg
--rw-r--r--   0 root         (0) root         (0)     5185 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gq.bd7daf33.svg
--rw-r--r--   0 root         (0) root         (0)      815 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gr.07bedadf.svg
--rw-r--r--   0 root         (0) root         (0)      872 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gr.25dd3287.svg
--rw-r--r--   0 root         (0) root         (0)    35105 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gs.60368968.svg
--rw-r--r--   0 root         (0) root         (0)    34612 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gs.b2836676.svg
--rw-r--r--   0 root         (0) root         (0)    37811 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gt.1a24ed67.svg
--rw-r--r--   0 root         (0) root         (0)    37811 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gt.825f7286.svg
--rw-r--r--   0 root         (0) root         (0)     4630 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gu.05f0ab85.svg
--rw-r--r--   0 root         (0) root         (0)     4854 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gu.19b114eb.svg
--rw-r--r--   0 root         (0) root         (0)      889 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gw.bcd1eddb.svg
--rw-r--r--   0 root         (0) root         (0)      813 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gw.c97f3f94.svg
--rw-r--r--   0 root         (0) root         (0)      481 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gy.6327f72a.svg
--rw-r--r--   0 root         (0) root         (0)      488 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gy.e11d0234.svg
--rw-r--r--   0 root         (0) root         (0)     3554 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/hk.b199a9ee.svg
--rw-r--r--   0 root         (0) root         (0)     3503 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/hk.c72bba0e.svg
--rw-r--r--   0 root         (0) root         (0)     1308 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/hm.4aa61657.svg
--rw-r--r--   0 root         (0) root         (0)     1324 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/hm.d4b3d393.svg
--rw-r--r--   0 root         (0) root         (0)     1112 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/hn.08ad78b2.svg
--rw-r--r--   0 root         (0) root         (0)     1116 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/hn.44cee191.svg
--rw-r--r--   0 root         (0) root         (0)    41785 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/hr.078b1bf9.svg
--rw-r--r--   0 root         (0) root         (0)    41588 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/hr.1f4e28b8.svg
--rw-r--r--   0 root         (0) root         (0)    15301 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ht.6943447c.svg
--rw-r--r--   0 root         (0) root         (0)    15215 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ht.7ca68737.svg
--rw-r--r--   0 root         (0) root         (0)      274 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/hu.692e97ca.svg
--rw-r--r--   0 root         (0) root         (0)      276 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/hu.b10d3f8e.svg
--rw-r--r--   0 root         (0) root         (0)      239 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/id.94464e47.svg
--rw-r--r--   0 root         (0) root         (0)      237 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/id.a05dc04c.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ie.5154112a.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ie.e23b25d1.svg
--rw-r--r--   0 root         (0) root         (0)      848 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/il.150f4c5f.svg
--rw-r--r--   0 root         (0) root         (0)      895 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/il.e02a66d3.svg
--rw-r--r--   0 root         (0) root         (0)    10253 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/im.25166c91.svg
--rw-r--r--   0 root         (0) root         (0)     9925 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/im.942419c5.svg
--rw-r--r--   0 root         (0) root         (0)     1074 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/in.954929a0.svg
--rw-r--r--   0 root         (0) root         (0)     1088 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/in.bd0d4f19.svg
--rw-r--r--   0 root         (0) root         (0)    27443 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/io.a59923ab.svg
--rw-r--r--   0 root         (0) root         (0)    27465 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/io.fa003484.svg
--rw-r--r--   0 root         (0) root         (0)     1476 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/iq.1232a5c2.svg
--rw-r--r--   0 root         (0) root         (0)     1481 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/iq.9a48d678.svg
--rw-r--r--   0 root         (0) root         (0)    15448 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ir.1ed24953.svg
--rw-r--r--   0 root         (0) root         (0)    15360 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ir.bc7ae9e1.svg
--rw-r--r--   0 root         (0) root         (0)      518 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/is.cad57f19.svg
--rw-r--r--   0 root         (0) root         (0)      526 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/is.eea59326.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/it.039b4527.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/it.e8516fc7.svg
--rw-r--r--   0 root         (0) root         (0)     4699 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/je.1684dacc.svg
--rw-r--r--   0 root         (0) root         (0)     4718 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/je.3ed72a25.svg
--rw-r--r--   0 root         (0) root         (0)     1120 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/jellyfin.7b53a541.svg
--rw-r--r--   0 root         (0) root         (0)      389 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/jm.2357530e.svg
--rw-r--r--   0 root         (0) root         (0)      389 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/jm.479f30fe.svg
--rw-r--r--   0 root         (0) root         (0)      691 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/jo.06fbaa2c.svg
--rw-r--r--   0 root         (0) root         (0)      714 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/jo.7ac45a65.svg
--rw-r--r--   0 root         (0) root         (0)      497 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/jp.1795778c.svg
--rw-r--r--   0 root         (0) root         (0)      481 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/jp.b6063838.svg
--rw-r--r--   0 root         (0) root         (0)     1380 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ke.6dbfffd5.svg
--rw-r--r--   0 root         (0) root         (0)     1492 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ke.769bb975.svg
--rw-r--r--   0 root         (0) root         (0)     3334 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kg.96c12490.svg
--rw-r--r--   0 root         (0) root         (0)     3383 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kg.daded53c.svg
--rw-r--r--   0 root         (0) root         (0)     7282 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kh.8eeb1634.svg
--rw-r--r--   0 root         (0) root         (0)     7283 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kh.b10339d6.svg
--rw-r--r--   0 root         (0) root         (0)     5950 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ki.033ff9ce.svg
--rw-r--r--   0 root         (0) root         (0)     5815 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ki.89e43a21.svg
--rw-r--r--   0 root         (0) root         (0)     1058 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/km.1e3bd5fe.svg
--rw-r--r--   0 root         (0) root         (0)     1041 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/km.3ffb0228.svg
--rw-r--r--   0 root         (0) root         (0)      813 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kn.0c16fe68.svg
--rw-r--r--   0 root         (0) root         (0)      817 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kn.8f2e7b29.svg
--rw-r--r--   0 root         (0) root         (0)     1370 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kodi.d18f8d23.svg
--rw-r--r--   0 root         (0) root         (0)      789 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kp.0f5253d8.svg
--rw-r--r--   0 root         (0) root         (0)      852 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kp.f4ff9e76.svg
--rw-r--r--   0 root         (0) root         (0)     1725 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kr.0dc8b972.svg
--rw-r--r--   0 root         (0) root         (0)     1819 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kr.0f5e1116.svg
--rw-r--r--   0 root         (0) root         (0)      503 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kw.3b4f3ea3.svg
--rw-r--r--   0 root         (0) root         (0)      507 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kw.830d3755.svg
--rw-r--r--   0 root         (0) root         (0)    22455 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ky.be81d90b.svg
--rw-r--r--   0 root         (0) root         (0)    21834 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ky.e3b76b32.svg
--rw-r--r--   0 root         (0) root         (0)    11422 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kz.32ac1036.svg
--rw-r--r--   0 root         (0) root         (0)    11334 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kz.579ac0f9.svg
--rw-r--r--   0 root         (0) root         (0)      454 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/la.e583f8ec.svg
--rw-r--r--   0 root         (0) root         (0)      504 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/la.f71017ef.svg
--rw-r--r--   0 root         (0) root         (0)     2750 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/lb.8eea508a.svg
--rw-r--r--   0 root         (0) root         (0)     2811 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/lb.bdbeb8f1.svg
--rw-r--r--   0 root         (0) root         (0)      370 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/lc.25f644a6.svg
--rw-r--r--   0 root         (0) root         (0)      370 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/lc.68bd77ae.svg
--rw-r--r--   0 root         (0) root         (0)     8318 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/li.8dc1ed79.svg
--rw-r--r--   0 root         (0) root         (0)     8341 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/li.d7e2a871.svg
--rw-r--r--   0 root         (0) root         (0)    11326 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/lk.42c41c61.svg
--rw-r--r--   0 root         (0) root         (0)    11338 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/lk.e52240d6.svg
--rw-r--r--   0 root         (0) root         (0)      721 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/lr.5b84ff00.svg
--rw-r--r--   0 root         (0) root         (0)      694 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/lr.9a67cd3d.svg
--rw-r--r--   0 root         (0) root         (0)     1219 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ls.6d444cae.svg
--rw-r--r--   0 root         (0) root         (0)     1242 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ls.fe1da403.svg
--rw-r--r--   0 root         (0) root         (0)      442 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/lt.03a2e8c1.svg
--rw-r--r--   0 root         (0) root         (0)      442 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/lt.b57ea2a8.svg
--rw-r--r--   0 root         (0) root         (0)      228 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/lu.93878a1b.svg
--rw-r--r--   0 root         (0) root         (0)      232 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/lu.e3bdc6d3.svg
--rw-r--r--   0 root         (0) root         (0)      237 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/lv.1853e3a0.svg
--rw-r--r--   0 root         (0) root         (0)      233 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/lv.679c099e.svg
--rw-r--r--   0 root         (0) root         (0)      531 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ly.05f8732e.svg
--rw-r--r--   0 root         (0) root         (0)      530 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ly.b9e750ff.svg
--rw-r--r--   0 root         (0) root         (0)      250 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ma.65053fc4.svg
--rw-r--r--   0 root         (0) root         (0)      250 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ma.88ada30c.svg
--rw-r--r--   0 root         (0) root         (0)      237 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mc.2c03ea5c.svg
--rw-r--r--   0 root         (0) root         (0)      237 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mc.89b532e8.svg
--rw-r--r--   0 root         (0) root         (0)    11264 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/md.646818c3.svg
--rw-r--r--   0 root         (0) root         (0)    11368 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/md.a56562ee.svg
--rw-r--r--   0 root         (0) root         (0)    63990 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/me.2e71b778.svg
--rw-r--r--   0 root         (0) root         (0)    62977 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/me.f05548f2.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mf.70d09a4a.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mf.7da6b3d2.svg
--rw-r--r--   0 root         (0) root         (0)      302 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mg.09ca17b2.svg
--rw-r--r--   0 root         (0) root         (0)      302 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mg.b3fff4a6.svg
--rw-r--r--   0 root         (0) root         (0)      741 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mh.3fd69bb2.svg
--rw-r--r--   0 root         (0) root         (0)      763 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mh.f6cbc774.svg
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mk.4234a248.svg
--rw-r--r--   0 root         (0) root         (0)      382 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mk.e5412079.svg
--rw-r--r--   0 root         (0) root         (0)      279 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ml.3fad079e.svg
--rw-r--r--   0 root         (0) root         (0)      276 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ml.4f0dba9e.svg
--rw-r--r--   0 root         (0) root         (0)      865 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mm.8ac1f094.svg
--rw-r--r--   0 root         (0) root         (0)      848 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mm.adaa2111.svg
--rw-r--r--   0 root         (0) root         (0)     1253 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mn.78547af0.svg
--rw-r--r--   0 root         (0) root         (0)     1259 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mn.a4bcb0e6.svg
--rw-r--r--   0 root         (0) root         (0)     1547 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mo.2f0d2c15.svg
--rw-r--r--   0 root         (0) root         (0)     1511 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mo.c8198565.svg
--rw-r--r--   0 root         (0) root         (0)    23656 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mp.2acb5506.svg
--rw-r--r--   0 root         (0) root         (0)    23415 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mp.eeeefff6.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mq.145a7657.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mq.bb36a8fc.svg
--rw-r--r--   0 root         (0) root         (0)      447 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mr.dd34eae8.svg
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mr.e91e06ea.svg
--rw-r--r--   0 root         (0) root         (0)     6785 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ms.2025cd7d.svg
--rw-r--r--   0 root         (0) root         (0)     6693 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ms.b13001dc.svg
--rw-r--r--   0 root         (0) root         (0)    10513 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mt.b6f71c85.svg
--rw-r--r--   0 root         (0) root         (0)     8803 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mt.cff39ee0.svg
--rw-r--r--   0 root         (0) root         (0)      319 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mu.51f71163.svg
--rw-r--r--   0 root         (0) root         (0)      319 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mu.a926c232.svg
--rw-r--r--   0 root         (0) root         (0)      307 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mv.2c8b92b5.svg
--rw-r--r--   0 root         (0) root         (0)      289 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mv.ba4de4fd.svg
--rw-r--r--   0 root         (0) root         (0)     3708 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mw.0b005148.svg
--rw-r--r--   0 root         (0) root         (0)     3891 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mw.f704f4bb.svg
--rw-r--r--   0 root         (0) root         (0)    95527 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mx.1b615ec2.svg
--rw-r--r--   0 root         (0) root         (0)    91037 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mx.8a36b075.svg
--rw-r--r--   0 root         (0) root         (0)     1279 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/my.4109ae71.svg
--rw-r--r--   0 root         (0) root         (0)     1271 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/my.69c87fc5.svg
--rw-r--r--   0 root         (0) root         (0)     2618 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mz.1377650b.svg
--rw-r--r--   0 root         (0) root         (0)     2601 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mz.2c96acb1.svg
--rw-r--r--   0 root         (0) root         (0)      980 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/na.7adf4344.svg
--rw-r--r--   0 root         (0) root         (0)     1002 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/na.e0503926.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/nc.96fa6a4b.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/nc.b5a5d41b.svg
--rw-r--r--   0 root         (0) root         (0)      276 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ne.d11b82c6.svg
--rw-r--r--   0 root         (0) root         (0)      282 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ne.d4fe4faa.svg
--rw-r--r--   0 root         (0) root         (0)     5595 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/nf.1e8c700b.svg
--rw-r--r--   0 root         (0) root         (0)     5842 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/nf.a7166b00.svg
--rw-r--r--   0 root         (0) root         (0)      260 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ng.51059407.svg
--rw-r--r--   0 root         (0) root         (0)      260 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ng.c3b42ad2.svg
--rw-r--r--   0 root         (0) root         (0)    18572 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ni.5b80bac0.svg
--rw-r--r--   0 root         (0) root         (0)    18632 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ni.cc7eb514.svg
--rw-r--r--   0 root         (0) root         (0)      239 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/nl.dd138444.svg
--rw-r--r--   0 root         (0) root         (0)      245 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/nl.e415f0e7.svg
--rw-r--r--   0 root         (0) root         (0)      321 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/no.26996afa.svg
--rw-r--r--   0 root         (0) root         (0)      321 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/no.70157234.svg
--rw-r--r--   0 root         (0) root         (0)     1058 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/np.954177a0.svg
--rw-r--r--   0 root         (0) root         (0)     1196 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/np.f7b8a5c3.svg
--rw-r--r--   0 root         (0) root         (0)      645 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/nr.2c66d218.svg
--rw-r--r--   0 root         (0) root         (0)      668 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/nr.a4f0e762.svg
--rw-r--r--   0 root         (0) root         (0)     1742 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/nu.26551dc2.svg
--rw-r--r--   0 root         (0) root         (0)     1730 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/nu.860bbe8a.svg
--rw-r--r--   0 root         (0) root         (0)     2974 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/nz.38d0d690.svg
--rw-r--r--   0 root         (0) root         (0)     2999 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/nz.c77ae58d.svg
--rw-r--r--   0 root         (0) root         (0)    22825 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/om.3f5691ca.svg
--rw-r--r--   0 root         (0) root         (0)    22841 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/om.ff034f9e.svg
--rw-r--r--   0 root         (0) root         (0)      743 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pa.6dc8212a.svg
--rw-r--r--   0 root         (0) root         (0)      659 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pa.acde3214.svg
--rw-r--r--   0 root         (0) root         (0)    74209 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pe.5a3b0bc5.svg
--rw-r--r--   0 root         (0) root         (0)    73524 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pe.5c2ced95.svg
--rw-r--r--   0 root         (0) root         (0)     4288 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pf.9f06082b.svg
--rw-r--r--   0 root         (0) root         (0)     4230 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pf.f6ae1bc8.svg
--rw-r--r--   0 root         (0) root         (0)     1667 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pg.26847b33.svg
--rw-r--r--   0 root         (0) root         (0)     2099 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pg.66c8dc3b.svg
--rw-r--r--   0 root         (0) root         (0)     1578 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ph.12e2b123.svg
--rw-r--r--   0 root         (0) root         (0)     1522 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ph.f215833e.svg
--rw-r--r--   0 root         (0) root         (0)      740 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pk.0bbf58be.svg
--rw-r--r--   0 root         (0) root         (0)      691 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pk.32b55f6f.svg
--rw-r--r--   0 root         (0) root         (0)      222 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pl.03886843.svg
--rw-r--r--   0 root         (0) root         (0)      222 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pl.a1350f0c.svg
--rw-r--r--   0 root         (0) root         (0)      191 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/plex.7a4e22a6.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pm.7a6beab5.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pm.a5590fa3.svg
--rw-r--r--   0 root         (0) root         (0)     8592 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pn.00a9342b.svg
--rw-r--r--   0 root         (0) root         (0)    10939 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pn.715fd11d.svg
--rw-r--r--   0 root         (0) root         (0)      619 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pr.391a48e2.svg
--rw-r--r--   0 root         (0) root         (0)      631 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pr.b37cbdc4.svg
--rw-r--r--   0 root         (0) root         (0)      541 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ps.1af72ed4.svg
--rw-r--r--   0 root         (0) root         (0)      555 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ps.96bcac74.svg
--rw-r--r--   0 root         (0) root         (0)     8748 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pt.0703cc3a.svg
--rw-r--r--   0 root         (0) root         (0)     8369 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pt.351b87cb.svg
--rw-r--r--   0 root         (0) root         (0)      464 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pw.17220ffb.svg
--rw-r--r--   0 root         (0) root         (0)      509 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pw.6d8e7ce0.svg
--rw-r--r--   0 root         (0) root         (0)    17460 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/py.25cc39e3.svg
--rw-r--r--   0 root         (0) root         (0)    17301 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/py.c20318c9.svg
--rw-r--r--   0 root         (0) root         (0)      356 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/qa.7e695788.svg
--rw-r--r--   0 root         (0) root         (0)      359 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/qa.86452d7a.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/re.b8140129.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/re.cf143c2f.svg
--rw-r--r--   0 root         (0) root         (0)      305 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ro.67f8501e.svg
--rw-r--r--   0 root         (0) root         (0)      305 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ro.cab93784.svg
--rw-r--r--   0 root         (0) root         (0)   187637 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/rs.23638d75.svg
--rw-r--r--   0 root         (0) root         (0)   187500 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/rs.ae2e3422.svg
--rw-r--r--   0 root         (0) root         (0)      290 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ru.ccd50623.svg
--rw-r--r--   0 root         (0) root         (0)      286 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ru.edd8b008.svg
--rw-r--r--   0 root         (0) root         (0)      748 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/rw.87d5d899.svg
--rw-r--r--   0 root         (0) root         (0)      747 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/rw.d118aacd.svg
--rw-r--r--   0 root         (0) root         (0)    10225 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sa.5bfbe72b.svg
--rw-r--r--   0 root         (0) root         (0)    10290 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sa.f0a8997b.svg
--rw-r--r--   0 root         (0) root         (0)      947 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sb.1c406073.svg
--rw-r--r--   0 root         (0) root         (0)      952 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sb.b0db5b0a.svg
--rw-r--r--   0 root         (0) root         (0)      570 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sc.0452f14c.svg
--rw-r--r--   0 root         (0) root         (0)      565 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sc.cdc20672.svg
--rw-r--r--   0 root         (0) root         (0)      491 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sd.0e619868.svg
--rw-r--r--   0 root         (0) root         (0)      493 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sd.da3b68ee.svg
--rw-r--r--   0 root         (0) root         (0)      685 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/se.7e499d82.svg
--rw-r--r--   0 root         (0) root         (0)      698 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/se.7ec71700.svg
--rw-r--r--   0 root         (0) root         (0)      951 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sg.4f0e8eff.svg
--rw-r--r--   0 root         (0) root         (0)      886 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sg.8a63b009.svg
--rw-r--r--   0 root         (0) root         (0)    29664 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sh.46e2588d.svg
--rw-r--r--   0 root         (0) root         (0)    30261 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sh.681f8fff.svg
--rw-r--r--   0 root         (0) root         (0)     2049 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/si.2a428364.svg
--rw-r--r--   0 root         (0) root         (0)     2065 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/si.d9d425c0.svg
--rw-r--r--   0 root         (0) root         (0)      321 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sj.638e6522.svg
--rw-r--r--   0 root         (0) root         (0)      321 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sj.92c583b8.svg
--rw-r--r--   0 root         (0) root         (0)     1203 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sk.7998d1f5.svg
--rw-r--r--   0 root         (0) root         (0)     1178 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sk.93c91c0b.svg
--rw-r--r--   0 root         (0) root         (0)      275 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sl.d8378c47.svg
--rw-r--r--   0 root         (0) root         (0)      438 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sl.eb9dda3f.svg
--rw-r--r--   0 root         (0) root         (0)    15876 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sm.0ba901f4.svg
--rw-r--r--   0 root         (0) root         (0)    15947 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sm.5e2fc188.svg
--rw-r--r--   0 root         (0) root         (0)      424 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sn.4247b831.svg
--rw-r--r--   0 root         (0) root         (0)      414 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sn.98923b55.svg
--rw-r--r--   0 root         (0) root         (0)      491 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/so.2d18a203.svg
--rw-r--r--   0 root         (0) root         (0)      498 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/so.45f08b28.svg
--rw-r--r--   0 root         (0) root         (0)      315 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sr.cb178d98.svg
--rw-r--r--   0 root         (0) root         (0)      320 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sr.d66c1240.svg
--rw-r--r--   0 root         (0) root         (0)      386 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ss.caedfdf2.svg
--rw-r--r--   0 root         (0) root         (0)      397 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ss.db181f81.svg
--rw-r--r--   0 root         (0) root         (0)      920 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/st.a70042c6.svg
--rw-r--r--   0 root         (0) root         (0)      916 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/st.ecc4827f.svg
--rw-r--r--   0 root         (0) root         (0)    84167 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sv.9501935a.svg
--rw-r--r--   0 root         (0) root         (0)    83639 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sv.f67839a6.svg
--rw-r--r--   0 root         (0) root         (0)    13097 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sx.77e864f0.svg
--rw-r--r--   0 root         (0) root         (0)    13294 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sx.c0e6297a.svg
--rw-r--r--   0 root         (0) root         (0)      565 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sy.2b3eac89.svg
--rw-r--r--   0 root         (0) root         (0)      579 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sy.7fe894df.svg
--rw-r--r--   0 root         (0) root         (0)     6747 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sz.70b6fc50.svg
--rw-r--r--   0 root         (0) root         (0)     6700 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sz.eb01cd9f.svg
--rw-r--r--   0 root         (0) root         (0)    14766 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tc.30ccd48e.svg
--rw-r--r--   0 root         (0) root         (0)    14507 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tc.651466dd.svg
--rw-r--r--   0 root         (0) root         (0)      267 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/td.5d622e26.svg
--rw-r--r--   0 root         (0) root         (0)      279 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/td.f1319408.svg
--rw-r--r--   0 root         (0) root         (0)     1196 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tf.27cbe00b.svg
--rw-r--r--   0 root         (0) root         (0)     1088 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tf.a1757237.svg
--rw-r--r--   0 root         (0) root         (0)      722 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tg.b492a751.svg
--rw-r--r--   0 root         (0) root         (0)      733 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tg.d04f874c.svg
--rw-r--r--   0 root         (0) root         (0)      288 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/th.79b63a8a.svg
--rw-r--r--   0 root         (0) root         (0)      287 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/th.b8e24edb.svg
--rw-r--r--   0 root         (0) root         (0)     1785 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tj.b7dafe8d.svg
--rw-r--r--   0 root         (0) root         (0)     1828 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tj.d3a42312.svg
--rw-r--r--   0 root         (0) root         (0)      788 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tk.6c1f520c.svg
--rw-r--r--   0 root         (0) root         (0)      778 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tk.f87f794b.svg
--rw-r--r--   0 root         (0) root         (0)      597 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tl.85904d79.svg
--rw-r--r--   0 root         (0) root         (0)      577 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tl.ca9af3c0.svg
--rw-r--r--   0 root         (0) root         (0)    31846 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tm.762df128.svg
--rw-r--r--   0 root         (0) root         (0)    32561 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tm.e467552c.svg
--rw-r--r--   0 root         (0) root         (0)      740 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tn.cc3ab493.svg
--rw-r--r--   0 root         (0) root         (0)      750 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tn.ff4c5190.svg
--rw-r--r--   0 root         (0) root         (0)      355 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/to.8dd22284.svg
--rw-r--r--   0 root         (0) root         (0)      361 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/to.9748a967.svg
--rw-r--r--   0 root         (0) root         (0)      554 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tr.87e40d5c.svg
--rw-r--r--   0 root         (0) root         (0)      575 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tr.fc8c91dd.svg
--rw-r--r--   0 root         (0) root         (0)      320 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tt.4acf6cc2.svg
--rw-r--r--   0 root         (0) root         (0)      315 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tt.5a459e81.svg
--rw-r--r--   0 root         (0) root         (0)     2296 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tv.9717b553.svg
--rw-r--r--   0 root         (0) root         (0)     2163 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tv.a8ff4939.svg
--rw-r--r--   0 root         (0) root         (0)      957 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tw.45c8a106.svg
--rw-r--r--   0 root         (0) root         (0)      942 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tw.c0cf9ea7.svg
--rw-r--r--   0 root         (0) root         (0)      602 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tz.1abfbb38.svg
--rw-r--r--   0 root         (0) root         (0)      543 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tz.c27fd405.svg
--rw-r--r--   0 root         (0) root         (0)      238 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ua.04fa0e67.svg
--rw-r--r--   0 root         (0) root         (0)      238 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ua.63d75c84.svg
--rw-r--r--   0 root         (0) root         (0)     3953 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ug.5ac71e98.svg
--rw-r--r--   0 root         (0) root         (0)     4034 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ug.5ae165a2.svg
--rw-r--r--   0 root         (0) root         (0)     3972 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/um.582dd57b.svg
--rw-r--r--   0 root         (0) root         (0)     4517 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/um.b38f913c.svg
--rw-r--r--   0 root         (0) root         (0)    20221 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/un.2df110d6.svg
--rw-r--r--   0 root         (0) root         (0)    20456 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/un.58a4a02a.svg
--rw-r--r--   0 root         (0) root         (0)     3921 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/us.6c459052.svg
--rw-r--r--   0 root         (0) root         (0)     4461 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/us.99e04236.svg
--rw-r--r--   0 root         (0) root         (0)     1715 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/uy.69cf8938.svg
--rw-r--r--   0 root         (0) root         (0)     1718 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/uy.b70ac310.svg
--rw-r--r--   0 root         (0) root         (0)     1454 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/uz.7f8823a2.svg
--rw-r--r--   0 root         (0) root         (0)     1454 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/uz.d53abc35.svg
--rw-r--r--   0 root         (0) root         (0)    91211 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/va.7efb8ba6.svg
--rw-r--r--   0 root         (0) root         (0)    90846 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/va.abcb42e8.svg
--rw-r--r--   0 root         (0) root         (0)      451 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/vc.37cf5ba1.svg
--rw-r--r--   0 root         (0) root         (0)      498 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/vc.3e4ac6d4.svg
--rw-r--r--   0 root         (0) root         (0)     1168 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ve.4cd0e3ed.svg
--rw-r--r--   0 root         (0) root         (0)     1188 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ve.9cd63506.svg
--rw-r--r--   0 root         (0) root         (0)    24993 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/vg.025b8b6a.svg
--rw-r--r--   0 root         (0) root         (0)    24793 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/vg.ae3b6f7e.svg
--rw-r--r--   0 root         (0) root         (0)     8711 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/vi.293e6f1c.svg
--rw-r--r--   0 root         (0) root         (0)     8757 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/vi.f920eec7.svg
--rw-r--r--   0 root         (0) root         (0)      498 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/vn.11dd1cf6.svg
--rw-r--r--   0 root         (0) root         (0)      488 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/vn.9ec4ca4d.svg
--rw-r--r--   0 root         (0) root         (0)     3768 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/vu.5d2d7643.svg
--rw-r--r--   0 root         (0) root         (0)     3735 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/vu.b7a8d91a.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/wf.69c77016.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/wf.9ca6f4bc.svg
--rw-r--r--   0 root         (0) root         (0)      693 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ws.15c7a17c.svg
--rw-r--r--   0 root         (0) root         (0)      706 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ws.d2e19e5a.svg
--rw-r--r--   0 root         (0) root         (0)     9003 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/xk.16b6bb85.svg
--rw-r--r--   0 root         (0) root         (0)     9679 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/xk.ca7843be.svg
--rw-r--r--   0 root         (0) root         (0)      275 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ye.0b3f3c76.svg
--rw-r--r--   0 root         (0) root         (0)      275 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ye.bb567731.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/yt.332bd5d3.svg
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/yt.c33641ca.svg
--rw-r--r--   0 root         (0) root         (0)      872 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/za.2fa94205.svg
--rw-r--r--   0 root         (0) root         (0)      853 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/za.42e033a9.svg
--rw-r--r--   0 root         (0) root         (0)     5503 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/zm.92477cab.svg
--rw-r--r--   0 root         (0) root         (0)     5419 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/zm.ce5363b7.svg
--rw-r--r--   0 root         (0) root         (0)     6759 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/zw.6a535c1e.svg
--rw-r--r--   0 root         (0) root         (0)     6780 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/zw.f488cb8a.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.351315 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/
--rw-r--r--   0 root         (0) root         (0)      420 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1088.8670f8f4.js
--rw-r--r--   0 root         (0) root         (0)     1049 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1088.8670f8f4.js.map
--rw-r--r--   0 root         (0) root         (0)    35353 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1259.11016ad1.js
--rw-r--r--   0 root         (0) root         (0)    97910 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1259.11016ad1.js.map
--rw-r--r--   0 root         (0) root         (0)    13278 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1449.475ec524.js
--rw-r--r--   0 root         (0) root         (0)    43973 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1449.475ec524.js.map
--rw-r--r--   0 root         (0) root         (0)     9432 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1512.3e4f99fd.js
--rw-r--r--   0 root         (0) root         (0)    21297 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1512.3e4f99fd.js.map
--rw-r--r--   0 root         (0) root         (0)    16017 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1587.e2ebe369.js
--rw-r--r--   0 root         (0) root         (0)    48235 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1587.e2ebe369.js.map
--rw-r--r--   0 root         (0) root         (0)     1111 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/169.8bb8df7d.js
--rw-r--r--   0 root         (0) root         (0)     2916 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/169.8bb8df7d.js.map
--rw-r--r--   0 root         (0) root         (0)     1931 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1706.97f9b825.js
--rw-r--r--   0 root         (0) root         (0)     4723 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1706.97f9b825.js.map
--rw-r--r--   0 root         (0) root         (0)    22004 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1807.586a24d4.js
--rw-r--r--   0 root         (0) root         (0)    60878 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1807.586a24d4.js.map
--rw-r--r--   0 root         (0) root         (0)     3339 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1949.9d6edfd8.js
--rw-r--r--   0 root         (0) root         (0)     9056 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1949.9d6edfd8.js.map
--rw-r--r--   0 root         (0) root         (0)     2575 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2106.6553ebed.js
--rw-r--r--   0 root         (0) root         (0)     7033 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2106.6553ebed.js.map
--rw-r--r--   0 root         (0) root         (0)     4924 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2140.10cab5fd.js
--rw-r--r--   0 root         (0) root         (0)    15185 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2140.10cab5fd.js.map
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2183.2941880a.js
--rw-r--r--   0 root         (0) root         (0)     1086 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2183.2941880a.js.map
--rw-r--r--   0 root         (0) root         (0)     1038 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2200.9fc9fd95.js
--rw-r--r--   0 root         (0) root         (0)     2498 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2200.9fc9fd95.js.map
--rw-r--r--   0 root         (0) root         (0)      863 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2217.30568f1a.js
--rw-r--r--   0 root         (0) root         (0)     2227 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2217.30568f1a.js.map
--rw-r--r--   0 root         (0) root         (0)     1010 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2460.9845df8e.js
--rw-r--r--   0 root         (0) root         (0)     2479 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2460.9845df8e.js.map
--rw-r--r--   0 root         (0) root         (0)    55875 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2509.efc0bf4c.js
--rw-r--r--   0 root         (0) root         (0)   141746 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2509.efc0bf4c.js.map
--rw-r--r--   0 root         (0) root         (0)      444 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2614.7997d726.js
--rw-r--r--   0 root         (0) root         (0)     1114 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2614.7997d726.js.map
--rw-r--r--   0 root         (0) root         (0)      415 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2732.28f617e8.js
--rw-r--r--   0 root         (0) root         (0)     1036 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2732.28f617e8.js.map
--rw-r--r--   0 root         (0) root         (0)     1744 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2853.47a43033.js
--rw-r--r--   0 root         (0) root         (0)     5624 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2853.47a43033.js.map
--rw-r--r--   0 root         (0) root         (0)     1044 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2892.2d33f676.js
--rw-r--r--   0 root         (0) root         (0)     3070 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2892.2d33f676.js.map
--rw-r--r--   0 root         (0) root         (0)     2482 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2893.b037e7d2.js
--rw-r--r--   0 root         (0) root         (0)     5660 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2893.b037e7d2.js.map
--rw-r--r--   0 root         (0) root         (0)     5450 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2976.e8a9eb12.js
--rw-r--r--   0 root         (0) root         (0)    16326 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2976.e8a9eb12.js.map
--rw-r--r--   0 root         (0) root         (0)    10076 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3083.8440bfa8.js
--rw-r--r--   0 root         (0) root         (0)    28154 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3083.8440bfa8.js.map
--rw-r--r--   0 root         (0) root         (0)      764 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3322.5ee98346.js
--rw-r--r--   0 root         (0) root         (0)     2088 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3322.5ee98346.js.map
--rw-r--r--   0 root         (0) root         (0)     2607 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3368.7ff6fca3.js
--rw-r--r--   0 root         (0) root         (0)     6949 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3368.7ff6fca3.js.map
--rw-r--r--   0 root         (0) root         (0)     5282 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3369.71760407.js
--rw-r--r--   0 root         (0) root         (0)    11158 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3369.71760407.js.map
--rw-r--r--   0 root         (0) root         (0)    10107 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3400.1021c9a8.js
--rw-r--r--   0 root         (0) root         (0)    28210 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3400.1021c9a8.js.map
--rw-r--r--   0 root         (0) root         (0)     1805 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/342.d3c0f8f2.js
--rw-r--r--   0 root         (0) root         (0)     5953 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/342.d3c0f8f2.js.map
--rw-r--r--   0 root         (0) root         (0)      452 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3518.40e74ddb.js
--rw-r--r--   0 root         (0) root         (0)     1131 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3518.40e74ddb.js.map
--rw-r--r--   0 root         (0) root         (0)    45695 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3553.125dc216.js
--rw-r--r--   0 root         (0) root         (0)   114423 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3553.125dc216.js.map
--rw-r--r--   0 root         (0) root         (0)     1220 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3559.da067b47.js
--rw-r--r--   0 root         (0) root         (0)     3059 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3559.da067b47.js.map
--rw-r--r--   0 root         (0) root         (0)     1737 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3732.17c9c669.js
--rw-r--r--   0 root         (0) root         (0)     5607 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3732.17c9c669.js.map
--rw-r--r--   0 root         (0) root         (0)     2316 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3835.878348e2.js
--rw-r--r--   0 root         (0) root         (0)     9498 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3835.878348e2.js.map
--rw-r--r--   0 root         (0) root         (0)     5620 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3924.9592f111.js
--rw-r--r--   0 root         (0) root         (0)    14954 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3924.9592f111.js.map
--rw-r--r--   0 root         (0) root         (0)     7918 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/4053.1a106579.js
--rw-r--r--   0 root         (0) root         (0)    19391 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/4053.1a106579.js.map
--rw-r--r--   0 root         (0) root         (0)      633 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/4221.292aeb44.js
--rw-r--r--   0 root         (0) root         (0)     2174 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/4221.292aeb44.js.map
--rw-r--r--   0 root         (0) root         (0)     1416 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/446.178d2754.js
--rw-r--r--   0 root         (0) root         (0)     4379 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/446.178d2754.js.map
--rw-r--r--   0 root         (0) root         (0)     7765 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/4589.c6a12ddf.js
--rw-r--r--   0 root         (0) root         (0)    18764 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/4589.c6a12ddf.js.map
--rw-r--r--   0 root         (0) root         (0)     1201 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/4619.ea41fd5e.js
--rw-r--r--   0 root         (0) root         (0)     3333 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/4619.ea41fd5e.js.map
--rw-r--r--   0 root         (0) root         (0)     6803 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/472.05f32d73.js
--rw-r--r--   0 root         (0) root         (0)    18143 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/472.05f32d73.js.map
--rw-r--r--   0 root         (0) root         (0)      444 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/4765.7ad68124.js
--rw-r--r--   0 root         (0) root         (0)     1114 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/4765.7ad68124.js.map
--rw-r--r--   0 root         (0) root         (0)      125 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5207.7f241e21.js
--rw-r--r--   0 root         (0) root         (0)    27243 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5285.551ed2ce.js
--rw-r--r--   0 root         (0) root         (0)    74761 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5285.551ed2ce.js.map
--rw-r--r--   0 root         (0) root         (0)     9111 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5324.a449638b.js
--rw-r--r--   0 root         (0) root         (0)    20342 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5324.a449638b.js.map
--rw-r--r--   0 root         (0) root         (0)     4526 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5329.7bf8697f.js
--rw-r--r--   0 root         (0) root         (0)     9566 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5329.7bf8697f.js.map
--rw-r--r--   0 root         (0) root         (0)     1449 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5578.7c9eef7c.js
--rw-r--r--   0 root         (0) root         (0)     3571 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5578.7c9eef7c.js.map
--rw-r--r--   0 root         (0) root         (0)     2183 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5638.f1abcb64.js
--rw-r--r--   0 root         (0) root         (0)     5966 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5638.f1abcb64.js.map
--rw-r--r--   0 root         (0) root         (0)     2717 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5762.0d8fb9cb.js
--rw-r--r--   0 root         (0) root         (0)     8162 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5762.0d8fb9cb.js.map
--rw-r--r--   0 root         (0) root         (0)     7421 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5795.8f7061d6.js
--rw-r--r--   0 root         (0) root         (0)    22573 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5795.8f7061d6.js.map
--rw-r--r--   0 root         (0) root         (0)    15417 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5931.bcf6cfaf.js
--rw-r--r--   0 root         (0) root         (0)    41562 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5931.bcf6cfaf.js.map
--rw-r--r--   0 root         (0) root         (0)    29283 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6062.2509fe58.js
--rw-r--r--   0 root         (0) root         (0)    63711 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6062.2509fe58.js.map
--rw-r--r--   0 root         (0) root         (0)     4988 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6123.0a491498.js
--rw-r--r--   0 root         (0) root         (0)    15776 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6123.0a491498.js.map
--rw-r--r--   0 root         (0) root         (0)     9419 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6148.70084131.js
--rw-r--r--   0 root         (0) root         (0)    21271 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6148.70084131.js.map
--rw-r--r--   0 root         (0) root         (0)     2947 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6324.9d695c83.js
--rw-r--r--   0 root         (0) root         (0)     7263 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6324.9d695c83.js.map
--rw-r--r--   0 root         (0) root         (0)     1288 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6362.7e4f1ac1.js
--rw-r--r--   0 root         (0) root         (0)     3000 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6362.7e4f1ac1.js.map
--rw-r--r--   0 root         (0) root         (0)      121 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/65.ae7df477.js
--rw-r--r--   0 root         (0) root         (0)     1498 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6523.6faff1f9.js
--rw-r--r--   0 root         (0) root         (0)     4426 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6523.6faff1f9.js.map
--rw-r--r--   0 root         (0) root         (0)      357 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6640.a6538b3b.js
--rw-r--r--   0 root         (0) root         (0)      995 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6640.a6538b3b.js.map
--rw-r--r--   0 root         (0) root         (0)     4404 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/667.f23239a7.js
--rw-r--r--   0 root         (0) root         (0)    12046 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/667.f23239a7.js.map
--rw-r--r--   0 root         (0) root         (0)     1747 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7089.f4d74b4a.js
--rw-r--r--   0 root         (0) root         (0)     5634 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7089.f4d74b4a.js.map
--rw-r--r--   0 root         (0) root         (0)     8258 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/729.f4de5689.js
--rw-r--r--   0 root         (0) root         (0)    19267 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/729.f4de5689.js.map
--rw-r--r--   0 root         (0) root         (0)     9685 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7381.66ebc1f2.js
--rw-r--r--   0 root         (0) root         (0)    21916 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7381.66ebc1f2.js.map
--rw-r--r--   0 root         (0) root         (0)     1441 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/746.4c6b0061.js
--rw-r--r--   0 root         (0) root         (0)     3351 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/746.4c6b0061.js.map
--rw-r--r--   0 root         (0) root         (0)     1804 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7590.014063f7.js
--rw-r--r--   0 root         (0) root         (0)     4865 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7590.014063f7.js.map
--rw-r--r--   0 root         (0) root         (0)      450 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7819.15635e35.js
--rw-r--r--   0 root         (0) root         (0)     1133 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7819.15635e35.js.map
--rw-r--r--   0 root         (0) root         (0)    15147 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7841.8b124a1f.js
--rw-r--r--   0 root         (0) root         (0)    45071 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7841.8b124a1f.js.map
--rw-r--r--   0 root         (0) root         (0)    15987 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7878.98038a22.js
--rw-r--r--   0 root         (0) root         (0)    46669 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7878.98038a22.js.map
--rw-r--r--   0 root         (0) root         (0)    46543 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7880.b455063a.js
--rw-r--r--   0 root         (0) root         (0)   111831 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7880.b455063a.js.map
--rw-r--r--   0 root         (0) root         (0)     3614 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7898.0426589e.js
--rw-r--r--   0 root         (0) root         (0)    10984 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7898.0426589e.js.map
--rw-r--r--   0 root         (0) root         (0)    11595 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7968.d677b422.js
--rw-r--r--   0 root         (0) root         (0)    28428 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7968.d677b422.js.map
--rw-r--r--   0 root         (0) root         (0)     9430 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/813.1fe7c13a.js
--rw-r--r--   0 root         (0) root         (0)    21299 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/813.1fe7c13a.js.map
--rw-r--r--   0 root         (0) root         (0)     1209 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8179.bd308864.js
--rw-r--r--   0 root         (0) root         (0)     3576 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8179.bd308864.js.map
--rw-r--r--   0 root         (0) root         (0)     2365 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8391.40c294c5.js
--rw-r--r--   0 root         (0) root         (0)     9602 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8391.40c294c5.js.map
--rw-r--r--   0 root         (0) root         (0)    10871 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8498.f8eb1c87.js
--rw-r--r--   0 root         (0) root         (0)    24374 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8498.f8eb1c87.js.map
--rw-r--r--   0 root         (0) root         (0)     1974 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8621.a437ee11.js
--rw-r--r--   0 root         (0) root         (0)     8339 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8621.a437ee11.js.map
--rw-r--r--   0 root         (0) root         (0)      845 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8769.ad2a69a1.js
--rw-r--r--   0 root         (0) root         (0)     2196 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8769.ad2a69a1.js.map
--rw-r--r--   0 root         (0) root         (0)      432 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8784.9c4e51b9.js
--rw-r--r--   0 root         (0) root         (0)     1085 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8784.9c4e51b9.js.map
--rw-r--r--   0 root         (0) root         (0)     5921 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8825.25b100b4.js
--rw-r--r--   0 root         (0) root         (0)    12073 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8825.25b100b4.js.map
--rw-r--r--   0 root         (0) root         (0)     1749 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/886.9ff7c1ce.js
--rw-r--r--   0 root         (0) root         (0)     5730 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/886.9ff7c1ce.js.map
--rw-r--r--   0 root         (0) root         (0)     9419 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8895.a4a700ec.js
--rw-r--r--   0 root         (0) root         (0)    21271 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8895.a4a700ec.js.map
--rw-r--r--   0 root         (0) root         (0)     8768 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8930.be445a5e.js
--rw-r--r--   0 root         (0) root         (0)    19222 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8930.be445a5e.js.map
--rw-r--r--   0 root         (0) root         (0)     1382 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9091.4b4643b0.js
--rw-r--r--   0 root         (0) root         (0)     2078 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9091.4b4643b0.js.map
--rw-r--r--   0 root         (0) root         (0)    11781 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9211.d1e09f60.js
--rw-r--r--   0 root         (0) root         (0)    42175 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9211.d1e09f60.js.map
--rw-r--r--   0 root         (0) root         (0)     9427 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9334.455b4593.js
--rw-r--r--   0 root         (0) root         (0)    21287 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9334.455b4593.js.map
--rw-r--r--   0 root         (0) root         (0)    49081 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9381.dc2f4776.js
--rw-r--r--   0 root         (0) root         (0)   160106 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9381.dc2f4776.js.map
--rw-r--r--   0 root         (0) root         (0)     4116 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9461.1fd0b115.js
--rw-r--r--   0 root         (0) root         (0)    13714 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9461.1fd0b115.js.map
--rw-r--r--   0 root         (0) root         (0)    30136 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9751.5b8fcd4c.js
--rw-r--r--   0 root         (0) root         (0)    94584 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9751.5b8fcd4c.js.map
--rw-r--r--   0 root         (0) root         (0)    10765 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/980.e9d022c5.js
--rw-r--r--   0 root         (0) root         (0)    38863 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/980.e9d022c5.js.map
--rw-r--r--   0 root         (0) root         (0)     2490 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/984.bedc7c00.js
--rw-r--r--   0 root         (0) root         (0)     9879 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/984.bedc7c00.js.map
--rw-r--r--   0 root         (0) root         (0)     5531 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9962.d22f669b.js
--rw-r--r--   0 root         (0) root         (0)    15548 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9962.d22f669b.js.map
--rw-r--r--   0 root         (0) root         (0)    88297 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/app.62f4493a.js
--rw-r--r--   0 root         (0) root         (0)   265688 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/app.62f4493a.js.map
--rw-r--r--   0 root         (0) root         (0)  1089172 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/chunk-vendors.c084e94c.js
--rw-r--r--   0 root         (0) root         (0)  2999782 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/chunk-vendors.c084e94c.js.map
--rw-r--r--   0 root         (0) root         (0)    14450 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/workbox-5b385ed2.js
--rw-r--r--   0 root         (0) root         (0)   137845 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/http/webapp/dist/workbox-5b385ed2.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.351315 platypush-1.0.3/platypush/backend/nodered/
--rw-r--r--   0 root         (0) root         (0)     1611 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/nodered/__init__.py
--rw-r--r--   0 root         (0) root         (0)      174 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/nodered/manifest.json
--rw-r--r--   0 root         (0) root         (0)      865 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/nodered/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.354648 platypush-1.0.3/platypush/backend/redis/
--rw-r--r--   0 root         (0) root         (0)     3116 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)      145 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/redis/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.354648 platypush-1.0.3/platypush/backend/tcp/
--rw-r--r--   0 root         (0) root         (0)     4732 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/tcp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      143 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/backend/tcp/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.354648 platypush-1.0.3/platypush/builder/
--rw-r--r--   0 root         (0) root         (0)       58 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/builder/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6017 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/builder/_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.354648 platypush-1.0.3/platypush/bus/
--rw-r--r--   0 root         (0) root         (0)     4685 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/bus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1763 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/bus/redis.py
--rw-r--r--   0 root         (0) root         (0)     4962 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.354648 platypush-1.0.3/platypush/commands/
--rw-r--r--   0 root         (0) root         (0)      186 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2142 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/commands/_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.354648 platypush-1.0.3/platypush/commands/_commands/
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/commands/_commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      437 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/commands/_commands/_app_ctrl.py
--rw-r--r--   0 root         (0) root         (0)     1971 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/commands/_reader.py
--rw-r--r--   0 root         (0) root         (0)     4933 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/commands/_stream.py
--rw-r--r--   0 root         (0) root         (0)      578 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/commands/_writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.354648 platypush-1.0.3/platypush/common/
--rw-r--r--   0 root         (0) root         (0)     1912 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)      991 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/_types.py
--rw-r--r--   0 root         (0) root         (0)      102 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/cmd_stream.py
--rw-r--r--   0 root         (0) root         (0)     1119 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/db.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.357982 platypush-1.0.3/platypush/common/gstreamer/
--rw-r--r--   0 root         (0) root         (0)     5729 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/gstreamer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.357982 platypush-1.0.3/platypush/common/reflection/
--rw-r--r--   0 root         (0) root         (0)       91 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/reflection/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.357982 platypush-1.0.3/platypush/common/reflection/_model/
--rw-r--r--   0 root         (0) root         (0)      312 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/reflection/_model/__init__.py
--rw-r--r--   0 root         (0) root         (0)      125 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/reflection/_model/action.py
--rw-r--r--   0 root         (0) root         (0)      630 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/reflection/_model/argument.py
--rw-r--r--   0 root         (0) root         (0)     2123 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/reflection/_model/component.py
--rw-r--r--   0 root         (0) root         (0)       55 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/reflection/_model/constants.py
--rw-r--r--   0 root         (0) root         (0)      596 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/reflection/_model/constructor.py
--rw-r--r--   0 root         (0) root         (0)    10771 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/reflection/_model/integration.py
--rw-r--r--   0 root         (0) root         (0)     3240 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/reflection/_model/message.py
--rw-r--r--   0 root         (0) root         (0)      437 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/reflection/_model/returns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.357982 platypush-1.0.3/platypush/common/reflection/_parser/
--rw-r--r--   0 root         (0) root         (0)       78 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/reflection/_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2744 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/reflection/_parser/context.py
--rw-r--r--   0 root         (0) root         (0)     5708 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/reflection/_parser/docstring.py
--rw-r--r--   0 root         (0) root         (0)     6897 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/reflection/_parser/rst.py
--rw-r--r--   0 root         (0) root         (0)      142 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/reflection/_parser/state.py
--rw-r--r--   0 root         (0) root         (0)      309 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/reflection/_serialize.py
--rw-r--r--   0 root         (0) root         (0)      278 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/reflection/_utils.py
--rw-r--r--   0 root         (0) root         (0)      314 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/sensors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.357982 platypush-1.0.3/platypush/common/spotify/
--rw-r--r--   0 root         (0) root         (0)    14862 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/common/spotify/__init__.py
--rw-r--r--   0 root         (0) root         (0)   284994 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/components.json.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.361315 platypush-1.0.3/platypush/config/
--rw-r--r--   0 root         (0) root         (0)    22023 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43853 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/config/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.361315 platypush-1.0.3/platypush/config/systemd/
--rw-r--r--   0 root         (0) root         (0)       85 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/config/systemd/platypush-sysusers.conf
--rw-r--r--   0 root         (0) root         (0)       92 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/config/systemd/platypush-tmpfile.conf
--rw-r--r--   0 root         (0) root         (0)     1075 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/config/systemd/platypush.service
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.361315 platypush-1.0.3/platypush/context/
--rw-r--r--   0 root         (0) root         (0)     6724 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/context/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.361315 platypush-1.0.3/platypush/cron/
--rw-r--r--   0 root         (0) root         (0)      426 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/cron/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7745 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/cron/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.364649 platypush-1.0.3/platypush/entities/
--rw-r--r--   0 root         (0) root         (0)     2402 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11185 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.364649 platypush-1.0.3/platypush/entities/_engine/
--rw-r--r--   0 root         (0) root         (0)     5053 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/_engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1503 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/_engine/queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.367982 platypush-1.0.3/platypush/entities/_engine/repo/
--rw-r--r--   0 root         (0) root         (0)     3326 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/_engine/repo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6369 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/_engine/repo/db.py
--rw-r--r--   0 root         (0) root         (0)      602 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/_engine/repo/helpers.py
--rw-r--r--   0 root         (0) root         (0)     7489 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/_engine/repo/merger.py
--rw-r--r--   0 root         (0) root         (0)      642 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/acceleration.py
--rw-r--r--   0 root         (0) root         (0)     1270 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/alarm.py
--rw-r--r--   0 root         (0) root         (0)      787 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/assistants.py
--rw-r--r--   0 root         (0) root         (0)      840 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/audio.py
--rw-r--r--   0 root         (0) root         (0)      687 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/batteries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.367982 platypush-1.0.3/platypush/entities/bluetooth/
--rw-r--r--   0 root         (0) root         (0)      138 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/bluetooth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5143 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/bluetooth/_device.py
--rw-r--r--   0 root         (0) root         (0)     3908 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/bluetooth/_service.py
--rw-r--r--   0 root         (0) root         (0)      552 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/buttons.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/cloud.py
--rw-r--r--   0 root         (0) root         (0)      581 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/contact.py
--rw-r--r--   0 root         (0) root         (0)      596 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/devices.py
--rw-r--r--   0 root         (0) root         (0)      803 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/dimmers.py
--rw-r--r--   0 root         (0) root         (0)      585 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/distance.py
--rw-r--r--   0 root         (0) root         (0)     1650 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/electricity.py
--rw-r--r--   0 root         (0) root         (0)      593 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/heart.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/humidity.py
--rw-r--r--   0 root         (0) root         (0)      525 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/illuminance.py
--rw-r--r--   0 root         (0) root         (0)     1159 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/lights.py
--rw-r--r--   0 root         (0) root         (0)      701 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/linkquality.py
--rw-r--r--   0 root         (0) root         (0)      630 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/magnetism.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.367982 platypush-1.0.3/platypush/entities/managers/
--rw-r--r--   0 root         (0) root         (0)     6210 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/managers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2027 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/managers/assistants.py
--rw-r--r--   0 root         (0) root         (0)      988 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/managers/cloud.py
--rw-r--r--   0 root         (0) root         (0)      571 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/managers/lights.py
--rw-r--r--   0 root         (0) root         (0)      176 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/managers/sensors.py
--rw-r--r--   0 root         (0) root         (0)     1592 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/managers/switches.py
--rw-r--r--   0 root         (0) root         (0)     1451 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/managers/weather.py
--rw-r--r--   0 root         (0) root         (0)      507 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/motion.py
--rw-r--r--   0 root         (0) root         (0)      704 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/ping.py
--rw-r--r--   0 root         (0) root         (0)      585 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/presence.py
--rw-r--r--   0 root         (0) root         (0)      582 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/pressure.py
--rw-r--r--   0 root         (0) root         (0)     6114 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/sensors.py
--rw-r--r--   0 root         (0) root         (0)      590 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/steps.py
--rw-r--r--   0 root         (0) root         (0)      944 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/switches.py
--rw-r--r--   0 root         (0) root         (0)     7027 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/system.py
--rw-r--r--   0 root         (0) root         (0)      525 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/temperature.py
--rw-r--r--   0 root         (0) root         (0)     1657 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/three_axis.py
--rw-r--r--   0 root         (0) root         (0)      584 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/time.py
--rw-r--r--   0 root         (0) root         (0)      620 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/variables.py
--rw-r--r--   0 root         (0) root         (0)     1392 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/weather.py
--rw-r--r--   0 root         (0) root         (0)      574 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/entities/weight.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.367982 platypush-1.0.3/platypush/event/
--rw-r--r--   0 root         (0) root         (0)     1976 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/event/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7090 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/event/hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.367982 platypush-1.0.3/platypush/event/processor/
--rw-r--r--   0 root         (0) root         (0)     2498 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/event/processor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.374649 platypush-1.0.3/platypush/events/
--rw-r--r--   0 root         (0) root         (0)    11119 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)      760 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/adafruit.py
--rw-r--r--   0 root         (0) root         (0)      961 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/alarm.py
--rw-r--r--   0 root         (0) root         (0)      300 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/application.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.377982 platypush-1.0.3/platypush/events/assistant/
--rw-r--r--   0 root         (0) root         (0)     9984 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/assistant/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.377982 platypush-1.0.3/platypush/events/bluetooth/
--rw-r--r--   0 root         (0) root         (0)     4397 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/bluetooth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1546 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/camera.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.377982 platypush-1.0.3/platypush/events/chat/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/chat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2215 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/chat/slack.py
--rw-r--r--   0 root         (0) root         (0)      200 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/clipboard.py
--rw-r--r--   0 root         (0) root         (0)      686 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/custom.py
--rw-r--r--   0 root         (0) root         (0)      859 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/dbus.py
--rw-r--r--   0 root         (0) root         (0)      503 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/distance.py
--rw-r--r--   0 root         (0) root         (0)      664 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/entities.py
--rw-r--r--   0 root         (0) root         (0)      725 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/file.py
--rw-r--r--   0 root         (0) root         (0)     1595 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/flic.py
--rw-r--r--   0 root         (0) root         (0)      322 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/foursquare.py
--rw-r--r--   0 root         (0) root         (0)      573 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/geo.py
--rw-r--r--   0 root         (0) root         (0)     4157 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/github.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.377982 platypush-1.0.3/platypush/events/google/
--rw-r--r--   0 root         (0) root         (0)      696 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/google/__init__.py
--rw-r--r--   0 root         (0) root         (0)      340 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/google/pubsub.py
--rw-r--r--   0 root         (0) root         (0)     1198 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/gotify.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.377982 platypush-1.0.3/platypush/events/gpio/
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/gpio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2184 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/gps.py
--rw-r--r--   0 root         (0) root         (0)     1223 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/hid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.377982 platypush-1.0.3/platypush/events/http/
--rw-r--r--   0 root         (0) root         (0)      509 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2521 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/http/hook.py
--rw-r--r--   0 root         (0) root         (0)     1149 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/http/rss.py
--rw-r--r--   0 root         (0) root         (0)     2553 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/inotify.py
--rw-r--r--   0 root         (0) root         (0)     5407 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/irc.py
--rw-r--r--   0 root         (0) root         (0)      982 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/joystick.py
--rw-r--r--   0 root         (0) root         (0)      897 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/kafka.py
--rw-r--r--   0 root         (0) root         (0)     2729 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/light.py
--rw-r--r--   0 root         (0) root         (0)      928 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/linode.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.377982 platypush-1.0.3/platypush/events/log/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)      825 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/log/http.py
--rw-r--r--   0 root         (0) root         (0)      796 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/mail.py
--rw-r--r--   0 root         (0) root         (0)     7060 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/matrix.py
--rw-r--r--   0 root         (0) root         (0)     3358 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/media.py
--rw-r--r--   0 root         (0) root         (0)     1392 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/midi.py
--rw-r--r--   0 root         (0) root         (0)      403 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/mqtt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.377982 platypush-1.0.3/platypush/events/music/
--rw-r--r--   0 root         (0) root         (0)     3759 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/music/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2654 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/music/snapcast.py
--rw-r--r--   0 root         (0) root         (0)      347 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/music/tidal.py
--rw-r--r--   0 root         (0) root         (0)     3672 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/nextcloud.py
--rw-r--r--   0 root         (0) root         (0)     2222 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/nfc.py
--rw-r--r--   0 root         (0) root         (0)     1128 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/ngrok.py
--rw-r--r--   0 root         (0) root         (0)     2862 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/ntfy.py
--rw-r--r--   0 root         (0) root         (0)     1479 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/ping.py
--rw-r--r--   0 root         (0) root         (0)     5060 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/pushbullet.py
--rw-r--r--   0 root         (0) root         (0)      471 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/qrcode.py
--rw-r--r--   0 root         (0) root         (0)      992 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/rss.py
--rw-r--r--   0 root         (0) root         (0)      934 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/scard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.377982 platypush-1.0.3/platypush/events/sensor/
--rw-r--r--   0 root         (0) root         (0)      961 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/sensor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.377982 platypush-1.0.3/platypush/events/sensor/ir/
--rw-r--r--   0 root         (0) root         (0)      862 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/sensor/ir/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1261 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/sensor/leap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.377982 platypush-1.0.3/platypush/events/sensor/light/
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/sensor/light/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.377982 platypush-1.0.3/platypush/events/serial/
--rw-r--r--   0 root         (0) root         (0)      495 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/serial/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1649 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/sound.py
--rw-r--r--   0 root         (0) root         (0)     1347 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/stt.py
--rw-r--r--   0 root         (0) root         (0)      894 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/sun.py
--rw-r--r--   0 root         (0) root         (0)     2210 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/telegram.py
--rw-r--r--   0 root         (0) root         (0)     1946 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/tensorflow.py
--rw-r--r--   0 root         (0) root         (0)     2572 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/torrent.py
--rw-r--r--   0 root         (0) root         (0)     1981 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/trello.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.377982 platypush-1.0.3/platypush/events/video/
--rw-r--r--   0 root         (0) root         (0)     1253 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/video/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4113 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/weather.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.377982 platypush-1.0.3/platypush/events/web/
--rw-r--r--   0 root         (0) root         (0)      875 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/web/__init__.py
--rw-r--r--   0 root         (0) root         (0)      391 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/web/widget.py
--rw-r--r--   0 root         (0) root         (0)      436 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/websocket.py
--rw-r--r--   0 root         (0) root         (0)     9969 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/xmpp.py
--rw-r--r--   0 root         (0) root         (0)      413 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/zeroborg.py
--rw-r--r--   0 root         (0) root         (0)     1485 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/zeroconf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.381316 platypush-1.0.3/platypush/events/zigbee/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/zigbee/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5542 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/zigbee/mqtt.py
--rw-r--r--   0 root         (0) root         (0)     5480 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/events/zwave.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.381316 platypush-1.0.3/platypush/exceptions/
--rw-r--r--   0 root         (0) root         (0)      542 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1281 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/exceptions/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.171309 platypush-1.0.3/platypush/install/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.381316 platypush-1.0.3/platypush/install/docker/
--rw-r--r--   0 root         (0) root         (0)     1127 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/install/docker/alpine.Dockerfile
--rw-r--r--   0 root         (0) root         (0)     1263 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/install/docker/debian.Dockerfile
--rw-r--r--   0 root         (0) root         (0)     1260 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/install/docker/fedora.Dockerfile
--rw-r--r--   0 root         (0) root         (0)     1263 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/install/docker/ubuntu.Dockerfile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.381316 platypush-1.0.3/platypush/install/requirements/
--rw-r--r--   0 root         (0) root         (0)      277 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/install/requirements/alpine.txt
--rw-r--r--   0 root         (0) root         (0)      337 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/install/requirements/arch.txt
--rw-r--r--   0 root         (0) root         (0)      391 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/install/requirements/debian.txt
--rw-r--r--   0 root         (0) root         (0)      376 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/install/requirements/fedora.txt
--rw-r--r--   0 root         (0) root         (0)      391 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/install/requirements/ubuntu.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.381316 platypush-1.0.3/platypush/install/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.381316 platypush-1.0.3/platypush/install/scripts/alpine/
--rw-r--r--   0 root         (0) root         (0)       45 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/install/scripts/alpine/PKGCMD
--rwxr-xr-x   0 root         (0) root         (0)      945 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/install/scripts/alpine/install.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.381316 platypush-1.0.3/platypush/install/scripts/arch/
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/install/scripts/arch/PKGCMD
--rwxr-xr-x   0 root         (0) root         (0)      945 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/install/scripts/arch/install.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.381316 platypush-1.0.3/platypush/install/scripts/debian/
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/install/scripts/debian/PKGCMD
--rwxr-xr-x   0 root         (0) root         (0)      945 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/install/scripts/debian/install.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.381316 platypush-1.0.3/platypush/install/scripts/fedora/
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/install/scripts/fedora/PKGCMD
--rwxr-xr-x   0 root         (0) root         (0)      945 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/install/scripts/fedora/install.sh
--rwxr-xr-x   0 root         (0) root         (0)      945 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/install/scripts/install.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.381316 platypush-1.0.3/platypush/install/scripts/ubuntu/
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/install/scripts/ubuntu/PKGCMD
--rwxr-xr-x   0 root         (0) root         (0)      945 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/install/scripts/ubuntu/install.sh
--rw-r--r--   0 root         (0) root         (0)      574 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.384649 platypush-1.0.3/platypush/message/
--rw-r--r--   0 root         (0) root         (0)     6007 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.391316 platypush-1.0.3/platypush/message/event/
--rw-r--r--   0 root         (0) root         (0)    11119 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/__init__.py
--rw-r--r--   0 root         (0) root         (0)      760 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/adafruit.py
--rw-r--r--   0 root         (0) root         (0)      961 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/alarm.py
--rw-r--r--   0 root         (0) root         (0)      300 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/application.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.391316 platypush-1.0.3/platypush/message/event/assistant/
--rw-r--r--   0 root         (0) root         (0)     9984 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/assistant/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.391316 platypush-1.0.3/platypush/message/event/bluetooth/
--rw-r--r--   0 root         (0) root         (0)     4397 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/bluetooth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1546 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/camera.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.391316 platypush-1.0.3/platypush/message/event/chat/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/chat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2215 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/chat/slack.py
--rw-r--r--   0 root         (0) root         (0)      200 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/clipboard.py
--rw-r--r--   0 root         (0) root         (0)      686 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/custom.py
--rw-r--r--   0 root         (0) root         (0)      859 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/dbus.py
--rw-r--r--   0 root         (0) root         (0)      503 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/distance.py
--rw-r--r--   0 root         (0) root         (0)      664 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/entities.py
--rw-r--r--   0 root         (0) root         (0)      725 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/file.py
--rw-r--r--   0 root         (0) root         (0)     1595 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/flic.py
--rw-r--r--   0 root         (0) root         (0)      322 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/foursquare.py
--rw-r--r--   0 root         (0) root         (0)      573 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/geo.py
--rw-r--r--   0 root         (0) root         (0)     4157 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/github.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.391316 platypush-1.0.3/platypush/message/event/google/
--rw-r--r--   0 root         (0) root         (0)      696 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/google/__init__.py
--rw-r--r--   0 root         (0) root         (0)      340 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/google/pubsub.py
--rw-r--r--   0 root         (0) root         (0)     1198 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/gotify.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.391316 platypush-1.0.3/platypush/message/event/gpio/
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/gpio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2184 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/gps.py
--rw-r--r--   0 root         (0) root         (0)     1223 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/hid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.391316 platypush-1.0.3/platypush/message/event/http/
--rw-r--r--   0 root         (0) root         (0)      509 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2521 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/http/hook.py
--rw-r--r--   0 root         (0) root         (0)     1149 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/http/rss.py
--rw-r--r--   0 root         (0) root         (0)     2553 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/inotify.py
--rw-r--r--   0 root         (0) root         (0)     5407 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/irc.py
--rw-r--r--   0 root         (0) root         (0)      982 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/joystick.py
--rw-r--r--   0 root         (0) root         (0)      897 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/kafka.py
--rw-r--r--   0 root         (0) root         (0)     2729 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/light.py
--rw-r--r--   0 root         (0) root         (0)      928 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/linode.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.391316 platypush-1.0.3/platypush/message/event/log/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)      825 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/log/http.py
--rw-r--r--   0 root         (0) root         (0)      796 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/mail.py
--rw-r--r--   0 root         (0) root         (0)     7060 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/matrix.py
--rw-r--r--   0 root         (0) root         (0)     3358 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/media.py
--rw-r--r--   0 root         (0) root         (0)     1392 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/midi.py
--rw-r--r--   0 root         (0) root         (0)      403 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/mqtt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.391316 platypush-1.0.3/platypush/message/event/music/
--rw-r--r--   0 root         (0) root         (0)     3759 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/music/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2654 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/music/snapcast.py
--rw-r--r--   0 root         (0) root         (0)      347 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/music/tidal.py
--rw-r--r--   0 root         (0) root         (0)     3672 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/nextcloud.py
--rw-r--r--   0 root         (0) root         (0)     2222 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/nfc.py
--rw-r--r--   0 root         (0) root         (0)     1128 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/ngrok.py
--rw-r--r--   0 root         (0) root         (0)     2862 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/ntfy.py
--rw-r--r--   0 root         (0) root         (0)     1479 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/ping.py
--rw-r--r--   0 root         (0) root         (0)     5060 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/pushbullet.py
--rw-r--r--   0 root         (0) root         (0)      471 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/qrcode.py
--rw-r--r--   0 root         (0) root         (0)      992 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/rss.py
--rw-r--r--   0 root         (0) root         (0)      934 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/scard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.391316 platypush-1.0.3/platypush/message/event/sensor/
--rw-r--r--   0 root         (0) root         (0)      961 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/sensor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.394650 platypush-1.0.3/platypush/message/event/sensor/ir/
--rw-r--r--   0 root         (0) root         (0)      862 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/sensor/ir/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1261 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/sensor/leap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.394650 platypush-1.0.3/platypush/message/event/sensor/light/
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/sensor/light/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.394650 platypush-1.0.3/platypush/message/event/serial/
--rw-r--r--   0 root         (0) root         (0)      495 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/serial/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1649 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/sound.py
--rw-r--r--   0 root         (0) root         (0)     1347 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/stt.py
--rw-r--r--   0 root         (0) root         (0)      894 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/sun.py
--rw-r--r--   0 root         (0) root         (0)     2210 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/telegram.py
--rw-r--r--   0 root         (0) root         (0)     1946 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/tensorflow.py
--rw-r--r--   0 root         (0) root         (0)     2572 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/torrent.py
--rw-r--r--   0 root         (0) root         (0)     1981 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/trello.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.394650 platypush-1.0.3/platypush/message/event/video/
--rw-r--r--   0 root         (0) root         (0)     1253 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/video/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4113 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/weather.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.394650 platypush-1.0.3/platypush/message/event/web/
--rw-r--r--   0 root         (0) root         (0)      875 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/web/__init__.py
--rw-r--r--   0 root         (0) root         (0)      391 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/web/widget.py
--rw-r--r--   0 root         (0) root         (0)      436 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/websocket.py
--rw-r--r--   0 root         (0) root         (0)     9969 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/xmpp.py
--rw-r--r--   0 root         (0) root         (0)      413 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/zeroborg.py
--rw-r--r--   0 root         (0) root         (0)     1485 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/zeroconf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.394650 platypush-1.0.3/platypush/message/event/zigbee/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/zigbee/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5542 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/zigbee/mqtt.py
--rw-r--r--   0 root         (0) root         (0)     5480 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/event/zwave.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.394650 platypush-1.0.3/platypush/message/request/
--rw-r--r--   0 root         (0) root         (0)    11283 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.394650 platypush-1.0.3/platypush/message/response/
--rw-r--r--   0 root         (0) root         (0)     2964 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/message/response/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.394650 platypush-1.0.3/platypush/migrations/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.394650 platypush-1.0.3/platypush/migrations/alembic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.394650 platypush-1.0.3/platypush/migrations/alembic/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     3540 2024-05-31 01:03:46.000000 platypush-1.0.3/platypush/migrations/alembic/__pycache__/env.cpython-312.pyc
--rw-r--r--   0 root         (0) root         (0)     2747 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/migrations/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      510 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/migrations/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.394650 platypush-1.0.3/platypush/migrations/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     1343 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/migrations/alembic/versions/0876439530cb_added_password_hashing_parameters_to_.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.394650 platypush-1.0.3/platypush/migrations/alembic/versions/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     2247 2024-05-31 01:03:46.000000 platypush-1.0.3/platypush/migrations/alembic/versions/__pycache__/0876439530cb_added_password_hashing_parameters_to_.cpython-312.pyc
--rw-r--r--   0 root         (0) root         (0)     5485 2024-05-31 01:03:46.000000 platypush-1.0.3/platypush/migrations/alembic/versions/__pycache__/c39ac404119b_migrate_variable_table.cpython-312.pyc
--rw-r--r--   0 root         (0) root         (0)      619 2024-05-31 01:03:46.000000 platypush-1.0.3/platypush/migrations/alembic/versions/__pycache__/d030953a871d_base_alembic_version.cpython-312.pyc
--rw-r--r--   0 root         (0) root         (0)     4308 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/migrations/alembic/versions/c39ac404119b_migrate_variable_table.py
--rw-r--r--   0 root         (0) root         (0)      304 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/migrations/alembic/versions/d030953a871d_base_alembic_version.py
--rw-r--r--   0 root         (0) root         (0)     3180 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/migrations/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.394650 platypush-1.0.3/platypush/platydock/
--rwxr-xr-x   0 root         (0) root         (0)     9341 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/platydock/__init__.py
--rw-r--r--   0 root         (0) root         (0)       66 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/platydock/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.397983 platypush-1.0.3/platypush/platyvenv/
--rwxr-xr-x   0 root         (0) root         (0)     6281 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/platyvenv/__init__.py
--rw-r--r--   0 root         (0) root         (0)       66 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/platyvenv/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.397983 platypush-1.0.3/platypush/plugins/
--rw-r--r--   0 root         (0) root         (0)    10705 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.397983 platypush-1.0.3/platypush/plugins/adafruit/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/adafruit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.397983 platypush-1.0.3/platypush/plugins/adafruit/io/
--rw-r--r--   0 root         (0) root         (0)    10842 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/adafruit/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)      382 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/adafruit/io/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.397983 platypush-1.0.3/platypush/plugins/alarm/
--rw-r--r--   0 root         (0) root         (0)    21516 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/alarm/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13182 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/alarm/_model.py
--rw-r--r--   0 root         (0) root         (0)      493 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/alarm/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.397983 platypush-1.0.3/platypush/plugins/application/
--rw-r--r--   0 root         (0) root         (0)     2929 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/application/__init__.py
--rw-r--r--   0 root         (0) root         (0)      150 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/application/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.397983 platypush-1.0.3/platypush/plugins/arduino/
--rw-r--r--   0 root         (0) root         (0)    17864 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/arduino/__init__.py
--rw-r--r--   0 root         (0) root         (0)      398 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/arduino/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.397983 platypush-1.0.3/platypush/plugins/assistant/
--rw-r--r--   0 root         (0) root         (0)    11081 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/assistant/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.397983 platypush-1.0.3/platypush/plugins/assistant/google/
--rw-r--r--   0 root         (0) root         (0)    11883 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/assistant/google/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2209 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/assistant/google/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.397983 platypush-1.0.3/platypush/plugins/assistant/picovoice/
--rw-r--r--   0 root         (0) root         (0)    30836 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/assistant/picovoice/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14075 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/assistant/picovoice/_assistant.py
--rw-r--r--   0 root         (0) root         (0)     1196 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/assistant/picovoice/_context.py
--rw-r--r--   0 root         (0) root         (0)      175 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/assistant/picovoice/_intent.py
--rw-r--r--   0 root         (0) root         (0)     5022 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/assistant/picovoice/_recorder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.401317 platypush-1.0.3/platypush/plugins/assistant/picovoice/_speech/
--rw-r--r--   0 root         (0) root         (0)       71 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/assistant/picovoice/_speech/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5147 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/assistant/picovoice/_speech/_base.py
--rw-r--r--   0 root         (0) root         (0)     2647 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/assistant/picovoice/_speech/_intent.py
--rw-r--r--   0 root         (0) root         (0)     6431 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/assistant/picovoice/_speech/_processor.py
--rw-r--r--   0 root         (0) root         (0)     3485 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/assistant/picovoice/_speech/_stt.py
--rw-r--r--   0 root         (0) root         (0)      233 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/assistant/picovoice/_state.py
--rw-r--r--   0 root         (0) root         (0)     1195 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/assistant/picovoice/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.401317 platypush-1.0.3/platypush/plugins/autoremote/
--rw-r--r--   0 root         (0) root         (0)     8111 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/autoremote/__init__.py
--rw-r--r--   0 root         (0) root         (0)      149 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/autoremote/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.401317 platypush-1.0.3/platypush/plugins/bluetooth/
--rw-r--r--   0 root         (0) root         (0)    23785 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.401317 platypush-1.0.3/platypush/plugins/bluetooth/_ble/
--rw-r--r--   0 root         (0) root         (0)       80 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_ble/__init__.py
--rw-r--r--   0 root         (0) root         (0)      815 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_ble/_cache.py
--rw-r--r--   0 root         (0) root         (0)      477 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_ble/_connection.py
--rw-r--r--   0 root         (0) root         (0)     7961 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_ble/_event_handler.py
--rw-r--r--   0 root         (0) root         (0)    14830 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_ble/_manager.py
--rw-r--r--   0 root         (0) root         (0)    11919 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_ble/_mappers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.401317 platypush-1.0.3/platypush/plugins/bluetooth/_ble/_plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_ble/_plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1847 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_ble/_plugins/switchbot.py
--rw-r--r--   0 root         (0) root         (0)     6367 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_cache.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.404650 platypush-1.0.3/platypush/plugins/bluetooth/_file/
--rw-r--r--   0 root         (0) root         (0)       58 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_file/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3025 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_file/sender.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.404650 platypush-1.0.3/platypush/plugins/bluetooth/_legacy/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_legacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.404650 platypush-1.0.3/platypush/plugins/bluetooth/_legacy/_manager/
--rw-r--r--   0 root         (0) root         (0)       62 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_legacy/_manager/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12004 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_legacy/_manager/_base.py
--rw-r--r--   0 root         (0) root         (0)     1882 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_legacy/_manager/_connection.py
--rw-r--r--   0 root         (0) root         (0)     2253 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_legacy/_manager/_service.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_legacy/_manager/_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.404650 platypush-1.0.3/platypush/plugins/bluetooth/_legacy/_model/
--rw-r--r--   0 root         (0) root         (0)      170 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_legacy/_model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2475 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_legacy/_model/_device.py
--rw-r--r--   0 root         (0) root         (0)     1664 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_legacy/_model/_services.py
--rw-r--r--   0 root         (0) root         (0)     6000 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.404650 platypush-1.0.3/platypush/plugins/bluetooth/_model/
--rw-r--r--   0 root         (0) root         (0)      267 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.404650 platypush-1.0.3/platypush/plugins/bluetooth/_model/_classes/
--rw-r--r--   0 root         (0) root         (0)      185 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_model/_classes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1742 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_model/_classes/_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.404650 platypush-1.0.3/platypush/plugins/bluetooth/_model/_classes/_device/
--rw-r--r--   0 root         (0) root         (0)      138 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_model/_classes/_device/__init__.py
--rw-r--r--   0 root         (0) root         (0)      907 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_model/_classes/_device/_major.py
--rw-r--r--   0 root         (0) root         (0)     9793 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_model/_classes/_device/_minor.py
--rw-r--r--   0 root         (0) root         (0)      833 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_model/_classes/_service.py
--rw-r--r--   0 root         (0) root         (0)      884 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_model/_protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.404650 platypush-1.0.3/platypush/plugins/bluetooth/_model/_service/
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_model/_service/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6234 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_model/_service/_directory.py
--rw-r--r--   0 root         (0) root         (0)     1068 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_model/_service/_directory.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.407984 platypush-1.0.3/platypush/plugins/bluetooth/_plugins/
--rw-r--r--   0 root         (0) root         (0)      125 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_plugins/_base.py
--rw-r--r--   0 root         (0) root         (0)     1278 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_plugins/_scanner.py
--rw-r--r--   0 root         (0) root         (0)     1337 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/_types.py
--rw-r--r--   0 root         (0) root         (0)     1576 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/manifest.json
--rw-r--r--   0 root         (0) root         (0)      306 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/bluetooth/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.407984 platypush-1.0.3/platypush/plugins/calendar/
--rw-r--r--   0 root         (0) root         (0)     4150 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/calendar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.407984 platypush-1.0.3/platypush/plugins/calendar/ical/
--rw-r--r--   0 root         (0) root         (0)     3807 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/calendar/ical/__init__.py
--rw-r--r--   0 root         (0) root         (0)      384 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/calendar/ical/manifest.json
--rw-r--r--   0 root         (0) root         (0)      147 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/calendar/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.407984 platypush-1.0.3/platypush/plugins/camera/
--rw-r--r--   0 root         (0) root         (0)    39220 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.407984 platypush-1.0.3/platypush/plugins/camera/android/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/android/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.407984 platypush-1.0.3/platypush/plugins/camera/android/ipcam/
--rw-r--r--   0 root         (0) root         (0)    11555 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/android/ipcam/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/android/ipcam/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.407984 platypush-1.0.3/platypush/plugins/camera/cv/
--rw-r--r--   0 root         (0) root         (0)     3168 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/cv/__init__.py
--rw-r--r--   0 root         (0) root         (0)      599 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/cv/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.407984 platypush-1.0.3/platypush/plugins/camera/ffmpeg/
--rw-r--r--   0 root         (0) root         (0)     3722 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/ffmpeg/__init__.py
--rw-r--r--   0 root         (0) root         (0)      552 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/ffmpeg/manifest.json
--rw-r--r--   0 root         (0) root         (0)      472 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/ffmpeg/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.407984 platypush-1.0.3/platypush/plugins/camera/gstreamer/
--rw-r--r--   0 root         (0) root         (0)     2627 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/gstreamer/__init__.py
--rw-r--r--   0 root         (0) root         (0)      699 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/gstreamer/manifest.json
--rw-r--r--   0 root         (0) root         (0)      201 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/gstreamer/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.407984 platypush-1.0.3/platypush/plugins/camera/ir/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/ir/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.407984 platypush-1.0.3/platypush/plugins/camera/ir/mlx90640/
--rw-r--r--   0 root         (0) root         (0)     4028 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/ir/mlx90640/__init__.py
--rw-r--r--   0 root         (0) root         (0)      574 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/ir/mlx90640/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.407984 platypush-1.0.3/platypush/plugins/camera/model/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3078 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/model/camera.py
--rw-r--r--   0 root         (0) root         (0)      256 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/model/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.411317 platypush-1.0.3/platypush/plugins/camera/model/writer/
--rw-r--r--   0 root         (0) root         (0)     3919 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/model/writer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1233 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/model/writer/cv.py
--rw-r--r--   0 root         (0) root         (0)     6138 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/model/writer/ffmpeg.py
--rw-r--r--   0 root         (0) root         (0)     1744 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/model/writer/image.py
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/model/writer/index.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.411317 platypush-1.0.3/platypush/plugins/camera/model/writer/preview/
--rw-r--r--   0 root         (0) root         (0)      855 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/model/writer/preview/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1618 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/model/writer/preview/ffplay.py
--rw-r--r--   0 root         (0) root         (0)     1837 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/model/writer/preview/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.411317 platypush-1.0.3/platypush/plugins/camera/model/writer/preview/wx/
--rw-r--r--   0 root         (0) root         (0)     1405 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/model/writer/preview/wx/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1844 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/model/writer/preview/wx/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.411317 platypush-1.0.3/platypush/plugins/camera/pi/
--rw-r--r--   0 root         (0) root         (0)    10390 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/pi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.411317 platypush-1.0.3/platypush/plugins/camera/pi/legacy/
--rw-r--r--   0 root         (0) root         (0)    10679 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/pi/legacy/__init__.py
--rw-r--r--   0 root         (0) root         (0)      575 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/pi/legacy/manifest.json
--rw-r--r--   0 root         (0) root         (0)     1383 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/pi/legacy/model.py
--rw-r--r--   0 root         (0) root         (0)      569 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/pi/manifest.json
--rw-r--r--   0 root         (0) root         (0)      620 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/camera/pi/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.411317 platypush-1.0.3/platypush/plugins/chat/
--rw-r--r--   0 root         (0) root         (0)      209 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/chat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.411317 platypush-1.0.3/platypush/plugins/clipboard/
--rw-r--r--   0 root         (0) root         (0)     1644 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/clipboard/__init__.py
--rw-r--r--   0 root         (0) root         (0)      402 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/clipboard/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.411317 platypush-1.0.3/platypush/plugins/config/
--rw-r--r--   0 root         (0) root         (0)     1547 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)      145 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/config/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.414651 platypush-1.0.3/platypush/plugins/csv/
--rw-r--r--   0 root         (0) root         (0)     6529 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/csv/__init__.py
--rw-r--r--   0 root         (0) root         (0)      142 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/csv/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.414651 platypush-1.0.3/platypush/plugins/cups/
--rw-r--r--   0 root         (0) root         (0)    12657 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/cups/__init__.py
--rw-r--r--   0 root         (0) root         (0)      380 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/cups/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.414651 platypush-1.0.3/platypush/plugins/db/
--rw-r--r--   0 root         (0) root         (0)    18785 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)      141 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/db/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.414651 platypush-1.0.3/platypush/plugins/dbus/
--rw-r--r--   0 root         (0) root         (0)    16340 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/dbus/__init__.py
--rw-r--r--   0 root         (0) root         (0)      583 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/dbus/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.414651 platypush-1.0.3/platypush/plugins/dropbox/
--rw-r--r--   0 root         (0) root         (0)    14982 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/dropbox/__init__.py
--rw-r--r--   0 root         (0) root         (0)      322 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/dropbox/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.414651 platypush-1.0.3/platypush/plugins/entities/
--rw-r--r--   0 root         (0) root         (0)     9492 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/entities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      107 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/entities/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.414651 platypush-1.0.3/platypush/plugins/esp/
--rw-r--r--   0 root         (0) root         (0)    58863 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/esp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      142 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/esp/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.414651 platypush-1.0.3/platypush/plugins/esp/models/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/esp/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12447 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/esp/models/connection.py
--rw-r--r--   0 root         (0) root         (0)     1171 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/esp/models/device.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.414651 platypush-1.0.3/platypush/plugins/ffmpeg/
--rw-r--r--   0 root         (0) root         (0)     5701 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/ffmpeg/__init__.py
--rw-r--r--   0 root         (0) root         (0)      368 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/ffmpeg/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.414651 platypush-1.0.3/platypush/plugins/file/
--rw-r--r--   0 root         (0) root         (0)     5488 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/file/__init__.py
--rw-r--r--   0 root         (0) root         (0)      143 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/file/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.414651 platypush-1.0.3/platypush/plugins/file/monitor/
--rw-r--r--   0 root         (0) root         (0)     5251 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/file/monitor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.417984 platypush-1.0.3/platypush/plugins/file/monitor/entities/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/file/monitor/entities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3477 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/file/monitor/entities/handlers.py
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/file/monitor/entities/resources.py
--rw-r--r--   0 root         (0) root         (0)      562 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/file/monitor/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.417984 platypush-1.0.3/platypush/plugins/flic/
--rw-r--r--   0 root         (0) root         (0)     4892 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/flic/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32369 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/flic/fliclib.py
--rw-r--r--   0 root         (0) root         (0)      201 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/flic/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.417984 platypush-1.0.3/platypush/plugins/foursquare/
--rw-r--r--   0 root         (0) root         (0)    16769 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/foursquare/__init__.py
--rw-r--r--   0 root         (0) root         (0)      220 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/foursquare/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.417984 platypush-1.0.3/platypush/plugins/github/
--rw-r--r--   0 root         (0) root         (0)     9312 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/github/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/github/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.417984 platypush-1.0.3/platypush/plugins/google/
--rw-r--r--   0 root         (0) root         (0)     4662 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/google/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.417984 platypush-1.0.3/platypush/plugins/google/calendar/
--rw-r--r--   0 root         (0) root         (0)     3649 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/google/calendar/__init__.py
--rw-r--r--   0 root         (0) root         (0)      823 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/google/calendar/manifest.json
--rw-r--r--   0 root         (0) root         (0)     4747 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/google/credentials.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.417984 platypush-1.0.3/platypush/plugins/google/drive/
--rw-r--r--   0 root         (0) root         (0)    13292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/google/drive/__init__.py
--rw-r--r--   0 root         (0) root         (0)      820 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/google/drive/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.417984 platypush-1.0.3/platypush/plugins/google/mail/
--rw-r--r--   0 root         (0) root         (0)     5756 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/google/mail/__init__.py
--rw-r--r--   0 root         (0) root         (0)      819 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/google/mail/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.417984 platypush-1.0.3/platypush/plugins/google/maps/
--rw-r--r--   0 root         (0) root         (0)    10525 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/google/maps/__init__.py
--rw-r--r--   0 root         (0) root         (0)      819 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/google/maps/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.417984 platypush-1.0.3/platypush/plugins/google/pubsub/
--rw-r--r--   0 root         (0) root         (0)     7863 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/google/pubsub/__init__.py
--rw-r--r--   0 root         (0) root         (0)      928 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/google/pubsub/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.421317 platypush-1.0.3/platypush/plugins/google/translate/
--rw-r--r--   0 root         (0) root         (0)     4693 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/google/translate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      858 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/google/translate/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.421317 platypush-1.0.3/platypush/plugins/gotify/
--rw-r--r--   0 root         (0) root         (0)     6992 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/gotify/__init__.py
--rw-r--r--   0 root         (0) root         (0)      203 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/gotify/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.421317 platypush-1.0.3/platypush/plugins/gpio/
--rw-r--r--   0 root         (0) root         (0)     6466 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/gpio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      221 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/gpio/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.421317 platypush-1.0.3/platypush/plugins/gpio/zeroborg/
--rw-r--r--   0 root         (0) root         (0)     5368 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/gpio/zeroborg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.421317 platypush-1.0.3/platypush/plugins/gpio/zeroborg/lib/
--rw-r--r--   0 root         (0) root         (0)    31497 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/gpio/zeroborg/lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/gpio/zeroborg/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.421317 platypush-1.0.3/platypush/plugins/gps/
--rw-r--r--   0 root         (0) root         (0)     6667 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/gps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1041 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/gps/_model.py
--rw-r--r--   0 root         (0) root         (0)      611 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/gps/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.421317 platypush-1.0.3/platypush/plugins/graphite/
--rw-r--r--   0 root         (0) root         (0)     1819 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/graphite/__init__.py
--rw-r--r--   0 root         (0) root         (0)      147 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/graphite/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.421317 platypush-1.0.3/platypush/plugins/hid/
--rw-r--r--   0 root         (0) root         (0)     8254 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/hid/__init__.py
--rw-r--r--   0 root         (0) root         (0)      666 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/hid/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.421317 platypush-1.0.3/platypush/plugins/http/
--rw-r--r--   0 root         (0) root         (0)     5599 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)      143 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/http/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.421317 platypush-1.0.3/platypush/plugins/http/webpage/
--rw-r--r--   0 root         (0) root         (0)    11483 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/http/webpage/__init__.py
--rw-r--r--   0 root         (0) root         (0)      552 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/http/webpage/manifest.json
--rwxr-xr-x   0 root         (0) root         (0)     1043 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/http/webpage/mercury-parser.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.421317 platypush-1.0.3/platypush/plugins/ifttt/
--rw-r--r--   0 root         (0) root         (0)     2141 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/ifttt/__init__.py
--rw-r--r--   0 root         (0) root         (0)      144 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/ifttt/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.424651 platypush-1.0.3/platypush/plugins/inspect/
--rw-r--r--   0 root         (0) root         (0)    10852 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/inspect/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7553 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/inspect/_cache.py
--rw-r--r--   0 root         (0) root         (0)      578 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/inspect/_serialize.py
--rw-r--r--   0 root         (0) root         (0)      146 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/inspect/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.424651 platypush-1.0.3/platypush/plugins/irc/
--rw-r--r--   0 root         (0) root         (0)    13611 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/irc/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19629 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/irc/_bot.py
--rw-r--r--   0 root         (0) root         (0)     2013 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/irc/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.424651 platypush-1.0.3/platypush/plugins/joystick/
--rw-r--r--   0 root         (0) root         (0)     3720 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/joystick/__init__.py
--rw-r--r--   0 root         (0) root         (0)   119434 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/joystick/_inputs.py
--rw-r--r--   0 root         (0) root         (0)     6133 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/joystick/_manager.py
--rw-r--r--   0 root         (0) root         (0)      967 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/joystick/_state.py
--rw-r--r--   0 root         (0) root         (0)      324 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/joystick/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.424651 platypush-1.0.3/platypush/plugins/kafka/
--rw-r--r--   0 root         (0) root         (0)     8234 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/kafka/__init__.py
--rw-r--r--   0 root         (0) root         (0)      322 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/kafka/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.424651 platypush-1.0.3/platypush/plugins/lastfm/
--rw-r--r--   0 root         (0) root         (0)     6134 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/lastfm/__init__.py
--rw-r--r--   0 root         (0) root         (0)      362 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/lastfm/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.424651 platypush-1.0.3/platypush/plugins/lcd/
--rw-r--r--   0 root         (0) root         (0)     5771 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/lcd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.424651 platypush-1.0.3/platypush/plugins/lcd/gpio/
--rw-r--r--   0 root         (0) root         (0)     3666 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/lcd/gpio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      190 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/lcd/gpio/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.424651 platypush-1.0.3/platypush/plugins/lcd/i2c/
--rw-r--r--   0 root         (0) root         (0)     3492 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/lcd/i2c/__init__.py
--rw-r--r--   0 root         (0) root         (0)      189 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/lcd/i2c/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.427984 platypush-1.0.3/platypush/plugins/leap/
--rw-r--r--   0 root         (0) root         (0)     9165 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/leap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      463 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/leap/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.427984 platypush-1.0.3/platypush/plugins/light/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/light/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.427984 platypush-1.0.3/platypush/plugins/light/hue/
--rw-r--r--   0 root         (0) root         (0)    41305 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/light/hue/__init__.py
--rw-r--r--   0 root         (0) root         (0)      477 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/light/hue/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.427984 platypush-1.0.3/platypush/plugins/linode/
--rw-r--r--   0 root         (0) root         (0)     8350 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/linode/__init__.py
--rw-r--r--   0 root         (0) root         (0)      252 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/linode/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.427984 platypush-1.0.3/platypush/plugins/log/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/log/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.427984 platypush-1.0.3/platypush/plugins/log/http/
--rw-r--r--   0 root         (0) root         (0)     5589 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/log/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/log/http/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.427984 platypush-1.0.3/platypush/plugins/logger/
--rw-r--r--   0 root         (0) root         (0)     1141 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/logger/__init__.py
--rw-r--r--   0 root         (0) root         (0)      145 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/logger/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.427984 platypush-1.0.3/platypush/plugins/luma/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/luma/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.427984 platypush-1.0.3/platypush/plugins/luma/oled/
--rw-r--r--   0 root         (0) root         (0)    14122 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/luma/oled/__init__.py
--rw-r--r--   0 root         (0) root         (0)      175 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/luma/oled/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.427984 platypush-1.0.3/platypush/plugins/mail/
--rw-r--r--   0 root         (0) root         (0)    39125 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mail/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3415 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mail/_account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.427984 platypush-1.0.3/platypush/plugins/mail/_model/
--rw-r--r--   0 root         (0) root         (0)      319 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mail/_model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.431318 platypush-1.0.3/platypush/plugins/mail/_model/_config/
--rw-r--r--   0 root         (0) root         (0)      127 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mail/_model/_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1180 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mail/_model/_config/_account.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mail/_model/_config/_server.py
--rw-r--r--   0 root         (0) root         (0)     7195 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mail/_model/_mail.py
--rw-r--r--   0 root         (0) root         (0)      528 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mail/_model/_transport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.431318 platypush-1.0.3/platypush/plugins/mail/_plugin/
--rw-r--r--   0 root         (0) root         (0)      228 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mail/_plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3463 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mail/_plugin/_base.py
--rw-r--r--   0 root         (0) root         (0)     3609 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mail/_plugin/_in.py
--rw-r--r--   0 root         (0) root         (0)     4164 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mail/_plugin/_out.py
--rw-r--r--   0 root         (0) root         (0)      937 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mail/_plugin/_utils.py
--rw-r--r--   0 root         (0) root         (0)     2203 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mail/_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.431318 platypush-1.0.3/platypush/plugins/mail/imap/
--rw-r--r--   0 root         (0) root         (0)    10322 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mail/imap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      619 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mail/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.431318 platypush-1.0.3/platypush/plugins/mail/smtp/
--rw-r--r--   0 root         (0) root         (0)     2044 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mail/smtp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.431318 platypush-1.0.3/platypush/plugins/mailgun/
--rw-r--r--   0 root         (0) root         (0)     2988 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mailgun/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mailgun/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.431318 platypush-1.0.3/platypush/plugins/mastodon/
--rw-r--r--   0 root         (0) root         (0)    55621 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mastodon/__init__.py
--rw-r--r--   0 root         (0) root         (0)      107 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mastodon/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.431318 platypush-1.0.3/platypush/plugins/matrix/
--rw-r--r--   0 root         (0) root         (0)    29149 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/matrix/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30994 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/matrix/client.py
--rw-r--r--   0 root         (0) root         (0)     1670 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/matrix/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.431318 platypush-1.0.3/platypush/plugins/media/
--rw-r--r--   0 root         (0) root         (0)    25014 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.431318 platypush-1.0.3/platypush/plugins/media/chromecast/
--rw-r--r--   0 root         (0) root         (0)    23031 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/chromecast/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2398 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/chromecast/_listener.py
--rw-r--r--   0 root         (0) root         (0)      861 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/chromecast/_subtitles.py
--rw-r--r--   0 root         (0) root         (0)     1640 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/chromecast/_utils.py
--rw-r--r--   0 root         (0) root         (0)      343 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/chromecast/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.434651 platypush-1.0.3/platypush/plugins/media/gstreamer/
--rw-r--r--   0 root         (0) root         (0)     7127 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/gstreamer/__init__.py
--rw-r--r--   0 root         (0) root         (0)      471 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/gstreamer/manifest.json
--rw-r--r--   0 root         (0) root         (0)     1783 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/gstreamer/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.434651 platypush-1.0.3/platypush/plugins/media/jellyfin/
--rw-r--r--   0 root         (0) root         (0)    12071 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/jellyfin/__init__.py
--rw-r--r--   0 root         (0) root         (0)      113 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/jellyfin/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.434651 platypush-1.0.3/platypush/plugins/media/kodi/
--rw-r--r--   0 root         (0) root         (0)    22266 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/kodi/__init__.py
--rw-r--r--   0 root         (0) root         (0)      273 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/kodi/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.434651 platypush-1.0.3/platypush/plugins/media/lib/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3392 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/lib/plexcast.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.434651 platypush-1.0.3/platypush/plugins/media/mplayer/
--rw-r--r--   0 root         (0) root         (0)    25835 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/mplayer/__init__.py
--rw-r--r--   0 root         (0) root         (0)      378 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/mplayer/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.434651 platypush-1.0.3/platypush/plugins/media/mpv/
--rw-r--r--   0 root         (0) root         (0)    15631 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/mpv/__init__.py
--rw-r--r--   0 root         (0) root         (0)      485 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/mpv/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.434651 platypush-1.0.3/platypush/plugins/media/omxplayer/
--rw-r--r--   0 root         (0) root         (0)    12995 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/omxplayer/__init__.py
--rw-r--r--   0 root         (0) root         (0)      269 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/omxplayer/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.434651 platypush-1.0.3/platypush/plugins/media/plex/
--rw-r--r--   0 root         (0) root         (0)    15190 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/plex/__init__.py
--rw-r--r--   0 root         (0) root         (0)      174 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/plex/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.434651 platypush-1.0.3/platypush/plugins/media/search/
--rw-r--r--   0 root         (0) root         (0)      901 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/search/__init__.py
--rw-r--r--   0 root         (0) root         (0)      808 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/search/jellyfin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.437985 platypush-1.0.3/platypush/plugins/media/search/local/
--rw-r--r--   0 root         (0) root         (0)    10121 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/search/local/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2749 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/search/local/db.py
--rw-r--r--   0 root         (0) root         (0)     2367 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/search/local/metadata.py
--rw-r--r--   0 root         (0) root         (0)     2283 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/search/plex.py
--rw-r--r--   0 root         (0) root         (0)      521 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/search/torrent.py
--rw-r--r--   0 root         (0) root         (0)      595 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/search/youtube.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.437985 platypush-1.0.3/platypush/plugins/media/subtitles/
--rw-r--r--   0 root         (0) root         (0)     7137 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/subtitles/__init__.py
--rw-r--r--   0 root         (0) root         (0)      262 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/subtitles/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.437985 platypush-1.0.3/platypush/plugins/media/vlc/
--rw-r--r--   0 root         (0) root         (0)    16443 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/vlc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      468 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/vlc/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.437985 platypush-1.0.3/platypush/plugins/media/webtorrent/
--rw-r--r--   0 root         (0) root         (0)    17156 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/webtorrent/__init__.py
--rw-r--r--   0 root         (0) root         (0)      155 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/media/webtorrent/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.437985 platypush-1.0.3/platypush/plugins/midi/
--rw-r--r--   0 root         (0) root         (0)    10804 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/midi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5467 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/midi/_model.py
--rw-r--r--   0 root         (0) root         (0)      641 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/midi/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.437985 platypush-1.0.3/platypush/plugins/ml/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/ml/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.437985 platypush-1.0.3/platypush/plugins/ml/cv/
--rw-r--r--   0 root         (0) root         (0)     2822 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/ml/cv/__init__.py
--rw-r--r--   0 root         (0) root         (0)      479 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/ml/cv/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.437985 platypush-1.0.3/platypush/plugins/mobile/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mobile/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.437985 platypush-1.0.3/platypush/plugins/mobile/join/
--rw-r--r--   0 root         (0) root         (0)    16171 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mobile/join/__init__.py
--rw-r--r--   0 root         (0) root         (0)      150 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mobile/join/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.437985 platypush-1.0.3/platypush/plugins/mqtt/
--rw-r--r--   0 root         (0) root         (0)    18655 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mqtt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7604 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mqtt/_client.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/mqtt/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.437985 platypush-1.0.3/platypush/plugins/music/
--rw-r--r--   0 root         (0) root         (0)     2937 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/music/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.441318 platypush-1.0.3/platypush/plugins/music/mopidy/
--rw-r--r--   0 root         (0) root         (0)    35393 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/music/mopidy/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16095 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/music/mopidy/_client.py
--rw-r--r--   0 root         (0) root         (0)       62 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/music/mopidy/_common.py
--rw-r--r--   0 root         (0) root         (0)      439 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/music/mopidy/_conf.py
--rw-r--r--   0 root         (0) root         (0)      207 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/music/mopidy/_exc.py
--rw-r--r--   0 root         (0) root         (0)      859 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/music/mopidy/_playlist.py
--rw-r--r--   0 root         (0) root         (0)     1266 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/music/mopidy/_status.py
--rw-r--r--   0 root         (0) root         (0)     1414 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/music/mopidy/_sync.py
--rw-r--r--   0 root         (0) root         (0)     1627 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/music/mopidy/_task.py
--rw-r--r--   0 root         (0) root         (0)     1480 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/music/mopidy/_track.py
--rw-r--r--   0 root         (0) root         (0)      898 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/music/mopidy/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.441318 platypush-1.0.3/platypush/plugins/music/mpd/
--rw-r--r--   0 root         (0) root         (0)    27060 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/music/mpd/__init__.py
--rw-r--r--   0 root         (0) root         (0)      175 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/music/mpd/_conf.py
--rw-r--r--   0 root         (0) root         (0)     5295 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/music/mpd/_listener.py
--rw-r--r--   0 root         (0) root         (0)      662 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/music/mpd/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.441318 platypush-1.0.3/platypush/plugins/music/snapcast/
--rw-r--r--   0 root         (0) root         (0)    31741 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/music/snapcast/__init__.py
--rw-r--r--   0 root         (0) root         (0)      153 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/music/snapcast/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.441318 platypush-1.0.3/platypush/plugins/music/spotify/
--rw-r--r--   0 root         (0) root         (0)    36503 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/music/spotify/__init__.py
--rw-r--r--   0 root         (0) root         (0)      152 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/music/spotify/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.441318 platypush-1.0.3/platypush/plugins/music/tidal/
--rw-r--r--   0 root         (0) root         (0)    12571 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/music/tidal/__init__.py
--rw-r--r--   0 root         (0) root         (0)      260 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/music/tidal/manifest.json
--rw-r--r--   0 root         (0) root         (0)     1597 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/music/tidal/workers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.444651 platypush-1.0.3/platypush/plugins/nextcloud/
--rw-r--r--   0 root         (0) root         (0)    44114 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/nextcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)      389 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/nextcloud/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.444651 platypush-1.0.3/platypush/plugins/nfc/
--rw-r--r--   0 root         (0) root         (0)     9106 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/nfc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      431 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/nfc/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.444651 platypush-1.0.3/platypush/plugins/ngrok/
--rw-r--r--   0 root         (0) root         (0)     5900 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/ngrok/__init__.py
--rw-r--r--   0 root         (0) root         (0)      569 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/ngrok/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.444651 platypush-1.0.3/platypush/plugins/nmap/
--rw-r--r--   0 root         (0) root         (0)      976 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/nmap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      143 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/nmap/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.444651 platypush-1.0.3/platypush/plugins/ntfy/
--rw-r--r--   0 root         (0) root         (0)     9817 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/ntfy/__init__.py
--rw-r--r--   0 root         (0) root         (0)      199 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/ntfy/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.444651 platypush-1.0.3/platypush/plugins/openai/
--rw-r--r--   0 root         (0) root         (0)    10127 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/openai/__init__.py
--rw-r--r--   0 root         (0) root         (0)       87 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/openai/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.444651 platypush-1.0.3/platypush/plugins/otp/
--rw-r--r--   0 root         (0) root         (0)     8357 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/otp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      352 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/otp/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.444651 platypush-1.0.3/platypush/plugins/pihole/
--rw-r--r--   0 root         (0) root         (0)    16748 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/pihole/__init__.py
--rw-r--r--   0 root         (0) root         (0)      145 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/pihole/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.444651 platypush-1.0.3/platypush/plugins/ping/
--rw-r--r--   0 root         (0) root         (0)     8189 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/ping/__init__.py
--rw-r--r--   0 root         (0) root         (0)      422 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/ping/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.444651 platypush-1.0.3/platypush/plugins/pushbullet/
--rw-r--r--   0 root         (0) root         (0)    13984 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/pushbullet/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1395 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/pushbullet/listener.py
--rw-r--r--   0 root         (0) root         (0)      772 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/pushbullet/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.444651 platypush-1.0.3/platypush/plugins/pwm/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/pwm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.447985 platypush-1.0.3/platypush/plugins/pwm/pca9685/
--rw-r--r--   0 root         (0) root         (0)     5791 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/pwm/pca9685/__init__.py
--rw-r--r--   0 root         (0) root         (0)      198 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/pwm/pca9685/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.447985 platypush-1.0.3/platypush/plugins/qrcode/
--rw-r--r--   0 root         (0) root         (0)     6369 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/qrcode/__init__.py
--rw-r--r--   0 root         (0) root         (0)      741 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/qrcode/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.447985 platypush-1.0.3/platypush/plugins/redis/
--rw-r--r--   0 root         (0) root         (0)     2786 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)      144 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/redis/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.447985 platypush-1.0.3/platypush/plugins/rss/
--rw-r--r--   0 root         (0) root         (0)    13318 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/rss/__init__.py
--rw-r--r--   0 root         (0) root         (0)      628 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/rss/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.447985 platypush-1.0.3/platypush/plugins/rtorrent/
--rw-r--r--   0 root         (0) root         (0)    18201 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/rtorrent/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1139 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/rtorrent/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.447985 platypush-1.0.3/platypush/plugins/sensor/
--rw-r--r--   0 root         (0) root         (0)    14853 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sensor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.447985 platypush-1.0.3/platypush/plugins/sensor/bme280/
--rw-r--r--   0 root         (0) root         (0)     3706 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sensor/bme280/__init__.py
--rw-r--r--   0 root         (0) root         (0)      409 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sensor/bme280/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.447985 platypush-1.0.3/platypush/plugins/sensor/dht/
--rw-r--r--   0 root         (0) root         (0)     4084 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sensor/dht/__init__.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sensor/dht/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.447985 platypush-1.0.3/platypush/plugins/sensor/distance/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sensor/distance/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.447985 platypush-1.0.3/platypush/plugins/sensor/distance/vl53l1x/
--rw-r--r--   0 root         (0) root         (0)     3546 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sensor/distance/vl53l1x/__init__.py
--rw-r--r--   0 root         (0) root         (0)      271 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sensor/distance/vl53l1x/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.447985 platypush-1.0.3/platypush/plugins/sensor/envirophat/
--rw-r--r--   0 root         (0) root         (0)     5016 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sensor/envirophat/__init__.py
--rw-r--r--   0 root         (0) root         (0)      408 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sensor/envirophat/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.447985 platypush-1.0.3/platypush/plugins/sensor/hcsr04/
--rw-r--r--   0 root         (0) root         (0)     5554 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sensor/hcsr04/__init__.py
--rw-r--r--   0 root         (0) root         (0)      470 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sensor/hcsr04/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.447985 platypush-1.0.3/platypush/plugins/sensor/lis3dh/
--rw-r--r--   0 root         (0) root         (0)     2258 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sensor/lis3dh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.451318 platypush-1.0.3/platypush/plugins/sensor/lis3dh/lib/
--rw-r--r--   0 root         (0) root         (0)    11260 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sensor/lis3dh/lib/LIS3DH.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sensor/lis3dh/lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)      407 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sensor/lis3dh/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.451318 platypush-1.0.3/platypush/plugins/sensor/ltr559/
--rw-r--r--   0 root         (0) root         (0)     2132 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sensor/ltr559/__init__.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sensor/ltr559/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.451318 platypush-1.0.3/platypush/plugins/sensor/mcp3008/
--rw-r--r--   0 root         (0) root         (0)     6825 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sensor/mcp3008/__init__.py
--rw-r--r--   0 root         (0) root         (0)      411 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sensor/mcp3008/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.451318 platypush-1.0.3/platypush/plugins/sensor/pmw3901/
--rw-r--r--   0 root         (0) root         (0)     5295 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sensor/pmw3901/__init__.py
--rw-r--r--   0 root         (0) root         (0)      402 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sensor/pmw3901/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.451318 platypush-1.0.3/platypush/plugins/serial/
--rw-r--r--   0 root         (0) root         (0)    14631 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/serial/__init__.py
--rw-r--r--   0 root         (0) root         (0)      436 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/serial/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.451318 platypush-1.0.3/platypush/plugins/shell/
--rw-r--r--   0 root         (0) root         (0)     4257 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/shell/__init__.py
--rw-r--r--   0 root         (0) root         (0)      144 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/shell/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.451318 platypush-1.0.3/platypush/plugins/slack/
--rw-r--r--   0 root         (0) root         (0)    10161 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/slack/__init__.py
--rw-r--r--   0 root         (0) root         (0)      661 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/slack/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.451318 platypush-1.0.3/platypush/plugins/smartthings/
--rw-r--r--   0 root         (0) root         (0)    35133 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/smartthings/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17121 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/smartthings/_mappers.py
--rw-r--r--   0 root         (0) root         (0)      181 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/smartthings/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.451318 platypush-1.0.3/platypush/plugins/sound/
--rw-r--r--   0 root         (0) root         (0)    18537 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.454652 platypush-1.0.3/platypush/plugins/sound/_converters/
--rw-r--r--   0 root         (0) root         (0)      295 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_converters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8995 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_converters/_base.py
--rw-r--r--   0 root         (0) root         (0)     1376 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_converters/_from_raw.py
--rw-r--r--   0 root         (0) root         (0)     1614 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_converters/_to_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.454652 platypush-1.0.3/platypush/plugins/sound/_manager/
--rw-r--r--   0 root         (0) root         (0)       60 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_manager/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3687 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_manager/_device.py
--rw-r--r--   0 root         (0) root         (0)    10651 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_manager/_main.py
--rw-r--r--   0 root         (0) root         (0)     7477 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_manager/_stream.py
--rw-r--r--   0 root         (0) root         (0)      737 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.454652 platypush-1.0.3/platypush/plugins/sound/_streams/
--rw-r--r--   0 root         (0) root         (0)      161 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_streams/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15916 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_streams/_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.454652 platypush-1.0.3/platypush/plugins/sound/_streams/_player/
--rw-r--r--   0 root         (0) root         (0)       58 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_streams/_player/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2944 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_streams/_player/_base.py
--rw-r--r--   0 root         (0) root         (0)      938 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_streams/_player/_resource.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.454652 platypush-1.0.3/platypush/plugins/sound/_streams/_player/_synth/
--rw-r--r--   0 root         (0) root         (0)      105 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_streams/_player/_synth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2527 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_streams/_player/_synth/_base.py
--rw-r--r--   0 root         (0) root         (0)     2999 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_streams/_player/_synth/_generator.py
--rw-r--r--   0 root         (0) root         (0)     3412 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_streams/_player/_synth/_mix.py
--rw-r--r--   0 root         (0) root         (0)     2442 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_streams/_player/_synth/_output.py
--rw-r--r--   0 root         (0) root         (0)     3114 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_streams/_player/_synth/_parser.py
--rw-r--r--   0 root         (0) root         (0)     3543 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_streams/_player/_synth/_player.py
--rw-r--r--   0 root         (0) root         (0)     7199 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_streams/_player/_synth/_sound.py
--rw-r--r--   0 root         (0) root         (0)     2718 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_streams/_recorder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.454652 platypush-1.0.3/platypush/plugins/sound/_utils/
--rw-r--r--   0 root         (0) root         (0)       71 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      771 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/_utils/_convert.py
--rw-r--r--   0 root         (0) root         (0)     1280 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sound/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.457985 platypush-1.0.3/platypush/plugins/ssh/
--rw-r--r--   0 root         (0) root         (0)    29807 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/ssh/__init__.py
--rw-r--r--   0 root         (0) root         (0)      369 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/ssh/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.457985 platypush-1.0.3/platypush/plugins/ssh/tunnel/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/ssh/tunnel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2207 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/ssh/tunnel/forward.py
--rw-r--r--   0 root         (0) root         (0)     1985 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/ssh/tunnel/reverse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.457985 platypush-1.0.3/platypush/plugins/sun/
--rw-r--r--   0 root         (0) root         (0)     3501 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sun/__init__.py
--rw-r--r--   0 root         (0) root         (0)      274 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/sun/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.457985 platypush-1.0.3/platypush/plugins/switch/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/switch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.457985 platypush-1.0.3/platypush/plugins/switch/tplink/
--rw-r--r--   0 root         (0) root         (0)     7615 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/switch/tplink/__init__.py
--rw-r--r--   0 root         (0) root         (0)      177 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/switch/tplink/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.457985 platypush-1.0.3/platypush/plugins/switch/wemo/
--rw-r--r--   0 root         (0) root         (0)     6684 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/switch/wemo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2329 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/switch/wemo/lib.py
--rw-r--r--   0 root         (0) root         (0)      150 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/switch/wemo/manifest.json
--rw-r--r--   0 root         (0) root         (0)     1005 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/switch/wemo/scanner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.457985 platypush-1.0.3/platypush/plugins/switchbot/
--rw-r--r--   0 root         (0) root         (0)    37338 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/switchbot/__init__.py
--rw-r--r--   0 root         (0) root         (0)      838 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/switchbot/_constants.py
--rw-r--r--   0 root         (0) root         (0)     4309 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/switchbot/_setters.py
--rw-r--r--   0 root         (0) root         (0)      148 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/switchbot/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.457985 platypush-1.0.3/platypush/plugins/system/
--rw-r--r--   0 root         (0) root         (0)    21396 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/system/__init__.py
--rw-r--r--   0 root         (0) root         (0)      376 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/system/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.457985 platypush-1.0.3/platypush/plugins/tcp/
--rw-r--r--   0 root         (0) root         (0)     3763 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/tcp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      142 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/tcp/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.461319 platypush-1.0.3/platypush/plugins/telegram/
--rw-r--r--   0 root         (0) root         (0)    43311 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/telegram/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/telegram/_bridge.py
--rw-r--r--   0 root         (0) root         (0)     1765 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/telegram/_model.py
--rw-r--r--   0 root         (0) root         (0)     9092 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/telegram/_service.py
--rw-r--r--   0 root         (0) root         (0)      429 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/telegram/_utils.py
--rw-r--r--   0 root         (0) root         (0)      681 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/telegram/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.461319 platypush-1.0.3/platypush/plugins/tensorflow/
--rw-r--r--   0 root         (0) root         (0)    55458 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1381 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/tensorflow/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.461319 platypush-1.0.3/platypush/plugins/todoist/
--rw-r--r--   0 root         (0) root         (0)     5812 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/todoist/__init__.py
--rw-r--r--   0 root         (0) root         (0)      178 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/todoist/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.461319 platypush-1.0.3/platypush/plugins/torrent/
--rw-r--r--   0 root         (0) root         (0)    21966 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/torrent/__init__.py
--rw-r--r--   0 root         (0) root         (0)      400 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/torrent/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.461319 platypush-1.0.3/platypush/plugins/trello/
--rw-r--r--   0 root         (0) root         (0)    36307 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/trello/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2734 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/trello/_model.py
--rw-r--r--   0 root         (0) root         (0)      401 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/trello/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.461319 platypush-1.0.3/platypush/plugins/tts/
--rw-r--r--   0 root         (0) root         (0)     1681 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/tts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.461319 platypush-1.0.3/platypush/plugins/tts/google/
--rw-r--r--   0 root         (0) root         (0)     5101 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/tts/google/__init__.py
--rw-r--r--   0 root         (0) root         (0)      623 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/tts/google/manifest.json
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/tts/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.461319 platypush-1.0.3/platypush/plugins/tts/mimic3/
--rw-r--r--   0 root         (0) root         (0)     3855 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/tts/mimic3/__init__.py
--rw-r--r--   0 root         (0) root         (0)      586 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/tts/mimic3/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.461319 platypush-1.0.3/platypush/plugins/tts/picovoice/
--rw-r--r--   0 root         (0) root         (0)     6245 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/tts/picovoice/__init__.py
--rw-r--r--   0 root         (0) root         (0)      507 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/tts/picovoice/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.464652 platypush-1.0.3/platypush/plugins/tv/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/tv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.464652 platypush-1.0.3/platypush/plugins/tv/samsung/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/tv/samsung/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.464652 platypush-1.0.3/platypush/plugins/tv/samsung/ws/
--rw-r--r--   0 root         (0) root         (0)    14011 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/tv/samsung/ws/__init__.py
--rw-r--r--   0 root         (0) root         (0)      181 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/tv/samsung/ws/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.464652 platypush-1.0.3/platypush/plugins/twilio/
--rw-r--r--   0 root         (0) root         (0)    29227 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/twilio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      266 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/twilio/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.464652 platypush-1.0.3/platypush/plugins/udp/
--rw-r--r--   0 root         (0) root         (0)     1756 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/udp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      142 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/udp/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.464652 platypush-1.0.3/platypush/plugins/user/
--rw-r--r--   0 root         (0) root         (0)     6743 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/user/__init__.py
--rw-r--r--   0 root         (0) root         (0)      143 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/user/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.464652 platypush-1.0.3/platypush/plugins/utils/
--rw-r--r--   0 root         (0) root         (0)    11092 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      144 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/utils/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.464652 platypush-1.0.3/platypush/plugins/variable/
--rw-r--r--   0 root         (0) root         (0)     5941 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/variable/__init__.py
--rw-r--r--   0 root         (0) root         (0)      147 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/variable/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.464652 platypush-1.0.3/platypush/plugins/wallabag/
--rw-r--r--   0 root         (0) root         (0)    16091 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/wallabag/__init__.py
--rw-r--r--   0 root         (0) root         (0)       89 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/wallabag/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.464652 platypush-1.0.3/platypush/plugins/weather/
--rw-r--r--   0 root         (0) root         (0)     4251 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/weather/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.464652 platypush-1.0.3/platypush/plugins/weather/buienradar/
--rw-r--r--   0 root         (0) root         (0)     3168 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/weather/buienradar/__init__.py
--rw-r--r--   0 root         (0) root         (0)      255 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/weather/buienradar/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.464652 platypush-1.0.3/platypush/plugins/weather/openweathermap/
--rw-r--r--   0 root         (0) root         (0)     5509 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/weather/openweathermap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      231 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/weather/openweathermap/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.467985 platypush-1.0.3/platypush/plugins/websocket/
--rw-r--r--   0 root         (0) root         (0)     7560 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/websocket/__init__.py
--rw-r--r--   0 root         (0) root         (0)      274 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/websocket/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.467985 platypush-1.0.3/platypush/plugins/xmpp/
--rw-r--r--   0 root         (0) root         (0)    23442 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      408 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_base.py
--rw-r--r--   0 root         (0) root         (0)      605 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.467985 platypush-1.0.3/platypush/plugins/xmpp/_handlers/
--rw-r--r--   0 root         (0) root         (0)      751 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      505 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_handlers/_base.py
--rw-r--r--   0 root         (0) root         (0)      970 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_handlers/_connection.py
--rw-r--r--   0 root         (0) root         (0)     4010 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_handlers/_conversation.py
--rw-r--r--   0 root         (0) root         (0)      658 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_handlers/_discover.py
--rw-r--r--   0 root         (0) root         (0)     1062 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_handlers/_message.py
--rw-r--r--   0 root         (0) root         (0)      373 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_handlers/_ping.py
--rw-r--r--   0 root         (0) root         (0)     3346 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_handlers/_presence.py
--rw-r--r--   0 root         (0) root         (0)      378 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_handlers/_pubsub.py
--rw-r--r--   0 root         (0) root         (0)      482 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_handlers/_registry.py
--rw-r--r--   0 root         (0) root         (0)    18552 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_handlers/_room.py
--rw-r--r--   0 root         (0) root         (0)     3903 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_handlers/_roster.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.471319 platypush-1.0.3/platypush/plugins/xmpp/_mixins/
--rw-r--r--   0 root         (0) root         (0)      375 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_mixins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1601 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_mixins/_async.py
--rw-r--r--   0 root         (0) root         (0)     1601 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_mixins/_base.py
--rw-r--r--   0 root         (0) root         (0)      487 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_mixins/_config.py
--rw-r--r--   0 root         (0) root         (0)      515 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_mixins/_event_state.py
--rw-r--r--   0 root         (0) root         (0)     3316 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_mixins/_events.py
--rw-r--r--   0 root         (0) root         (0)     1008 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_mixins/_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.471319 platypush-1.0.3/platypush/plugins/xmpp/_state/
--rw-r--r--   0 root         (0) root         (0)      152 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_state/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5602 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_state/_model.py
--rw-r--r--   0 root         (0) root         (0)     4332 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_state/_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.471319 platypush-1.0.3/platypush/plugins/xmpp/_types/
--rw-r--r--   0 root         (0) root         (0)      216 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_types/__init__.py
--rw-r--r--   0 root         (0) root         (0)      584 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_types/_errors.py
--rw-r--r--   0 root         (0) root         (0)     1684 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_types/_invite.py
--rw-r--r--   0 root         (0) root         (0)      338 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/_types/_presence.py
--rw-r--r--   0 root         (0) root         (0)     2362 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/xmpp/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.471319 platypush-1.0.3/platypush/plugins/youtube/
--rw-r--r--   0 root         (0) root         (0)     6414 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/youtube/__init__.py
--rw-r--r--   0 root         (0) root         (0)      337 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/youtube/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.471319 platypush-1.0.3/platypush/plugins/zeroconf/
--rw-r--r--   0 root         (0) root         (0)     5888 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/zeroconf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      456 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/zeroconf/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.471319 platypush-1.0.3/platypush/plugins/zigbee/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/zigbee/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.471319 platypush-1.0.3/platypush/plugins/zigbee/mqtt/
--rw-r--r--   0 root         (0) root         (0)    89045 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/zigbee/mqtt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2353 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/zigbee/mqtt/_state.py
--rw-r--r--   0 root         (0) root         (0)     2658 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/zigbee/mqtt/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.471319 platypush-1.0.3/platypush/plugins/zwave/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/zwave/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2706 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/zwave/_constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.471319 platypush-1.0.3/platypush/plugins/zwave/mqtt/
--rw-r--r--   0 root         (0) root         (0)    79655 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/zwave/mqtt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2555 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/zwave/mqtt/_state.py
--rw-r--r--   0 root         (0) root         (0)     1177 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/plugins/zwave/mqtt/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.474652 platypush-1.0.3/platypush/procedure/
--rw-r--r--   0 root         (0) root         (0)    18056 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/procedure/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.474652 platypush-1.0.3/platypush/process/
--rw-r--r--   0 root         (0) root         (0)     3680 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/process/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.474652 platypush-1.0.3/platypush/runner/
--rw-r--r--   0 root         (0) root         (0)      436 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/runner/__init__.py
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/runner/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1720 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/runner/_app.py
--rw-r--r--   0 root         (0) root         (0)     2678 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/runner/_runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.477986 platypush-1.0.3/platypush/schemas/
--rw-r--r--   0 root         (0) root         (0)     3145 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3502 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/cups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.477986 platypush-1.0.3/platypush/schemas/dataclasses/
--rw-r--r--   0 root         (0) root         (0)     1739 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/dataclasses/__init__.py
--rw-r--r--   0 root         (0) root         (0)      792 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/dbus.py
--rw-r--r--   0 root         (0) root         (0)     3197 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/esp.py
--rw-r--r--   0 root         (0) root         (0)     1497 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/gotify.py
--rw-r--r--   0 root         (0) root         (0)     3909 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/gps.py
--rw-r--r--   0 root         (0) root         (0)     2263 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/hid.py
--rw-r--r--   0 root         (0) root         (0)     4149 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/irc.py
--rw-r--r--   0 root         (0) root         (0)     4138 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/joystick.py
--rw-r--r--   0 root         (0) root         (0)    10453 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/linode.py
--rw-r--r--   0 root         (0) root         (0)      941 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/maps.py
--rw-r--r--   0 root         (0) root         (0)     5956 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/mastodon.py
--rw-r--r--   0 root         (0) root         (0)     9974 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/matrix.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.477986 platypush-1.0.3/platypush/schemas/media/
--rw-r--r--   0 root         (0) root         (0)     1363 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/media/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3771 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/media/jellyfin.py
--rw-r--r--   0 root         (0) root         (0)    10917 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/mopidy.py
--rw-r--r--   0 root         (0) root         (0)      791 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/ngrok.py
--rw-r--r--   0 root         (0) root         (0)     3344 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/pihole.py
--rw-r--r--   0 root         (0) root         (0)     1246 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/ping.py
--rw-r--r--   0 root         (0) root         (0)     6476 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/piped.py
--rw-r--r--   0 root         (0) root         (0)     8040 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/pushbullet.py
--rw-r--r--   0 root         (0) root         (0)     3698 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/qrcode.py
--rw-r--r--   0 root         (0) root         (0)     1265 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/rss.py
--rw-r--r--   0 root         (0) root         (0)     1386 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/slack.py
--rw-r--r--   0 root         (0) root         (0)    12347 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/spotify.py
--rw-r--r--   0 root         (0) root         (0)      992 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/sun.py
--rw-r--r--   0 root         (0) root         (0)      365 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/switch.py
--rw-r--r--   0 root         (0) root         (0)     8416 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/switchbot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.477986 platypush-1.0.3/platypush/schemas/system/
--rw-r--r--   0 root         (0) root         (0)     1303 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/__init__.py
--rw-r--r--   0 root         (0) root         (0)      333 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.481319 platypush-1.0.3/platypush/schemas/system/_battery/
--rw-r--r--   0 root         (0) root         (0)      104 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_battery/__init__.py
--rw-r--r--   0 root         (0) root         (0)      619 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_battery/_base.py
--rw-r--r--   0 root         (0) root         (0)      935 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_battery/_model.py
--rw-r--r--   0 root         (0) root         (0)      184 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_battery/_schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.481319 platypush-1.0.3/platypush/schemas/system/_connection/
--rw-r--r--   0 root         (0) root         (0)      116 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_connection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1149 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_connection/_base.py
--rw-r--r--   0 root         (0) root         (0)     2383 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_connection/_model.py
--rw-r--r--   0 root         (0) root         (0)      199 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_connection/_schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.481319 platypush-1.0.3/platypush/schemas/system/_cpu/
--rw-r--r--   0 root         (0) root         (0)      340 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_cpu/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1563 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_cpu/_base.py
--rw-r--r--   0 root         (0) root         (0)     3997 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_cpu/_model.py
--rw-r--r--   0 root         (0) root         (0)      495 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_cpu/_schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.481319 platypush-1.0.3/platypush/schemas/system/_disk/
--rw-r--r--   0 root         (0) root         (0)       93 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_disk/__init__.py
--rw-r--r--   0 root         (0) root         (0)      625 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_disk/_base.py
--rw-r--r--   0 root         (0) root         (0)     2846 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_disk/_model.py
--rw-r--r--   0 root         (0) root         (0)      169 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_disk/_schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.481319 platypush-1.0.3/platypush/schemas/system/_fan/
--rw-r--r--   0 root         (0) root         (0)       88 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_fan/__init__.py
--rw-r--r--   0 root         (0) root         (0)      359 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_fan/_base.py
--rw-r--r--   0 root         (0) root         (0)      690 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_fan/_model.py
--rw-r--r--   0 root         (0) root         (0)      164 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_fan/_schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.481319 platypush-1.0.3/platypush/schemas/system/_memory/
--rw-r--r--   0 root         (0) root         (0)      181 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_memory/__init__.py
--rw-r--r--   0 root         (0) root         (0)      423 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_memory/_base.py
--rw-r--r--   0 root         (0) root         (0)     2312 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_memory/_model.py
--rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_memory/_schemas.py
--rw-r--r--   0 root         (0) root         (0)      574 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.484653 platypush-1.0.3/platypush/schemas/system/_network/
--rw-r--r--   0 root         (0) root         (0)      152 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_network/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1239 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_network/_base.py
--rw-r--r--   0 root         (0) root         (0)     4610 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_network/_model.py
--rw-r--r--   0 root         (0) root         (0)      235 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_network/_schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.484653 platypush-1.0.3/platypush/schemas/system/_process/
--rw-r--r--   0 root         (0) root         (0)      104 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_process/__init__.py
--rw-r--r--   0 root         (0) root         (0)      850 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_process/_base.py
--rw-r--r--   0 root         (0) root         (0)     2539 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_process/_model.py
--rw-r--r--   0 root         (0) root         (0)      184 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_process/_schemas.py
--rw-r--r--   0 root         (0) root         (0)      213 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.484653 platypush-1.0.3/platypush/schemas/system/_temperature/
--rw-r--r--   0 root         (0) root         (0)      120 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_temperature/__init__.py
--rw-r--r--   0 root         (0) root         (0)      375 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_temperature/_base.py
--rw-r--r--   0 root         (0) root         (0)     1209 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_temperature/_model.py
--rw-r--r--   0 root         (0) root         (0)      204 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_temperature/_schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.484653 platypush-1.0.3/platypush/schemas/system/_user/
--rw-r--r--   0 root         (0) root         (0)       92 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)      590 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_user/_base.py
--rw-r--r--   0 root         (0) root         (0)      980 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_user/_model.py
--rw-r--r--   0 root         (0) root         (0)      169 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/system/_user/_schemas.py
--rw-r--r--   0 root         (0) root         (0)     5620 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/telegram.py
--rw-r--r--   0 root         (0) root         (0)      782 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/tensorflow.py
--rw-r--r--   0 root         (0) root         (0)     6295 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/tidal.py
--rw-r--r--   0 root         (0) root         (0)     6881 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/todoist.py
--rw-r--r--   0 root         (0) root         (0)    12008 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/trello.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.484653 platypush-1.0.3/platypush/schemas/tts/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/tts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1027 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/tts/mimic3.py
--rw-r--r--   0 root         (0) root         (0)     3208 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/wallabag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.484653 platypush-1.0.3/platypush/schemas/weather/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/weather/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4009 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/weather/buienradar.py
--rw-r--r--   0 root         (0) root         (0)     4911 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/schemas/weather/openweathermap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.484653 platypush-1.0.3/platypush/user/
--rw-r--r--   0 root         (0) root         (0)    11989 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/user/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.487986 platypush-1.0.3/platypush/utils/
--rw-r--r--   0 root         (0) root         (0)    23115 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22068 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/utils/manifest.py
--rw-r--r--   0 root         (0) root         (0)     1462 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/utils/media.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.487986 platypush-1.0.3/platypush/utils/mock/
--rw-r--r--   0 root         (0) root         (0)     5653 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/utils/mock/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2161 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/utils/mock/modules.py
--rw-r--r--   0 root         (0) root         (0)     1309 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/utils/ngrok.py
--rw-r--r--   0 root         (0) root         (0)     1699 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/utils/threads.py
--rw-r--r--   0 root         (0) root         (0)     4165 2024-05-31 01:03:24.000000 platypush-1.0.3/platypush/utils/workers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.487986 platypush-1.0.3/platypush.egg-info/
--rw-r--r--   0 root         (0) root         (0)    56629 2024-05-31 01:06:35.000000 platypush-1.0.3/platypush.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    95808 2024-05-31 01:06:36.000000 platypush-1.0.3/platypush.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 01:06:35.000000 platypush-1.0.3/platypush.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2024-05-31 01:06:35.000000 platypush-1.0.3/platypush.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     3159 2024-05-31 01:06:35.000000 platypush-1.0.3/platypush.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-31 01:06:35.000000 platypush-1.0.3/platypush.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      203 2024-05-31 01:03:24.000000 platypush-1.0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      415 2024-05-31 01:06:36.504654 platypush-1.0.3/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     3180 2024-05-31 01:03:24.000000 platypush-1.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 01:06:36.487986 platypush-1.0.3/tests/
--rw-r--r--   0 root         (0) root         (0)      680 2024-05-31 01:03:24.000000 platypush-1.0.3/tests/test_cron.py
--rw-r--r--   0 root         (0) root         (0)     3823 2024-05-31 01:03:24.000000 platypush-1.0.3/tests/test_event_parse.py
--rw-r--r--   0 root         (0) root         (0)     2658 2024-05-31 01:03:24.000000 platypush-1.0.3/tests/test_http.py
--rw-r--r--   0 root         (0) root         (0)     2055 2024-05-31 01:03:24.000000 platypush-1.0.3/tests/test_procedure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.863482 platypush-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-05-31 18:02:50.000000 platypush-1.0.4/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      280 2024-05-31 18:02:50.000000 platypush-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    56629 2024-05-31 18:06:00.863482 platypush-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    45388 2024-05-31 18:02:50.000000 platypush-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.550138 platypush-1.0.4/platypush/
+-rw-r--r--   0 root         (0) root         (0)      930 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       42 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.550138 platypush-1.0.4/platypush/app/
+-rw-r--r--   0 root         (0) root         (0)       84 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/app/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    17899 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/app/_app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.550138 platypush-1.0.4/platypush/backend/
+-rw-r--r--   0 root         (0) root         (0)    16878 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.550138 platypush-1.0.4/platypush/backend/http/
+-rw-r--r--   0 root         (0) root         (0)    18042 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.550138 platypush-1.0.4/platypush/backend/http/app/
+-rw-r--r--   0 root         (0) root         (0)      945 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.550138 platypush-1.0.4/platypush/backend/http/app/mixins/
+-rw-r--r--   0 root         (0) root         (0)     5021 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/mixins/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.553472 platypush-1.0.4/platypush/backend/http/app/routes/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/routes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1980 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/routes/auth.py
+-rw-r--r--   0 root         (0) root         (0)      611 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/routes/dashboard.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/routes/execute.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/routes/hook.py
+-rw-r--r--   0 root         (0) root         (0)      501 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/routes/index.py
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/routes/login.py
+-rw-r--r--   0 root         (0) root         (0)     5412 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/routes/logo.py
+-rw-r--r--   0 root         (0) root         (0)      990 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/routes/logout.py
+-rw-r--r--   0 root         (0) root         (0)      570 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/routes/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.553472 platypush-1.0.4/platypush/backend/http/app/routes/plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/routes/plugins/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.553472 platypush-1.0.4/platypush/backend/http/app/routes/plugins/camera/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/routes/plugins/camera/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/routes/plugins/camera/pi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.553472 platypush-1.0.4/platypush/backend/http/app/routes/plugins/qrcode/
+-rw-r--r--   0 root         (0) root         (0)      854 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/routes/plugins/qrcode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1057 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/routes/plugins/spotify.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.553472 platypush-1.0.4/platypush/backend/http/app/routes/plugins/tts/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/routes/plugins/tts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3776 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/routes/pwa.py
+-rw-r--r--   0 root         (0) root         (0)     2314 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/routes/register.py
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/routes/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.553472 platypush-1.0.4/platypush/backend/http/app/streaming/
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/streaming/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4457 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/streaming/_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.553472 platypush-1.0.4/platypush/backend/http/app/streaming/plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/streaming/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4223 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/streaming/plugins/camera.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.556805 platypush-1.0.4/platypush/backend/http/app/streaming/plugins/media/
+-rw-r--r--   0 root         (0) root         (0)      138 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/streaming/plugins/media/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      472 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/streaming/plugins/media/_constants.py
+-rw-r--r--   0 root         (0) root         (0)     1318 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/streaming/plugins/media/_register.py
+-rw-r--r--   0 root         (0) root         (0)     1097 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/streaming/plugins/media/_registry.py
+-rw-r--r--   0 root         (0) root         (0)     4429 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/streaming/plugins/media/_stream.py
+-rw-r--r--   0 root         (0) root         (0)     4168 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/streaming/plugins/media/_subtitles.py
+-rw-r--r--   0 root         (0) root         (0)      821 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/streaming/plugins/media/_unregister.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/streaming/plugins/sound.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.556805 platypush-1.0.4/platypush/backend/http/app/utils/
+-rw-r--r--   0 root         (0) root         (0)      763 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.556805 platypush-1.0.4/platypush/backend/http/app/utils/auth/
+-rw-r--r--   0 root         (0) root         (0)     5346 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/utils/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      478 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/utils/auth/status.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/utils/bus.py
+-rw-r--r--   0 root         (0) root         (0)      801 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/utils/routes.py
+-rw-r--r--   0 root         (0) root         (0)     1114 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/utils/streaming.py
+-rw-r--r--   0 root         (0) root         (0)     1013 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/utils/ws.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.556805 platypush-1.0.4/platypush/backend/http/app/ws/
+-rw-r--r--   0 root         (0) root         (0)       68 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/ws/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/ws/_base.py
+-rw-r--r--   0 root         (0) root         (0)     1786 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/ws/cmd.py
+-rw-r--r--   0 root         (0) root         (0)     1350 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/ws/events.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/app/ws/requests.py
+-rw-r--r--   0 root         (0) root         (0)      144 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.556805 platypush-1.0.4/platypush/backend/http/media/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/media/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.556805 platypush-1.0.4/platypush/backend/http/media/handlers/
+-rw-r--r--   0 root         (0) root         (0)     3364 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/media/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/media/handlers/file.py
+-rw-r--r--   0 root         (0) root         (0)     4014 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.523471 platypush-1.0.4/platypush/backend/http/webapp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.560139 platypush-1.0.4/platypush/backend/http/webapp/dist/
+-rw-r--r--   0 root         (0) root         (0)    16958 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.560139 platypush-1.0.4/platypush/backend/http/webapp/dist/fonts/
+-rw-r--r--   0 root         (0) root         (0)   154584 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/fonts/Poppins.ttf
+-rw-r--r--   0 root         (0) root         (0)      151 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/fonts/poppins.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.560139 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/
+-rw-r--r--   0 root         (0) root         (0)     1120 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/jellyfin.svg
+-rw-r--r--   0 root         (0) root         (0)     1370 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/kodi.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.523471 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.563472 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/01d.png
+-rw-r--r--   0 root         (0) root         (0)     4338 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/01n.png
+-rw-r--r--   0 root         (0) root         (0)     1624 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/02d.png
+-rw-r--r--   0 root         (0) root         (0)     4297 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/02n.png
+-rw-r--r--   0 root         (0) root         (0)     1571 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/03d.png
+-rw-r--r--   0 root         (0) root         (0)     3887 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/03n.png
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/04d.png
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/04n.png
+-rw-r--r--   0 root         (0) root         (0)     1612 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/09d.png
+-rw-r--r--   0 root         (0) root         (0)     1612 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/09n.png
+-rw-r--r--   0 root         (0) root         (0)     1700 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/10d.png
+-rw-r--r--   0 root         (0) root         (0)     1700 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/10n.png
+-rw-r--r--   0 root         (0) root         (0)     1994 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/11d.png
+-rw-r--r--   0 root         (0) root         (0)     1994 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/11n.png
+-rw-r--r--   0 root         (0) root         (0)     1191 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/13d.png
+-rw-r--r--   0 root         (0) root         (0)     1191 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/13n.png
+-rw-r--r--   0 root         (0) root         (0)     1041 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/50d.png
+-rw-r--r--   0 root         (0) root         (0)     1041 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/50n.png
+-rw-r--r--   0 root         (0) root         (0)     1195 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/unknown.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.566806 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/01d.png
+-rw-r--r--   0 root         (0) root         (0)     4338 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/01n.png
+-rw-r--r--   0 root         (0) root         (0)     1624 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/02d.png
+-rw-r--r--   0 root         (0) root         (0)     4297 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/02n.png
+-rw-r--r--   0 root         (0) root         (0)     1571 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/03d.png
+-rw-r--r--   0 root         (0) root         (0)     3887 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/03n.png
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/04d.png
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/04n.png
+-rw-r--r--   0 root         (0) root         (0)     1612 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/09d.png
+-rw-r--r--   0 root         (0) root         (0)     1612 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/09n.png
+-rw-r--r--   0 root         (0) root         (0)     1700 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/10d.png
+-rw-r--r--   0 root         (0) root         (0)     1700 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/10n.png
+-rw-r--r--   0 root         (0) root         (0)     1994 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/11d.png
+-rw-r--r--   0 root         (0) root         (0)     1994 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/11n.png
+-rw-r--r--   0 root         (0) root         (0)     1191 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/13d.png
+-rw-r--r--   0 root         (0) root         (0)     1191 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/13n.png
+-rw-r--r--   0 root         (0) root         (0)     1041 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/50d.png
+-rw-r--r--   0 root         (0) root         (0)     1041 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/50n.png
+-rw-r--r--   0 root         (0) root         (0)     1195 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/unknown.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.566806 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/
+-rw-r--r--   0 root         (0) root         (0)     1333 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/01d.png
+-rw-r--r--   0 root         (0) root         (0)     2489 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/01n.png
+-rw-r--r--   0 root         (0) root         (0)     1871 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/02d.png
+-rw-r--r--   0 root         (0) root         (0)     3888 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/02n.png
+-rw-r--r--   0 root         (0) root         (0)     1762 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/03d.png
+-rw-r--r--   0 root         (0) root         (0)     3363 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/03n.png
+-rw-r--r--   0 root         (0) root         (0)     1203 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/04d.png
+-rw-r--r--   0 root         (0) root         (0)     1203 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/04n.png
+-rw-r--r--   0 root         (0) root         (0)     1826 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/09d.png
+-rw-r--r--   0 root         (0) root         (0)     1826 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/09n.png
+-rw-r--r--   0 root         (0) root         (0)     1890 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/10d.png
+-rw-r--r--   0 root         (0) root         (0)     1890 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/10n.png
+-rw-r--r--   0 root         (0) root         (0)     2178 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/11d.png
+-rw-r--r--   0 root         (0) root         (0)     2178 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/11n.png
+-rw-r--r--   0 root         (0) root         (0)     1502 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/13d.png
+-rw-r--r--   0 root         (0) root         (0)     1502 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/13n.png
+-rw-r--r--   0 root         (0) root         (0)     1211 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/50d.png
+-rw-r--r--   0 root         (0) root         (0)     1211 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/50n.png
+-rw-r--r--   0 root         (0) root         (0)     1396 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/unknown.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.570139 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/
+-rw-r--r--   0 root         (0) root         (0)     1333 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/01d.png
+-rw-r--r--   0 root         (0) root         (0)     2489 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/01n.png
+-rw-r--r--   0 root         (0) root         (0)     1871 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/02d.png
+-rw-r--r--   0 root         (0) root         (0)     3888 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/02n.png
+-rw-r--r--   0 root         (0) root         (0)     1762 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/03d.png
+-rw-r--r--   0 root         (0) root         (0)     3363 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/03n.png
+-rw-r--r--   0 root         (0) root         (0)     1203 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/04d.png
+-rw-r--r--   0 root         (0) root         (0)     1203 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/04n.png
+-rw-r--r--   0 root         (0) root         (0)     1826 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/09d.png
+-rw-r--r--   0 root         (0) root         (0)     1826 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/09n.png
+-rw-r--r--   0 root         (0) root         (0)     1890 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/10d.png
+-rw-r--r--   0 root         (0) root         (0)     1890 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/10n.png
+-rw-r--r--   0 root         (0) root         (0)     2178 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/11d.png
+-rw-r--r--   0 root         (0) root         (0)     2178 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/11n.png
+-rw-r--r--   0 root         (0) root         (0)     1502 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/13d.png
+-rw-r--r--   0 root         (0) root         (0)     1502 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/13n.png
+-rw-r--r--   0 root         (0) root         (0)     1211 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/50d.png
+-rw-r--r--   0 root         (0) root         (0)     1211 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/50n.png
+-rw-r--r--   0 root         (0) root         (0)     1396 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/unknown.png
+-rw-r--r--   0 root         (0) root         (0)      191 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/plex.svg
+-rw-r--r--   0 root         (0) root         (0)     4057 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/smartthings.png
+-rw-r--r--   0 root         (0) root         (0)     4034 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/z-wave.png
+-rw-r--r--   0 root         (0) root         (0)      632 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/icons/zigbee.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.570139 platypush-1.0.4/platypush/backend/http/webapp/dist/img/
+-rw-r--r--   0 root         (0) root         (0)    11833 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/img/dashboard-bg-light.jpg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.573473 platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/
+-rw-r--r--   0 root         (0) root         (0)    12675 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/android-chrome-192x192.png
+-rw-r--r--   0 root         (0) root         (0)    48520 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/android-chrome-512x512.png
+-rw-r--r--   0 root         (0) root         (0)    12675 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/android-chrome-maskable-192x192.png
+-rw-r--r--   0 root         (0) root         (0)    48520 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/android-chrome-maskable-512x512.png
+-rw-r--r--   0 root         (0) root         (0)     7644 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon-120x120.png
+-rw-r--r--   0 root         (0) root         (0)     9796 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon-152x152.png
+-rw-r--r--   0 root         (0) root         (0)    11988 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon-180x180.png
+-rw-r--r--   0 root         (0) root         (0)     3744 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon-60x60.png
+-rw-r--r--   0 root         (0) root         (0)     4786 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon-76x76.png
+-rw-r--r--   0 root         (0) root         (0)    11988 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon.png
+-rw-r--r--   0 root         (0) root         (0)     4675 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/favicon-16x16.png
+-rw-r--r--   0 root         (0) root         (0)     1694 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/favicon-32x32.png
+-rw-r--r--   0 root         (0) root         (0)     4677 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/favicon.svg
+-rw-r--r--   0 root         (0) root         (0)    20814 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/logo-256x256.png
+-rw-r--r--   0 root         (0) root         (0)     9248 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/msapplication-icon-144x144.png
+-rw-r--r--   0 root         (0) root         (0)     9654 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/mstile-150x150.png
+-rw-r--r--   0 root         (0) root         (0)     4675 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/safari-pinned-tab.svg
+-rw-r--r--   0 root         (0) root         (0)    20925 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/img/logo.png
+-rw-r--r--   0 root         (0) root         (0)    32701 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/img/spinner.gif
+-rw-r--r--   0 root         (0) root         (0)     1573 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/index.html
+-rw-r--r--   0 root         (0) root         (0)      551 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/manifest.json
+-rw-r--r--   0 root         (0) root         (0)    43705 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/service-worker.js
+-rw-r--r--   0 root         (0) root         (0)    91952 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/service-worker.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.523471 platypush-1.0.4/platypush/backend/http/webapp/dist/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.590140 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/
+-rw-r--r--   0 root         (0) root         (0)   106570 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/1259.ad51b86e.css
+-rw-r--r--   0 root         (0) root         (0)    29794 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/1391.8fb65128.css
+-rw-r--r--   0 root         (0) root         (0)   149888 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/1449.bf964828.css
+-rw-r--r--   0 root         (0) root         (0)   154136 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/1587.f52aafce.css
+-rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/169.9ec6abc1.css
+-rw-r--r--   0 root         (0) root         (0)    35140 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/1706.c1e22194.css
+-rw-r--r--   0 root         (0) root         (0)   205770 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/1807.333a022f.css
+-rw-r--r--   0 root         (0) root         (0)    30556 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/1949.d8d63590.css
+-rw-r--r--   0 root         (0) root         (0)    53589 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/2140.08e216c1.css
+-rw-r--r--   0 root         (0) root         (0)    30675 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/2154.20cf0934.css
+-rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/2217.da1b8fd6.css
+-rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/2460.83acd505.css
+-rw-r--r--   0 root         (0) root         (0)    31886 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/2461.1fc0b5b4.css
+-rw-r--r--   0 root         (0) root         (0)   371529 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/2509.77a756c6.css
+-rw-r--r--   0 root         (0) root         (0)    31962 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/2844.23273db2.css
+-rw-r--r--   0 root         (0) root         (0)    29745 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/2892.3a7569e7.css
+-rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/2893.21a9931c.css
+-rw-r--r--   0 root         (0) root         (0)    29790 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/2976.bafd7cea.css
+-rw-r--r--   0 root         (0) root         (0)    30412 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/2992.f8bddaf0.css
+-rw-r--r--   0 root         (0) root         (0)    35106 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/3368.467cedc6.css
+-rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/3369.69c504e7.css
+-rw-r--r--   0 root         (0) root         (0)    30629 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/3390.481c441e.css
+-rw-r--r--   0 root         (0) root         (0)   251755 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/3553.6d93b4b8.css
+-rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/3559.5665c422.css
+-rw-r--r--   0 root         (0) root         (0)    30173 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/3661.c12867e9.css
+-rw-r--r--   0 root         (0) root         (0)    30854 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/3671.e6547429.css
+-rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/3826.53d49948.css
+-rw-r--r--   0 root         (0) root         (0)    34817 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/3835.91d8befb.css
+-rw-r--r--   0 root         (0) root         (0)    33195 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/3924.e7e714bc.css
+-rw-r--r--   0 root         (0) root         (0)    34753 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/4221.76c11dc1.css
+-rw-r--r--   0 root         (0) root         (0)    30121 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/446.e0a96773.css
+-rw-r--r--   0 root         (0) root         (0)    31611 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/4589.d7fd389b.css
+-rw-r--r--   0 root         (0) root         (0)    37383 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/472.20f2f41f.css
+-rw-r--r--   0 root         (0) root         (0)    29820 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/4790.3ef3568e.css
+-rw-r--r--   0 root         (0) root         (0)    29745 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/5059.e5cd6fe3.css
+-rw-r--r--   0 root         (0) root         (0)    22679 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/5207.e1e8949a.css
+-rw-r--r--   0 root         (0) root         (0)   182984 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/5285.2250c5c9.css
+-rw-r--r--   0 root         (0) root         (0)    34710 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/5329.2f2c6a0e.css
+-rw-r--r--   0 root         (0) root         (0)    30285 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/5638.05ee3a45.css
+-rw-r--r--   0 root         (0) root         (0)    65509 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/5795.3b193db6.css
+-rw-r--r--   0 root         (0) root         (0)    29749 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/5833.e1e503a2.css
+-rw-r--r--   0 root         (0) root         (0)    34872 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/5906.52ba6beb.css
+-rw-r--r--   0 root         (0) root         (0)    30308 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/5931.e6c8f94d.css
+-rw-r--r--   0 root         (0) root         (0)   161995 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/6062.b6571ed4.css
+-rw-r--r--   0 root         (0) root         (0)    32679 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/6079.f88a21ae.css
+-rw-r--r--   0 root         (0) root         (0)    35248 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/6324.bb3e2171.css
+-rw-r--r--   0 root         (0) root         (0)    26608 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/65.cb15a9a6.css
+-rw-r--r--   0 root         (0) root         (0)    30129 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/6523.d6576265.css
+-rw-r--r--   0 root         (0) root         (0)    49371 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/6561.77bbcd33.css
+-rw-r--r--   0 root         (0) root         (0)    30152 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/6579.04ad63dc.css
+-rw-r--r--   0 root         (0) root         (0)    35642 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/669.73188f7e.css
+-rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/729.16b20067.css
+-rw-r--r--   0 root         (0) root         (0)    29885 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/746.18c59228.css
+-rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/7590.b45a8e92.css
+-rw-r--r--   0 root         (0) root         (0)    32924 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/7651.9b63654f.css
+-rw-r--r--   0 root         (0) root         (0)    32383 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/7841.2a1ced53.css
+-rw-r--r--   0 root         (0) root         (0)    35431 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/7878.e3469993.css
+-rw-r--r--   0 root         (0) root         (0)   181061 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/7880.4f4a202a.css
+-rw-r--r--   0 root         (0) root         (0)    60270 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/7968.29db26b1.css
+-rw-r--r--   0 root         (0) root         (0)    24683 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/8039.e77a760e.css
+-rw-r--r--   0 root         (0) root         (0)    30722 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/8069.111183af.css
+-rw-r--r--   0 root         (0) root         (0)    29809 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/8179.b5fb83f9.css
+-rw-r--r--   0 root         (0) root         (0)    34712 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/8391.b5dd11a9.css
+-rw-r--r--   0 root         (0) root         (0)    35341 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/8498.3676728c.css
+-rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/8621.5db86eb0.css
+-rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/8769.fda642fb.css
+-rw-r--r--   0 root         (0) root         (0)    34655 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/8825.f608e2c2.css
+-rw-r--r--   0 root         (0) root         (0)    34997 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/8989.63c7ae13.css
+-rw-r--r--   0 root         (0) root         (0)    30070 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/906.80f1f8a3.css
+-rw-r--r--   0 root         (0) root         (0)    30034 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/9211.b8dcc633.css
+-rw-r--r--   0 root         (0) root         (0)   189438 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/9381.ade341db.css
+-rw-r--r--   0 root         (0) root         (0)    35171 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/9461.79136fbe.css
+-rw-r--r--   0 root         (0) root         (0)   207104 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/9751.0631f530.css
+-rw-r--r--   0 root         (0) root         (0)    35151 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/980.b4628099.css
+-rw-r--r--   0 root         (0) root         (0)    34712 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/984.0c88349b.css
+-rw-r--r--   0 root         (0) root         (0)    59998 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/9962.eb89f1f6.css
+-rw-r--r--   0 root         (0) root         (0)  1037999 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/app.200dd9cf.css
+-rw-r--r--   0 root         (0) root         (0)    27965 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/chunk-vendors.a2412607.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.593473 platypush-1.0.4/platypush/backend/http/webapp/dist/static/fonts/
+-rw-r--r--   0 root         (0) root         (0)   209128 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/fonts/fa-brands-400.5d18d427.ttf
+-rw-r--r--   0 root         (0) root         (0)   117852 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/fonts/fa-brands-400.87587a68.woff2
+-rw-r--r--   0 root         (0) root         (0)    25392 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/fonts/fa-regular-400.3ccdbd3d.woff2
+-rw-r--r--   0 root         (0) root         (0)    67860 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/fonts/fa-regular-400.81482cd4.ttf
+-rw-r--r--   0 root         (0) root         (0)   156400 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/fonts/fa-solid-900.0b0cc8a6.woff2
+-rw-r--r--   0 root         (0) root         (0)   420332 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/fonts/fa-solid-900.69d3141a.ttf
+-rw-r--r--   0 root         (0) root         (0)   325936 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/fonts/lato-medium-italic.1996cc15.woff
+-rw-r--r--   0 root         (0) root         (0)   194608 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/fonts/lato-medium-italic.1e312dd9.woff2
+-rw-r--r--   0 root         (0) root         (0)   182144 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/fonts/lato-medium.13fcde4c.woff2
+-rw-r--r--   0 root         (0) root         (0)   305920 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/fonts/lato-medium.b41c3821.woff
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.676809 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/
+-rw-r--r--   0 root         (0) root         (0)    32679 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ad.cb33f69a.svg
+-rw-r--r--   0 root         (0) root         (0)    33893 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ad.fa8477e6.svg
+-rw-r--r--   0 root         (0) root         (0)      254 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ae.a3f5e295.svg
+-rw-r--r--   0 root         (0) root         (0)      262 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ae.f06e0095.svg
+-rw-r--r--   0 root         (0) root         (0)    21257 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/af.89591ab0.svg
+-rw-r--r--   0 root         (0) root         (0)    21123 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/af.8ca96393.svg
+-rw-r--r--   0 root         (0) root         (0)      743 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ag.4c37bc2e.svg
+-rw-r--r--   0 root         (0) root         (0)      761 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ag.56074d55.svg
+-rw-r--r--   0 root         (0) root         (0)    47971 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ai.70eefdc0.svg
+-rw-r--r--   0 root         (0) root         (0)    42204 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ai.893d1179.svg
+-rw-r--r--   0 root         (0) root         (0)     3220 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/al.b16acdb2.svg
+-rw-r--r--   0 root         (0) root         (0)     3218 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/al.e0864b5d.svg
+-rw-r--r--   0 root         (0) root         (0)      223 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/am.00f0fec4.svg
+-rw-r--r--   0 root         (0) root         (0)      231 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/am.a566904f.svg
+-rw-r--r--   0 root         (0) root         (0)     1601 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ao.3df23f21.svg
+-rw-r--r--   0 root         (0) root         (0)     1601 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ao.c0c32201.svg
+-rw-r--r--   0 root         (0) root         (0)     3180 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/aq.1b8c45a6.svg
+-rw-r--r--   0 root         (0) root         (0)     2969 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/aq.aa242c4a.svg
+-rw-r--r--   0 root         (0) root         (0)     3500 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ar.22a3116e.svg
+-rw-r--r--   0 root         (0) root         (0)     3427 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ar.d3238270.svg
+-rw-r--r--   0 root         (0) root         (0)     8082 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/as.10ed1a23.svg
+-rw-r--r--   0 root         (0) root         (0)     7838 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/as.4a330654.svg
+-rw-r--r--   0 root         (0) root         (0)      240 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/at.02a64279.svg
+-rw-r--r--   0 root         (0) root         (0)      242 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/at.94cde74c.svg
+-rw-r--r--   0 root         (0) root         (0)     1330 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/au.cc65fc07.svg
+-rw-r--r--   0 root         (0) root         (0)     1317 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/au.dbcdef2c.svg
+-rw-r--r--   0 root         (0) root         (0)     9945 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/aw.abbad4ac.svg
+-rw-r--r--   0 root         (0) root         (0)    12084 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/aw.be4540eb.svg
+-rw-r--r--   0 root         (0) root         (0)      541 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ax.371c7af2.svg
+-rw-r--r--   0 root         (0) root         (0)      553 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ax.91eea523.svg
+-rw-r--r--   0 root         (0) root         (0)      512 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/az.0e2f1d1a.svg
+-rw-r--r--   0 root         (0) root         (0)      498 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/az.f399f1c8.svg
+-rw-r--r--   0 root         (0) root         (0)     1304 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ba.032070d4.svg
+-rw-r--r--   0 root         (0) root         (0)     1242 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ba.e167b08f.svg
+-rw-r--r--   0 root         (0) root         (0)      610 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bb.23a15e67.svg
+-rw-r--r--   0 root         (0) root         (0)      613 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bb.b800513b.svg
+-rw-r--r--   0 root         (0) root         (0)      192 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bd.c1abcb00.svg
+-rw-r--r--   0 root         (0) root         (0)      190 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bd.c4a5f0e2.svg
+-rw-r--r--   0 root         (0) root         (0)      290 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/be.29774a37.svg
+-rw-r--r--   0 root         (0) root         (0)      290 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/be.3eb14701.svg
+-rw-r--r--   0 root         (0) root         (0)      383 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bf.2334e919.svg
+-rw-r--r--   0 root         (0) root         (0)      357 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bf.4ffd5dc6.svg
+-rw-r--r--   0 root         (0) root         (0)      286 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bg.700f100c.svg
+-rw-r--r--   0 root         (0) root         (0)      294 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bg.d0a49130.svg
+-rw-r--r--   0 root         (0) root         (0)      543 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bh.2a884f6c.svg
+-rw-r--r--   0 root         (0) root         (0)      569 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bh.3968dfe0.svg
+-rw-r--r--   0 root         (0) root         (0)     1045 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bi.211d0f9e.svg
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bi.ae3bb248.svg
+-rw-r--r--   0 root         (0) root         (0)      499 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bj.2cdc8a62.svg
+-rw-r--r--   0 root         (0) root         (0)      496 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bj.aba95ad2.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bl.04966866.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bl.3e69e968.svg
+-rw-r--r--   0 root         (0) root         (0)    22617 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bm.e6903c8e.svg
+-rw-r--r--   0 root         (0) root         (0)    22304 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bm.e69e40c4.svg
+-rw-r--r--   0 root         (0) root         (0)    14506 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bn.07911e0c.svg
+-rw-r--r--   0 root         (0) root         (0)    14367 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bn.4d91734a.svg
+-rw-r--r--   0 root         (0) root         (0)   117922 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bo.03595499.svg
+-rw-r--r--   0 root         (0) root         (0)   119582 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bo.9c1d9ef8.svg
+-rw-r--r--   0 root         (0) root         (0)      224 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bq.747d8177.svg
+-rw-r--r--   0 root         (0) root         (0)      228 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bq.b9355bec.svg
+-rw-r--r--   0 root         (0) root         (0)     7816 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/br.058a5086.svg
+-rw-r--r--   0 root         (0) root         (0)     8231 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/br.fe030c1c.svg
+-rw-r--r--   0 root         (0) root         (0)      568 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bs.d228cbb2.svg
+-rw-r--r--   0 root         (0) root         (0)      546 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bs.ef0a29ed.svg
+-rw-r--r--   0 root         (0) root         (0)    25138 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bt.3f8ecb9b.svg
+-rw-r--r--   0 root         (0) root         (0)    25318 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bt.fc241981.svg
+-rw-r--r--   0 root         (0) root         (0)      582 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bv.5503f03a.svg
+-rw-r--r--   0 root         (0) root         (0)      579 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bv.7f7cd26f.svg
+-rw-r--r--   0 root         (0) root         (0)      254 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bw.494aae64.svg
+-rw-r--r--   0 root         (0) root         (0)      252 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bw.b767df8c.svg
+-rw-r--r--   0 root         (0) root         (0)     6086 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/by.78d2c3c9.svg
+-rw-r--r--   0 root         (0) root         (0)     5956 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/by.fba98c48.svg
+-rw-r--r--   0 root         (0) root         (0)    47095 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bz.14c3376a.svg
+-rw-r--r--   0 root         (0) root         (0)    46832 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bz.5e0ef548.svg
+-rw-r--r--   0 root         (0) root         (0)      705 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ca.163ac200.svg
+-rw-r--r--   0 root         (0) root         (0)      725 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ca.a2ab234d.svg
+-rw-r--r--   0 root         (0) root         (0)     3089 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cc.51960f85.svg
+-rw-r--r--   0 root         (0) root         (0)     3135 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cc.813adff8.svg
+-rw-r--r--   0 root         (0) root         (0)      349 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cd.39186ec2.svg
+-rw-r--r--   0 root         (0) root         (0)      507 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cd.b4bd46ee.svg
+-rw-r--r--   0 root         (0) root         (0)      685 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cf.b5702729.svg
+-rw-r--r--   0 root         (0) root         (0)      632 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cf.fe1120e9.svg
+-rw-r--r--   0 root         (0) root         (0)      469 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cg.00603842.svg
+-rw-r--r--   0 root         (0) root         (0)      481 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cg.12414c99.svg
+-rw-r--r--   0 root         (0) root         (0)      295 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ch.7376c9c3.svg
+-rw-r--r--   0 root         (0) root         (0)      297 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ch.a558d859.svg
+-rw-r--r--   0 root         (0) root         (0)      280 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ci.1251a8e3.svg
+-rw-r--r--   0 root         (0) root         (0)      283 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ci.425a24c2.svg
+-rw-r--r--   0 root         (0) root         (0)     1843 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ck.4e83dd3e.svg
+-rw-r--r--   0 root         (0) root         (0)     1884 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ck.6303aa5b.svg
+-rw-r--r--   0 root         (0) root         (0)      574 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cl.0917a91e.svg
+-rw-r--r--   0 root         (0) root         (0)      557 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cl.b5974a35.svg
+-rw-r--r--   0 root         (0) root         (0)      824 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cm.253adb39.svg
+-rw-r--r--   0 root         (0) root         (0)      824 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cm.853e2843.svg
+-rw-r--r--   0 root         (0) root         (0)      743 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cn.38f63e1e.svg
+-rw-r--r--   0 root         (0) root         (0)      801 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cn.e1b166eb.svg
+-rw-r--r--   0 root         (0) root         (0)      289 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/co.33e249d8.svg
+-rw-r--r--   0 root         (0) root         (0)      289 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/co.b5cbc817.svg
+-rw-r--r--   0 root         (0) root         (0)      293 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cr.2e572846.svg
+-rw-r--r--   0 root         (0) root         (0)      293 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cr.336eb7d3.svg
+-rw-r--r--   0 root         (0) root         (0)      573 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cu.c2a6f0ed.svg
+-rw-r--r--   0 root         (0) root         (0)      616 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cu.d6e33f19.svg
+-rw-r--r--   0 root         (0) root         (0)     1409 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cv.5ea64968.svg
+-rw-r--r--   0 root         (0) root         (0)     1357 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cv.b3ab83f5.svg
+-rw-r--r--   0 root         (0) root         (0)      675 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cw.0e14b0b7.svg
+-rw-r--r--   0 root         (0) root         (0)      682 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cw.9b9b7ed5.svg
+-rw-r--r--   0 root         (0) root         (0)     2505 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cx.da5de6d2.svg
+-rw-r--r--   0 root         (0) root         (0)     2466 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cx.e04e07e8.svg
+-rw-r--r--   0 root         (0) root         (0)     6024 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cy.834e6240.svg
+-rw-r--r--   0 root         (0) root         (0)     5930 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cy.bfcfd736.svg
+-rw-r--r--   0 root         (0) root         (0)      480 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cz.aa114964.svg
+-rw-r--r--   0 root         (0) root         (0)      478 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cz.b5f98a6b.svg
+-rw-r--r--   0 root         (0) root         (0)    11833 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/dashboard-bg-light.06da6eab.jpg
+-rw-r--r--   0 root         (0) root         (0)      213 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/de.8e159e6e.svg
+-rw-r--r--   0 root         (0) root         (0)      221 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/de.b827ac51.svg
+-rw-r--r--   0 root         (0) root         (0)      585 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/dj.4197a18a.svg
+-rw-r--r--   0 root         (0) root         (0)      585 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/dj.925748d5.svg
+-rw-r--r--   0 root         (0) root         (0)      239 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/dk.3ca1caed.svg
+-rw-r--r--   0 root         (0) root         (0)      235 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/dk.a867eeef.svg
+-rw-r--r--   0 root         (0) root         (0)    16480 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/dm.7ddb00ac.svg
+-rw-r--r--   0 root         (0) root         (0)    15992 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/dm.bca6d70c.svg
+-rw-r--r--   0 root         (0) root         (0)   391693 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/do.81097daa.svg
+-rw-r--r--   0 root         (0) root         (0)   394127 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/do.954f0f3e.svg
+-rw-r--r--   0 root         (0) root         (0)      309 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/dz.76d47b01.svg
+-rw-r--r--   0 root         (0) root         (0)      298 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/dz.b7e2fbce.svg
+-rw-r--r--   0 root         (0) root         (0)    29916 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ec.0029f514.svg
+-rw-r--r--   0 root         (0) root         (0)    29359 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ec.5f387e2f.svg
+-rw-r--r--   0 root         (0) root         (0)      321 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ee.1b4839e0.svg
+-rw-r--r--   0 root         (0) root         (0)      352 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ee.828384a8.svg
+-rw-r--r--   0 root         (0) root         (0)     9964 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/eg.38443fa6.svg
+-rw-r--r--   0 root         (0) root         (0)     9978 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/eg.5756a758.svg
+-rw-r--r--   0 root         (0) root         (0)      823 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/eh.82bd1c7b.svg
+-rw-r--r--   0 root         (0) root         (0)      873 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/eh.f8d7b64f.svg
+-rw-r--r--   0 root         (0) root         (0)     3202 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/er.bf5b134b.svg
+-rw-r--r--   0 root         (0) root         (0)     3388 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/er.e932abe1.svg
+-rw-r--r--   0 root         (0) root         (0)      258 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/es-ct.64a68954.svg
+-rw-r--r--   0 root         (0) root         (0)      257 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/es-ct.69469f50.svg
+-rw-r--r--   0 root         (0) root         (0)    93922 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/es.7dd46df0.svg
+-rw-r--r--   0 root         (0) root         (0)    92061 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/es.de5915e5.svg
+-rw-r--r--   0 root         (0) root         (0)     1239 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/et.82e8eb21.svg
+-rw-r--r--   0 root         (0) root         (0)     1240 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/et.a998a1b2.svg
+-rw-r--r--   0 root         (0) root         (0)     1249 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/eu.4c6e130f.svg
+-rw-r--r--   0 root         (0) root         (0)     1250 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/eu.aba724b1.svg
+-rw-r--r--   0 root         (0) root         (0)      240 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/fi.0cd85b78.svg
+-rw-r--r--   0 root         (0) root         (0)      237 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/fi.3be6b378.svg
+-rw-r--r--   0 root         (0) root         (0)    27208 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/fj.ac9c916f.svg
+-rw-r--r--   0 root         (0) root         (0)    27355 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/fj.e8d3e00b.svg
+-rw-r--r--   0 root         (0) root         (0)    30431 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/fk.af0350f8.svg
+-rw-r--r--   0 root         (0) root         (0)    30626 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/fk.db55fa14.svg
+-rw-r--r--   0 root         (0) root         (0)      759 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/fm.3491efc7.svg
+-rw-r--r--   0 root         (0) root         (0)      770 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/fm.78d44caa.svg
+-rw-r--r--   0 root         (0) root         (0)      534 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/fo.1da81e3a.svg
+-rw-r--r--   0 root         (0) root         (0)      564 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/fo.72949ad1.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/fr.3565b8f4.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/fr.9cb70285.svg
+-rw-r--r--   0 root         (0) root         (0)      278 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ga.3e474381.svg
+-rw-r--r--   0 root         (0) root         (0)      274 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ga.59f7d865.svg
+-rw-r--r--   0 root         (0) root         (0)      232 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gb-eng.0fac6e79.svg
+-rw-r--r--   0 root         (0) root         (0)      242 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gb-eng.513dcf1b.svg
+-rw-r--r--   0 root         (0) root         (0)    26859 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gb-nir.2b7d2c3a.svg
+-rw-r--r--   0 root         (0) root         (0)    25348 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gb-nir.f59817d6.svg
+-rw-r--r--   0 root         (0) root         (0)      239 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gb-sct.f5001e5d.svg
+-rw-r--r--   0 root         (0) root         (0)      231 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gb-sct.fee55173.svg
+-rw-r--r--   0 root         (0) root         (0)     9183 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gb-wls.13481560.svg
+-rw-r--r--   0 root         (0) root         (0)     9076 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gb-wls.95b2cfab.svg
+-rw-r--r--   0 root         (0) root         (0)      795 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gb.2aafb374.svg
+-rw-r--r--   0 root         (0) root         (0)      837 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gb.7a456bb2.svg
+-rw-r--r--   0 root         (0) root         (0)     1831 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gd.04ea09b7.svg
+-rw-r--r--   0 root         (0) root         (0)     1687 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gd.60b96978.svg
+-rw-r--r--   0 root         (0) root         (0)     1397 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ge.b7b65b55.svg
+-rw-r--r--   0 root         (0) root         (0)     1541 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ge.c7190912.svg
+-rw-r--r--   0 root         (0) root         (0)      261 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gf.531f9e07.svg
+-rw-r--r--   0 root         (0) root         (0)      258 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gf.90f438a3.svg
+-rw-r--r--   0 root         (0) root         (0)      595 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gg.3aebc3ce.svg
+-rw-r--r--   0 root         (0) root         (0)      625 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gg.65174039.svg
+-rw-r--r--   0 root         (0) root         (0)      296 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gh.af443995.svg
+-rw-r--r--   0 root         (0) root         (0)      281 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gh.f2b6baac.svg
+-rw-r--r--   0 root         (0) root         (0)     2949 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gi.302c2506.svg
+-rw-r--r--   0 root         (0) root         (0)     2957 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gi.7beea6ed.svg
+-rw-r--r--   0 root         (0) root         (0)      226 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gl.551d0783.svg
+-rw-r--r--   0 root         (0) root         (0)      240 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gl.6a5c17b0.svg
+-rw-r--r--   0 root         (0) root         (0)      540 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gm.0e00e9d4.svg
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gm.1724dc37.svg
+-rw-r--r--   0 root         (0) root         (0)      295 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gn.54a75b28.svg
+-rw-r--r--   0 root         (0) root         (0)      295 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gn.7c96520b.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gp.4327060f.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gp.f8adbf5c.svg
+-rw-r--r--   0 root         (0) root         (0)     5277 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gq.b1679302.svg
+-rw-r--r--   0 root         (0) root         (0)     5185 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gq.bd7daf33.svg
+-rw-r--r--   0 root         (0) root         (0)      815 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gr.07bedadf.svg
+-rw-r--r--   0 root         (0) root         (0)      872 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gr.25dd3287.svg
+-rw-r--r--   0 root         (0) root         (0)    35105 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gs.60368968.svg
+-rw-r--r--   0 root         (0) root         (0)    34612 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gs.b2836676.svg
+-rw-r--r--   0 root         (0) root         (0)    37811 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gt.1a24ed67.svg
+-rw-r--r--   0 root         (0) root         (0)    37811 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gt.825f7286.svg
+-rw-r--r--   0 root         (0) root         (0)     4630 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gu.05f0ab85.svg
+-rw-r--r--   0 root         (0) root         (0)     4854 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gu.19b114eb.svg
+-rw-r--r--   0 root         (0) root         (0)      889 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gw.bcd1eddb.svg
+-rw-r--r--   0 root         (0) root         (0)      813 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gw.c97f3f94.svg
+-rw-r--r--   0 root         (0) root         (0)      481 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gy.6327f72a.svg
+-rw-r--r--   0 root         (0) root         (0)      488 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gy.e11d0234.svg
+-rw-r--r--   0 root         (0) root         (0)     3554 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/hk.b199a9ee.svg
+-rw-r--r--   0 root         (0) root         (0)     3503 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/hk.c72bba0e.svg
+-rw-r--r--   0 root         (0) root         (0)     1308 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/hm.4aa61657.svg
+-rw-r--r--   0 root         (0) root         (0)     1324 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/hm.d4b3d393.svg
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/hn.08ad78b2.svg
+-rw-r--r--   0 root         (0) root         (0)     1116 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/hn.44cee191.svg
+-rw-r--r--   0 root         (0) root         (0)    41785 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/hr.078b1bf9.svg
+-rw-r--r--   0 root         (0) root         (0)    41588 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/hr.1f4e28b8.svg
+-rw-r--r--   0 root         (0) root         (0)    15301 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ht.6943447c.svg
+-rw-r--r--   0 root         (0) root         (0)    15215 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ht.7ca68737.svg
+-rw-r--r--   0 root         (0) root         (0)      274 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/hu.692e97ca.svg
+-rw-r--r--   0 root         (0) root         (0)      276 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/hu.b10d3f8e.svg
+-rw-r--r--   0 root         (0) root         (0)      239 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/id.94464e47.svg
+-rw-r--r--   0 root         (0) root         (0)      237 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/id.a05dc04c.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ie.5154112a.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ie.e23b25d1.svg
+-rw-r--r--   0 root         (0) root         (0)      848 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/il.150f4c5f.svg
+-rw-r--r--   0 root         (0) root         (0)      895 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/il.e02a66d3.svg
+-rw-r--r--   0 root         (0) root         (0)    10253 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/im.25166c91.svg
+-rw-r--r--   0 root         (0) root         (0)     9925 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/im.942419c5.svg
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/in.954929a0.svg
+-rw-r--r--   0 root         (0) root         (0)     1088 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/in.bd0d4f19.svg
+-rw-r--r--   0 root         (0) root         (0)    27443 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/io.a59923ab.svg
+-rw-r--r--   0 root         (0) root         (0)    27465 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/io.fa003484.svg
+-rw-r--r--   0 root         (0) root         (0)     1476 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/iq.1232a5c2.svg
+-rw-r--r--   0 root         (0) root         (0)     1481 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/iq.9a48d678.svg
+-rw-r--r--   0 root         (0) root         (0)    15448 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ir.1ed24953.svg
+-rw-r--r--   0 root         (0) root         (0)    15360 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ir.bc7ae9e1.svg
+-rw-r--r--   0 root         (0) root         (0)      518 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/is.cad57f19.svg
+-rw-r--r--   0 root         (0) root         (0)      526 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/is.eea59326.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/it.039b4527.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/it.e8516fc7.svg
+-rw-r--r--   0 root         (0) root         (0)     4699 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/je.1684dacc.svg
+-rw-r--r--   0 root         (0) root         (0)     4718 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/je.3ed72a25.svg
+-rw-r--r--   0 root         (0) root         (0)     1120 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/jellyfin.7b53a541.svg
+-rw-r--r--   0 root         (0) root         (0)      389 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/jm.2357530e.svg
+-rw-r--r--   0 root         (0) root         (0)      389 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/jm.479f30fe.svg
+-rw-r--r--   0 root         (0) root         (0)      691 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/jo.06fbaa2c.svg
+-rw-r--r--   0 root         (0) root         (0)      714 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/jo.7ac45a65.svg
+-rw-r--r--   0 root         (0) root         (0)      497 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/jp.1795778c.svg
+-rw-r--r--   0 root         (0) root         (0)      481 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/jp.b6063838.svg
+-rw-r--r--   0 root         (0) root         (0)     1380 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ke.6dbfffd5.svg
+-rw-r--r--   0 root         (0) root         (0)     1492 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ke.769bb975.svg
+-rw-r--r--   0 root         (0) root         (0)     3334 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kg.96c12490.svg
+-rw-r--r--   0 root         (0) root         (0)     3383 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kg.daded53c.svg
+-rw-r--r--   0 root         (0) root         (0)     7282 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kh.8eeb1634.svg
+-rw-r--r--   0 root         (0) root         (0)     7283 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kh.b10339d6.svg
+-rw-r--r--   0 root         (0) root         (0)     5950 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ki.033ff9ce.svg
+-rw-r--r--   0 root         (0) root         (0)     5815 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ki.89e43a21.svg
+-rw-r--r--   0 root         (0) root         (0)     1058 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/km.1e3bd5fe.svg
+-rw-r--r--   0 root         (0) root         (0)     1041 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/km.3ffb0228.svg
+-rw-r--r--   0 root         (0) root         (0)      813 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kn.0c16fe68.svg
+-rw-r--r--   0 root         (0) root         (0)      817 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kn.8f2e7b29.svg
+-rw-r--r--   0 root         (0) root         (0)     1370 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kodi.d18f8d23.svg
+-rw-r--r--   0 root         (0) root         (0)      789 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kp.0f5253d8.svg
+-rw-r--r--   0 root         (0) root         (0)      852 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kp.f4ff9e76.svg
+-rw-r--r--   0 root         (0) root         (0)     1725 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kr.0dc8b972.svg
+-rw-r--r--   0 root         (0) root         (0)     1819 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kr.0f5e1116.svg
+-rw-r--r--   0 root         (0) root         (0)      503 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kw.3b4f3ea3.svg
+-rw-r--r--   0 root         (0) root         (0)      507 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kw.830d3755.svg
+-rw-r--r--   0 root         (0) root         (0)    22455 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ky.be81d90b.svg
+-rw-r--r--   0 root         (0) root         (0)    21834 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ky.e3b76b32.svg
+-rw-r--r--   0 root         (0) root         (0)    11422 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kz.32ac1036.svg
+-rw-r--r--   0 root         (0) root         (0)    11334 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kz.579ac0f9.svg
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/la.e583f8ec.svg
+-rw-r--r--   0 root         (0) root         (0)      504 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/la.f71017ef.svg
+-rw-r--r--   0 root         (0) root         (0)     2750 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/lb.8eea508a.svg
+-rw-r--r--   0 root         (0) root         (0)     2811 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/lb.bdbeb8f1.svg
+-rw-r--r--   0 root         (0) root         (0)      370 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/lc.25f644a6.svg
+-rw-r--r--   0 root         (0) root         (0)      370 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/lc.68bd77ae.svg
+-rw-r--r--   0 root         (0) root         (0)     8318 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/li.8dc1ed79.svg
+-rw-r--r--   0 root         (0) root         (0)     8341 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/li.d7e2a871.svg
+-rw-r--r--   0 root         (0) root         (0)    11326 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/lk.42c41c61.svg
+-rw-r--r--   0 root         (0) root         (0)    11338 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/lk.e52240d6.svg
+-rw-r--r--   0 root         (0) root         (0)      721 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/lr.5b84ff00.svg
+-rw-r--r--   0 root         (0) root         (0)      694 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/lr.9a67cd3d.svg
+-rw-r--r--   0 root         (0) root         (0)     1219 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ls.6d444cae.svg
+-rw-r--r--   0 root         (0) root         (0)     1242 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ls.fe1da403.svg
+-rw-r--r--   0 root         (0) root         (0)      442 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/lt.03a2e8c1.svg
+-rw-r--r--   0 root         (0) root         (0)      442 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/lt.b57ea2a8.svg
+-rw-r--r--   0 root         (0) root         (0)      228 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/lu.93878a1b.svg
+-rw-r--r--   0 root         (0) root         (0)      232 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/lu.e3bdc6d3.svg
+-rw-r--r--   0 root         (0) root         (0)      237 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/lv.1853e3a0.svg
+-rw-r--r--   0 root         (0) root         (0)      233 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/lv.679c099e.svg
+-rw-r--r--   0 root         (0) root         (0)      531 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ly.05f8732e.svg
+-rw-r--r--   0 root         (0) root         (0)      530 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ly.b9e750ff.svg
+-rw-r--r--   0 root         (0) root         (0)      250 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ma.65053fc4.svg
+-rw-r--r--   0 root         (0) root         (0)      250 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ma.88ada30c.svg
+-rw-r--r--   0 root         (0) root         (0)      237 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mc.2c03ea5c.svg
+-rw-r--r--   0 root         (0) root         (0)      237 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mc.89b532e8.svg
+-rw-r--r--   0 root         (0) root         (0)    11264 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/md.646818c3.svg
+-rw-r--r--   0 root         (0) root         (0)    11368 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/md.a56562ee.svg
+-rw-r--r--   0 root         (0) root         (0)    63990 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/me.2e71b778.svg
+-rw-r--r--   0 root         (0) root         (0)    62977 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/me.f05548f2.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mf.70d09a4a.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mf.7da6b3d2.svg
+-rw-r--r--   0 root         (0) root         (0)      302 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mg.09ca17b2.svg
+-rw-r--r--   0 root         (0) root         (0)      302 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mg.b3fff4a6.svg
+-rw-r--r--   0 root         (0) root         (0)      741 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mh.3fd69bb2.svg
+-rw-r--r--   0 root         (0) root         (0)      763 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mh.f6cbc774.svg
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mk.4234a248.svg
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mk.e5412079.svg
+-rw-r--r--   0 root         (0) root         (0)      279 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ml.3fad079e.svg
+-rw-r--r--   0 root         (0) root         (0)      276 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ml.4f0dba9e.svg
+-rw-r--r--   0 root         (0) root         (0)      865 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mm.8ac1f094.svg
+-rw-r--r--   0 root         (0) root         (0)      848 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mm.adaa2111.svg
+-rw-r--r--   0 root         (0) root         (0)     1253 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mn.78547af0.svg
+-rw-r--r--   0 root         (0) root         (0)     1259 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mn.a4bcb0e6.svg
+-rw-r--r--   0 root         (0) root         (0)     1547 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mo.2f0d2c15.svg
+-rw-r--r--   0 root         (0) root         (0)     1511 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mo.c8198565.svg
+-rw-r--r--   0 root         (0) root         (0)    23656 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mp.2acb5506.svg
+-rw-r--r--   0 root         (0) root         (0)    23415 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mp.eeeefff6.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mq.145a7657.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mq.bb36a8fc.svg
+-rw-r--r--   0 root         (0) root         (0)      447 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mr.dd34eae8.svg
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mr.e91e06ea.svg
+-rw-r--r--   0 root         (0) root         (0)     6785 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ms.2025cd7d.svg
+-rw-r--r--   0 root         (0) root         (0)     6693 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ms.b13001dc.svg
+-rw-r--r--   0 root         (0) root         (0)    10513 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mt.b6f71c85.svg
+-rw-r--r--   0 root         (0) root         (0)     8803 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mt.cff39ee0.svg
+-rw-r--r--   0 root         (0) root         (0)      319 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mu.51f71163.svg
+-rw-r--r--   0 root         (0) root         (0)      319 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mu.a926c232.svg
+-rw-r--r--   0 root         (0) root         (0)      307 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mv.2c8b92b5.svg
+-rw-r--r--   0 root         (0) root         (0)      289 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mv.ba4de4fd.svg
+-rw-r--r--   0 root         (0) root         (0)     3708 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mw.0b005148.svg
+-rw-r--r--   0 root         (0) root         (0)     3891 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mw.f704f4bb.svg
+-rw-r--r--   0 root         (0) root         (0)    95527 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mx.1b615ec2.svg
+-rw-r--r--   0 root         (0) root         (0)    91037 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mx.8a36b075.svg
+-rw-r--r--   0 root         (0) root         (0)     1279 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/my.4109ae71.svg
+-rw-r--r--   0 root         (0) root         (0)     1271 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/my.69c87fc5.svg
+-rw-r--r--   0 root         (0) root         (0)     2618 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mz.1377650b.svg
+-rw-r--r--   0 root         (0) root         (0)     2601 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mz.2c96acb1.svg
+-rw-r--r--   0 root         (0) root         (0)      980 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/na.7adf4344.svg
+-rw-r--r--   0 root         (0) root         (0)     1002 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/na.e0503926.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/nc.96fa6a4b.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/nc.b5a5d41b.svg
+-rw-r--r--   0 root         (0) root         (0)      276 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ne.d11b82c6.svg
+-rw-r--r--   0 root         (0) root         (0)      282 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ne.d4fe4faa.svg
+-rw-r--r--   0 root         (0) root         (0)     5595 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/nf.1e8c700b.svg
+-rw-r--r--   0 root         (0) root         (0)     5842 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/nf.a7166b00.svg
+-rw-r--r--   0 root         (0) root         (0)      260 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ng.51059407.svg
+-rw-r--r--   0 root         (0) root         (0)      260 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ng.c3b42ad2.svg
+-rw-r--r--   0 root         (0) root         (0)    18572 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ni.5b80bac0.svg
+-rw-r--r--   0 root         (0) root         (0)    18632 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ni.cc7eb514.svg
+-rw-r--r--   0 root         (0) root         (0)      239 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/nl.dd138444.svg
+-rw-r--r--   0 root         (0) root         (0)      245 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/nl.e415f0e7.svg
+-rw-r--r--   0 root         (0) root         (0)      321 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/no.26996afa.svg
+-rw-r--r--   0 root         (0) root         (0)      321 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/no.70157234.svg
+-rw-r--r--   0 root         (0) root         (0)     1058 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/np.954177a0.svg
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/np.f7b8a5c3.svg
+-rw-r--r--   0 root         (0) root         (0)      645 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/nr.2c66d218.svg
+-rw-r--r--   0 root         (0) root         (0)      668 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/nr.a4f0e762.svg
+-rw-r--r--   0 root         (0) root         (0)     1742 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/nu.26551dc2.svg
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/nu.860bbe8a.svg
+-rw-r--r--   0 root         (0) root         (0)     2974 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/nz.38d0d690.svg
+-rw-r--r--   0 root         (0) root         (0)     2999 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/nz.c77ae58d.svg
+-rw-r--r--   0 root         (0) root         (0)    22825 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/om.3f5691ca.svg
+-rw-r--r--   0 root         (0) root         (0)    22841 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/om.ff034f9e.svg
+-rw-r--r--   0 root         (0) root         (0)      743 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pa.6dc8212a.svg
+-rw-r--r--   0 root         (0) root         (0)      659 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pa.acde3214.svg
+-rw-r--r--   0 root         (0) root         (0)    74209 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pe.5a3b0bc5.svg
+-rw-r--r--   0 root         (0) root         (0)    73524 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pe.5c2ced95.svg
+-rw-r--r--   0 root         (0) root         (0)     4288 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pf.9f06082b.svg
+-rw-r--r--   0 root         (0) root         (0)     4230 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pf.f6ae1bc8.svg
+-rw-r--r--   0 root         (0) root         (0)     1667 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pg.26847b33.svg
+-rw-r--r--   0 root         (0) root         (0)     2099 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pg.66c8dc3b.svg
+-rw-r--r--   0 root         (0) root         (0)     1578 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ph.12e2b123.svg
+-rw-r--r--   0 root         (0) root         (0)     1522 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ph.f215833e.svg
+-rw-r--r--   0 root         (0) root         (0)      740 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pk.0bbf58be.svg
+-rw-r--r--   0 root         (0) root         (0)      691 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pk.32b55f6f.svg
+-rw-r--r--   0 root         (0) root         (0)      222 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pl.03886843.svg
+-rw-r--r--   0 root         (0) root         (0)      222 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pl.a1350f0c.svg
+-rw-r--r--   0 root         (0) root         (0)      191 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/plex.7a4e22a6.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pm.7a6beab5.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pm.a5590fa3.svg
+-rw-r--r--   0 root         (0) root         (0)     8592 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pn.00a9342b.svg
+-rw-r--r--   0 root         (0) root         (0)    10939 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pn.715fd11d.svg
+-rw-r--r--   0 root         (0) root         (0)      619 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pr.391a48e2.svg
+-rw-r--r--   0 root         (0) root         (0)      631 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pr.b37cbdc4.svg
+-rw-r--r--   0 root         (0) root         (0)      541 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ps.1af72ed4.svg
+-rw-r--r--   0 root         (0) root         (0)      555 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ps.96bcac74.svg
+-rw-r--r--   0 root         (0) root         (0)     8748 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pt.0703cc3a.svg
+-rw-r--r--   0 root         (0) root         (0)     8369 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pt.351b87cb.svg
+-rw-r--r--   0 root         (0) root         (0)      464 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pw.17220ffb.svg
+-rw-r--r--   0 root         (0) root         (0)      509 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pw.6d8e7ce0.svg
+-rw-r--r--   0 root         (0) root         (0)    17460 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/py.25cc39e3.svg
+-rw-r--r--   0 root         (0) root         (0)    17301 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/py.c20318c9.svg
+-rw-r--r--   0 root         (0) root         (0)      356 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/qa.7e695788.svg
+-rw-r--r--   0 root         (0) root         (0)      359 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/qa.86452d7a.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/re.b8140129.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/re.cf143c2f.svg
+-rw-r--r--   0 root         (0) root         (0)      305 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ro.67f8501e.svg
+-rw-r--r--   0 root         (0) root         (0)      305 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ro.cab93784.svg
+-rw-r--r--   0 root         (0) root         (0)   187637 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/rs.23638d75.svg
+-rw-r--r--   0 root         (0) root         (0)   187500 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/rs.ae2e3422.svg
+-rw-r--r--   0 root         (0) root         (0)      290 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ru.ccd50623.svg
+-rw-r--r--   0 root         (0) root         (0)      286 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ru.edd8b008.svg
+-rw-r--r--   0 root         (0) root         (0)      748 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/rw.87d5d899.svg
+-rw-r--r--   0 root         (0) root         (0)      747 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/rw.d118aacd.svg
+-rw-r--r--   0 root         (0) root         (0)    10225 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sa.5bfbe72b.svg
+-rw-r--r--   0 root         (0) root         (0)    10290 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sa.f0a8997b.svg
+-rw-r--r--   0 root         (0) root         (0)      947 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sb.1c406073.svg
+-rw-r--r--   0 root         (0) root         (0)      952 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sb.b0db5b0a.svg
+-rw-r--r--   0 root         (0) root         (0)      570 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sc.0452f14c.svg
+-rw-r--r--   0 root         (0) root         (0)      565 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sc.cdc20672.svg
+-rw-r--r--   0 root         (0) root         (0)      491 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sd.0e619868.svg
+-rw-r--r--   0 root         (0) root         (0)      493 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sd.da3b68ee.svg
+-rw-r--r--   0 root         (0) root         (0)      685 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/se.7e499d82.svg
+-rw-r--r--   0 root         (0) root         (0)      698 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/se.7ec71700.svg
+-rw-r--r--   0 root         (0) root         (0)      951 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sg.4f0e8eff.svg
+-rw-r--r--   0 root         (0) root         (0)      886 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sg.8a63b009.svg
+-rw-r--r--   0 root         (0) root         (0)    29664 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sh.46e2588d.svg
+-rw-r--r--   0 root         (0) root         (0)    30261 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sh.681f8fff.svg
+-rw-r--r--   0 root         (0) root         (0)     2049 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/si.2a428364.svg
+-rw-r--r--   0 root         (0) root         (0)     2065 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/si.d9d425c0.svg
+-rw-r--r--   0 root         (0) root         (0)      321 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sj.638e6522.svg
+-rw-r--r--   0 root         (0) root         (0)      321 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sj.92c583b8.svg
+-rw-r--r--   0 root         (0) root         (0)     1203 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sk.7998d1f5.svg
+-rw-r--r--   0 root         (0) root         (0)     1178 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sk.93c91c0b.svg
+-rw-r--r--   0 root         (0) root         (0)      275 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sl.d8378c47.svg
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sl.eb9dda3f.svg
+-rw-r--r--   0 root         (0) root         (0)    15876 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sm.0ba901f4.svg
+-rw-r--r--   0 root         (0) root         (0)    15947 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sm.5e2fc188.svg
+-rw-r--r--   0 root         (0) root         (0)      424 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sn.4247b831.svg
+-rw-r--r--   0 root         (0) root         (0)      414 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sn.98923b55.svg
+-rw-r--r--   0 root         (0) root         (0)      491 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/so.2d18a203.svg
+-rw-r--r--   0 root         (0) root         (0)      498 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/so.45f08b28.svg
+-rw-r--r--   0 root         (0) root         (0)      315 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sr.cb178d98.svg
+-rw-r--r--   0 root         (0) root         (0)      320 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sr.d66c1240.svg
+-rw-r--r--   0 root         (0) root         (0)      386 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ss.caedfdf2.svg
+-rw-r--r--   0 root         (0) root         (0)      397 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ss.db181f81.svg
+-rw-r--r--   0 root         (0) root         (0)      920 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/st.a70042c6.svg
+-rw-r--r--   0 root         (0) root         (0)      916 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/st.ecc4827f.svg
+-rw-r--r--   0 root         (0) root         (0)    84167 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sv.9501935a.svg
+-rw-r--r--   0 root         (0) root         (0)    83639 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sv.f67839a6.svg
+-rw-r--r--   0 root         (0) root         (0)    13097 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sx.77e864f0.svg
+-rw-r--r--   0 root         (0) root         (0)    13294 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sx.c0e6297a.svg
+-rw-r--r--   0 root         (0) root         (0)      565 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sy.2b3eac89.svg
+-rw-r--r--   0 root         (0) root         (0)      579 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sy.7fe894df.svg
+-rw-r--r--   0 root         (0) root         (0)     6747 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sz.70b6fc50.svg
+-rw-r--r--   0 root         (0) root         (0)     6700 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sz.eb01cd9f.svg
+-rw-r--r--   0 root         (0) root         (0)    14766 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tc.30ccd48e.svg
+-rw-r--r--   0 root         (0) root         (0)    14507 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tc.651466dd.svg
+-rw-r--r--   0 root         (0) root         (0)      267 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/td.5d622e26.svg
+-rw-r--r--   0 root         (0) root         (0)      279 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/td.f1319408.svg
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tf.27cbe00b.svg
+-rw-r--r--   0 root         (0) root         (0)     1088 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tf.a1757237.svg
+-rw-r--r--   0 root         (0) root         (0)      722 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tg.b492a751.svg
+-rw-r--r--   0 root         (0) root         (0)      733 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tg.d04f874c.svg
+-rw-r--r--   0 root         (0) root         (0)      288 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/th.79b63a8a.svg
+-rw-r--r--   0 root         (0) root         (0)      287 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/th.b8e24edb.svg
+-rw-r--r--   0 root         (0) root         (0)     1785 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tj.b7dafe8d.svg
+-rw-r--r--   0 root         (0) root         (0)     1828 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tj.d3a42312.svg
+-rw-r--r--   0 root         (0) root         (0)      788 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tk.6c1f520c.svg
+-rw-r--r--   0 root         (0) root         (0)      778 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tk.f87f794b.svg
+-rw-r--r--   0 root         (0) root         (0)      597 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tl.85904d79.svg
+-rw-r--r--   0 root         (0) root         (0)      577 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tl.ca9af3c0.svg
+-rw-r--r--   0 root         (0) root         (0)    31846 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tm.762df128.svg
+-rw-r--r--   0 root         (0) root         (0)    32561 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tm.e467552c.svg
+-rw-r--r--   0 root         (0) root         (0)      740 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tn.cc3ab493.svg
+-rw-r--r--   0 root         (0) root         (0)      750 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tn.ff4c5190.svg
+-rw-r--r--   0 root         (0) root         (0)      355 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/to.8dd22284.svg
+-rw-r--r--   0 root         (0) root         (0)      361 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/to.9748a967.svg
+-rw-r--r--   0 root         (0) root         (0)      554 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tr.87e40d5c.svg
+-rw-r--r--   0 root         (0) root         (0)      575 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tr.fc8c91dd.svg
+-rw-r--r--   0 root         (0) root         (0)      320 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tt.4acf6cc2.svg
+-rw-r--r--   0 root         (0) root         (0)      315 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tt.5a459e81.svg
+-rw-r--r--   0 root         (0) root         (0)     2296 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tv.9717b553.svg
+-rw-r--r--   0 root         (0) root         (0)     2163 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tv.a8ff4939.svg
+-rw-r--r--   0 root         (0) root         (0)      957 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tw.45c8a106.svg
+-rw-r--r--   0 root         (0) root         (0)      942 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tw.c0cf9ea7.svg
+-rw-r--r--   0 root         (0) root         (0)      602 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tz.1abfbb38.svg
+-rw-r--r--   0 root         (0) root         (0)      543 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tz.c27fd405.svg
+-rw-r--r--   0 root         (0) root         (0)      238 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ua.04fa0e67.svg
+-rw-r--r--   0 root         (0) root         (0)      238 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ua.63d75c84.svg
+-rw-r--r--   0 root         (0) root         (0)     3953 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ug.5ac71e98.svg
+-rw-r--r--   0 root         (0) root         (0)     4034 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ug.5ae165a2.svg
+-rw-r--r--   0 root         (0) root         (0)     3972 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/um.582dd57b.svg
+-rw-r--r--   0 root         (0) root         (0)     4517 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/um.b38f913c.svg
+-rw-r--r--   0 root         (0) root         (0)    20221 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/un.2df110d6.svg
+-rw-r--r--   0 root         (0) root         (0)    20456 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/un.58a4a02a.svg
+-rw-r--r--   0 root         (0) root         (0)     3921 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/us.6c459052.svg
+-rw-r--r--   0 root         (0) root         (0)     4461 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/us.99e04236.svg
+-rw-r--r--   0 root         (0) root         (0)     1715 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/uy.69cf8938.svg
+-rw-r--r--   0 root         (0) root         (0)     1718 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/uy.b70ac310.svg
+-rw-r--r--   0 root         (0) root         (0)     1454 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/uz.7f8823a2.svg
+-rw-r--r--   0 root         (0) root         (0)     1454 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/uz.d53abc35.svg
+-rw-r--r--   0 root         (0) root         (0)    91211 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/va.7efb8ba6.svg
+-rw-r--r--   0 root         (0) root         (0)    90846 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/va.abcb42e8.svg
+-rw-r--r--   0 root         (0) root         (0)      451 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/vc.37cf5ba1.svg
+-rw-r--r--   0 root         (0) root         (0)      498 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/vc.3e4ac6d4.svg
+-rw-r--r--   0 root         (0) root         (0)     1168 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ve.4cd0e3ed.svg
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ve.9cd63506.svg
+-rw-r--r--   0 root         (0) root         (0)    24993 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/vg.025b8b6a.svg
+-rw-r--r--   0 root         (0) root         (0)    24793 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/vg.ae3b6f7e.svg
+-rw-r--r--   0 root         (0) root         (0)     8711 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/vi.293e6f1c.svg
+-rw-r--r--   0 root         (0) root         (0)     8757 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/vi.f920eec7.svg
+-rw-r--r--   0 root         (0) root         (0)      498 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/vn.11dd1cf6.svg
+-rw-r--r--   0 root         (0) root         (0)      488 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/vn.9ec4ca4d.svg
+-rw-r--r--   0 root         (0) root         (0)     3768 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/vu.5d2d7643.svg
+-rw-r--r--   0 root         (0) root         (0)     3735 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/vu.b7a8d91a.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/wf.69c77016.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/wf.9ca6f4bc.svg
+-rw-r--r--   0 root         (0) root         (0)      693 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ws.15c7a17c.svg
+-rw-r--r--   0 root         (0) root         (0)      706 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ws.d2e19e5a.svg
+-rw-r--r--   0 root         (0) root         (0)     9003 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/xk.16b6bb85.svg
+-rw-r--r--   0 root         (0) root         (0)     9679 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/xk.ca7843be.svg
+-rw-r--r--   0 root         (0) root         (0)      275 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ye.0b3f3c76.svg
+-rw-r--r--   0 root         (0) root         (0)      275 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ye.bb567731.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/yt.332bd5d3.svg
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/yt.c33641ca.svg
+-rw-r--r--   0 root         (0) root         (0)      872 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/za.2fa94205.svg
+-rw-r--r--   0 root         (0) root         (0)      853 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/za.42e033a9.svg
+-rw-r--r--   0 root         (0) root         (0)     5503 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/zm.92477cab.svg
+-rw-r--r--   0 root         (0) root         (0)     5419 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/zm.ce5363b7.svg
+-rw-r--r--   0 root         (0) root         (0)     6759 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/zw.6a535c1e.svg
+-rw-r--r--   0 root         (0) root         (0)     6780 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/zw.f488cb8a.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.706810 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/
+-rw-r--r--   0 root         (0) root         (0)      420 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1088.8670f8f4.js
+-rw-r--r--   0 root         (0) root         (0)     1049 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1088.8670f8f4.js.map
+-rw-r--r--   0 root         (0) root         (0)    35353 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1259.11016ad1.js
+-rw-r--r--   0 root         (0) root         (0)    97910 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1259.11016ad1.js.map
+-rw-r--r--   0 root         (0) root         (0)    13278 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1449.475ec524.js
+-rw-r--r--   0 root         (0) root         (0)    43973 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1449.475ec524.js.map
+-rw-r--r--   0 root         (0) root         (0)     9432 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1512.3e4f99fd.js
+-rw-r--r--   0 root         (0) root         (0)    21297 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1512.3e4f99fd.js.map
+-rw-r--r--   0 root         (0) root         (0)    16017 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1587.e2ebe369.js
+-rw-r--r--   0 root         (0) root         (0)    48235 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1587.e2ebe369.js.map
+-rw-r--r--   0 root         (0) root         (0)     1111 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/169.8bb8df7d.js
+-rw-r--r--   0 root         (0) root         (0)     2916 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/169.8bb8df7d.js.map
+-rw-r--r--   0 root         (0) root         (0)     1931 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1706.97f9b825.js
+-rw-r--r--   0 root         (0) root         (0)     4723 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1706.97f9b825.js.map
+-rw-r--r--   0 root         (0) root         (0)    22004 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1807.586a24d4.js
+-rw-r--r--   0 root         (0) root         (0)    60878 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1807.586a24d4.js.map
+-rw-r--r--   0 root         (0) root         (0)     3339 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1949.9d6edfd8.js
+-rw-r--r--   0 root         (0) root         (0)     9056 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1949.9d6edfd8.js.map
+-rw-r--r--   0 root         (0) root         (0)     2575 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2106.6553ebed.js
+-rw-r--r--   0 root         (0) root         (0)     7033 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2106.6553ebed.js.map
+-rw-r--r--   0 root         (0) root         (0)     4924 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2140.10cab5fd.js
+-rw-r--r--   0 root         (0) root         (0)    15185 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2140.10cab5fd.js.map
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2183.2941880a.js
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2183.2941880a.js.map
+-rw-r--r--   0 root         (0) root         (0)     1038 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2200.9fc9fd95.js
+-rw-r--r--   0 root         (0) root         (0)     2498 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2200.9fc9fd95.js.map
+-rw-r--r--   0 root         (0) root         (0)      863 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2217.30568f1a.js
+-rw-r--r--   0 root         (0) root         (0)     2227 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2217.30568f1a.js.map
+-rw-r--r--   0 root         (0) root         (0)     1010 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2460.9845df8e.js
+-rw-r--r--   0 root         (0) root         (0)     2479 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2460.9845df8e.js.map
+-rw-r--r--   0 root         (0) root         (0)    55875 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2509.efc0bf4c.js
+-rw-r--r--   0 root         (0) root         (0)   141746 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2509.efc0bf4c.js.map
+-rw-r--r--   0 root         (0) root         (0)      444 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2614.7997d726.js
+-rw-r--r--   0 root         (0) root         (0)     1114 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2614.7997d726.js.map
+-rw-r--r--   0 root         (0) root         (0)      415 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2732.28f617e8.js
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2732.28f617e8.js.map
+-rw-r--r--   0 root         (0) root         (0)     1744 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2853.47a43033.js
+-rw-r--r--   0 root         (0) root         (0)     5624 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2853.47a43033.js.map
+-rw-r--r--   0 root         (0) root         (0)     1044 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2892.2d33f676.js
+-rw-r--r--   0 root         (0) root         (0)     3070 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2892.2d33f676.js.map
+-rw-r--r--   0 root         (0) root         (0)     2482 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2893.b037e7d2.js
+-rw-r--r--   0 root         (0) root         (0)     5660 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2893.b037e7d2.js.map
+-rw-r--r--   0 root         (0) root         (0)     5450 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2976.e8a9eb12.js
+-rw-r--r--   0 root         (0) root         (0)    16326 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2976.e8a9eb12.js.map
+-rw-r--r--   0 root         (0) root         (0)    10076 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3083.8440bfa8.js
+-rw-r--r--   0 root         (0) root         (0)    28154 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3083.8440bfa8.js.map
+-rw-r--r--   0 root         (0) root         (0)      764 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3322.5ee98346.js
+-rw-r--r--   0 root         (0) root         (0)     2088 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3322.5ee98346.js.map
+-rw-r--r--   0 root         (0) root         (0)     2607 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3368.7ff6fca3.js
+-rw-r--r--   0 root         (0) root         (0)     6949 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3368.7ff6fca3.js.map
+-rw-r--r--   0 root         (0) root         (0)     5282 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3369.71760407.js
+-rw-r--r--   0 root         (0) root         (0)    11158 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3369.71760407.js.map
+-rw-r--r--   0 root         (0) root         (0)    10107 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3400.1021c9a8.js
+-rw-r--r--   0 root         (0) root         (0)    28210 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3400.1021c9a8.js.map
+-rw-r--r--   0 root         (0) root         (0)     1805 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/342.d3c0f8f2.js
+-rw-r--r--   0 root         (0) root         (0)     5953 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/342.d3c0f8f2.js.map
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3518.40e74ddb.js
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3518.40e74ddb.js.map
+-rw-r--r--   0 root         (0) root         (0)    45695 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3553.125dc216.js
+-rw-r--r--   0 root         (0) root         (0)   114423 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3553.125dc216.js.map
+-rw-r--r--   0 root         (0) root         (0)     1220 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3559.da067b47.js
+-rw-r--r--   0 root         (0) root         (0)     3059 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3559.da067b47.js.map
+-rw-r--r--   0 root         (0) root         (0)     1737 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3732.17c9c669.js
+-rw-r--r--   0 root         (0) root         (0)     5607 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3732.17c9c669.js.map
+-rw-r--r--   0 root         (0) root         (0)     2316 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3835.878348e2.js
+-rw-r--r--   0 root         (0) root         (0)     9498 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3835.878348e2.js.map
+-rw-r--r--   0 root         (0) root         (0)     5620 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3924.9592f111.js
+-rw-r--r--   0 root         (0) root         (0)    14954 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3924.9592f111.js.map
+-rw-r--r--   0 root         (0) root         (0)     7918 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/4053.1a106579.js
+-rw-r--r--   0 root         (0) root         (0)    19391 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/4053.1a106579.js.map
+-rw-r--r--   0 root         (0) root         (0)      633 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/4221.292aeb44.js
+-rw-r--r--   0 root         (0) root         (0)     2174 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/4221.292aeb44.js.map
+-rw-r--r--   0 root         (0) root         (0)     1416 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/446.178d2754.js
+-rw-r--r--   0 root         (0) root         (0)     4379 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/446.178d2754.js.map
+-rw-r--r--   0 root         (0) root         (0)     7765 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/4589.c6a12ddf.js
+-rw-r--r--   0 root         (0) root         (0)    18764 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/4589.c6a12ddf.js.map
+-rw-r--r--   0 root         (0) root         (0)     1201 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/4619.ea41fd5e.js
+-rw-r--r--   0 root         (0) root         (0)     3333 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/4619.ea41fd5e.js.map
+-rw-r--r--   0 root         (0) root         (0)     6803 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/472.05f32d73.js
+-rw-r--r--   0 root         (0) root         (0)    18143 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/472.05f32d73.js.map
+-rw-r--r--   0 root         (0) root         (0)      444 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/4765.7ad68124.js
+-rw-r--r--   0 root         (0) root         (0)     1114 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/4765.7ad68124.js.map
+-rw-r--r--   0 root         (0) root         (0)      125 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5207.7f241e21.js
+-rw-r--r--   0 root         (0) root         (0)    27243 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5285.551ed2ce.js
+-rw-r--r--   0 root         (0) root         (0)    74761 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5285.551ed2ce.js.map
+-rw-r--r--   0 root         (0) root         (0)     9111 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5324.a449638b.js
+-rw-r--r--   0 root         (0) root         (0)    20342 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5324.a449638b.js.map
+-rw-r--r--   0 root         (0) root         (0)     4526 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5329.7bf8697f.js
+-rw-r--r--   0 root         (0) root         (0)     9566 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5329.7bf8697f.js.map
+-rw-r--r--   0 root         (0) root         (0)     1449 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5578.7c9eef7c.js
+-rw-r--r--   0 root         (0) root         (0)     3571 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5578.7c9eef7c.js.map
+-rw-r--r--   0 root         (0) root         (0)     2183 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5638.f1abcb64.js
+-rw-r--r--   0 root         (0) root         (0)     5966 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5638.f1abcb64.js.map
+-rw-r--r--   0 root         (0) root         (0)     2717 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5762.0d8fb9cb.js
+-rw-r--r--   0 root         (0) root         (0)     8162 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5762.0d8fb9cb.js.map
+-rw-r--r--   0 root         (0) root         (0)     7421 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5795.8f7061d6.js
+-rw-r--r--   0 root         (0) root         (0)    22573 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5795.8f7061d6.js.map
+-rw-r--r--   0 root         (0) root         (0)    15417 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5931.bcf6cfaf.js
+-rw-r--r--   0 root         (0) root         (0)    41562 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5931.bcf6cfaf.js.map
+-rw-r--r--   0 root         (0) root         (0)    29283 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6062.2509fe58.js
+-rw-r--r--   0 root         (0) root         (0)    63711 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6062.2509fe58.js.map
+-rw-r--r--   0 root         (0) root         (0)     4988 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6123.0a491498.js
+-rw-r--r--   0 root         (0) root         (0)    15776 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6123.0a491498.js.map
+-rw-r--r--   0 root         (0) root         (0)     9419 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6148.70084131.js
+-rw-r--r--   0 root         (0) root         (0)    21271 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6148.70084131.js.map
+-rw-r--r--   0 root         (0) root         (0)     2947 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6324.9d695c83.js
+-rw-r--r--   0 root         (0) root         (0)     7263 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6324.9d695c83.js.map
+-rw-r--r--   0 root         (0) root         (0)     1288 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6362.7e4f1ac1.js
+-rw-r--r--   0 root         (0) root         (0)     3000 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6362.7e4f1ac1.js.map
+-rw-r--r--   0 root         (0) root         (0)      121 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/65.ae7df477.js
+-rw-r--r--   0 root         (0) root         (0)     1498 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6523.6faff1f9.js
+-rw-r--r--   0 root         (0) root         (0)     4426 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6523.6faff1f9.js.map
+-rw-r--r--   0 root         (0) root         (0)      357 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6640.a6538b3b.js
+-rw-r--r--   0 root         (0) root         (0)      995 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6640.a6538b3b.js.map
+-rw-r--r--   0 root         (0) root         (0)     4404 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/667.f23239a7.js
+-rw-r--r--   0 root         (0) root         (0)    12046 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/667.f23239a7.js.map
+-rw-r--r--   0 root         (0) root         (0)     1747 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7089.f4d74b4a.js
+-rw-r--r--   0 root         (0) root         (0)     5634 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7089.f4d74b4a.js.map
+-rw-r--r--   0 root         (0) root         (0)     8258 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/729.f4de5689.js
+-rw-r--r--   0 root         (0) root         (0)    19267 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/729.f4de5689.js.map
+-rw-r--r--   0 root         (0) root         (0)     9685 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7381.66ebc1f2.js
+-rw-r--r--   0 root         (0) root         (0)    21916 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7381.66ebc1f2.js.map
+-rw-r--r--   0 root         (0) root         (0)     1441 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/746.4c6b0061.js
+-rw-r--r--   0 root         (0) root         (0)     3351 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/746.4c6b0061.js.map
+-rw-r--r--   0 root         (0) root         (0)     1804 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7590.014063f7.js
+-rw-r--r--   0 root         (0) root         (0)     4865 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7590.014063f7.js.map
+-rw-r--r--   0 root         (0) root         (0)      450 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7819.15635e35.js
+-rw-r--r--   0 root         (0) root         (0)     1133 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7819.15635e35.js.map
+-rw-r--r--   0 root         (0) root         (0)    15147 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7841.8b124a1f.js
+-rw-r--r--   0 root         (0) root         (0)    45071 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7841.8b124a1f.js.map
+-rw-r--r--   0 root         (0) root         (0)    15987 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7878.98038a22.js
+-rw-r--r--   0 root         (0) root         (0)    46669 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7878.98038a22.js.map
+-rw-r--r--   0 root         (0) root         (0)    46543 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7880.b455063a.js
+-rw-r--r--   0 root         (0) root         (0)   111831 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7880.b455063a.js.map
+-rw-r--r--   0 root         (0) root         (0)     3614 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7898.0426589e.js
+-rw-r--r--   0 root         (0) root         (0)    10984 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7898.0426589e.js.map
+-rw-r--r--   0 root         (0) root         (0)    11595 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7968.d677b422.js
+-rw-r--r--   0 root         (0) root         (0)    28428 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7968.d677b422.js.map
+-rw-r--r--   0 root         (0) root         (0)     9430 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/813.1fe7c13a.js
+-rw-r--r--   0 root         (0) root         (0)    21299 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/813.1fe7c13a.js.map
+-rw-r--r--   0 root         (0) root         (0)     1209 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8179.bd308864.js
+-rw-r--r--   0 root         (0) root         (0)     3576 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8179.bd308864.js.map
+-rw-r--r--   0 root         (0) root         (0)     2365 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8391.40c294c5.js
+-rw-r--r--   0 root         (0) root         (0)     9602 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8391.40c294c5.js.map
+-rw-r--r--   0 root         (0) root         (0)    10871 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8498.f8eb1c87.js
+-rw-r--r--   0 root         (0) root         (0)    24374 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8498.f8eb1c87.js.map
+-rw-r--r--   0 root         (0) root         (0)     1974 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8621.a437ee11.js
+-rw-r--r--   0 root         (0) root         (0)     8339 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8621.a437ee11.js.map
+-rw-r--r--   0 root         (0) root         (0)      845 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8769.ad2a69a1.js
+-rw-r--r--   0 root         (0) root         (0)     2196 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8769.ad2a69a1.js.map
+-rw-r--r--   0 root         (0) root         (0)      432 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8784.9c4e51b9.js
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8784.9c4e51b9.js.map
+-rw-r--r--   0 root         (0) root         (0)     5921 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8825.25b100b4.js
+-rw-r--r--   0 root         (0) root         (0)    12073 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8825.25b100b4.js.map
+-rw-r--r--   0 root         (0) root         (0)     1749 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/886.9ff7c1ce.js
+-rw-r--r--   0 root         (0) root         (0)     5730 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/886.9ff7c1ce.js.map
+-rw-r--r--   0 root         (0) root         (0)     9419 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8895.a4a700ec.js
+-rw-r--r--   0 root         (0) root         (0)    21271 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8895.a4a700ec.js.map
+-rw-r--r--   0 root         (0) root         (0)     8768 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8930.be445a5e.js
+-rw-r--r--   0 root         (0) root         (0)    19222 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8930.be445a5e.js.map
+-rw-r--r--   0 root         (0) root         (0)     1382 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9091.4b4643b0.js
+-rw-r--r--   0 root         (0) root         (0)     2078 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9091.4b4643b0.js.map
+-rw-r--r--   0 root         (0) root         (0)    11781 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9211.d1e09f60.js
+-rw-r--r--   0 root         (0) root         (0)    42175 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9211.d1e09f60.js.map
+-rw-r--r--   0 root         (0) root         (0)     9427 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9334.455b4593.js
+-rw-r--r--   0 root         (0) root         (0)    21287 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9334.455b4593.js.map
+-rw-r--r--   0 root         (0) root         (0)    49081 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9381.dc2f4776.js
+-rw-r--r--   0 root         (0) root         (0)   160106 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9381.dc2f4776.js.map
+-rw-r--r--   0 root         (0) root         (0)     4116 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9461.1fd0b115.js
+-rw-r--r--   0 root         (0) root         (0)    13714 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9461.1fd0b115.js.map
+-rw-r--r--   0 root         (0) root         (0)    30136 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9751.5b8fcd4c.js
+-rw-r--r--   0 root         (0) root         (0)    94584 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9751.5b8fcd4c.js.map
+-rw-r--r--   0 root         (0) root         (0)    10765 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/980.e9d022c5.js
+-rw-r--r--   0 root         (0) root         (0)    38863 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/980.e9d022c5.js.map
+-rw-r--r--   0 root         (0) root         (0)     2490 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/984.bedc7c00.js
+-rw-r--r--   0 root         (0) root         (0)     9879 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/984.bedc7c00.js.map
+-rw-r--r--   0 root         (0) root         (0)     5531 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9962.d22f669b.js
+-rw-r--r--   0 root         (0) root         (0)    15548 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9962.d22f669b.js.map
+-rw-r--r--   0 root         (0) root         (0)    88297 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/app.62f4493a.js
+-rw-r--r--   0 root         (0) root         (0)   265688 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/app.62f4493a.js.map
+-rw-r--r--   0 root         (0) root         (0)  1089172 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/chunk-vendors.c084e94c.js
+-rw-r--r--   0 root         (0) root         (0)  2999782 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/chunk-vendors.c084e94c.js.map
+-rw-r--r--   0 root         (0) root         (0)    14450 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/workbox-5b385ed2.js
+-rw-r--r--   0 root         (0) root         (0)   137845 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/http/webapp/dist/workbox-5b385ed2.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.710144 platypush-1.0.4/platypush/backend/nodered/
+-rw-r--r--   0 root         (0) root         (0)     1611 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/nodered/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      174 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/nodered/manifest.json
+-rw-r--r--   0 root         (0) root         (0)      865 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/nodered/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.710144 platypush-1.0.4/platypush/backend/redis/
+-rw-r--r--   0 root         (0) root         (0)     3116 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      145 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/redis/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.710144 platypush-1.0.4/platypush/backend/tcp/
+-rw-r--r--   0 root         (0) root         (0)     4732 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/tcp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      143 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/backend/tcp/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.713477 platypush-1.0.4/platypush/builder/
+-rw-r--r--   0 root         (0) root         (0)       58 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/builder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6017 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/builder/_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.713477 platypush-1.0.4/platypush/bus/
+-rw-r--r--   0 root         (0) root         (0)     4685 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/bus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1763 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/bus/redis.py
+-rw-r--r--   0 root         (0) root         (0)     4962 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.713477 platypush-1.0.4/platypush/commands/
+-rw-r--r--   0 root         (0) root         (0)      186 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2142 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/commands/_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.713477 platypush-1.0.4/platypush/commands/_commands/
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/commands/_commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      437 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/commands/_commands/_app_ctrl.py
+-rw-r--r--   0 root         (0) root         (0)     1971 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/commands/_reader.py
+-rw-r--r--   0 root         (0) root         (0)     4933 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/commands/_stream.py
+-rw-r--r--   0 root         (0) root         (0)      578 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/commands/_writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.713477 platypush-1.0.4/platypush/common/
+-rw-r--r--   0 root         (0) root         (0)     1912 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      991 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/_types.py
+-rw-r--r--   0 root         (0) root         (0)      102 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/cmd_stream.py
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/db.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.713477 platypush-1.0.4/platypush/common/gstreamer/
+-rw-r--r--   0 root         (0) root         (0)     5729 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/gstreamer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.713477 platypush-1.0.4/platypush/common/reflection/
+-rw-r--r--   0 root         (0) root         (0)       91 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/reflection/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.716811 platypush-1.0.4/platypush/common/reflection/_model/
+-rw-r--r--   0 root         (0) root         (0)      312 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/reflection/_model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      125 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/reflection/_model/action.py
+-rw-r--r--   0 root         (0) root         (0)      630 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/reflection/_model/argument.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/reflection/_model/component.py
+-rw-r--r--   0 root         (0) root         (0)       55 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/reflection/_model/constants.py
+-rw-r--r--   0 root         (0) root         (0)      596 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/reflection/_model/constructor.py
+-rw-r--r--   0 root         (0) root         (0)    10771 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/reflection/_model/integration.py
+-rw-r--r--   0 root         (0) root         (0)     3240 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/reflection/_model/message.py
+-rw-r--r--   0 root         (0) root         (0)      437 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/reflection/_model/returns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.716811 platypush-1.0.4/platypush/common/reflection/_parser/
+-rw-r--r--   0 root         (0) root         (0)       78 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/reflection/_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2744 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/reflection/_parser/context.py
+-rw-r--r--   0 root         (0) root         (0)     5708 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/reflection/_parser/docstring.py
+-rw-r--r--   0 root         (0) root         (0)     6897 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/reflection/_parser/rst.py
+-rw-r--r--   0 root         (0) root         (0)      142 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/reflection/_parser/state.py
+-rw-r--r--   0 root         (0) root         (0)      309 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/reflection/_serialize.py
+-rw-r--r--   0 root         (0) root         (0)      278 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/reflection/_utils.py
+-rw-r--r--   0 root         (0) root         (0)      314 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/sensors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.716811 platypush-1.0.4/platypush/common/spotify/
+-rw-r--r--   0 root         (0) root         (0)    14862 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/common/spotify/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   289402 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/components.json.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.716811 platypush-1.0.4/platypush/config/
+-rw-r--r--   0 root         (0) root         (0)    22023 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43853 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/config/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.720144 platypush-1.0.4/platypush/config/systemd/
+-rw-r--r--   0 root         (0) root         (0)       85 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/config/systemd/platypush-sysusers.conf
+-rw-r--r--   0 root         (0) root         (0)       92 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/config/systemd/platypush-tmpfile.conf
+-rw-r--r--   0 root         (0) root         (0)     1075 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/config/systemd/platypush.service
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.720144 platypush-1.0.4/platypush/context/
+-rw-r--r--   0 root         (0) root         (0)     6724 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/context/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.720144 platypush-1.0.4/platypush/cron/
+-rw-r--r--   0 root         (0) root         (0)      426 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/cron/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7745 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/cron/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.723478 platypush-1.0.4/platypush/entities/
+-rw-r--r--   0 root         (0) root         (0)     2405 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11166 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.723478 platypush-1.0.4/platypush/entities/_engine/
+-rw-r--r--   0 root         (0) root         (0)     5053 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/_engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1503 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/_engine/queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.723478 platypush-1.0.4/platypush/entities/_engine/repo/
+-rw-r--r--   0 root         (0) root         (0)     3326 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/_engine/repo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6369 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/_engine/repo/db.py
+-rw-r--r--   0 root         (0) root         (0)      602 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/_engine/repo/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     7489 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/_engine/repo/merger.py
+-rw-r--r--   0 root         (0) root         (0)      642 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/acceleration.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/alarm.py
+-rw-r--r--   0 root         (0) root         (0)      787 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/assistants.py
+-rw-r--r--   0 root         (0) root         (0)      840 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/audio.py
+-rw-r--r--   0 root         (0) root         (0)      687 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/batteries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.726811 platypush-1.0.4/platypush/entities/bluetooth/
+-rw-r--r--   0 root         (0) root         (0)      138 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/bluetooth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5143 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/bluetooth/_device.py
+-rw-r--r--   0 root         (0) root         (0)     3908 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/bluetooth/_service.py
+-rw-r--r--   0 root         (0) root         (0)      552 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/buttons.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/cloud.py
+-rw-r--r--   0 root         (0) root         (0)      581 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/contact.py
+-rw-r--r--   0 root         (0) root         (0)      596 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/devices.py
+-rw-r--r--   0 root         (0) root         (0)      803 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/dimmers.py
+-rw-r--r--   0 root         (0) root         (0)      585 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/distance.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/electricity.py
+-rw-r--r--   0 root         (0) root         (0)      593 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/heart.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/humidity.py
+-rw-r--r--   0 root         (0) root         (0)      525 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/illuminance.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/lights.py
+-rw-r--r--   0 root         (0) root         (0)      701 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/linkquality.py
+-rw-r--r--   0 root         (0) root         (0)      630 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/magnetism.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.726811 platypush-1.0.4/platypush/entities/managers/
+-rw-r--r--   0 root         (0) root         (0)     6174 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/managers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/managers/assistants.py
+-rw-r--r--   0 root         (0) root         (0)      988 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/managers/cloud.py
+-rw-r--r--   0 root         (0) root         (0)      571 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/managers/lights.py
+-rw-r--r--   0 root         (0) root         (0)      176 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/managers/sensors.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/managers/switches.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/managers/weather.py
+-rw-r--r--   0 root         (0) root         (0)      507 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/motion.py
+-rw-r--r--   0 root         (0) root         (0)      704 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/ping.py
+-rw-r--r--   0 root         (0) root         (0)      585 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/presence.py
+-rw-r--r--   0 root         (0) root         (0)      582 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/pressure.py
+-rw-r--r--   0 root         (0) root         (0)     6114 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/sensors.py
+-rw-r--r--   0 root         (0) root         (0)      590 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/steps.py
+-rw-r--r--   0 root         (0) root         (0)      944 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/switches.py
+-rw-r--r--   0 root         (0) root         (0)     7027 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/system.py
+-rw-r--r--   0 root         (0) root         (0)      525 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/temperature.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/three_axis.py
+-rw-r--r--   0 root         (0) root         (0)      584 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/time.py
+-rw-r--r--   0 root         (0) root         (0)      620 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/variables.py
+-rw-r--r--   0 root         (0) root         (0)     1392 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/weather.py
+-rw-r--r--   0 root         (0) root         (0)      574 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/entities/weight.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.726811 platypush-1.0.4/platypush/event/
+-rw-r--r--   0 root         (0) root         (0)     1976 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/event/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7090 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/event/hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.726811 platypush-1.0.4/platypush/event/processor/
+-rw-r--r--   0 root         (0) root         (0)     2498 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/event/processor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.733478 platypush-1.0.4/platypush/events/
+-rw-r--r--   0 root         (0) root         (0)    11119 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      760 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/adafruit.py
+-rw-r--r--   0 root         (0) root         (0)      961 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/alarm.py
+-rw-r--r--   0 root         (0) root         (0)      300 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/application.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.733478 platypush-1.0.4/platypush/events/assistant/
+-rw-r--r--   0 root         (0) root         (0)     9968 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/assistant/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.733478 platypush-1.0.4/platypush/events/bluetooth/
+-rw-r--r--   0 root         (0) root         (0)     4397 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/bluetooth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/camera.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.733478 platypush-1.0.4/platypush/events/chat/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/chat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2215 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/chat/slack.py
+-rw-r--r--   0 root         (0) root         (0)      200 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/clipboard.py
+-rw-r--r--   0 root         (0) root         (0)      686 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/custom.py
+-rw-r--r--   0 root         (0) root         (0)      859 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/dbus.py
+-rw-r--r--   0 root         (0) root         (0)      503 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/distance.py
+-rw-r--r--   0 root         (0) root         (0)      664 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/entities.py
+-rw-r--r--   0 root         (0) root         (0)      725 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/file.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/flic.py
+-rw-r--r--   0 root         (0) root         (0)      322 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/foursquare.py
+-rw-r--r--   0 root         (0) root         (0)      573 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/geo.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/github.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.736811 platypush-1.0.4/platypush/events/google/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/google/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      340 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/google/pubsub.py
+-rw-r--r--   0 root         (0) root         (0)     1198 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/gotify.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.736811 platypush-1.0.4/platypush/events/gpio/
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/gpio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2184 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/gps.py
+-rw-r--r--   0 root         (0) root         (0)     1223 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/hid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.736811 platypush-1.0.4/platypush/events/http/
+-rw-r--r--   0 root         (0) root         (0)      509 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2521 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/http/hook.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/http/rss.py
+-rw-r--r--   0 root         (0) root         (0)     2553 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/inotify.py
+-rw-r--r--   0 root         (0) root         (0)     5407 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/irc.py
+-rw-r--r--   0 root         (0) root         (0)      982 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/joystick.py
+-rw-r--r--   0 root         (0) root         (0)      897 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/kafka.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/light.py
+-rw-r--r--   0 root         (0) root         (0)      928 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/linode.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.736811 platypush-1.0.4/platypush/events/log/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      825 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/log/http.py
+-rw-r--r--   0 root         (0) root         (0)      796 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/mail.py
+-rw-r--r--   0 root         (0) root         (0)     7060 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/matrix.py
+-rw-r--r--   0 root         (0) root         (0)     3358 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/media.py
+-rw-r--r--   0 root         (0) root         (0)     1392 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/midi.py
+-rw-r--r--   0 root         (0) root         (0)      403 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/mqtt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.736811 platypush-1.0.4/platypush/events/music/
+-rw-r--r--   0 root         (0) root         (0)     3759 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/music/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/music/snapcast.py
+-rw-r--r--   0 root         (0) root         (0)      347 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/music/tidal.py
+-rw-r--r--   0 root         (0) root         (0)     3672 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/nextcloud.py
+-rw-r--r--   0 root         (0) root         (0)     2222 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/nfc.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/ngrok.py
+-rw-r--r--   0 root         (0) root         (0)     2862 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/ntfy.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/ping.py
+-rw-r--r--   0 root         (0) root         (0)     5060 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/pushbullet.py
+-rw-r--r--   0 root         (0) root         (0)      471 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/qrcode.py
+-rw-r--r--   0 root         (0) root         (0)      992 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/rss.py
+-rw-r--r--   0 root         (0) root         (0)      934 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/scard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.736811 platypush-1.0.4/platypush/events/sensor/
+-rw-r--r--   0 root         (0) root         (0)      961 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/sensor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.736811 platypush-1.0.4/platypush/events/sensor/ir/
+-rw-r--r--   0 root         (0) root         (0)      862 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/sensor/ir/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/sensor/leap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.736811 platypush-1.0.4/platypush/events/sensor/light/
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/sensor/light/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.736811 platypush-1.0.4/platypush/events/serial/
+-rw-r--r--   0 root         (0) root         (0)      495 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/serial/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/sound.py
+-rw-r--r--   0 root         (0) root         (0)     1347 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/stt.py
+-rw-r--r--   0 root         (0) root         (0)      894 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/sun.py
+-rw-r--r--   0 root         (0) root         (0)     2210 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/telegram.py
+-rw-r--r--   0 root         (0) root         (0)     1946 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/tensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     2572 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/torrent.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/trello.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.736811 platypush-1.0.4/platypush/events/video/
+-rw-r--r--   0 root         (0) root         (0)     1253 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/video/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4113 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/weather.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.736811 platypush-1.0.4/platypush/events/web/
+-rw-r--r--   0 root         (0) root         (0)      875 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/web/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      391 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/web/widget.py
+-rw-r--r--   0 root         (0) root         (0)      436 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/websocket.py
+-rw-r--r--   0 root         (0) root         (0)     9969 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/xmpp.py
+-rw-r--r--   0 root         (0) root         (0)      413 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/zeroborg.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/zeroconf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.736811 platypush-1.0.4/platypush/events/zigbee/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/zigbee/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5542 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/zigbee/mqtt.py
+-rw-r--r--   0 root         (0) root         (0)     5480 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/events/zwave.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.740145 platypush-1.0.4/platypush/exceptions/
+-rw-r--r--   0 root         (0) root         (0)      542 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1281 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/exceptions/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.526804 platypush-1.0.4/platypush/install/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.740145 platypush-1.0.4/platypush/install/docker/
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/install/docker/alpine.Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     1263 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/install/docker/debian.Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     1260 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/install/docker/fedora.Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     1263 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/install/docker/ubuntu.Dockerfile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.740145 platypush-1.0.4/platypush/install/requirements/
+-rw-r--r--   0 root         (0) root         (0)      277 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/install/requirements/alpine.txt
+-rw-r--r--   0 root         (0) root         (0)      337 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/install/requirements/arch.txt
+-rw-r--r--   0 root         (0) root         (0)      391 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/install/requirements/debian.txt
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/install/requirements/fedora.txt
+-rw-r--r--   0 root         (0) root         (0)      391 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/install/requirements/ubuntu.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.740145 platypush-1.0.4/platypush/install/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.740145 platypush-1.0.4/platypush/install/scripts/alpine/
+-rw-r--r--   0 root         (0) root         (0)       45 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/install/scripts/alpine/PKGCMD
+-rwxr-xr-x   0 root         (0) root         (0)      945 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/install/scripts/alpine/install.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.740145 platypush-1.0.4/platypush/install/scripts/arch/
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/install/scripts/arch/PKGCMD
+-rwxr-xr-x   0 root         (0) root         (0)      945 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/install/scripts/arch/install.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.740145 platypush-1.0.4/platypush/install/scripts/debian/
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/install/scripts/debian/PKGCMD
+-rwxr-xr-x   0 root         (0) root         (0)      945 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/install/scripts/debian/install.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.740145 platypush-1.0.4/platypush/install/scripts/fedora/
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/install/scripts/fedora/PKGCMD
+-rwxr-xr-x   0 root         (0) root         (0)      945 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/install/scripts/fedora/install.sh
+-rwxr-xr-x   0 root         (0) root         (0)      945 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/install/scripts/install.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.740145 platypush-1.0.4/platypush/install/scripts/ubuntu/
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/install/scripts/ubuntu/PKGCMD
+-rwxr-xr-x   0 root         (0) root         (0)      945 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/install/scripts/ubuntu/install.sh
+-rw-r--r--   0 root         (0) root         (0)      574 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.740145 platypush-1.0.4/platypush/message/
+-rw-r--r--   0 root         (0) root         (0)     6007 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.750145 platypush-1.0.4/platypush/message/event/
+-rw-r--r--   0 root         (0) root         (0)    11119 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      760 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/adafruit.py
+-rw-r--r--   0 root         (0) root         (0)      961 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/alarm.py
+-rw-r--r--   0 root         (0) root         (0)      300 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/application.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.750145 platypush-1.0.4/platypush/message/event/assistant/
+-rw-r--r--   0 root         (0) root         (0)     9968 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/assistant/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.750145 platypush-1.0.4/platypush/message/event/bluetooth/
+-rw-r--r--   0 root         (0) root         (0)     4397 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/bluetooth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/camera.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.750145 platypush-1.0.4/platypush/message/event/chat/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/chat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2215 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/chat/slack.py
+-rw-r--r--   0 root         (0) root         (0)      200 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/clipboard.py
+-rw-r--r--   0 root         (0) root         (0)      686 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/custom.py
+-rw-r--r--   0 root         (0) root         (0)      859 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/dbus.py
+-rw-r--r--   0 root         (0) root         (0)      503 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/distance.py
+-rw-r--r--   0 root         (0) root         (0)      664 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/entities.py
+-rw-r--r--   0 root         (0) root         (0)      725 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/file.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/flic.py
+-rw-r--r--   0 root         (0) root         (0)      322 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/foursquare.py
+-rw-r--r--   0 root         (0) root         (0)      573 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/geo.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/github.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.750145 platypush-1.0.4/platypush/message/event/google/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/google/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      340 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/google/pubsub.py
+-rw-r--r--   0 root         (0) root         (0)     1198 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/gotify.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.750145 platypush-1.0.4/platypush/message/event/gpio/
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/gpio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2184 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/gps.py
+-rw-r--r--   0 root         (0) root         (0)     1223 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/hid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.750145 platypush-1.0.4/platypush/message/event/http/
+-rw-r--r--   0 root         (0) root         (0)      509 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2521 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/http/hook.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/http/rss.py
+-rw-r--r--   0 root         (0) root         (0)     2553 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/inotify.py
+-rw-r--r--   0 root         (0) root         (0)     5407 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/irc.py
+-rw-r--r--   0 root         (0) root         (0)      982 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/joystick.py
+-rw-r--r--   0 root         (0) root         (0)      897 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/kafka.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/light.py
+-rw-r--r--   0 root         (0) root         (0)      928 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/linode.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.750145 platypush-1.0.4/platypush/message/event/log/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      825 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/log/http.py
+-rw-r--r--   0 root         (0) root         (0)      796 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/mail.py
+-rw-r--r--   0 root         (0) root         (0)     7060 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/matrix.py
+-rw-r--r--   0 root         (0) root         (0)     3358 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/media.py
+-rw-r--r--   0 root         (0) root         (0)     1392 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/midi.py
+-rw-r--r--   0 root         (0) root         (0)      403 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/mqtt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.750145 platypush-1.0.4/platypush/message/event/music/
+-rw-r--r--   0 root         (0) root         (0)     3759 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/music/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/music/snapcast.py
+-rw-r--r--   0 root         (0) root         (0)      347 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/music/tidal.py
+-rw-r--r--   0 root         (0) root         (0)     3672 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/nextcloud.py
+-rw-r--r--   0 root         (0) root         (0)     2222 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/nfc.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/ngrok.py
+-rw-r--r--   0 root         (0) root         (0)     2862 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/ntfy.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/ping.py
+-rw-r--r--   0 root         (0) root         (0)     5060 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/pushbullet.py
+-rw-r--r--   0 root         (0) root         (0)      471 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/qrcode.py
+-rw-r--r--   0 root         (0) root         (0)      992 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/rss.py
+-rw-r--r--   0 root         (0) root         (0)      934 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/scard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.750145 platypush-1.0.4/platypush/message/event/sensor/
+-rw-r--r--   0 root         (0) root         (0)      961 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/sensor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.753479 platypush-1.0.4/platypush/message/event/sensor/ir/
+-rw-r--r--   0 root         (0) root         (0)      862 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/sensor/ir/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/sensor/leap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.753479 platypush-1.0.4/platypush/message/event/sensor/light/
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/sensor/light/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.753479 platypush-1.0.4/platypush/message/event/serial/
+-rw-r--r--   0 root         (0) root         (0)      495 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/serial/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/sound.py
+-rw-r--r--   0 root         (0) root         (0)     1347 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/stt.py
+-rw-r--r--   0 root         (0) root         (0)      894 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/sun.py
+-rw-r--r--   0 root         (0) root         (0)     2210 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/telegram.py
+-rw-r--r--   0 root         (0) root         (0)     1946 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/tensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     2572 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/torrent.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/trello.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.753479 platypush-1.0.4/platypush/message/event/video/
+-rw-r--r--   0 root         (0) root         (0)     1253 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/video/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4113 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/weather.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.753479 platypush-1.0.4/platypush/message/event/web/
+-rw-r--r--   0 root         (0) root         (0)      875 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/web/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      391 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/web/widget.py
+-rw-r--r--   0 root         (0) root         (0)      436 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/websocket.py
+-rw-r--r--   0 root         (0) root         (0)     9969 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/xmpp.py
+-rw-r--r--   0 root         (0) root         (0)      413 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/zeroborg.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/zeroconf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.753479 platypush-1.0.4/platypush/message/event/zigbee/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/zigbee/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5542 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/zigbee/mqtt.py
+-rw-r--r--   0 root         (0) root         (0)     5480 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/event/zwave.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.753479 platypush-1.0.4/platypush/message/request/
+-rw-r--r--   0 root         (0) root         (0)    11283 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.753479 platypush-1.0.4/platypush/message/response/
+-rw-r--r--   0 root         (0) root         (0)     2964 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/message/response/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.753479 platypush-1.0.4/platypush/migrations/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.753479 platypush-1.0.4/platypush/migrations/alembic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.753479 platypush-1.0.4/platypush/migrations/alembic/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     3540 2024-05-31 18:03:15.000000 platypush-1.0.4/platypush/migrations/alembic/__pycache__/env.cpython-312.pyc
+-rw-r--r--   0 root         (0) root         (0)     2747 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/migrations/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      510 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/migrations/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.753479 platypush-1.0.4/platypush/migrations/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     1343 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/migrations/alembic/versions/0876439530cb_added_password_hashing_parameters_to_.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.753479 platypush-1.0.4/platypush/migrations/alembic/versions/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     2247 2024-05-31 18:03:15.000000 platypush-1.0.4/platypush/migrations/alembic/versions/__pycache__/0876439530cb_added_password_hashing_parameters_to_.cpython-312.pyc
+-rw-r--r--   0 root         (0) root         (0)     5485 2024-05-31 18:03:15.000000 platypush-1.0.4/platypush/migrations/alembic/versions/__pycache__/c39ac404119b_migrate_variable_table.cpython-312.pyc
+-rw-r--r--   0 root         (0) root         (0)      619 2024-05-31 18:03:15.000000 platypush-1.0.4/platypush/migrations/alembic/versions/__pycache__/d030953a871d_base_alembic_version.cpython-312.pyc
+-rw-r--r--   0 root         (0) root         (0)     4308 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/migrations/alembic/versions/c39ac404119b_migrate_variable_table.py
+-rw-r--r--   0 root         (0) root         (0)      304 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/migrations/alembic/versions/d030953a871d_base_alembic_version.py
+-rw-r--r--   0 root         (0) root         (0)     3180 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/migrations/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.753479 platypush-1.0.4/platypush/platydock/
+-rwxr-xr-x   0 root         (0) root         (0)     9341 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/platydock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/platydock/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.756812 platypush-1.0.4/platypush/platyvenv/
+-rwxr-xr-x   0 root         (0) root         (0)     6281 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/platyvenv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/platyvenv/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.756812 platypush-1.0.4/platypush/plugins/
+-rw-r--r--   0 root         (0) root         (0)    10705 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.756812 platypush-1.0.4/platypush/plugins/adafruit/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/adafruit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.756812 platypush-1.0.4/platypush/plugins/adafruit/io/
+-rw-r--r--   0 root         (0) root         (0)    10842 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/adafruit/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/adafruit/io/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.756812 platypush-1.0.4/platypush/plugins/alarm/
+-rw-r--r--   0 root         (0) root         (0)    21516 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/alarm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13182 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/alarm/_model.py
+-rw-r--r--   0 root         (0) root         (0)      493 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/alarm/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.756812 platypush-1.0.4/platypush/plugins/application/
+-rw-r--r--   0 root         (0) root         (0)     2929 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/application/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      150 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/application/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.756812 platypush-1.0.4/platypush/plugins/arduino/
+-rw-r--r--   0 root         (0) root         (0)    17864 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/arduino/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      398 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/arduino/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.756812 platypush-1.0.4/platypush/plugins/assistant/
+-rw-r--r--   0 root         (0) root         (0)    11081 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/assistant/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.756812 platypush-1.0.4/platypush/plugins/assistant/google/
+-rw-r--r--   0 root         (0) root         (0)    11883 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/assistant/google/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2209 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/assistant/google/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.756812 platypush-1.0.4/platypush/plugins/assistant/picovoice/
+-rw-r--r--   0 root         (0) root         (0)    30836 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/assistant/picovoice/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14075 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/assistant/picovoice/_assistant.py
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/assistant/picovoice/_context.py
+-rw-r--r--   0 root         (0) root         (0)      175 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/assistant/picovoice/_intent.py
+-rw-r--r--   0 root         (0) root         (0)     5022 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/assistant/picovoice/_recorder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.760146 platypush-1.0.4/platypush/plugins/assistant/picovoice/_speech/
+-rw-r--r--   0 root         (0) root         (0)       71 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/assistant/picovoice/_speech/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5147 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/assistant/picovoice/_speech/_base.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/assistant/picovoice/_speech/_intent.py
+-rw-r--r--   0 root         (0) root         (0)     6431 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/assistant/picovoice/_speech/_processor.py
+-rw-r--r--   0 root         (0) root         (0)     3485 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/assistant/picovoice/_speech/_stt.py
+-rw-r--r--   0 root         (0) root         (0)      233 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/assistant/picovoice/_state.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/assistant/picovoice/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.760146 platypush-1.0.4/platypush/plugins/autoremote/
+-rw-r--r--   0 root         (0) root         (0)     8111 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/autoremote/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      149 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/autoremote/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.760146 platypush-1.0.4/platypush/plugins/bluetooth/
+-rw-r--r--   0 root         (0) root         (0)    23785 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.760146 platypush-1.0.4/platypush/plugins/bluetooth/_ble/
+-rw-r--r--   0 root         (0) root         (0)       80 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_ble/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      815 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_ble/_cache.py
+-rw-r--r--   0 root         (0) root         (0)      477 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_ble/_connection.py
+-rw-r--r--   0 root         (0) root         (0)     7960 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_ble/_event_handler.py
+-rw-r--r--   0 root         (0) root         (0)    14830 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_ble/_manager.py
+-rw-r--r--   0 root         (0) root         (0)    11919 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_ble/_mappers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.760146 platypush-1.0.4/platypush/plugins/bluetooth/_ble/_plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_ble/_plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1847 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_ble/_plugins/switchbot.py
+-rw-r--r--   0 root         (0) root         (0)     6367 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_cache.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.763479 platypush-1.0.4/platypush/plugins/bluetooth/_file/
+-rw-r--r--   0 root         (0) root         (0)       58 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_file/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3025 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_file/sender.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.763479 platypush-1.0.4/platypush/plugins/bluetooth/_legacy/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_legacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.763479 platypush-1.0.4/platypush/plugins/bluetooth/_legacy/_manager/
+-rw-r--r--   0 root         (0) root         (0)       62 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_legacy/_manager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12004 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_legacy/_manager/_base.py
+-rw-r--r--   0 root         (0) root         (0)     1882 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_legacy/_manager/_connection.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_legacy/_manager/_service.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_legacy/_manager/_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.763479 platypush-1.0.4/platypush/plugins/bluetooth/_legacy/_model/
+-rw-r--r--   0 root         (0) root         (0)      170 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_legacy/_model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2475 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_legacy/_model/_device.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_legacy/_model/_services.py
+-rw-r--r--   0 root         (0) root         (0)     6000 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.763479 platypush-1.0.4/platypush/plugins/bluetooth/_model/
+-rw-r--r--   0 root         (0) root         (0)      267 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.763479 platypush-1.0.4/platypush/plugins/bluetooth/_model/_classes/
+-rw-r--r--   0 root         (0) root         (0)      185 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_model/_classes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_model/_classes/_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.763479 platypush-1.0.4/platypush/plugins/bluetooth/_model/_classes/_device/
+-rw-r--r--   0 root         (0) root         (0)      138 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_model/_classes/_device/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      907 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_model/_classes/_device/_major.py
+-rw-r--r--   0 root         (0) root         (0)     9793 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_model/_classes/_device/_minor.py
+-rw-r--r--   0 root         (0) root         (0)      833 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_model/_classes/_service.py
+-rw-r--r--   0 root         (0) root         (0)      884 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_model/_protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.763479 platypush-1.0.4/platypush/plugins/bluetooth/_model/_service/
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_model/_service/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6234 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_model/_service/_directory.py
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_model/_service/_directory.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.766812 platypush-1.0.4/platypush/plugins/bluetooth/_plugins/
+-rw-r--r--   0 root         (0) root         (0)      125 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_plugins/_base.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_plugins/_scanner.py
+-rw-r--r--   0 root         (0) root         (0)     1337 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/_types.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/manifest.json
+-rw-r--r--   0 root         (0) root         (0)      306 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/bluetooth/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.766812 platypush-1.0.4/platypush/plugins/calendar/
+-rw-r--r--   0 root         (0) root         (0)     4150 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/calendar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.766812 platypush-1.0.4/platypush/plugins/calendar/ical/
+-rw-r--r--   0 root         (0) root         (0)     3862 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/calendar/ical/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/calendar/ical/manifest.json
+-rw-r--r--   0 root         (0) root         (0)      147 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/calendar/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.766812 platypush-1.0.4/platypush/plugins/camera/
+-rw-r--r--   0 root         (0) root         (0)    39220 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.766812 platypush-1.0.4/platypush/plugins/camera/android/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/android/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.766812 platypush-1.0.4/platypush/plugins/camera/android/ipcam/
+-rw-r--r--   0 root         (0) root         (0)    11555 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/android/ipcam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/android/ipcam/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.766812 platypush-1.0.4/platypush/plugins/camera/cv/
+-rw-r--r--   0 root         (0) root         (0)     3168 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/cv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      599 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/cv/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.766812 platypush-1.0.4/platypush/plugins/camera/ffmpeg/
+-rw-r--r--   0 root         (0) root         (0)     3722 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/ffmpeg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      552 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/ffmpeg/manifest.json
+-rw-r--r--   0 root         (0) root         (0)      472 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/ffmpeg/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.766812 platypush-1.0.4/platypush/plugins/camera/gstreamer/
+-rw-r--r--   0 root         (0) root         (0)     2627 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/gstreamer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      699 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/gstreamer/manifest.json
+-rw-r--r--   0 root         (0) root         (0)      201 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/gstreamer/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.766812 platypush-1.0.4/platypush/plugins/camera/ir/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/ir/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.766812 platypush-1.0.4/platypush/plugins/camera/ir/mlx90640/
+-rw-r--r--   0 root         (0) root         (0)     4028 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/ir/mlx90640/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      574 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/ir/mlx90640/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.770146 platypush-1.0.4/platypush/plugins/camera/model/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/model/camera.py
+-rw-r--r--   0 root         (0) root         (0)      256 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/model/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.770146 platypush-1.0.4/platypush/plugins/camera/model/writer/
+-rw-r--r--   0 root         (0) root         (0)     3919 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/model/writer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1233 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/model/writer/cv.py
+-rw-r--r--   0 root         (0) root         (0)     6138 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/model/writer/ffmpeg.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/model/writer/image.py
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/model/writer/index.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.770146 platypush-1.0.4/platypush/plugins/camera/model/writer/preview/
+-rw-r--r--   0 root         (0) root         (0)      855 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/model/writer/preview/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1618 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/model/writer/preview/ffplay.py
+-rw-r--r--   0 root         (0) root         (0)     1837 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/model/writer/preview/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.770146 platypush-1.0.4/platypush/plugins/camera/model/writer/preview/wx/
+-rw-r--r--   0 root         (0) root         (0)     1405 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/model/writer/preview/wx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/model/writer/preview/wx/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.770146 platypush-1.0.4/platypush/plugins/camera/pi/
+-rw-r--r--   0 root         (0) root         (0)    10390 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/pi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.770146 platypush-1.0.4/platypush/plugins/camera/pi/legacy/
+-rw-r--r--   0 root         (0) root         (0)    10679 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/pi/legacy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      575 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/pi/legacy/manifest.json
+-rw-r--r--   0 root         (0) root         (0)     1383 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/pi/legacy/model.py
+-rw-r--r--   0 root         (0) root         (0)      569 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/pi/manifest.json
+-rw-r--r--   0 root         (0) root         (0)      620 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/camera/pi/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.770146 platypush-1.0.4/platypush/plugins/chat/
+-rw-r--r--   0 root         (0) root         (0)      209 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/chat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.770146 platypush-1.0.4/platypush/plugins/clipboard/
+-rw-r--r--   0 root         (0) root         (0)     1644 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/clipboard/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      402 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/clipboard/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.770146 platypush-1.0.4/platypush/plugins/config/
+-rw-r--r--   0 root         (0) root         (0)     1547 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      145 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/config/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.773479 platypush-1.0.4/platypush/plugins/csv/
+-rw-r--r--   0 root         (0) root         (0)     6529 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/csv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      142 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/csv/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.773479 platypush-1.0.4/platypush/plugins/cups/
+-rw-r--r--   0 root         (0) root         (0)    12657 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/cups/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/cups/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.773479 platypush-1.0.4/platypush/plugins/db/
+-rw-r--r--   0 root         (0) root         (0)    18785 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      141 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/db/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.773479 platypush-1.0.4/platypush/plugins/dbus/
+-rw-r--r--   0 root         (0) root         (0)    16340 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/dbus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      583 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/dbus/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.773479 platypush-1.0.4/platypush/plugins/dropbox/
+-rw-r--r--   0 root         (0) root         (0)    14982 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/dropbox/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      322 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/dropbox/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.773479 platypush-1.0.4/platypush/plugins/entities/
+-rw-r--r--   0 root         (0) root         (0)     9492 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/entities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      107 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/entities/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.773479 platypush-1.0.4/platypush/plugins/esp/
+-rw-r--r--   0 root         (0) root         (0)    58863 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/esp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      142 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/esp/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.773479 platypush-1.0.4/platypush/plugins/esp/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/esp/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12447 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/esp/models/connection.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/esp/models/device.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.773479 platypush-1.0.4/platypush/plugins/ffmpeg/
+-rw-r--r--   0 root         (0) root         (0)     5701 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/ffmpeg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      368 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/ffmpeg/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.773479 platypush-1.0.4/platypush/plugins/file/
+-rw-r--r--   0 root         (0) root         (0)     5488 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/file/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      143 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/file/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.776813 platypush-1.0.4/platypush/plugins/file/monitor/
+-rw-r--r--   0 root         (0) root         (0)     5251 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/file/monitor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.776813 platypush-1.0.4/platypush/plugins/file/monitor/entities/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/file/monitor/entities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3477 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/file/monitor/entities/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/file/monitor/entities/resources.py
+-rw-r--r--   0 root         (0) root         (0)      562 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/file/monitor/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.776813 platypush-1.0.4/platypush/plugins/flic/
+-rw-r--r--   0 root         (0) root         (0)     4892 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/flic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32369 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/flic/fliclib.py
+-rw-r--r--   0 root         (0) root         (0)      201 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/flic/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.776813 platypush-1.0.4/platypush/plugins/foursquare/
+-rw-r--r--   0 root         (0) root         (0)    16769 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/foursquare/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      220 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/foursquare/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.776813 platypush-1.0.4/platypush/plugins/github/
+-rw-r--r--   0 root         (0) root         (0)     9312 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/github/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/github/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.776813 platypush-1.0.4/platypush/plugins/google/
+-rw-r--r--   0 root         (0) root         (0)     4662 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/google/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.776813 platypush-1.0.4/platypush/plugins/google/calendar/
+-rw-r--r--   0 root         (0) root         (0)     3640 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/google/calendar/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      823 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/google/calendar/manifest.json
+-rw-r--r--   0 root         (0) root         (0)     4747 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/google/credentials.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.776813 platypush-1.0.4/platypush/plugins/google/drive/
+-rw-r--r--   0 root         (0) root         (0)    13292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/google/drive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      820 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/google/drive/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.776813 platypush-1.0.4/platypush/plugins/google/mail/
+-rw-r--r--   0 root         (0) root         (0)     5756 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/google/mail/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      819 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/google/mail/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.776813 platypush-1.0.4/platypush/plugins/google/maps/
+-rw-r--r--   0 root         (0) root         (0)    10525 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/google/maps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      819 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/google/maps/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.776813 platypush-1.0.4/platypush/plugins/google/pubsub/
+-rw-r--r--   0 root         (0) root         (0)     7863 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/google/pubsub/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      928 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/google/pubsub/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.780146 platypush-1.0.4/platypush/plugins/google/translate/
+-rw-r--r--   0 root         (0) root         (0)     4693 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/google/translate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      858 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/google/translate/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.780146 platypush-1.0.4/platypush/plugins/gotify/
+-rw-r--r--   0 root         (0) root         (0)     6992 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/gotify/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      203 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/gotify/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.780146 platypush-1.0.4/platypush/plugins/gpio/
+-rw-r--r--   0 root         (0) root         (0)     6466 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/gpio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      221 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/gpio/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.780146 platypush-1.0.4/platypush/plugins/gpio/zeroborg/
+-rw-r--r--   0 root         (0) root         (0)     5368 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/gpio/zeroborg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.780146 platypush-1.0.4/platypush/plugins/gpio/zeroborg/lib/
+-rw-r--r--   0 root         (0) root         (0)    31497 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/gpio/zeroborg/lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/gpio/zeroborg/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.780146 platypush-1.0.4/platypush/plugins/gps/
+-rw-r--r--   0 root         (0) root         (0)     6667 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/gps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1041 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/gps/_model.py
+-rw-r--r--   0 root         (0) root         (0)      611 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/gps/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.780146 platypush-1.0.4/platypush/plugins/graphite/
+-rw-r--r--   0 root         (0) root         (0)     1819 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/graphite/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      147 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/graphite/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.780146 platypush-1.0.4/platypush/plugins/hid/
+-rw-r--r--   0 root         (0) root         (0)     8254 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/hid/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      666 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/hid/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.780146 platypush-1.0.4/platypush/plugins/http/
+-rw-r--r--   0 root         (0) root         (0)     5599 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      143 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/http/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.780146 platypush-1.0.4/platypush/plugins/http/webpage/
+-rw-r--r--   0 root         (0) root         (0)    11483 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/http/webpage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      552 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/http/webpage/manifest.json
+-rwxr-xr-x   0 root         (0) root         (0)     1043 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/http/webpage/mercury-parser.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.783480 platypush-1.0.4/platypush/plugins/ifttt/
+-rw-r--r--   0 root         (0) root         (0)     2141 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/ifttt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      144 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/ifttt/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.783480 platypush-1.0.4/platypush/plugins/inspect/
+-rw-r--r--   0 root         (0) root         (0)    10852 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/inspect/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7553 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/inspect/_cache.py
+-rw-r--r--   0 root         (0) root         (0)      578 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/inspect/_serialize.py
+-rw-r--r--   0 root         (0) root         (0)      146 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/inspect/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.783480 platypush-1.0.4/platypush/plugins/irc/
+-rw-r--r--   0 root         (0) root         (0)    13611 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/irc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19629 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/irc/_bot.py
+-rw-r--r--   0 root         (0) root         (0)     2013 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/irc/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.783480 platypush-1.0.4/platypush/plugins/joystick/
+-rw-r--r--   0 root         (0) root         (0)     3720 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/joystick/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   119434 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/joystick/_inputs.py
+-rw-r--r--   0 root         (0) root         (0)     6133 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/joystick/_manager.py
+-rw-r--r--   0 root         (0) root         (0)      967 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/joystick/_state.py
+-rw-r--r--   0 root         (0) root         (0)      324 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/joystick/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.783480 platypush-1.0.4/platypush/plugins/kafka/
+-rw-r--r--   0 root         (0) root         (0)     8234 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/kafka/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      322 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/kafka/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.783480 platypush-1.0.4/platypush/plugins/lastfm/
+-rw-r--r--   0 root         (0) root         (0)     6134 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/lastfm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      362 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/lastfm/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.783480 platypush-1.0.4/platypush/plugins/lcd/
+-rw-r--r--   0 root         (0) root         (0)     5771 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/lcd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.783480 platypush-1.0.4/platypush/plugins/lcd/gpio/
+-rw-r--r--   0 root         (0) root         (0)     3666 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/lcd/gpio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      190 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/lcd/gpio/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.786813 platypush-1.0.4/platypush/plugins/lcd/i2c/
+-rw-r--r--   0 root         (0) root         (0)     3492 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/lcd/i2c/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      189 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/lcd/i2c/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.786813 platypush-1.0.4/platypush/plugins/leap/
+-rw-r--r--   0 root         (0) root         (0)     9165 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/leap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      463 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/leap/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.786813 platypush-1.0.4/platypush/plugins/light/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/light/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.786813 platypush-1.0.4/platypush/plugins/light/hue/
+-rw-r--r--   0 root         (0) root         (0)    41305 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/light/hue/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      477 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/light/hue/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.786813 platypush-1.0.4/platypush/plugins/linode/
+-rw-r--r--   0 root         (0) root         (0)     8350 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/linode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      252 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/linode/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.786813 platypush-1.0.4/platypush/plugins/log/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/log/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.786813 platypush-1.0.4/platypush/plugins/log/http/
+-rw-r--r--   0 root         (0) root         (0)     5589 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/log/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/log/http/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.786813 platypush-1.0.4/platypush/plugins/logger/
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/logger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      145 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/logger/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.786813 platypush-1.0.4/platypush/plugins/luma/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/luma/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.786813 platypush-1.0.4/platypush/plugins/luma/oled/
+-rw-r--r--   0 root         (0) root         (0)    14122 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/luma/oled/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      175 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/luma/oled/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.786813 platypush-1.0.4/platypush/plugins/mail/
+-rw-r--r--   0 root         (0) root         (0)    39125 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mail/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3415 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mail/_account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.786813 platypush-1.0.4/platypush/plugins/mail/_model/
+-rw-r--r--   0 root         (0) root         (0)      319 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mail/_model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.790146 platypush-1.0.4/platypush/plugins/mail/_model/_config/
+-rw-r--r--   0 root         (0) root         (0)      127 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mail/_model/_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mail/_model/_config/_account.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mail/_model/_config/_server.py
+-rw-r--r--   0 root         (0) root         (0)     7195 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mail/_model/_mail.py
+-rw-r--r--   0 root         (0) root         (0)      528 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mail/_model/_transport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.790146 platypush-1.0.4/platypush/plugins/mail/_plugin/
+-rw-r--r--   0 root         (0) root         (0)      228 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mail/_plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3463 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mail/_plugin/_base.py
+-rw-r--r--   0 root         (0) root         (0)     3609 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mail/_plugin/_in.py
+-rw-r--r--   0 root         (0) root         (0)     4164 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mail/_plugin/_out.py
+-rw-r--r--   0 root         (0) root         (0)      937 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mail/_plugin/_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2203 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mail/_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.790146 platypush-1.0.4/platypush/plugins/mail/imap/
+-rw-r--r--   0 root         (0) root         (0)    10322 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mail/imap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      619 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mail/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.790146 platypush-1.0.4/platypush/plugins/mail/smtp/
+-rw-r--r--   0 root         (0) root         (0)     2044 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mail/smtp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.790146 platypush-1.0.4/platypush/plugins/mailgun/
+-rw-r--r--   0 root         (0) root         (0)     2988 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mailgun/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mailgun/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.790146 platypush-1.0.4/platypush/plugins/mastodon/
+-rw-r--r--   0 root         (0) root         (0)    55621 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mastodon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      107 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mastodon/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.790146 platypush-1.0.4/platypush/plugins/matrix/
+-rw-r--r--   0 root         (0) root         (0)    29149 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/matrix/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30994 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/matrix/client.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/matrix/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.790146 platypush-1.0.4/platypush/plugins/media/
+-rw-r--r--   0 root         (0) root         (0)    25014 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.793480 platypush-1.0.4/platypush/plugins/media/chromecast/
+-rw-r--r--   0 root         (0) root         (0)    23031 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/chromecast/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2398 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/chromecast/_listener.py
+-rw-r--r--   0 root         (0) root         (0)      861 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/chromecast/_subtitles.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/chromecast/_utils.py
+-rw-r--r--   0 root         (0) root         (0)      343 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/chromecast/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.793480 platypush-1.0.4/platypush/plugins/media/gstreamer/
+-rw-r--r--   0 root         (0) root         (0)     7127 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/gstreamer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      471 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/gstreamer/manifest.json
+-rw-r--r--   0 root         (0) root         (0)     1783 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/gstreamer/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.793480 platypush-1.0.4/platypush/plugins/media/jellyfin/
+-rw-r--r--   0 root         (0) root         (0)    12071 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/jellyfin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      113 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/jellyfin/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.793480 platypush-1.0.4/platypush/plugins/media/kodi/
+-rw-r--r--   0 root         (0) root         (0)    22266 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/kodi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      273 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/kodi/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.793480 platypush-1.0.4/platypush/plugins/media/lib/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3392 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/lib/plexcast.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.793480 platypush-1.0.4/platypush/plugins/media/mplayer/
+-rw-r--r--   0 root         (0) root         (0)    25835 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/mplayer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/mplayer/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.793480 platypush-1.0.4/platypush/plugins/media/mpv/
+-rw-r--r--   0 root         (0) root         (0)    15631 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/mpv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      485 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/mpv/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.793480 platypush-1.0.4/platypush/plugins/media/omxplayer/
+-rw-r--r--   0 root         (0) root         (0)    12995 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/omxplayer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      269 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/omxplayer/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.793480 platypush-1.0.4/platypush/plugins/media/plex/
+-rw-r--r--   0 root         (0) root         (0)    15190 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/plex/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      174 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/plex/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.796813 platypush-1.0.4/platypush/plugins/media/search/
+-rw-r--r--   0 root         (0) root         (0)      901 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/search/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      808 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/search/jellyfin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.796813 platypush-1.0.4/platypush/plugins/media/search/local/
+-rw-r--r--   0 root         (0) root         (0)    10121 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/search/local/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2749 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/search/local/db.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/search/local/metadata.py
+-rw-r--r--   0 root         (0) root         (0)     2283 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/search/plex.py
+-rw-r--r--   0 root         (0) root         (0)      521 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/search/torrent.py
+-rw-r--r--   0 root         (0) root         (0)      595 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/search/youtube.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.796813 platypush-1.0.4/platypush/plugins/media/subtitles/
+-rw-r--r--   0 root         (0) root         (0)     7137 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/subtitles/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      262 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/subtitles/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.796813 platypush-1.0.4/platypush/plugins/media/vlc/
+-rw-r--r--   0 root         (0) root         (0)    16443 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/vlc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      468 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/vlc/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.796813 platypush-1.0.4/platypush/plugins/media/webtorrent/
+-rw-r--r--   0 root         (0) root         (0)    17156 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/webtorrent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      155 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/media/webtorrent/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.796813 platypush-1.0.4/platypush/plugins/midi/
+-rw-r--r--   0 root         (0) root         (0)    10804 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/midi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5467 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/midi/_model.py
+-rw-r--r--   0 root         (0) root         (0)      641 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/midi/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.796813 platypush-1.0.4/platypush/plugins/ml/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/ml/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.796813 platypush-1.0.4/platypush/plugins/ml/cv/
+-rw-r--r--   0 root         (0) root         (0)     2822 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/ml/cv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      479 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/ml/cv/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.796813 platypush-1.0.4/platypush/plugins/mobile/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mobile/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.796813 platypush-1.0.4/platypush/plugins/mobile/join/
+-rw-r--r--   0 root         (0) root         (0)    16171 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mobile/join/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      150 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mobile/join/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.796813 platypush-1.0.4/platypush/plugins/mqtt/
+-rw-r--r--   0 root         (0) root         (0)    18655 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mqtt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7604 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mqtt/_client.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/mqtt/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.800147 platypush-1.0.4/platypush/plugins/music/
+-rw-r--r--   0 root         (0) root         (0)     2937 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/music/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.800147 platypush-1.0.4/platypush/plugins/music/mopidy/
+-rw-r--r--   0 root         (0) root         (0)    35393 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/music/mopidy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16095 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/music/mopidy/_client.py
+-rw-r--r--   0 root         (0) root         (0)       62 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/music/mopidy/_common.py
+-rw-r--r--   0 root         (0) root         (0)      439 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/music/mopidy/_conf.py
+-rw-r--r--   0 root         (0) root         (0)      207 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/music/mopidy/_exc.py
+-rw-r--r--   0 root         (0) root         (0)      859 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/music/mopidy/_playlist.py
+-rw-r--r--   0 root         (0) root         (0)     1266 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/music/mopidy/_status.py
+-rw-r--r--   0 root         (0) root         (0)     1414 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/music/mopidy/_sync.py
+-rw-r--r--   0 root         (0) root         (0)     1627 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/music/mopidy/_task.py
+-rw-r--r--   0 root         (0) root         (0)     1480 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/music/mopidy/_track.py
+-rw-r--r--   0 root         (0) root         (0)      898 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/music/mopidy/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.800147 platypush-1.0.4/platypush/plugins/music/mpd/
+-rw-r--r--   0 root         (0) root         (0)    27060 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/music/mpd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      175 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/music/mpd/_conf.py
+-rw-r--r--   0 root         (0) root         (0)     5295 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/music/mpd/_listener.py
+-rw-r--r--   0 root         (0) root         (0)      662 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/music/mpd/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.800147 platypush-1.0.4/platypush/plugins/music/snapcast/
+-rw-r--r--   0 root         (0) root         (0)    31741 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/music/snapcast/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      153 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/music/snapcast/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.800147 platypush-1.0.4/platypush/plugins/music/spotify/
+-rw-r--r--   0 root         (0) root         (0)    36503 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/music/spotify/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      152 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/music/spotify/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.803480 platypush-1.0.4/platypush/plugins/music/tidal/
+-rw-r--r--   0 root         (0) root         (0)    12571 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/music/tidal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      260 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/music/tidal/manifest.json
+-rw-r--r--   0 root         (0) root         (0)     1597 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/music/tidal/workers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.803480 platypush-1.0.4/platypush/plugins/nextcloud/
+-rw-r--r--   0 root         (0) root         (0)    44114 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/nextcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      389 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/nextcloud/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.803480 platypush-1.0.4/platypush/plugins/nfc/
+-rw-r--r--   0 root         (0) root         (0)     9106 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/nfc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      431 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/nfc/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.803480 platypush-1.0.4/platypush/plugins/ngrok/
+-rw-r--r--   0 root         (0) root         (0)     5900 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/ngrok/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      569 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/ngrok/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.803480 platypush-1.0.4/platypush/plugins/nmap/
+-rw-r--r--   0 root         (0) root         (0)      976 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/nmap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      143 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/nmap/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.803480 platypush-1.0.4/platypush/plugins/ntfy/
+-rw-r--r--   0 root         (0) root         (0)     9817 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/ntfy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      199 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/ntfy/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.803480 platypush-1.0.4/platypush/plugins/openai/
+-rw-r--r--   0 root         (0) root         (0)    10127 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/openai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       87 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/openai/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.803480 platypush-1.0.4/platypush/plugins/otp/
+-rw-r--r--   0 root         (0) root         (0)     8357 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/otp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      352 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/otp/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.803480 platypush-1.0.4/platypush/plugins/pihole/
+-rw-r--r--   0 root         (0) root         (0)    16748 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/pihole/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      145 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/pihole/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.803480 platypush-1.0.4/platypush/plugins/ping/
+-rw-r--r--   0 root         (0) root         (0)     8189 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/ping/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      422 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/ping/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.803480 platypush-1.0.4/platypush/plugins/pushbullet/
+-rw-r--r--   0 root         (0) root         (0)    13984 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/pushbullet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1395 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/pushbullet/listener.py
+-rw-r--r--   0 root         (0) root         (0)      772 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/pushbullet/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.806814 platypush-1.0.4/platypush/plugins/pwm/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/pwm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.806814 platypush-1.0.4/platypush/plugins/pwm/pca9685/
+-rw-r--r--   0 root         (0) root         (0)     5791 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/pwm/pca9685/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      198 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/pwm/pca9685/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.806814 platypush-1.0.4/platypush/plugins/qrcode/
+-rw-r--r--   0 root         (0) root         (0)     6369 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/qrcode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      741 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/qrcode/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.806814 platypush-1.0.4/platypush/plugins/redis/
+-rw-r--r--   0 root         (0) root         (0)     2786 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      144 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/redis/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.806814 platypush-1.0.4/platypush/plugins/rss/
+-rw-r--r--   0 root         (0) root         (0)    13326 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/rss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      628 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/rss/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.806814 platypush-1.0.4/platypush/plugins/rtorrent/
+-rw-r--r--   0 root         (0) root         (0)    18201 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/rtorrent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/rtorrent/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.806814 platypush-1.0.4/platypush/plugins/sensor/
+-rw-r--r--   0 root         (0) root         (0)    14853 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sensor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.806814 platypush-1.0.4/platypush/plugins/sensor/bme280/
+-rw-r--r--   0 root         (0) root         (0)     3706 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sensor/bme280/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      409 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sensor/bme280/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.806814 platypush-1.0.4/platypush/plugins/sensor/dht/
+-rw-r--r--   0 root         (0) root         (0)     4084 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sensor/dht/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sensor/dht/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.806814 platypush-1.0.4/platypush/plugins/sensor/distance/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sensor/distance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.806814 platypush-1.0.4/platypush/plugins/sensor/distance/vl53l1x/
+-rw-r--r--   0 root         (0) root         (0)     3546 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sensor/distance/vl53l1x/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      271 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sensor/distance/vl53l1x/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.806814 platypush-1.0.4/platypush/plugins/sensor/envirophat/
+-rw-r--r--   0 root         (0) root         (0)     5016 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sensor/envirophat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      408 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sensor/envirophat/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.806814 platypush-1.0.4/platypush/plugins/sensor/hcsr04/
+-rw-r--r--   0 root         (0) root         (0)     5554 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sensor/hcsr04/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      470 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sensor/hcsr04/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.810147 platypush-1.0.4/platypush/plugins/sensor/lis3dh/
+-rw-r--r--   0 root         (0) root         (0)     2258 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sensor/lis3dh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.810147 platypush-1.0.4/platypush/plugins/sensor/lis3dh/lib/
+-rw-r--r--   0 root         (0) root         (0)    11260 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sensor/lis3dh/lib/LIS3DH.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sensor/lis3dh/lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      407 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sensor/lis3dh/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.810147 platypush-1.0.4/platypush/plugins/sensor/ltr559/
+-rw-r--r--   0 root         (0) root         (0)     2132 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sensor/ltr559/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sensor/ltr559/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.810147 platypush-1.0.4/platypush/plugins/sensor/mcp3008/
+-rw-r--r--   0 root         (0) root         (0)     6825 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sensor/mcp3008/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sensor/mcp3008/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.810147 platypush-1.0.4/platypush/plugins/sensor/pmw3901/
+-rw-r--r--   0 root         (0) root         (0)     5295 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sensor/pmw3901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      402 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sensor/pmw3901/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.810147 platypush-1.0.4/platypush/plugins/serial/
+-rw-r--r--   0 root         (0) root         (0)    14631 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/serial/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      436 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/serial/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.810147 platypush-1.0.4/platypush/plugins/shell/
+-rw-r--r--   0 root         (0) root         (0)     4257 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/shell/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      144 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/shell/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.810147 platypush-1.0.4/platypush/plugins/slack/
+-rw-r--r--   0 root         (0) root         (0)    10161 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/slack/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      661 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/slack/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.810147 platypush-1.0.4/platypush/plugins/smartthings/
+-rw-r--r--   0 root         (0) root         (0)    35133 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/smartthings/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17121 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/smartthings/_mappers.py
+-rw-r--r--   0 root         (0) root         (0)      181 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/smartthings/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.810147 platypush-1.0.4/platypush/plugins/sound/
+-rw-r--r--   0 root         (0) root         (0)    18537 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.813481 platypush-1.0.4/platypush/plugins/sound/_converters/
+-rw-r--r--   0 root         (0) root         (0)      295 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_converters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8995 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_converters/_base.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_converters/_from_raw.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_converters/_to_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.813481 platypush-1.0.4/platypush/plugins/sound/_manager/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_manager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3687 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_manager/_device.py
+-rw-r--r--   0 root         (0) root         (0)    10651 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_manager/_main.py
+-rw-r--r--   0 root         (0) root         (0)     7477 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_manager/_stream.py
+-rw-r--r--   0 root         (0) root         (0)      737 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.813481 platypush-1.0.4/platypush/plugins/sound/_streams/
+-rw-r--r--   0 root         (0) root         (0)      161 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_streams/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15916 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_streams/_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.813481 platypush-1.0.4/platypush/plugins/sound/_streams/_player/
+-rw-r--r--   0 root         (0) root         (0)       58 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_streams/_player/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2944 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_streams/_player/_base.py
+-rw-r--r--   0 root         (0) root         (0)      938 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_streams/_player/_resource.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.813481 platypush-1.0.4/platypush/plugins/sound/_streams/_player/_synth/
+-rw-r--r--   0 root         (0) root         (0)      105 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_streams/_player/_synth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2527 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_streams/_player/_synth/_base.py
+-rw-r--r--   0 root         (0) root         (0)     2999 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_streams/_player/_synth/_generator.py
+-rw-r--r--   0 root         (0) root         (0)     3412 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_streams/_player/_synth/_mix.py
+-rw-r--r--   0 root         (0) root         (0)     2442 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_streams/_player/_synth/_output.py
+-rw-r--r--   0 root         (0) root         (0)     3114 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_streams/_player/_synth/_parser.py
+-rw-r--r--   0 root         (0) root         (0)     3543 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_streams/_player/_synth/_player.py
+-rw-r--r--   0 root         (0) root         (0)     7199 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_streams/_player/_synth/_sound.py
+-rw-r--r--   0 root         (0) root         (0)     2718 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_streams/_recorder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.816814 platypush-1.0.4/platypush/plugins/sound/_utils/
+-rw-r--r--   0 root         (0) root         (0)       71 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      771 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/_utils/_convert.py
+-rw-r--r--   0 root         (0) root         (0)     1280 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sound/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.816814 platypush-1.0.4/platypush/plugins/ssh/
+-rw-r--r--   0 root         (0) root         (0)    29807 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/ssh/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      369 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/ssh/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.816814 platypush-1.0.4/platypush/plugins/ssh/tunnel/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/ssh/tunnel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/ssh/tunnel/forward.py
+-rw-r--r--   0 root         (0) root         (0)     1985 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/ssh/tunnel/reverse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.816814 platypush-1.0.4/platypush/plugins/sun/
+-rw-r--r--   0 root         (0) root         (0)     3509 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sun/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      274 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/sun/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.816814 platypush-1.0.4/platypush/plugins/switch/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/switch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.816814 platypush-1.0.4/platypush/plugins/switch/tplink/
+-rw-r--r--   0 root         (0) root         (0)     7615 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/switch/tplink/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      177 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/switch/tplink/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.816814 platypush-1.0.4/platypush/plugins/switch/wemo/
+-rw-r--r--   0 root         (0) root         (0)     6684 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/switch/wemo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2329 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/switch/wemo/lib.py
+-rw-r--r--   0 root         (0) root         (0)      150 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/switch/wemo/manifest.json
+-rw-r--r--   0 root         (0) root         (0)     1005 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/switch/wemo/scanner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.816814 platypush-1.0.4/platypush/plugins/switchbot/
+-rw-r--r--   0 root         (0) root         (0)    37338 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/switchbot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      838 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/switchbot/_constants.py
+-rw-r--r--   0 root         (0) root         (0)     4309 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/switchbot/_setters.py
+-rw-r--r--   0 root         (0) root         (0)      148 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/switchbot/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.816814 platypush-1.0.4/platypush/plugins/system/
+-rw-r--r--   0 root         (0) root         (0)    21396 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/system/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/system/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.820148 platypush-1.0.4/platypush/plugins/tcp/
+-rw-r--r--   0 root         (0) root         (0)     3763 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/tcp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      142 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/tcp/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.820148 platypush-1.0.4/platypush/plugins/telegram/
+-rw-r--r--   0 root         (0) root         (0)    43311 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/telegram/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/telegram/_bridge.py
+-rw-r--r--   0 root         (0) root         (0)     1765 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/telegram/_model.py
+-rw-r--r--   0 root         (0) root         (0)     9092 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/telegram/_service.py
+-rw-r--r--   0 root         (0) root         (0)      429 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/telegram/_utils.py
+-rw-r--r--   0 root         (0) root         (0)      681 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/telegram/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.820148 platypush-1.0.4/platypush/plugins/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)    55458 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/tensorflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1381 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/tensorflow/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.820148 platypush-1.0.4/platypush/plugins/todoist/
+-rw-r--r--   0 root         (0) root         (0)     5812 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/todoist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      178 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/todoist/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.820148 platypush-1.0.4/platypush/plugins/torrent/
+-rw-r--r--   0 root         (0) root         (0)    21966 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/torrent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      400 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/torrent/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.820148 platypush-1.0.4/platypush/plugins/trello/
+-rw-r--r--   0 root         (0) root         (0)    36307 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/trello/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2734 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/trello/_model.py
+-rw-r--r--   0 root         (0) root         (0)      401 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/trello/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.820148 platypush-1.0.4/platypush/plugins/tts/
+-rw-r--r--   0 root         (0) root         (0)     1681 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/tts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.820148 platypush-1.0.4/platypush/plugins/tts/google/
+-rw-r--r--   0 root         (0) root         (0)     5101 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/tts/google/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      623 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/tts/google/manifest.json
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/tts/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.820148 platypush-1.0.4/platypush/plugins/tts/mimic3/
+-rw-r--r--   0 root         (0) root         (0)     3855 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/tts/mimic3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      586 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/tts/mimic3/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.823481 platypush-1.0.4/platypush/plugins/tts/picovoice/
+-rw-r--r--   0 root         (0) root         (0)     6245 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/tts/picovoice/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      507 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/tts/picovoice/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.823481 platypush-1.0.4/platypush/plugins/tv/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/tv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.823481 platypush-1.0.4/platypush/plugins/tv/samsung/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/tv/samsung/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.823481 platypush-1.0.4/platypush/plugins/tv/samsung/ws/
+-rw-r--r--   0 root         (0) root         (0)    14011 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/tv/samsung/ws/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      181 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/tv/samsung/ws/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.823481 platypush-1.0.4/platypush/plugins/twilio/
+-rw-r--r--   0 root         (0) root         (0)    29227 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/twilio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      266 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/twilio/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.823481 platypush-1.0.4/platypush/plugins/udp/
+-rw-r--r--   0 root         (0) root         (0)     1756 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/udp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      142 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/udp/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.823481 platypush-1.0.4/platypush/plugins/user/
+-rw-r--r--   0 root         (0) root         (0)     6743 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      143 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/user/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.823481 platypush-1.0.4/platypush/plugins/utils/
+-rw-r--r--   0 root         (0) root         (0)    11092 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      144 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/utils/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.823481 platypush-1.0.4/platypush/plugins/variable/
+-rw-r--r--   0 root         (0) root         (0)     5941 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/variable/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      147 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/variable/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.823481 platypush-1.0.4/platypush/plugins/wallabag/
+-rw-r--r--   0 root         (0) root         (0)    16091 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/wallabag/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       89 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/wallabag/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.823481 platypush-1.0.4/platypush/plugins/weather/
+-rw-r--r--   0 root         (0) root         (0)     4251 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/weather/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.823481 platypush-1.0.4/platypush/plugins/weather/buienradar/
+-rw-r--r--   0 root         (0) root         (0)     3168 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/weather/buienradar/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      255 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/weather/buienradar/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.823481 platypush-1.0.4/platypush/plugins/weather/openweathermap/
+-rw-r--r--   0 root         (0) root         (0)     5509 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/weather/openweathermap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      231 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/weather/openweathermap/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.826815 platypush-1.0.4/platypush/plugins/websocket/
+-rw-r--r--   0 root         (0) root         (0)     7560 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/websocket/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      274 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/websocket/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.826815 platypush-1.0.4/platypush/plugins/xmpp/
+-rw-r--r--   0 root         (0) root         (0)    23442 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      408 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_base.py
+-rw-r--r--   0 root         (0) root         (0)      605 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.826815 platypush-1.0.4/platypush/plugins/xmpp/_handlers/
+-rw-r--r--   0 root         (0) root         (0)      751 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      505 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_handlers/_base.py
+-rw-r--r--   0 root         (0) root         (0)      970 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_handlers/_connection.py
+-rw-r--r--   0 root         (0) root         (0)     4010 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_handlers/_conversation.py
+-rw-r--r--   0 root         (0) root         (0)      658 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_handlers/_discover.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_handlers/_message.py
+-rw-r--r--   0 root         (0) root         (0)      373 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_handlers/_ping.py
+-rw-r--r--   0 root         (0) root         (0)     3346 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_handlers/_presence.py
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_handlers/_pubsub.py
+-rw-r--r--   0 root         (0) root         (0)      482 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_handlers/_registry.py
+-rw-r--r--   0 root         (0) root         (0)    18552 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_handlers/_room.py
+-rw-r--r--   0 root         (0) root         (0)     3903 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_handlers/_roster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.830148 platypush-1.0.4/platypush/plugins/xmpp/_mixins/
+-rw-r--r--   0 root         (0) root         (0)      375 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_mixins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_mixins/_async.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_mixins/_base.py
+-rw-r--r--   0 root         (0) root         (0)      487 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_mixins/_config.py
+-rw-r--r--   0 root         (0) root         (0)      515 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_mixins/_event_state.py
+-rw-r--r--   0 root         (0) root         (0)     3316 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_mixins/_events.py
+-rw-r--r--   0 root         (0) root         (0)     1008 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_mixins/_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.830148 platypush-1.0.4/platypush/plugins/xmpp/_state/
+-rw-r--r--   0 root         (0) root         (0)      152 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_state/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5602 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_state/_model.py
+-rw-r--r--   0 root         (0) root         (0)     4332 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_state/_serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.830148 platypush-1.0.4/platypush/plugins/xmpp/_types/
+-rw-r--r--   0 root         (0) root         (0)      216 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      584 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_types/_errors.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_types/_invite.py
+-rw-r--r--   0 root         (0) root         (0)      338 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/_types/_presence.py
+-rw-r--r--   0 root         (0) root         (0)     2362 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/xmpp/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.830148 platypush-1.0.4/platypush/plugins/youtube/
+-rw-r--r--   0 root         (0) root         (0)     6414 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/youtube/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      337 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/youtube/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.830148 platypush-1.0.4/platypush/plugins/zeroconf/
+-rw-r--r--   0 root         (0) root         (0)     5888 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/zeroconf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      456 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/zeroconf/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.830148 platypush-1.0.4/platypush/plugins/zigbee/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/zigbee/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.830148 platypush-1.0.4/platypush/plugins/zigbee/mqtt/
+-rw-r--r--   0 root         (0) root         (0)    89045 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/zigbee/mqtt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2353 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/zigbee/mqtt/_state.py
+-rw-r--r--   0 root         (0) root         (0)     2658 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/zigbee/mqtt/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.830148 platypush-1.0.4/platypush/plugins/zwave/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/zwave/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2706 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/zwave/_constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.830148 platypush-1.0.4/platypush/plugins/zwave/mqtt/
+-rw-r--r--   0 root         (0) root         (0)    79655 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/zwave/mqtt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2555 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/zwave/mqtt/_state.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/plugins/zwave/mqtt/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.833481 platypush-1.0.4/platypush/procedure/
+-rw-r--r--   0 root         (0) root         (0)    18056 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/procedure/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.833481 platypush-1.0.4/platypush/process/
+-rw-r--r--   0 root         (0) root         (0)     3680 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/process/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.833481 platypush-1.0.4/platypush/runner/
+-rw-r--r--   0 root         (0) root         (0)      436 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/runner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/runner/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1720 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/runner/_app.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/runner/_runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.836815 platypush-1.0.4/platypush/schemas/
+-rw-r--r--   0 root         (0) root         (0)     3145 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3502 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/cups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.836815 platypush-1.0.4/platypush/schemas/dataclasses/
+-rw-r--r--   0 root         (0) root         (0)     1739 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/dataclasses/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      792 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/dbus.py
+-rw-r--r--   0 root         (0) root         (0)     3197 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/esp.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/gotify.py
+-rw-r--r--   0 root         (0) root         (0)     3909 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/gps.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/hid.py
+-rw-r--r--   0 root         (0) root         (0)     4149 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/irc.py
+-rw-r--r--   0 root         (0) root         (0)     4138 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/joystick.py
+-rw-r--r--   0 root         (0) root         (0)    10453 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/linode.py
+-rw-r--r--   0 root         (0) root         (0)      941 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/maps.py
+-rw-r--r--   0 root         (0) root         (0)     5956 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/mastodon.py
+-rw-r--r--   0 root         (0) root         (0)     9974 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/matrix.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.836815 platypush-1.0.4/platypush/schemas/media/
+-rw-r--r--   0 root         (0) root         (0)     1363 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/media/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3771 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/media/jellyfin.py
+-rw-r--r--   0 root         (0) root         (0)    10917 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/mopidy.py
+-rw-r--r--   0 root         (0) root         (0)      791 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/ngrok.py
+-rw-r--r--   0 root         (0) root         (0)     3344 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/pihole.py
+-rw-r--r--   0 root         (0) root         (0)     1246 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/ping.py
+-rw-r--r--   0 root         (0) root         (0)     6476 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/piped.py
+-rw-r--r--   0 root         (0) root         (0)     8040 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/pushbullet.py
+-rw-r--r--   0 root         (0) root         (0)     3698 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/qrcode.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/rss.py
+-rw-r--r--   0 root         (0) root         (0)     1386 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/slack.py
+-rw-r--r--   0 root         (0) root         (0)    12347 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/spotify.py
+-rw-r--r--   0 root         (0) root         (0)      992 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/sun.py
+-rw-r--r--   0 root         (0) root         (0)      365 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/switch.py
+-rw-r--r--   0 root         (0) root         (0)     8416 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/switchbot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.836815 platypush-1.0.4/platypush/schemas/system/
+-rw-r--r--   0 root         (0) root         (0)     1303 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      333 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.840148 platypush-1.0.4/platypush/schemas/system/_battery/
+-rw-r--r--   0 root         (0) root         (0)      104 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_battery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      619 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_battery/_base.py
+-rw-r--r--   0 root         (0) root         (0)      935 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_battery/_model.py
+-rw-r--r--   0 root         (0) root         (0)      184 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_battery/_schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.840148 platypush-1.0.4/platypush/schemas/system/_connection/
+-rw-r--r--   0 root         (0) root         (0)      116 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_connection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_connection/_base.py
+-rw-r--r--   0 root         (0) root         (0)     2383 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_connection/_model.py
+-rw-r--r--   0 root         (0) root         (0)      199 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_connection/_schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.840148 platypush-1.0.4/platypush/schemas/system/_cpu/
+-rw-r--r--   0 root         (0) root         (0)      340 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_cpu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_cpu/_base.py
+-rw-r--r--   0 root         (0) root         (0)     3997 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_cpu/_model.py
+-rw-r--r--   0 root         (0) root         (0)      495 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_cpu/_schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.840148 platypush-1.0.4/platypush/schemas/system/_disk/
+-rw-r--r--   0 root         (0) root         (0)       93 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_disk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      625 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_disk/_base.py
+-rw-r--r--   0 root         (0) root         (0)     2846 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_disk/_model.py
+-rw-r--r--   0 root         (0) root         (0)      169 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_disk/_schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.840148 platypush-1.0.4/platypush/schemas/system/_fan/
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_fan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      359 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_fan/_base.py
+-rw-r--r--   0 root         (0) root         (0)      690 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_fan/_model.py
+-rw-r--r--   0 root         (0) root         (0)      164 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_fan/_schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.843482 platypush-1.0.4/platypush/schemas/system/_memory/
+-rw-r--r--   0 root         (0) root         (0)      181 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_memory/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      423 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_memory/_base.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_memory/_model.py
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_memory/_schemas.py
+-rw-r--r--   0 root         (0) root         (0)      574 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.843482 platypush-1.0.4/platypush/schemas/system/_network/
+-rw-r--r--   0 root         (0) root         (0)      152 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_network/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_network/_base.py
+-rw-r--r--   0 root         (0) root         (0)     4610 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_network/_model.py
+-rw-r--r--   0 root         (0) root         (0)      235 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_network/_schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.843482 platypush-1.0.4/platypush/schemas/system/_process/
+-rw-r--r--   0 root         (0) root         (0)      104 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_process/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      850 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_process/_base.py
+-rw-r--r--   0 root         (0) root         (0)     2539 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_process/_model.py
+-rw-r--r--   0 root         (0) root         (0)      184 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_process/_schemas.py
+-rw-r--r--   0 root         (0) root         (0)      213 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.843482 platypush-1.0.4/platypush/schemas/system/_temperature/
+-rw-r--r--   0 root         (0) root         (0)      120 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_temperature/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      375 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_temperature/_base.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_temperature/_model.py
+-rw-r--r--   0 root         (0) root         (0)      204 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_temperature/_schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.843482 platypush-1.0.4/platypush/schemas/system/_user/
+-rw-r--r--   0 root         (0) root         (0)       92 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      590 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_user/_base.py
+-rw-r--r--   0 root         (0) root         (0)      980 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_user/_model.py
+-rw-r--r--   0 root         (0) root         (0)      169 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/system/_user/_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     5620 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/telegram.py
+-rw-r--r--   0 root         (0) root         (0)      782 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/tensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     6295 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/tidal.py
+-rw-r--r--   0 root         (0) root         (0)     6881 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/todoist.py
+-rw-r--r--   0 root         (0) root         (0)    12008 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/trello.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.843482 platypush-1.0.4/platypush/schemas/tts/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/tts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/tts/mimic3.py
+-rw-r--r--   0 root         (0) root         (0)     3208 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/wallabag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.843482 platypush-1.0.4/platypush/schemas/weather/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/weather/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4009 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/weather/buienradar.py
+-rw-r--r--   0 root         (0) root         (0)     4911 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/schemas/weather/openweathermap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.843482 platypush-1.0.4/platypush/user/
+-rw-r--r--   0 root         (0) root         (0)    11900 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/user/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.846815 platypush-1.0.4/platypush/utils/
+-rw-r--r--   0 root         (0) root         (0)    23439 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22068 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/utils/manifest.py
+-rw-r--r--   0 root         (0) root         (0)     1462 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/utils/media.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.846815 platypush-1.0.4/platypush/utils/mock/
+-rw-r--r--   0 root         (0) root         (0)     5653 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/utils/mock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/utils/mock/modules.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/utils/ngrok.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/utils/threads.py
+-rw-r--r--   0 root         (0) root         (0)     4165 2024-05-31 18:02:50.000000 platypush-1.0.4/platypush/utils/workers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.846815 platypush-1.0.4/platypush.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    56629 2024-05-31 18:06:00.000000 platypush-1.0.4/platypush.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    95808 2024-05-31 18:06:00.000000 platypush-1.0.4/platypush.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 18:06:00.000000 platypush-1.0.4/platypush.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2024-05-31 18:06:00.000000 platypush-1.0.4/platypush.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     3159 2024-05-31 18:06:00.000000 platypush-1.0.4/platypush.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-31 18:06:00.000000 platypush-1.0.4/platypush.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      203 2024-05-31 18:02:50.000000 platypush-1.0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      415 2024-05-31 18:06:00.863482 platypush-1.0.4/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     3180 2024-05-31 18:02:50.000000 platypush-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 18:06:00.846815 platypush-1.0.4/tests/
+-rw-r--r--   0 root         (0) root         (0)      680 2024-05-31 18:02:50.000000 platypush-1.0.4/tests/test_cron.py
+-rw-r--r--   0 root         (0) root         (0)     3823 2024-05-31 18:02:50.000000 platypush-1.0.4/tests/test_event_parse.py
+-rw-r--r--   0 root         (0) root         (0)     2658 2024-05-31 18:02:50.000000 platypush-1.0.4/tests/test_http.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2024-05-31 18:02:50.000000 platypush-1.0.4/tests/test_procedure.py
```

### Comparing `platypush-1.0.3/LICENSE.txt` & `platypush-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/PKG-INFO` & `platypush-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platypush
-Version: 1.0.3
+Version: 1.0.4
 Summary: Platypush service
 Home-page: https://platypush.tech
 Author: Fabio Manganiello
 Author-email: fabio@manganiello.tech
 License: MIT
 Keywords: home-automation automation iot mqtt websockets redis dashboard notifications
 Classifier: Topic :: Utilities
```

### Comparing `platypush-1.0.3/README.md` & `platypush-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/__init__.py` & `platypush-1.0.4/platypush/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # Alias for platypush.event.hook.hook,
 # see https://git.platypush.tech/platypush/platypush/issues/399
 when = hook
 
 
 __author__ = 'Fabio Manganiello <fabio@manganiello.tech>'
-__version__ = '1.0.3'
+__version__ = '1.0.4'
 __all__ = [
     'Application',
     'Variable',
     'Config',
     'Event',
     'Request',
     'Response',
```

### Comparing `platypush-1.0.3/platypush/app/_app.py` & `platypush-1.0.4/platypush/app/_app.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/__init__.py` & `platypush-1.0.4/platypush/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/__init__.py` & `platypush-1.0.4/platypush/backend/http/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/__init__.py` & `platypush-1.0.4/platypush/backend/http/app/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/mixins/__init__.py` & `platypush-1.0.4/platypush/backend/http/app/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/routes/auth.py` & `platypush-1.0.4/platypush/backend/http/app/routes/auth.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/routes/dashboard.py` & `platypush-1.0.4/platypush/backend/http/app/routes/dashboard.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/routes/execute.py` & `platypush-1.0.4/platypush/backend/http/app/routes/execute.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/routes/hook.py` & `platypush-1.0.4/platypush/backend/http/app/routes/hook.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/routes/login.py` & `platypush-1.0.4/platypush/backend/http/app/routes/login.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import re
 
 from flask import Blueprint, request, redirect, render_template, make_response
 
 from platypush.backend.http.app import template_folder
 from platypush.backend.http.utils import HttpUtils
 from platypush.user import UserManager
+from platypush.utils import utcnow
 
 login = Blueprint('login', __name__, template_folder=template_folder)
 
 # Declare routes list
 __routes__ = [
     login,
 ]
@@ -33,19 +34,15 @@
         if user:
             return redirect(redirect_page, 302)  # lgtm [py/url-redirection]
 
     if request.form:
         username = request.form.get('username')
         password = request.form.get('password')
         remember = request.form.get('remember')
-        expires = (
-            datetime.datetime.now(datetime.UTC) + datetime.timedelta(days=365)
-            if remember
-            else None
-        )
+        expires = utcnow() + datetime.timedelta(days=365) if remember else None
 
         session = user_manager.create_user_session(
             username=username, password=password, expires_at=expires
         )
 
         if session:
             redirect_target = redirect(redirect_page, 302)  # lgtm [py/url-redirection]
```

### Comparing `platypush-1.0.3/platypush/backend/http/app/routes/logo.py` & `platypush-1.0.4/platypush/backend/http/app/routes/logo.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/routes/logout.py` & `platypush-1.0.4/platypush/backend/http/app/routes/logout.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/routes/plugin.py` & `platypush-1.0.4/platypush/backend/http/app/routes/plugin.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/routes/plugins/camera/pi.py` & `platypush-1.0.4/platypush/backend/http/app/routes/plugins/camera/pi.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/routes/plugins/qrcode/__init__.py` & `platypush-1.0.4/platypush/backend/http/app/routes/plugins/qrcode/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/routes/plugins/spotify.py` & `platypush-1.0.4/platypush/backend/http/app/routes/plugins/spotify.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/routes/pwa.py` & `platypush-1.0.4/platypush/backend/http/app/routes/pwa.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/routes/register.py` & `platypush-1.0.4/platypush/backend/http/app/routes/register.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import re
 
 from flask import Blueprint, request, redirect, render_template, make_response, abort
 
 from platypush.backend.http.app import template_folder
 from platypush.backend.http.utils import HttpUtils
 from platypush.user import UserManager
+from platypush.utils import utcnow
 
 register = Blueprint('register', __name__, template_folder=template_folder)
 
 # Declare routes list
 __routes__ = [
     register,
 ]
@@ -46,17 +47,15 @@
 
         if password == confirm_password:
             user_manager.create_user(username=username, password=password)
             session = user_manager.create_user_session(
                 username=username,
                 password=password,
                 expires_at=(
-                    datetime.datetime.now(datetime.UTC) + datetime.timedelta(days=1)
-                    if not remember
-                    else None
+                    utcnow() + datetime.timedelta(days=1) if not remember else None
                 ),
             )
 
             if session:
                 redirect_target = redirect(
                     redirect_page, 302
                 )  # lgtm [py/url-redirection]
```

### Comparing `platypush-1.0.3/platypush/backend/http/app/routes/resources.py` & `platypush-1.0.4/platypush/backend/http/app/routes/resources.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/streaming/_base.py` & `platypush-1.0.4/platypush/backend/http/app/streaming/_base.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/streaming/plugins/camera.py` & `platypush-1.0.4/platypush/backend/http/app/streaming/plugins/camera.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/streaming/plugins/media/_register.py` & `platypush-1.0.4/platypush/backend/http/app/streaming/plugins/media/_register.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/streaming/plugins/media/_registry.py` & `platypush-1.0.4/platypush/backend/http/app/streaming/plugins/media/_registry.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/streaming/plugins/media/_stream.py` & `platypush-1.0.4/platypush/backend/http/app/streaming/plugins/media/_stream.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/streaming/plugins/media/_subtitles.py` & `platypush-1.0.4/platypush/backend/http/app/streaming/plugins/media/_subtitles.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/streaming/plugins/media/_unregister.py` & `platypush-1.0.4/platypush/backend/http/app/streaming/plugins/media/_unregister.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/streaming/plugins/sound.py` & `platypush-1.0.4/platypush/backend/http/app/streaming/plugins/sound.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/utils/__init__.py` & `platypush-1.0.4/platypush/backend/http/app/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/utils/auth/__init__.py` & `platypush-1.0.4/platypush/backend/http/app/utils/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/utils/bus.py` & `platypush-1.0.4/platypush/backend/http/app/utils/bus.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/utils/logger.py` & `platypush-1.0.4/platypush/backend/http/app/utils/logger.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/utils/routes.py` & `platypush-1.0.4/platypush/backend/http/app/utils/routes.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/utils/streaming.py` & `platypush-1.0.4/platypush/backend/http/app/utils/streaming.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/utils/ws.py` & `platypush-1.0.4/platypush/backend/http/app/utils/ws.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/ws/_base.py` & `platypush-1.0.4/platypush/backend/http/app/ws/_base.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/ws/cmd.py` & `platypush-1.0.4/platypush/backend/http/app/ws/cmd.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/ws/events.py` & `platypush-1.0.4/platypush/backend/http/app/ws/events.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/app/ws/requests.py` & `platypush-1.0.4/platypush/backend/http/app/ws/requests.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/media/handlers/__init__.py` & `platypush-1.0.4/platypush/backend/http/media/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/media/handlers/file.py` & `platypush-1.0.4/platypush/backend/http/media/handlers/file.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/utils.py` & `platypush-1.0.4/platypush/backend/http/utils.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/favicon.ico` & `platypush-1.0.4/platypush/backend/http/webapp/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/fonts/Poppins.ttf` & `platypush-1.0.4/platypush/backend/http/webapp/dist/fonts/Poppins.ttf`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/jellyfin.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/jellyfin.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/kodi.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/kodi.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/01d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/01d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/01n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/01n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/02d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/02d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/02n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/02n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/03d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/03d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/03n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/03n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/04d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/04d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/04n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/04n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/09d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/09d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/09n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/09n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/10d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/10d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/10n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/10n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/11d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/11d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/11n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/11n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/13d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/13d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/13n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/13n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/50d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/50d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/50n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/50n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/black/unknown.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/black/unknown.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/01d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/01d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/01n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/01n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/02d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/02d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/02n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/02n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/03d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/03d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/03n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/03n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/04d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/04d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/04n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/04n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/09d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/09d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/09n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/09n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/10d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/10d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/10n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/10n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/11d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/11d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/11n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/11n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/13d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/13d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/13n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/13n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/50d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/50d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/50n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/50n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/dark/unknown.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/dark/unknown.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/01d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/01d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/01n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/01n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/02d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/02d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/02n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/02n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/03d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/03d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/03n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/03n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/04d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/04d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/04n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/04n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/09d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/09d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/09n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/09n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/10d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/10d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/10n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/10n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/11d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/11d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/11n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/11n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/13d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/13d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/13n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/13n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/50d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/50d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/50n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/50n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/light/unknown.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/light/unknown.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/01d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/01d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/01n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/01n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/02d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/02d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/02n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/02n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/03d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/03d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/03n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/03n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/04d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/04d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/04n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/04n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/09d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/09d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/09n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/09n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/10d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/10d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/10n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/10n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/11d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/11d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/11n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/11n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/13d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/13d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/13n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/13n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/50d.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/50d.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/50n.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/50n.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/openweathermap/white/unknown.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/openweathermap/white/unknown.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/smartthings.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/smartthings.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/z-wave.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/z-wave.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/icons/zigbee.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/icons/zigbee.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/img/dashboard-bg-light.jpg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/img/dashboard-bg-light.jpg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/android-chrome-192x192.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/android-chrome-512x512.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/android-chrome-maskable-192x192.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/android-chrome-maskable-192x192.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/android-chrome-maskable-512x512.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/android-chrome-maskable-512x512.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon-120x120.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon-152x152.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon-180x180.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon-60x60.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon-76x76.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/favicon-16x16.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/favicon-32x32.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/favicon.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/favicon.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/logo-256x256.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/logo-256x256.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/msapplication-icon-144x144.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/msapplication-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/mstile-150x150.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/img/icons/safari-pinned-tab.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/img/icons/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/img/logo.png` & `platypush-1.0.4/platypush/backend/http/webapp/dist/img/logo.png`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/img/spinner.gif` & `platypush-1.0.4/platypush/backend/http/webapp/dist/img/spinner.gif`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/index.html` & `platypush-1.0.4/platypush/backend/http/webapp/dist/index.html`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/manifest.json` & `platypush-1.0.4/platypush/backend/http/webapp/dist/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/service-worker.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/service-worker.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/service-worker.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/service-worker.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/1259.ad51b86e.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/1259.ad51b86e.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/1391.8fb65128.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/1391.8fb65128.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/1449.bf964828.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/1449.bf964828.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/1587.f52aafce.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/1587.f52aafce.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/169.9ec6abc1.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/169.9ec6abc1.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/1706.c1e22194.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/1706.c1e22194.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/1807.333a022f.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/1807.333a022f.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/1949.d8d63590.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/1949.d8d63590.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/2140.08e216c1.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/2140.08e216c1.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/2154.20cf0934.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/2154.20cf0934.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/2217.da1b8fd6.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/2217.da1b8fd6.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/2460.83acd505.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/2460.83acd505.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/2461.1fc0b5b4.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/2461.1fc0b5b4.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/2509.77a756c6.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/2509.77a756c6.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/2844.23273db2.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/2844.23273db2.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/2892.3a7569e7.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/2892.3a7569e7.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/2893.21a9931c.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/2893.21a9931c.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/2976.bafd7cea.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/2976.bafd7cea.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/2992.f8bddaf0.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/2992.f8bddaf0.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/3368.467cedc6.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/3368.467cedc6.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/3369.69c504e7.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/3369.69c504e7.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/3390.481c441e.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/3390.481c441e.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/3553.6d93b4b8.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/3553.6d93b4b8.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/3559.5665c422.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/3559.5665c422.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/3661.c12867e9.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/3661.c12867e9.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/3671.e6547429.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/3671.e6547429.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/3826.53d49948.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/3826.53d49948.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/3835.91d8befb.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/3835.91d8befb.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/3924.e7e714bc.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/3924.e7e714bc.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/4221.76c11dc1.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/4221.76c11dc1.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/446.e0a96773.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/446.e0a96773.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/4589.d7fd389b.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/4589.d7fd389b.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/472.20f2f41f.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/472.20f2f41f.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/4790.3ef3568e.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/4790.3ef3568e.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/5059.e5cd6fe3.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/5059.e5cd6fe3.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/5207.e1e8949a.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/5207.e1e8949a.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/5285.2250c5c9.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/5285.2250c5c9.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/5329.2f2c6a0e.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/5329.2f2c6a0e.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/5638.05ee3a45.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/5638.05ee3a45.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/5795.3b193db6.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/5795.3b193db6.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/5833.e1e503a2.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/5833.e1e503a2.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/5906.52ba6beb.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/5906.52ba6beb.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/5931.e6c8f94d.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/5931.e6c8f94d.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/6062.b6571ed4.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/6062.b6571ed4.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/6079.f88a21ae.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/6079.f88a21ae.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/6324.bb3e2171.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/6324.bb3e2171.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/65.cb15a9a6.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/65.cb15a9a6.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/6523.d6576265.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/6523.d6576265.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/6561.77bbcd33.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/6561.77bbcd33.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/6579.04ad63dc.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/6579.04ad63dc.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/669.73188f7e.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/669.73188f7e.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/729.16b20067.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/729.16b20067.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/746.18c59228.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/746.18c59228.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/7590.b45a8e92.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/7590.b45a8e92.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/7651.9b63654f.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/7651.9b63654f.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/7841.2a1ced53.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/7841.2a1ced53.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/7878.e3469993.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/7878.e3469993.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/7880.4f4a202a.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/7880.4f4a202a.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/7968.29db26b1.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/7968.29db26b1.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/8039.e77a760e.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/8039.e77a760e.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/8069.111183af.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/8069.111183af.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/8179.b5fb83f9.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/8179.b5fb83f9.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/8391.b5dd11a9.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/8391.b5dd11a9.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/8498.3676728c.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/8498.3676728c.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/8621.5db86eb0.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/8621.5db86eb0.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/8769.fda642fb.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/8769.fda642fb.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/8825.f608e2c2.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/8825.f608e2c2.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/8989.63c7ae13.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/8989.63c7ae13.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/906.80f1f8a3.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/906.80f1f8a3.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/9211.b8dcc633.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/9211.b8dcc633.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/9381.ade341db.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/9381.ade341db.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/9461.79136fbe.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/9461.79136fbe.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/9751.0631f530.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/9751.0631f530.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/980.b4628099.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/980.b4628099.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/984.0c88349b.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/984.0c88349b.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/9962.eb89f1f6.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/9962.eb89f1f6.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/app.200dd9cf.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/app.200dd9cf.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/css/chunk-vendors.a2412607.css` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/css/chunk-vendors.a2412607.css`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/fonts/fa-brands-400.5d18d427.ttf` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/fonts/fa-brands-400.5d18d427.ttf`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/fonts/fa-brands-400.87587a68.woff2` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/fonts/fa-brands-400.87587a68.woff2`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/fonts/fa-regular-400.3ccdbd3d.woff2` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/fonts/fa-regular-400.3ccdbd3d.woff2`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/fonts/fa-regular-400.81482cd4.ttf` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/fonts/fa-regular-400.81482cd4.ttf`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/fonts/fa-solid-900.0b0cc8a6.woff2` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/fonts/fa-solid-900.0b0cc8a6.woff2`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/fonts/fa-solid-900.69d3141a.ttf` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/fonts/fa-solid-900.69d3141a.ttf`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/fonts/lato-medium-italic.1996cc15.woff` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/fonts/lato-medium-italic.1996cc15.woff`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/fonts/lato-medium-italic.1e312dd9.woff2` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/fonts/lato-medium-italic.1e312dd9.woff2`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/fonts/lato-medium.13fcde4c.woff2` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/fonts/lato-medium.13fcde4c.woff2`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/fonts/lato-medium.b41c3821.woff` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/fonts/lato-medium.b41c3821.woff`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ad.cb33f69a.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ad.cb33f69a.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ad.fa8477e6.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ad.fa8477e6.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/af.89591ab0.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/af.89591ab0.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/af.8ca96393.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/af.8ca96393.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ag.4c37bc2e.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ag.4c37bc2e.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ag.56074d55.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ag.56074d55.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ai.70eefdc0.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ai.70eefdc0.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ai.893d1179.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ai.893d1179.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/al.b16acdb2.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/al.b16acdb2.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/al.e0864b5d.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/al.e0864b5d.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ao.3df23f21.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ao.3df23f21.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ao.c0c32201.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ao.c0c32201.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/aq.1b8c45a6.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/aq.1b8c45a6.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/aq.aa242c4a.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/aq.aa242c4a.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ar.22a3116e.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ar.22a3116e.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ar.d3238270.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ar.d3238270.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/as.10ed1a23.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/as.10ed1a23.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/as.4a330654.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/as.4a330654.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/au.cc65fc07.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/au.cc65fc07.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/au.dbcdef2c.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/au.dbcdef2c.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/aw.abbad4ac.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/aw.abbad4ac.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/aw.be4540eb.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/aw.be4540eb.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ax.371c7af2.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ax.371c7af2.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ax.91eea523.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ax.91eea523.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/az.0e2f1d1a.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/az.0e2f1d1a.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ba.032070d4.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ba.032070d4.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ba.e167b08f.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ba.e167b08f.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bb.23a15e67.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bb.23a15e67.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bb.b800513b.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bb.b800513b.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bh.2a884f6c.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bh.2a884f6c.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bh.3968dfe0.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bh.3968dfe0.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bi.211d0f9e.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bi.211d0f9e.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bi.ae3bb248.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bi.ae3bb248.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bm.e6903c8e.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bm.e6903c8e.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bm.e69e40c4.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bm.e69e40c4.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bn.07911e0c.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bn.07911e0c.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bn.4d91734a.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bn.4d91734a.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bo.03595499.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bo.03595499.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bo.9c1d9ef8.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bo.9c1d9ef8.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/br.058a5086.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/br.058a5086.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/br.fe030c1c.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/br.fe030c1c.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bs.d228cbb2.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bs.d228cbb2.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bs.ef0a29ed.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bs.ef0a29ed.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bt.3f8ecb9b.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bt.3f8ecb9b.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bt.fc241981.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bt.fc241981.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bv.5503f03a.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bv.5503f03a.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bv.7f7cd26f.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bv.7f7cd26f.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/by.78d2c3c9.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/by.78d2c3c9.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/by.fba98c48.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/by.fba98c48.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bz.14c3376a.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bz.14c3376a.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/bz.5e0ef548.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/bz.5e0ef548.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ca.163ac200.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ca.163ac200.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ca.a2ab234d.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ca.a2ab234d.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cc.51960f85.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cc.51960f85.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cc.813adff8.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cc.813adff8.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cf.b5702729.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cf.b5702729.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cf.fe1120e9.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cf.fe1120e9.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ck.4e83dd3e.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ck.4e83dd3e.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ck.6303aa5b.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ck.6303aa5b.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cl.0917a91e.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cl.0917a91e.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cl.b5974a35.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cl.b5974a35.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cm.253adb39.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cm.253adb39.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cm.853e2843.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cm.853e2843.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cn.38f63e1e.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cn.38f63e1e.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cn.e1b166eb.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cn.e1b166eb.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cu.c2a6f0ed.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cu.c2a6f0ed.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cu.d6e33f19.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cu.d6e33f19.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cv.5ea64968.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cv.5ea64968.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cv.b3ab83f5.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cv.b3ab83f5.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cw.0e14b0b7.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cw.0e14b0b7.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cw.9b9b7ed5.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cw.9b9b7ed5.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cx.da5de6d2.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cx.da5de6d2.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cx.e04e07e8.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cx.e04e07e8.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cy.834e6240.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cy.834e6240.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/cy.bfcfd736.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/cy.bfcfd736.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/dashboard-bg-light.06da6eab.jpg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/dashboard-bg-light.06da6eab.jpg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/dj.4197a18a.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/dj.4197a18a.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/dj.925748d5.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/dj.925748d5.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/dm.7ddb00ac.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/dm.7ddb00ac.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/dm.bca6d70c.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/dm.bca6d70c.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/do.81097daa.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/do.81097daa.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/do.954f0f3e.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/do.954f0f3e.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ec.0029f514.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ec.0029f514.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ec.5f387e2f.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ec.5f387e2f.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/eg.38443fa6.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/eg.38443fa6.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/eg.5756a758.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/eg.5756a758.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/eh.82bd1c7b.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/eh.82bd1c7b.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/eh.f8d7b64f.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/eh.f8d7b64f.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/er.bf5b134b.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/er.bf5b134b.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/er.e932abe1.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/er.e932abe1.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/es.7dd46df0.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/es.7dd46df0.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/es.de5915e5.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/es.de5915e5.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/et.82e8eb21.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/et.82e8eb21.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/et.a998a1b2.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/et.a998a1b2.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/eu.4c6e130f.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/eu.4c6e130f.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/eu.aba724b1.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/eu.aba724b1.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/fj.ac9c916f.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/fj.ac9c916f.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/fj.e8d3e00b.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/fj.e8d3e00b.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/fk.af0350f8.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/fk.af0350f8.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/fk.db55fa14.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/fk.db55fa14.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/fm.3491efc7.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/fm.3491efc7.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/fm.78d44caa.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/fm.78d44caa.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/fo.1da81e3a.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/fo.1da81e3a.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/fo.72949ad1.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/fo.72949ad1.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gb-nir.2b7d2c3a.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gb-nir.2b7d2c3a.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gb-nir.f59817d6.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gb-nir.f59817d6.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gb-wls.13481560.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gb-wls.13481560.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gb-wls.95b2cfab.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gb-wls.95b2cfab.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gb.2aafb374.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gb.2aafb374.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gb.7a456bb2.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gb.7a456bb2.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gd.04ea09b7.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gd.04ea09b7.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gd.60b96978.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gd.60b96978.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ge.b7b65b55.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ge.b7b65b55.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ge.c7190912.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ge.c7190912.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gg.3aebc3ce.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gg.3aebc3ce.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gg.65174039.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gg.65174039.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gi.302c2506.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gi.302c2506.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gi.7beea6ed.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gi.7beea6ed.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gm.0e00e9d4.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gm.0e00e9d4.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gq.b1679302.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gq.b1679302.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gq.bd7daf33.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gq.bd7daf33.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gr.07bedadf.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gr.07bedadf.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gr.25dd3287.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gr.25dd3287.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gs.60368968.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gs.60368968.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gs.b2836676.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gs.b2836676.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gt.1a24ed67.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gt.1a24ed67.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gt.825f7286.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gt.825f7286.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gu.05f0ab85.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gu.05f0ab85.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gu.19b114eb.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gu.19b114eb.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gw.bcd1eddb.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gw.bcd1eddb.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/gw.c97f3f94.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/gw.c97f3f94.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/hk.b199a9ee.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/hk.b199a9ee.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/hk.c72bba0e.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/hk.c72bba0e.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/hm.4aa61657.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/hm.4aa61657.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/hm.d4b3d393.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/hm.d4b3d393.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/hn.08ad78b2.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/hn.08ad78b2.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/hn.44cee191.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/hn.44cee191.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/hr.078b1bf9.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/hr.078b1bf9.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/hr.1f4e28b8.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/hr.1f4e28b8.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ht.6943447c.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ht.6943447c.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ht.7ca68737.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ht.7ca68737.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/il.150f4c5f.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/il.150f4c5f.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/il.e02a66d3.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/il.e02a66d3.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/im.25166c91.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/im.25166c91.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/im.942419c5.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/im.942419c5.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/in.954929a0.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/in.954929a0.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/in.bd0d4f19.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/in.bd0d4f19.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/io.a59923ab.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/io.a59923ab.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/io.fa003484.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/io.fa003484.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/iq.1232a5c2.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/iq.1232a5c2.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/iq.9a48d678.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/iq.9a48d678.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ir.1ed24953.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ir.1ed24953.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ir.bc7ae9e1.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ir.bc7ae9e1.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/is.cad57f19.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/is.cad57f19.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/is.eea59326.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/is.eea59326.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/je.1684dacc.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/je.1684dacc.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/je.3ed72a25.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/je.3ed72a25.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/jellyfin.7b53a541.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/jellyfin.7b53a541.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/jo.06fbaa2c.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/jo.06fbaa2c.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/jo.7ac45a65.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/jo.7ac45a65.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ke.6dbfffd5.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ke.6dbfffd5.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ke.769bb975.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ke.769bb975.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kg.96c12490.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kg.96c12490.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kg.daded53c.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kg.daded53c.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kh.8eeb1634.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kh.8eeb1634.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kh.b10339d6.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kh.b10339d6.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ki.033ff9ce.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ki.033ff9ce.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ki.89e43a21.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ki.89e43a21.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/km.1e3bd5fe.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/km.1e3bd5fe.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/km.3ffb0228.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/km.3ffb0228.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kn.0c16fe68.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kn.0c16fe68.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kn.8f2e7b29.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kn.8f2e7b29.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kodi.d18f8d23.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kodi.d18f8d23.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kp.0f5253d8.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kp.0f5253d8.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kp.f4ff9e76.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kp.f4ff9e76.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kr.0dc8b972.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kr.0dc8b972.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kr.0f5e1116.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kr.0f5e1116.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ky.be81d90b.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ky.be81d90b.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ky.e3b76b32.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ky.e3b76b32.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kz.32ac1036.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kz.32ac1036.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/kz.579ac0f9.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/kz.579ac0f9.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/lb.8eea508a.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/lb.8eea508a.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/lb.bdbeb8f1.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/lb.bdbeb8f1.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/li.8dc1ed79.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/li.8dc1ed79.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/li.d7e2a871.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/li.d7e2a871.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/lk.42c41c61.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/lk.42c41c61.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/lk.e52240d6.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/lk.e52240d6.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/lr.5b84ff00.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/lr.5b84ff00.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/lr.9a67cd3d.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/lr.9a67cd3d.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ls.6d444cae.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ls.6d444cae.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ls.fe1da403.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ls.fe1da403.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ly.05f8732e.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ly.05f8732e.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ly.b9e750ff.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ly.b9e750ff.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/md.646818c3.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/md.646818c3.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/md.a56562ee.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/md.a56562ee.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/me.2e71b778.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/me.2e71b778.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/me.f05548f2.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/me.f05548f2.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mh.3fd69bb2.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mh.3fd69bb2.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mh.f6cbc774.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mh.f6cbc774.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mm.8ac1f094.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mm.8ac1f094.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mm.adaa2111.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mm.adaa2111.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mn.78547af0.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mn.78547af0.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mn.a4bcb0e6.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mn.a4bcb0e6.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mo.2f0d2c15.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mo.2f0d2c15.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mo.c8198565.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mo.c8198565.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mp.2acb5506.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mp.2acb5506.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mp.eeeefff6.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mp.eeeefff6.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ms.2025cd7d.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ms.2025cd7d.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ms.b13001dc.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ms.b13001dc.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mt.b6f71c85.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mt.b6f71c85.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mt.cff39ee0.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mt.cff39ee0.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mw.0b005148.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mw.0b005148.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mw.f704f4bb.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mw.f704f4bb.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mx.1b615ec2.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mx.1b615ec2.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mx.8a36b075.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mx.8a36b075.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/my.4109ae71.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/my.4109ae71.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/my.69c87fc5.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/my.69c87fc5.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mz.1377650b.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mz.1377650b.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/mz.2c96acb1.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/mz.2c96acb1.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/na.7adf4344.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/na.7adf4344.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/na.e0503926.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/na.e0503926.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/nf.1e8c700b.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/nf.1e8c700b.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/nf.a7166b00.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/nf.a7166b00.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ni.5b80bac0.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ni.5b80bac0.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ni.cc7eb514.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ni.cc7eb514.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/np.954177a0.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/np.954177a0.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/np.f7b8a5c3.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/np.f7b8a5c3.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/nr.2c66d218.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/nr.2c66d218.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/nr.a4f0e762.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/nr.a4f0e762.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/nu.26551dc2.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/nu.26551dc2.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/nu.860bbe8a.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/nu.860bbe8a.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/nz.38d0d690.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/nz.38d0d690.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/nz.c77ae58d.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/nz.c77ae58d.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/om.3f5691ca.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/om.3f5691ca.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/om.ff034f9e.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/om.ff034f9e.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pa.6dc8212a.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pa.6dc8212a.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pa.acde3214.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pa.acde3214.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pe.5a3b0bc5.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pe.5a3b0bc5.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pe.5c2ced95.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pe.5c2ced95.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pf.9f06082b.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pf.9f06082b.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pf.f6ae1bc8.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pf.f6ae1bc8.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pg.26847b33.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pg.26847b33.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pg.66c8dc3b.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pg.66c8dc3b.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ph.12e2b123.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ph.12e2b123.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ph.f215833e.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ph.f215833e.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pk.0bbf58be.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pk.0bbf58be.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pk.32b55f6f.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pk.32b55f6f.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pn.00a9342b.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pn.00a9342b.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pn.715fd11d.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pn.715fd11d.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pr.391a48e2.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pr.391a48e2.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pr.b37cbdc4.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pr.b37cbdc4.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ps.1af72ed4.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ps.1af72ed4.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ps.96bcac74.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ps.96bcac74.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pt.0703cc3a.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pt.0703cc3a.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/pt.351b87cb.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/pt.351b87cb.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/py.25cc39e3.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/py.25cc39e3.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/py.c20318c9.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/py.c20318c9.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/rs.23638d75.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/rs.23638d75.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/rs.ae2e3422.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/rs.ae2e3422.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/rw.87d5d899.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/rw.87d5d899.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/rw.d118aacd.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/rw.d118aacd.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sa.5bfbe72b.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sa.5bfbe72b.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sa.f0a8997b.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sa.f0a8997b.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sb.1c406073.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sb.1c406073.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sb.b0db5b0a.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sb.b0db5b0a.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sc.0452f14c.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sc.0452f14c.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sc.cdc20672.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sc.cdc20672.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/se.7e499d82.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/se.7e499d82.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/se.7ec71700.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/se.7ec71700.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sg.4f0e8eff.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sg.4f0e8eff.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sg.8a63b009.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sg.8a63b009.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sh.46e2588d.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sh.46e2588d.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sh.681f8fff.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sh.681f8fff.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/si.2a428364.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/si.2a428364.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/si.d9d425c0.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/si.d9d425c0.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sk.7998d1f5.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sk.7998d1f5.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sk.93c91c0b.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sk.93c91c0b.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sm.0ba901f4.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sm.0ba901f4.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sm.5e2fc188.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sm.5e2fc188.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/st.a70042c6.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/st.a70042c6.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/st.ecc4827f.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/st.ecc4827f.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sv.9501935a.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sv.9501935a.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sv.f67839a6.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sv.f67839a6.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sx.77e864f0.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sx.77e864f0.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sx.c0e6297a.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sx.c0e6297a.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sy.2b3eac89.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sy.2b3eac89.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sy.7fe894df.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sy.7fe894df.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sz.70b6fc50.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sz.70b6fc50.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/sz.eb01cd9f.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/sz.eb01cd9f.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tc.30ccd48e.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tc.30ccd48e.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tc.651466dd.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tc.651466dd.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tf.27cbe00b.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tf.27cbe00b.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tf.a1757237.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tf.a1757237.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tg.b492a751.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tg.b492a751.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tg.d04f874c.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tg.d04f874c.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tj.b7dafe8d.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tj.b7dafe8d.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tj.d3a42312.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tj.d3a42312.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tk.6c1f520c.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tk.6c1f520c.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tk.f87f794b.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tk.f87f794b.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tl.85904d79.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tl.85904d79.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tl.ca9af3c0.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tl.ca9af3c0.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tm.762df128.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tm.762df128.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tm.e467552c.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tm.e467552c.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tn.cc3ab493.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tn.cc3ab493.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tn.ff4c5190.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tn.ff4c5190.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tr.87e40d5c.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tr.87e40d5c.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tr.fc8c91dd.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tr.fc8c91dd.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tv.9717b553.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tv.9717b553.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tv.a8ff4939.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tv.a8ff4939.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tw.45c8a106.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tw.45c8a106.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tw.c0cf9ea7.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tw.c0cf9ea7.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tz.1abfbb38.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tz.1abfbb38.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/tz.c27fd405.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/tz.c27fd405.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ug.5ac71e98.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ug.5ac71e98.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ug.5ae165a2.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ug.5ae165a2.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/um.582dd57b.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/um.582dd57b.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/um.b38f913c.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/um.b38f913c.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/un.2df110d6.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/un.2df110d6.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/un.58a4a02a.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/un.58a4a02a.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/us.6c459052.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/us.6c459052.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/us.99e04236.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/us.99e04236.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/uy.69cf8938.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/uy.69cf8938.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/uy.b70ac310.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/uy.b70ac310.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/uz.7f8823a2.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/uz.7f8823a2.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/uz.d53abc35.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/uz.d53abc35.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/va.7efb8ba6.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/va.7efb8ba6.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/va.abcb42e8.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/va.abcb42e8.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ve.4cd0e3ed.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ve.4cd0e3ed.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ve.9cd63506.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ve.9cd63506.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/vg.025b8b6a.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/vg.025b8b6a.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/vg.ae3b6f7e.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/vg.ae3b6f7e.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/vi.293e6f1c.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/vi.293e6f1c.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/vi.f920eec7.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/vi.f920eec7.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/vu.5d2d7643.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/vu.5d2d7643.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/vu.b7a8d91a.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/vu.b7a8d91a.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ws.15c7a17c.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ws.15c7a17c.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/ws.d2e19e5a.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/ws.d2e19e5a.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/xk.16b6bb85.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/xk.16b6bb85.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/xk.ca7843be.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/xk.ca7843be.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/za.2fa94205.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/za.2fa94205.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/za.42e033a9.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/za.42e033a9.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/zm.92477cab.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/zm.92477cab.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/zm.ce5363b7.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/zm.ce5363b7.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/zw.6a535c1e.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/zw.6a535c1e.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/img/zw.f488cb8a.svg` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/img/zw.f488cb8a.svg`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1088.8670f8f4.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1088.8670f8f4.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1259.11016ad1.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1259.11016ad1.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1259.11016ad1.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1259.11016ad1.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1449.475ec524.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1449.475ec524.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1449.475ec524.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1449.475ec524.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1512.3e4f99fd.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1512.3e4f99fd.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1512.3e4f99fd.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1512.3e4f99fd.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1587.e2ebe369.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1587.e2ebe369.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1587.e2ebe369.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1587.e2ebe369.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/169.8bb8df7d.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/169.8bb8df7d.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/169.8bb8df7d.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/169.8bb8df7d.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1706.97f9b825.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1706.97f9b825.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1706.97f9b825.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1706.97f9b825.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1807.586a24d4.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1807.586a24d4.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1807.586a24d4.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1807.586a24d4.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1949.9d6edfd8.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1949.9d6edfd8.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/1949.9d6edfd8.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/1949.9d6edfd8.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2106.6553ebed.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2106.6553ebed.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2106.6553ebed.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2106.6553ebed.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2140.10cab5fd.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2140.10cab5fd.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2140.10cab5fd.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2140.10cab5fd.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2183.2941880a.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2183.2941880a.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2200.9fc9fd95.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2200.9fc9fd95.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2200.9fc9fd95.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2200.9fc9fd95.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2217.30568f1a.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2217.30568f1a.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2217.30568f1a.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2217.30568f1a.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2460.9845df8e.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2460.9845df8e.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2460.9845df8e.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2460.9845df8e.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2509.efc0bf4c.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2509.efc0bf4c.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2509.efc0bf4c.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2509.efc0bf4c.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2614.7997d726.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2614.7997d726.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2732.28f617e8.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2732.28f617e8.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2853.47a43033.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2853.47a43033.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2853.47a43033.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2853.47a43033.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2892.2d33f676.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2892.2d33f676.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2892.2d33f676.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2892.2d33f676.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2893.b037e7d2.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2893.b037e7d2.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2893.b037e7d2.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2893.b037e7d2.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2976.e8a9eb12.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2976.e8a9eb12.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/2976.e8a9eb12.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/2976.e8a9eb12.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3083.8440bfa8.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3083.8440bfa8.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3083.8440bfa8.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3083.8440bfa8.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3322.5ee98346.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3322.5ee98346.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3322.5ee98346.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3322.5ee98346.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3368.7ff6fca3.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3368.7ff6fca3.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3368.7ff6fca3.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3368.7ff6fca3.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3369.71760407.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3369.71760407.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3369.71760407.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3369.71760407.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3400.1021c9a8.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3400.1021c9a8.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3400.1021c9a8.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3400.1021c9a8.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/342.d3c0f8f2.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/342.d3c0f8f2.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/342.d3c0f8f2.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/342.d3c0f8f2.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3518.40e74ddb.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3518.40e74ddb.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3553.125dc216.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3553.125dc216.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3553.125dc216.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3553.125dc216.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3559.da067b47.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3559.da067b47.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3559.da067b47.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3559.da067b47.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3732.17c9c669.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3732.17c9c669.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3732.17c9c669.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3732.17c9c669.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3835.878348e2.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3835.878348e2.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3835.878348e2.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3835.878348e2.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3924.9592f111.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3924.9592f111.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/3924.9592f111.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/3924.9592f111.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/4053.1a106579.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/4053.1a106579.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/4053.1a106579.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/4053.1a106579.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/4221.292aeb44.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/4221.292aeb44.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/4221.292aeb44.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/4221.292aeb44.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/446.178d2754.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/446.178d2754.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/446.178d2754.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/446.178d2754.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/4589.c6a12ddf.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/4589.c6a12ddf.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/4589.c6a12ddf.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/4589.c6a12ddf.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/4619.ea41fd5e.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/4619.ea41fd5e.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/4619.ea41fd5e.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/4619.ea41fd5e.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/472.05f32d73.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/472.05f32d73.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/472.05f32d73.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/472.05f32d73.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/4765.7ad68124.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/4765.7ad68124.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5285.551ed2ce.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5285.551ed2ce.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5285.551ed2ce.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5285.551ed2ce.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5324.a449638b.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5324.a449638b.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5324.a449638b.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5324.a449638b.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5329.7bf8697f.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5329.7bf8697f.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5329.7bf8697f.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5329.7bf8697f.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5578.7c9eef7c.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5578.7c9eef7c.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5578.7c9eef7c.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5578.7c9eef7c.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5638.f1abcb64.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5638.f1abcb64.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5638.f1abcb64.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5638.f1abcb64.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5762.0d8fb9cb.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5762.0d8fb9cb.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5762.0d8fb9cb.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5762.0d8fb9cb.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5795.8f7061d6.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5795.8f7061d6.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5795.8f7061d6.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5795.8f7061d6.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5931.bcf6cfaf.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5931.bcf6cfaf.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/5931.bcf6cfaf.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/5931.bcf6cfaf.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6062.2509fe58.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6062.2509fe58.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6062.2509fe58.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6062.2509fe58.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6123.0a491498.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6123.0a491498.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6123.0a491498.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6123.0a491498.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6148.70084131.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6148.70084131.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6148.70084131.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6148.70084131.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6324.9d695c83.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6324.9d695c83.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6324.9d695c83.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6324.9d695c83.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6362.7e4f1ac1.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6362.7e4f1ac1.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6362.7e4f1ac1.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6362.7e4f1ac1.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6523.6faff1f9.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6523.6faff1f9.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6523.6faff1f9.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6523.6faff1f9.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/6640.a6538b3b.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/6640.a6538b3b.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/667.f23239a7.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/667.f23239a7.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/667.f23239a7.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/667.f23239a7.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7089.f4d74b4a.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7089.f4d74b4a.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7089.f4d74b4a.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7089.f4d74b4a.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/729.f4de5689.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/729.f4de5689.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/729.f4de5689.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/729.f4de5689.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7381.66ebc1f2.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7381.66ebc1f2.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7381.66ebc1f2.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7381.66ebc1f2.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/746.4c6b0061.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/746.4c6b0061.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/746.4c6b0061.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/746.4c6b0061.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7590.014063f7.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7590.014063f7.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7590.014063f7.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7590.014063f7.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7819.15635e35.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7819.15635e35.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7841.8b124a1f.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7841.8b124a1f.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7841.8b124a1f.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7841.8b124a1f.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7878.98038a22.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7878.98038a22.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7878.98038a22.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7878.98038a22.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7880.b455063a.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7880.b455063a.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7880.b455063a.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7880.b455063a.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7898.0426589e.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7898.0426589e.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7898.0426589e.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7898.0426589e.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7968.d677b422.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7968.d677b422.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/7968.d677b422.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/7968.d677b422.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/813.1fe7c13a.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/813.1fe7c13a.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/813.1fe7c13a.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/813.1fe7c13a.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8179.bd308864.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8179.bd308864.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8179.bd308864.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8179.bd308864.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8391.40c294c5.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8391.40c294c5.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8391.40c294c5.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8391.40c294c5.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8498.f8eb1c87.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8498.f8eb1c87.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8498.f8eb1c87.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8498.f8eb1c87.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8621.a437ee11.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8621.a437ee11.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8621.a437ee11.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8621.a437ee11.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8769.ad2a69a1.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8769.ad2a69a1.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8769.ad2a69a1.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8769.ad2a69a1.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8784.9c4e51b9.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8784.9c4e51b9.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8825.25b100b4.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8825.25b100b4.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8825.25b100b4.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8825.25b100b4.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/886.9ff7c1ce.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/886.9ff7c1ce.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/886.9ff7c1ce.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/886.9ff7c1ce.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8895.a4a700ec.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8895.a4a700ec.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8895.a4a700ec.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8895.a4a700ec.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8930.be445a5e.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8930.be445a5e.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/8930.be445a5e.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/8930.be445a5e.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9091.4b4643b0.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9091.4b4643b0.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9091.4b4643b0.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9091.4b4643b0.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9211.d1e09f60.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9211.d1e09f60.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9211.d1e09f60.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9211.d1e09f60.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9334.455b4593.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9334.455b4593.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9334.455b4593.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9334.455b4593.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9381.dc2f4776.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9381.dc2f4776.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9381.dc2f4776.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9381.dc2f4776.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9461.1fd0b115.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9461.1fd0b115.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9461.1fd0b115.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9461.1fd0b115.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9751.5b8fcd4c.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9751.5b8fcd4c.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9751.5b8fcd4c.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9751.5b8fcd4c.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/980.e9d022c5.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/980.e9d022c5.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/980.e9d022c5.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/980.e9d022c5.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/984.bedc7c00.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/984.bedc7c00.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/984.bedc7c00.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/984.bedc7c00.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9962.d22f669b.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9962.d22f669b.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/9962.d22f669b.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/9962.d22f669b.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/app.62f4493a.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/app.62f4493a.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/app.62f4493a.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/app.62f4493a.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/chunk-vendors.c084e94c.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/chunk-vendors.c084e94c.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/static/js/chunk-vendors.c084e94c.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/static/js/chunk-vendors.c084e94c.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/workbox-5b385ed2.js` & `platypush-1.0.4/platypush/backend/http/webapp/dist/workbox-5b385ed2.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/http/webapp/dist/workbox-5b385ed2.js.map` & `platypush-1.0.4/platypush/backend/http/webapp/dist/workbox-5b385ed2.js.map`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/nodered/__init__.py` & `platypush-1.0.4/platypush/backend/nodered/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/nodered/runner.py` & `platypush-1.0.4/platypush/backend/nodered/runner.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/redis/__init__.py` & `platypush-1.0.4/platypush/backend/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/backend/tcp/__init__.py` & `platypush-1.0.4/platypush/backend/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/builder/_base.py` & `platypush-1.0.4/platypush/builder/_base.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/bus/__init__.py` & `platypush-1.0.4/platypush/bus/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/bus/redis.py` & `platypush-1.0.4/platypush/bus/redis.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/cli.py` & `platypush-1.0.4/platypush/cli.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/commands/_base.py` & `platypush-1.0.4/platypush/commands/_base.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/commands/_reader.py` & `platypush-1.0.4/platypush/commands/_reader.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/commands/_stream.py` & `platypush-1.0.4/platypush/commands/_stream.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/commands/_writer.py` & `platypush-1.0.4/platypush/commands/_writer.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/common/__init__.py` & `platypush-1.0.4/platypush/common/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/common/_types.py` & `platypush-1.0.4/platypush/common/_types.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/common/db.py` & `platypush-1.0.4/platypush/common/db.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/common/gstreamer/__init__.py` & `platypush-1.0.4/platypush/common/gstreamer/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/common/reflection/_model/argument.py` & `platypush-1.0.4/platypush/common/reflection/_model/argument.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/common/reflection/_model/component.py` & `platypush-1.0.4/platypush/common/reflection/_model/component.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/common/reflection/_model/constructor.py` & `platypush-1.0.4/platypush/common/reflection/_model/constructor.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/common/reflection/_model/integration.py` & `platypush-1.0.4/platypush/common/reflection/_model/integration.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/common/reflection/_model/message.py` & `platypush-1.0.4/platypush/common/reflection/_model/message.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/common/reflection/_parser/context.py` & `platypush-1.0.4/platypush/common/reflection/_parser/context.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/common/reflection/_parser/docstring.py` & `platypush-1.0.4/platypush/common/reflection/_parser/docstring.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/common/reflection/_parser/rst.py` & `platypush-1.0.4/platypush/common/reflection/_parser/rst.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/common/spotify/__init__.py` & `platypush-1.0.4/platypush/common/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/config/__init__.py` & `platypush-1.0.4/platypush/config/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/config/config.yaml` & `platypush-1.0.4/platypush/config/config.yaml`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/config/systemd/platypush.service` & `platypush-1.0.4/platypush/config/systemd/platypush.service`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/context/__init__.py` & `platypush-1.0.4/platypush/context/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/cron/scheduler.py` & `platypush-1.0.4/platypush/cron/scheduler.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/__init__.py` & `platypush-1.0.4/platypush/entities/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from datetime import datetime, timedelta, UTC
+from datetime import timedelta
 import logging
 from threading import Event
 from typing import Collection, Optional
 
+from platypush.utils import utcnow
+
 from ._base import (
     Entity,
     EntityKey,
     EntitySavedCallback,
     get_entities_registry,
     init_entities_db,
 )
@@ -41,16 +43,16 @@
 
 def get_entities_engine(timeout: Optional[float] = None) -> EntitiesEngine:
     """
     Return the running entities engine.
 
     :param timeout: Timeout in seconds (default: None).
     """
-    time_start = datetime.now(UTC)
-    while not timeout or (datetime.now(UTC) - time_start < timedelta(seconds=timeout)):
+    time_start = utcnow()
+    while not timeout or (utcnow() - time_start < timedelta(seconds=timeout)):
         if _engine:
             break
 
         Event().wait(1)
 
     if not _engine:
         raise TimeoutError('The entities engine has not been initialized')
```

### Comparing `platypush-1.0.3/platypush/entities/_base.py` & `platypush-1.0.4/platypush/entities/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import inspect
 import json
 import os
 import pathlib
 import subprocess
 import sys
 import types
-from datetime import datetime, UTC
+from datetime import datetime
 from typing import Callable, Dict, List, Optional, Set, Type, Tuple, Any
 
 import pkgutil
 
 from dateutil.tz import tzutc
 from sqlalchemy import (
     Boolean,
@@ -28,14 +28,15 @@
 from sqlalchemy.orm import ColumnProperty, backref, relationship
 from sqlalchemy.orm.exc import ObjectDeletedError
 
 import platypush
 from platypush.config import Config
 from platypush.common.db import Base, is_defined
 from platypush.message import JSONAble, Message
+from platypush.utils import utcnow
 
 EntityRegistryType = Dict[str, Type['Entity']]
 entities_registry: EntityRegistryType = {}
 
 EntityKey = Tuple[str, str]
 """ The entity's logical key, as an ``<external_id, plugin>`` tuple. """
 EntityMapping = Dict[EntityKey, 'Entity']
@@ -78,21 +79,19 @@
         is_read_only = Column(Boolean, default=False)
         is_write_only = Column(Boolean, default=False)
         is_query_disabled = Column(Boolean, default=False)
         is_configuration = Column(Boolean, default=False)
         external_url = Column(String)
         image_url = Column(String)
 
-        created_at = Column(
-            DateTime(timezone=False), default=datetime.now(UTC), nullable=False
-        )
+        created_at = Column(DateTime(timezone=False), default=utcnow(), nullable=False)
         updated_at = Column(
             DateTime(timezone=False),
-            default=datetime.now(UTC),
-            onupdate=datetime.now(UTC),
+            default=utcnow(),
+            onupdate=utcnow(),
         )
 
         parent = relationship(
             'Entity',
             remote_side=[id],
             uselist=False,
             lazy='joined',
```

### Comparing `platypush-1.0.3/platypush/entities/_engine/__init__.py` & `platypush-1.0.4/platypush/entities/_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/_engine/queue.py` & `platypush-1.0.4/platypush/entities/_engine/queue.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/_engine/repo/__init__.py` & `platypush-1.0.4/platypush/entities/_engine/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/_engine/repo/db.py` & `platypush-1.0.4/platypush/entities/_engine/repo/db.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/_engine/repo/helpers.py` & `platypush-1.0.4/platypush/entities/_engine/repo/helpers.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/_engine/repo/merger.py` & `platypush-1.0.4/platypush/entities/_engine/repo/merger.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/acceleration.py` & `platypush-1.0.4/platypush/entities/acceleration.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/alarm.py` & `platypush-1.0.4/platypush/entities/alarm.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/assistants.py` & `platypush-1.0.4/platypush/entities/assistants.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/audio.py` & `platypush-1.0.4/platypush/entities/audio.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/batteries.py` & `platypush-1.0.4/platypush/entities/batteries.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/bluetooth/_device.py` & `platypush-1.0.4/platypush/entities/bluetooth/_device.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/bluetooth/_service.py` & `platypush-1.0.4/platypush/entities/bluetooth/_service.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/buttons.py` & `platypush-1.0.4/platypush/entities/buttons.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/cloud.py` & `platypush-1.0.4/platypush/entities/cloud.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/contact.py` & `platypush-1.0.4/platypush/entities/contact.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/devices.py` & `platypush-1.0.4/platypush/entities/devices.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/dimmers.py` & `platypush-1.0.4/platypush/entities/dimmers.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/distance.py` & `platypush-1.0.4/platypush/entities/distance.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/electricity.py` & `platypush-1.0.4/platypush/entities/electricity.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/heart.py` & `platypush-1.0.4/platypush/entities/heart.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/humidity.py` & `platypush-1.0.4/platypush/entities/humidity.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/illuminance.py` & `platypush-1.0.4/platypush/entities/illuminance.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/lights.py` & `platypush-1.0.4/platypush/entities/lights.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/linkquality.py` & `platypush-1.0.4/platypush/entities/linkquality.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/magnetism.py` & `platypush-1.0.4/platypush/entities/magnetism.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/managers/__init__.py` & `platypush-1.0.4/platypush/entities/managers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import inspect
 import json
 from abc import ABC, abstractmethod
-from datetime import datetime, UTC
 from typing import Any, Optional, Dict, Collection, Type
 
 from platypush.config import Config
 from platypush.entities._base import Entity, EntitySavedCallback
-from platypush.utils import get_plugin_name_by_class, get_redis
+from platypush.utils import get_plugin_name_by_class, get_redis, utcnow
 
 _entity_registry_varname = '_platypush/plugin_entity_registry'
 
 
 class EntityManager(ABC):
     """
     Base mixin for all the integrations that support entities mapping.
@@ -73,15 +72,15 @@
 
             if entity.id and not entity.external_id:
                 # Entity IDs can only refer to the internal primary key
                 entity.external_id = entity.id
                 entity.id = None  # type: ignore
 
             entity.plugin = get_plugin_name_by_class(self.__class__)  # type: ignore
-            entity.updated_at = datetime.now(UTC)  # type: ignore
+            entity.updated_at = utcnow()  # type: ignore
             entity.children = self._normalize_entities(entity.children)
 
         return entities
 
     def publish_entities(
         self,
         entities: Optional[Collection[Any]],
```

### Comparing `platypush-1.0.3/platypush/entities/managers/assistants.py` & `platypush-1.0.4/platypush/entities/managers/assistants.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/managers/cloud.py` & `platypush-1.0.4/platypush/entities/managers/cloud.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/managers/lights.py` & `platypush-1.0.4/platypush/entities/managers/lights.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/managers/switches.py` & `platypush-1.0.4/platypush/entities/managers/switches.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/managers/weather.py` & `platypush-1.0.4/platypush/entities/managers/weather.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/ping.py` & `platypush-1.0.4/platypush/entities/ping.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/presence.py` & `platypush-1.0.4/platypush/entities/presence.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/pressure.py` & `platypush-1.0.4/platypush/entities/pressure.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/sensors.py` & `platypush-1.0.4/platypush/entities/sensors.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/steps.py` & `platypush-1.0.4/platypush/entities/steps.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/switches.py` & `platypush-1.0.4/platypush/entities/switches.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/system.py` & `platypush-1.0.4/platypush/entities/system.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/temperature.py` & `platypush-1.0.4/platypush/entities/temperature.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/three_axis.py` & `platypush-1.0.4/platypush/entities/three_axis.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/time.py` & `platypush-1.0.4/platypush/entities/time.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/variables.py` & `platypush-1.0.4/platypush/entities/variables.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/weather.py` & `platypush-1.0.4/platypush/entities/weather.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/entities/weight.py` & `platypush-1.0.4/platypush/entities/weight.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/event/__init__.py` & `platypush-1.0.4/platypush/event/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/event/hook.py` & `platypush-1.0.4/platypush/event/hook.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/event/processor/__init__.py` & `platypush-1.0.4/platypush/event/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/__init__.py` & `platypush-1.0.4/platypush/events/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/adafruit.py` & `platypush-1.0.4/platypush/events/adafruit.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/alarm.py` & `platypush-1.0.4/platypush/events/alarm.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/assistant/__init__.py` & `platypush-1.0.4/platypush/events/assistant/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,22 +15,20 @@
         self, *args, assistant: Optional[Union[str, AssistantPlugin]] = None, **kwargs
     ):
         """
         :param assistant: Name of the assistant plugin that triggered the event.
         """
         assistant = assistant or kwargs.get('assistant')
         if assistant:
-            assistant = (
+            kwargs['plugin'] = kwargs['_assistant'] = (
                 assistant
                 if isinstance(assistant, str)
                 else get_plugin_name_by_class(assistant.__class__)
             )
 
-            kwargs['_assistant'] = assistant
-
         super().__init__(*args, **kwargs)
 
     @property
     def assistant(self) -> Optional[AssistantPlugin]:
         assistant = self.args.get('_assistant')
         if not assistant:
             return None
```

### Comparing `platypush-1.0.3/platypush/events/bluetooth/__init__.py` & `platypush-1.0.4/platypush/events/bluetooth/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/camera.py` & `platypush-1.0.4/platypush/events/camera.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/chat/slack.py` & `platypush-1.0.4/platypush/events/chat/slack.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/custom.py` & `platypush-1.0.4/platypush/events/custom.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/dbus.py` & `platypush-1.0.4/platypush/events/dbus.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/entities.py` & `platypush-1.0.4/platypush/events/entities.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/file.py` & `platypush-1.0.4/platypush/events/file.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/flic.py` & `platypush-1.0.4/platypush/events/flic.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/geo.py` & `platypush-1.0.4/platypush/events/geo.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/github.py` & `platypush-1.0.4/platypush/events/github.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/google/__init__.py` & `platypush-1.0.4/platypush/events/google/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/gotify.py` & `platypush-1.0.4/platypush/events/gotify.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/gps.py` & `platypush-1.0.4/platypush/events/gps.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/hid.py` & `platypush-1.0.4/platypush/events/hid.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/http/hook.py` & `platypush-1.0.4/platypush/events/http/hook.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/http/rss.py` & `platypush-1.0.4/platypush/events/http/rss.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/inotify.py` & `platypush-1.0.4/platypush/events/inotify.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/irc.py` & `platypush-1.0.4/platypush/events/irc.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/joystick.py` & `platypush-1.0.4/platypush/events/joystick.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/kafka.py` & `platypush-1.0.4/platypush/events/kafka.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/light.py` & `platypush-1.0.4/platypush/events/light.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/linode.py` & `platypush-1.0.4/platypush/events/linode.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/log/http.py` & `platypush-1.0.4/platypush/events/log/http.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/mail.py` & `platypush-1.0.4/platypush/events/mail.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/matrix.py` & `platypush-1.0.4/platypush/events/matrix.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/media.py` & `platypush-1.0.4/platypush/events/media.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/midi.py` & `platypush-1.0.4/platypush/events/midi.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/music/__init__.py` & `platypush-1.0.4/platypush/events/music/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/music/snapcast.py` & `platypush-1.0.4/platypush/events/music/snapcast.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/nextcloud.py` & `platypush-1.0.4/platypush/events/nextcloud.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/nfc.py` & `platypush-1.0.4/platypush/events/nfc.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/ngrok.py` & `platypush-1.0.4/platypush/events/ngrok.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/ntfy.py` & `platypush-1.0.4/platypush/events/ntfy.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/ping.py` & `platypush-1.0.4/platypush/events/ping.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/pushbullet.py` & `platypush-1.0.4/platypush/events/pushbullet.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/rss.py` & `platypush-1.0.4/platypush/events/rss.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/scard.py` & `platypush-1.0.4/platypush/events/scard.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/sensor/__init__.py` & `platypush-1.0.4/platypush/events/sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/sensor/ir/__init__.py` & `platypush-1.0.4/platypush/events/sensor/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/sensor/leap.py` & `platypush-1.0.4/platypush/events/sensor/leap.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/sound.py` & `platypush-1.0.4/platypush/events/sound.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/stt.py` & `platypush-1.0.4/platypush/events/stt.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/sun.py` & `platypush-1.0.4/platypush/events/sun.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/telegram.py` & `platypush-1.0.4/platypush/events/telegram.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/tensorflow.py` & `platypush-1.0.4/platypush/events/tensorflow.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/torrent.py` & `platypush-1.0.4/platypush/events/torrent.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/trello.py` & `platypush-1.0.4/platypush/events/trello.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/video/__init__.py` & `platypush-1.0.4/platypush/events/video/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/weather.py` & `platypush-1.0.4/platypush/events/weather.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/web/__init__.py` & `platypush-1.0.4/platypush/events/web/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/xmpp.py` & `platypush-1.0.4/platypush/events/xmpp.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/zeroconf.py` & `platypush-1.0.4/platypush/events/zeroconf.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/zigbee/mqtt.py` & `platypush-1.0.4/platypush/events/zigbee/mqtt.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/events/zwave.py` & `platypush-1.0.4/platypush/events/zwave.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/exceptions/__init__.py` & `platypush-1.0.4/platypush/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/exceptions/user.py` & `platypush-1.0.4/platypush/exceptions/user.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/install/docker/alpine.Dockerfile` & `platypush-1.0.4/platypush/install/docker/alpine.Dockerfile`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/install/docker/debian.Dockerfile` & `platypush-1.0.4/platypush/install/docker/debian.Dockerfile`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/install/docker/fedora.Dockerfile` & `platypush-1.0.4/platypush/install/docker/fedora.Dockerfile`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/install/docker/ubuntu.Dockerfile` & `platypush-1.0.4/platypush/install/docker/ubuntu.Dockerfile`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/install/scripts/alpine/install.sh` & `platypush-1.0.4/platypush/install/scripts/alpine/install.sh`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/install/scripts/arch/install.sh` & `platypush-1.0.4/platypush/install/scripts/arch/install.sh`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/install/scripts/debian/install.sh` & `platypush-1.0.4/platypush/install/scripts/debian/install.sh`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/install/scripts/fedora/install.sh` & `platypush-1.0.4/platypush/install/scripts/fedora/install.sh`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/install/scripts/install.sh` & `platypush-1.0.4/platypush/install/scripts/install.sh`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/install/scripts/ubuntu/install.sh` & `platypush-1.0.4/platypush/install/scripts/ubuntu/install.sh`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/logger.py` & `platypush-1.0.4/platypush/logger.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/__init__.py` & `platypush-1.0.4/platypush/message/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/__init__.py` & `platypush-1.0.4/platypush/message/event/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/adafruit.py` & `platypush-1.0.4/platypush/message/event/adafruit.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/alarm.py` & `platypush-1.0.4/platypush/message/event/alarm.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/assistant/__init__.py` & `platypush-1.0.4/platypush/message/event/assistant/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,22 +15,20 @@
         self, *args, assistant: Optional[Union[str, AssistantPlugin]] = None, **kwargs
     ):
         """
         :param assistant: Name of the assistant plugin that triggered the event.
         """
         assistant = assistant or kwargs.get('assistant')
         if assistant:
-            assistant = (
+            kwargs['plugin'] = kwargs['_assistant'] = (
                 assistant
                 if isinstance(assistant, str)
                 else get_plugin_name_by_class(assistant.__class__)
             )
 
-            kwargs['_assistant'] = assistant
-
         super().__init__(*args, **kwargs)
 
     @property
     def assistant(self) -> Optional[AssistantPlugin]:
         assistant = self.args.get('_assistant')
         if not assistant:
             return None
```

### Comparing `platypush-1.0.3/platypush/message/event/bluetooth/__init__.py` & `platypush-1.0.4/platypush/message/event/bluetooth/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/camera.py` & `platypush-1.0.4/platypush/message/event/camera.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/chat/slack.py` & `platypush-1.0.4/platypush/message/event/chat/slack.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/custom.py` & `platypush-1.0.4/platypush/message/event/custom.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/dbus.py` & `platypush-1.0.4/platypush/message/event/dbus.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/entities.py` & `platypush-1.0.4/platypush/message/event/entities.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/file.py` & `platypush-1.0.4/platypush/message/event/file.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/flic.py` & `platypush-1.0.4/platypush/message/event/flic.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/geo.py` & `platypush-1.0.4/platypush/message/event/geo.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/github.py` & `platypush-1.0.4/platypush/message/event/github.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/google/__init__.py` & `platypush-1.0.4/platypush/message/event/google/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/gotify.py` & `platypush-1.0.4/platypush/message/event/gotify.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/gps.py` & `platypush-1.0.4/platypush/message/event/gps.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/hid.py` & `platypush-1.0.4/platypush/message/event/hid.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/http/hook.py` & `platypush-1.0.4/platypush/message/event/http/hook.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/http/rss.py` & `platypush-1.0.4/platypush/message/event/http/rss.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/inotify.py` & `platypush-1.0.4/platypush/message/event/inotify.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/irc.py` & `platypush-1.0.4/platypush/message/event/irc.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/joystick.py` & `platypush-1.0.4/platypush/message/event/joystick.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/kafka.py` & `platypush-1.0.4/platypush/message/event/kafka.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/light.py` & `platypush-1.0.4/platypush/message/event/light.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/linode.py` & `platypush-1.0.4/platypush/message/event/linode.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/log/http.py` & `platypush-1.0.4/platypush/message/event/log/http.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/mail.py` & `platypush-1.0.4/platypush/message/event/mail.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/matrix.py` & `platypush-1.0.4/platypush/message/event/matrix.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/media.py` & `platypush-1.0.4/platypush/message/event/media.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/midi.py` & `platypush-1.0.4/platypush/message/event/midi.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/music/__init__.py` & `platypush-1.0.4/platypush/message/event/music/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/music/snapcast.py` & `platypush-1.0.4/platypush/message/event/music/snapcast.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/nextcloud.py` & `platypush-1.0.4/platypush/message/event/nextcloud.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/nfc.py` & `platypush-1.0.4/platypush/message/event/nfc.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/ngrok.py` & `platypush-1.0.4/platypush/message/event/ngrok.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/ntfy.py` & `platypush-1.0.4/platypush/message/event/ntfy.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/ping.py` & `platypush-1.0.4/platypush/message/event/ping.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/pushbullet.py` & `platypush-1.0.4/platypush/message/event/pushbullet.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/rss.py` & `platypush-1.0.4/platypush/message/event/rss.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/scard.py` & `platypush-1.0.4/platypush/message/event/scard.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/sensor/__init__.py` & `platypush-1.0.4/platypush/message/event/sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/sensor/ir/__init__.py` & `platypush-1.0.4/platypush/message/event/sensor/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/sensor/leap.py` & `platypush-1.0.4/platypush/message/event/sensor/leap.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/sound.py` & `platypush-1.0.4/platypush/message/event/sound.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/stt.py` & `platypush-1.0.4/platypush/message/event/stt.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/sun.py` & `platypush-1.0.4/platypush/message/event/sun.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/telegram.py` & `platypush-1.0.4/platypush/message/event/telegram.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/tensorflow.py` & `platypush-1.0.4/platypush/message/event/tensorflow.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/torrent.py` & `platypush-1.0.4/platypush/message/event/torrent.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/trello.py` & `platypush-1.0.4/platypush/message/event/trello.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/video/__init__.py` & `platypush-1.0.4/platypush/message/event/video/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/weather.py` & `platypush-1.0.4/platypush/message/event/weather.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/web/__init__.py` & `platypush-1.0.4/platypush/message/event/web/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/xmpp.py` & `platypush-1.0.4/platypush/message/event/xmpp.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/zeroconf.py` & `platypush-1.0.4/platypush/message/event/zeroconf.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/zigbee/mqtt.py` & `platypush-1.0.4/platypush/message/event/zigbee/mqtt.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/event/zwave.py` & `platypush-1.0.4/platypush/message/event/zwave.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/request/__init__.py` & `platypush-1.0.4/platypush/message/request/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/message/response/__init__.py` & `platypush-1.0.4/platypush/message/response/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/migrations/alembic/__pycache__/env.cpython-312.pyc` & `platypush-1.0.4/platypush/migrations/alembic/__pycache__/env.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Fri May 31 01:03:24 2024 UTC, .py size: 2747 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 dc21 5966 bb0a 0000  .........!Yf....
+00000000: cb0d 0d0a 0000 0000 ca10 5a66 bb0a 0000  ..........Zf....
 00000010: e300 0000 0000 0000 0000 0000 0003 0000  ................
 00000020: 0000 0000 00f3 1c01 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
 00000040: 5a03 0100 6400 6403 6c02 6d04 5a04 0100  Z...d.d.l.m.Z...
 00000050: 6400 6404 6c05 6d06 5a06 0100 6400 6405  d.d.l.m.Z...d.d.
 00000060: 6c07 6d08 5a08 0100 6400 6406 6c09 6d0a  l.m.Z...d.d.l.m.
 00000070: 5a0a 0100 6506 6a16 0000 0000 0000 0000  Z...e.j.........
```

### Comparing `platypush-1.0.3/platypush/migrations/alembic/env.py` & `platypush-1.0.4/platypush/migrations/alembic/env.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/migrations/alembic/versions/0876439530cb_added_password_hashing_parameters_to_.py` & `platypush-1.0.4/platypush/migrations/alembic/versions/0876439530cb_added_password_hashing_parameters_to_.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/migrations/alembic/versions/__pycache__/0876439530cb_added_password_hashing_parameters_to_.cpython-312.pyc` & `platypush-1.0.4/platypush/migrations/alembic/versions/__pycache__/0876439530cb_added_password_hashing_parameters_to_.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Fri May 31 01:03:24 2024 UTC, .py size: 1343 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 dc21 5966 3f05 0000  .........!Yf?...
+00000000: cb0d 0d0a 0000 0000 ca10 5a66 3f05 0000  ..........Zf?...
 00000010: e300 0000 0000 0000 0000 0000 0002 0000  ................
 00000020: 0000 0000 00f3 3c00 0000 9700 6400 5a00  ......<.....d.Z.
 00000030: 6401 6402 6c01 6d02 5a02 0100 6401 6403  d.d.l.m.Z...d.d.
 00000040: 6c03 5a04 6404 5a05 6405 5a06 6403 5a07  l.Z.d.Z.d.Z.d.Z.
 00000050: 6403 5a08 6408 6406 8404 5a09 6408 6407  d.Z.d.d...Z.d.d.
 00000060: 8404 5a0a 7903 2909 7a8a 4164 6465 6420  ..Z.y.).z.Added 
 00000070: 7061 7373 776f 7264 2068 6173 6869 6e67  password hashing
```

### Comparing `platypush-1.0.3/platypush/migrations/alembic/versions/__pycache__/c39ac404119b_migrate_variable_table.cpython-312.pyc` & `platypush-1.0.4/platypush/migrations/alembic/versions/__pycache__/c39ac404119b_migrate_variable_table.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Fri May 31 01:03:24 2024 UTC, .py size: 4308 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 dc21 5966 d410 0000  .........!Yf....
+00000000: cb0d 0d0a 0000 0000 ca10 5a66 d410 0000  ..........Zf....
 00000010: e300 0000 0000 0000 0000 0000 0002 0000  ................
 00000020: 0000 0000 00f3 4800 0000 9700 6400 5a00  ......H.....d.Z.
 00000030: 6401 6402 6c01 5a02 6401 6403 6c03 6d04  d.d.l.Z.d.d.l.m.
 00000040: 5a04 0100 6401 6404 6c05 6d06 5a06 0100  Z...d.d.l.m.Z...
 00000050: 6405 5a07 6406 5a08 6402 5a09 6402 5a0a  d.Z.d.Z.d.Z.d.Z.
 00000060: 6409 6407 8404 5a0b 6409 6408 8404 5a0c  d.d...Z.d.d...Z.
 00000070: 7902 290a 7a71 4d69 6772 6174 6520 7661  y.).zqMigrate va
```

### Comparing `platypush-1.0.3/platypush/migrations/alembic/versions/__pycache__/d030953a871d_base_alembic_version.cpython-312.pyc` & `platypush-1.0.4/platypush/migrations/alembic/versions/__pycache__/d030953a871d_base_alembic_version.cpython-312.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xcb0d0d0a
-moddate:  0xdc215966 (Fri May 31 01:03:24 2024 UTC)
+moddate:  0xca105a66 (Fri May 31 18:02:50 2024 UTC)
 files sz: 304
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `platypush-1.0.3/platypush/migrations/alembic/versions/c39ac404119b_migrate_variable_table.py` & `platypush-1.0.4/platypush/migrations/alembic/versions/c39ac404119b_migrate_variable_table.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/migrations/alembic.ini` & `platypush-1.0.4/platypush/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/platydock/__init__.py` & `platypush-1.0.4/platypush/platydock/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/platyvenv/__init__.py` & `platypush-1.0.4/platypush/platyvenv/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/__init__.py` & `platypush-1.0.4/platypush/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/adafruit/io/__init__.py` & `platypush-1.0.4/platypush/plugins/adafruit/io/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/alarm/__init__.py` & `platypush-1.0.4/platypush/plugins/alarm/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/alarm/_model.py` & `platypush-1.0.4/platypush/plugins/alarm/_model.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/application/__init__.py` & `platypush-1.0.4/platypush/plugins/application/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/arduino/__init__.py` & `platypush-1.0.4/platypush/plugins/arduino/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/assistant/__init__.py` & `platypush-1.0.4/platypush/plugins/assistant/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/assistant/google/__init__.py` & `platypush-1.0.4/platypush/plugins/assistant/google/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/assistant/google/manifest.json` & `platypush-1.0.4/platypush/plugins/assistant/google/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/assistant/picovoice/__init__.py` & `platypush-1.0.4/platypush/plugins/assistant/picovoice/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/assistant/picovoice/_assistant.py` & `platypush-1.0.4/platypush/plugins/assistant/picovoice/_assistant.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/assistant/picovoice/_context.py` & `platypush-1.0.4/platypush/plugins/assistant/picovoice/_context.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/assistant/picovoice/_recorder.py` & `platypush-1.0.4/platypush/plugins/assistant/picovoice/_recorder.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/assistant/picovoice/_speech/_base.py` & `platypush-1.0.4/platypush/plugins/assistant/picovoice/_speech/_base.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/assistant/picovoice/_speech/_intent.py` & `platypush-1.0.4/platypush/plugins/assistant/picovoice/_speech/_intent.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/assistant/picovoice/_speech/_processor.py` & `platypush-1.0.4/platypush/plugins/assistant/picovoice/_speech/_processor.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/assistant/picovoice/_speech/_stt.py` & `platypush-1.0.4/platypush/plugins/assistant/picovoice/_speech/_stt.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/assistant/picovoice/manifest.json` & `platypush-1.0.4/platypush/plugins/assistant/picovoice/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/autoremote/__init__.py` & `platypush-1.0.4/platypush/plugins/autoremote/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/__init__.py` & `platypush-1.0.4/platypush/plugins/bluetooth/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/_ble/_cache.py` & `platypush-1.0.4/platypush/plugins/bluetooth/_ble/_cache.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/_ble/_event_handler.py` & `platypush-1.0.4/platypush/plugins/bluetooth/_ble/_event_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import datetime, timedelta, UTC
+from datetime import timedelta
 from logging import getLogger
 from queue import Queue
 from typing import Callable, Collection, Dict, Final, List, Optional, Type
 from uuid import UUID
 
 from bleak.backends.device import BLEDevice
 from bleak.backends.scanner import AdvertisementData
@@ -12,14 +12,15 @@
 from platypush.message.event.bluetooth import (
     BluetoothDeviceConnectedEvent,
     BluetoothDeviceDisconnectedEvent,
     BluetoothDeviceFoundEvent,
     BluetoothDeviceSignalUpdateEvent,
     BluetoothDeviceEvent,
 )
+from platypush.utils import utcnow
 
 from .._cache import EntityCache
 from .._model import ServiceClass
 from .._plugins import BaseBluetoothPlugin
 from .._types import DevicesBlacklist
 from ._cache import DeviceCache
 from ._mappers import device_to_entity
@@ -94,16 +95,15 @@
         and bool(old and old.rssi)
         and (
             _has_changed(old, new, 'rssi', tolerance=5)
             or _has_changed(old, new, 'tx_power', tolerance=5)
         )
         and (
             not (old and old.updated_at)
-            or datetime.now(UTC) - old.updated_at
-            >= timedelta(seconds=_rssi_update_interval)
+            or utcnow() - old.updated_at >= timedelta(seconds=_rssi_update_interval)
         )
     ),
 }
 """ A static ``BluetoothDeviceEvent -> MatchCallback`` mapping. """
 
 
 # pylint: disable=too-few-public-methods
```

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/_ble/_manager.py` & `platypush-1.0.4/platypush/plugins/bluetooth/_ble/_manager.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/_ble/_mappers.py` & `platypush-1.0.4/platypush/plugins/bluetooth/_ble/_mappers.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/_ble/_plugins/switchbot.py` & `platypush-1.0.4/platypush/plugins/bluetooth/_ble/_plugins/switchbot.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/_cache.py` & `platypush-1.0.4/platypush/plugins/bluetooth/_cache.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/_file/sender.py` & `platypush-1.0.4/platypush/plugins/bluetooth/_file/sender.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/_legacy/_manager/_base.py` & `platypush-1.0.4/platypush/plugins/bluetooth/_legacy/_manager/_base.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/_legacy/_manager/_connection.py` & `platypush-1.0.4/platypush/plugins/bluetooth/_legacy/_manager/_connection.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/_legacy/_manager/_service.py` & `platypush-1.0.4/platypush/plugins/bluetooth/_legacy/_manager/_service.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/_legacy/_model/_device.py` & `platypush-1.0.4/platypush/plugins/bluetooth/_legacy/_model/_device.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/_legacy/_model/_services.py` & `platypush-1.0.4/platypush/plugins/bluetooth/_legacy/_model/_services.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/_manager.py` & `platypush-1.0.4/platypush/plugins/bluetooth/_manager.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/_model/_classes/_base.py` & `platypush-1.0.4/platypush/plugins/bluetooth/_model/_classes/_base.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/_model/_classes/_device/_major.py` & `platypush-1.0.4/platypush/plugins/bluetooth/_model/_classes/_device/_major.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/_model/_classes/_device/_minor.py` & `platypush-1.0.4/platypush/plugins/bluetooth/_model/_classes/_device/_minor.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/_model/_classes/_service.py` & `platypush-1.0.4/platypush/plugins/bluetooth/_model/_classes/_service.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/_model/_protocol.py` & `platypush-1.0.4/platypush/plugins/bluetooth/_model/_protocol.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/_model/_service/_directory.py` & `platypush-1.0.4/platypush/plugins/bluetooth/_model/_service/_directory.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/_model/_service/_directory.pyi` & `platypush-1.0.4/platypush/plugins/bluetooth/_model/_service/_directory.pyi`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/_plugins/_base.py` & `platypush-1.0.4/platypush/plugins/bluetooth/_plugins/_base.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/_plugins/_scanner.py` & `platypush-1.0.4/platypush/plugins/bluetooth/_plugins/_scanner.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/_types.py` & `platypush-1.0.4/platypush/plugins/bluetooth/_types.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/bluetooth/manifest.json` & `platypush-1.0.4/platypush/plugins/bluetooth/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/calendar/__init__.py` & `platypush-1.0.4/platypush/plugins/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/calendar/ical/__init__.py` & `platypush-1.0.4/platypush/plugins/calendar/ical/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 import requests
 from typing import Optional
 
 from platypush.plugins import Plugin, action
 from platypush.plugins.calendar import CalendarInterface
+from platypush.utils import utcnow
 
 
 class CalendarIcalPlugin(Plugin, CalendarInterface):
     """
     iCal calendars plugin. Interact with remote calendars in iCal format.
     """
 
@@ -21,15 +22,15 @@
 
     @staticmethod
     def _convert_timestamp(event, attribute: str) -> Optional[str]:
         t = event.get(attribute)
         if not t:
             return
 
-        if type(t.dt) == datetime.date:
+        if isinstance(t.dt, datetime.date):
             return datetime.datetime(
                 t.dt.year, t.dt.month, t.dt.day, tzinfo=datetime.timezone.utc
             ).isoformat()
 
         return (
             datetime.datetime.utcfromtimestamp(t.dt.timestamp())
             .replace(tzinfo=datetime.timezone.utc)
@@ -38,29 +39,31 @@
 
     @classmethod
     def _translate_event(cls, event):
         return {
             'id': str(event.get('uid')) if event.get('uid') else None,
             'kind': 'calendar#event',
             'summary': str(event.get('summary')) if event.get('summary') else None,
-            'description': str(event.get('description'))
-            if event.get('description')
-            else None,
+            'description': (
+                str(event.get('description')) if event.get('description') else None
+            ),
             'status': str(event.get('status')).lower() if event.get('status') else None,
-            'responseStatus': str(event.get('partstat')).lower()
-            if event.get('partstat')
-            else None,
+            'responseStatus': (
+                str(event.get('partstat')).lower() if event.get('partstat') else None
+            ),
             'location': str(event.get('location')) if event.get('location') else None,
             'htmlLink': str(event.get('url')) if event.get('url') else None,
-            'organizer': {
-                'email': str(event.get('organizer')).replace('MAILTO:', ''),
-                'displayName': event.get('organizer').params.get('cn'),
-            }
-            if event.get('organizer')
-            else None,
+            'organizer': (
+                {
+                    'email': str(event.get('organizer')).replace('MAILTO:', ''),
+                    'displayName': event.get('organizer').params.get('cn'),
+                }
+                if event.get('organizer')
+                else None
+            ),
             'created': cls._convert_timestamp(event, 'created'),
             'updated': cls._convert_timestamp(event, 'last-modified'),
             'start': {
                 'dateTime': cls._convert_timestamp(event, 'dtstart'),
                 'timeZone': 'UTC',
             },
             'end': {
@@ -91,17 +94,15 @@
 
             event = self._translate_event(event)
 
             if (
                 event['status'] != 'cancelled'
                 and event['end'].get('dateTime')
                 and event['end']['dateTime']
-                >= datetime.datetime.utcnow()
-                .replace(tzinfo=datetime.timezone.utc)
-                .isoformat()
+                >= utcnow().replace(tzinfo=datetime.timezone.utc).isoformat()
                 and (
                     (
                         only_participating
                         and event.get('responseStatus')
                         in [None, 'accepted', 'tentative']
                     )
                     or not only_participating
```

### Comparing `platypush-1.0.3/platypush/plugins/camera/__init__.py` & `platypush-1.0.4/platypush/plugins/camera/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/android/ipcam/__init__.py` & `platypush-1.0.4/platypush/plugins/camera/android/ipcam/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/cv/__init__.py` & `platypush-1.0.4/platypush/plugins/camera/cv/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/cv/manifest.json` & `platypush-1.0.4/platypush/plugins/camera/cv/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/ffmpeg/__init__.py` & `platypush-1.0.4/platypush/plugins/camera/ffmpeg/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/ffmpeg/manifest.json` & `platypush-1.0.4/platypush/plugins/camera/ffmpeg/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/gstreamer/__init__.py` & `platypush-1.0.4/platypush/plugins/camera/gstreamer/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/gstreamer/manifest.json` & `platypush-1.0.4/platypush/plugins/camera/gstreamer/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/ir/mlx90640/__init__.py` & `platypush-1.0.4/platypush/plugins/camera/ir/mlx90640/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/ir/mlx90640/manifest.json` & `platypush-1.0.4/platypush/plugins/camera/ir/mlx90640/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/model/camera.py` & `platypush-1.0.4/platypush/plugins/camera/model/camera.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/model/writer/__init__.py` & `platypush-1.0.4/platypush/plugins/camera/model/writer/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/model/writer/cv.py` & `platypush-1.0.4/platypush/plugins/camera/model/writer/cv.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/model/writer/ffmpeg.py` & `platypush-1.0.4/platypush/plugins/camera/model/writer/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/model/writer/image.py` & `platypush-1.0.4/platypush/plugins/camera/model/writer/image.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/model/writer/index.py` & `platypush-1.0.4/platypush/plugins/camera/model/writer/index.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/model/writer/preview/__init__.py` & `platypush-1.0.4/platypush/plugins/camera/model/writer/preview/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/model/writer/preview/ffplay.py` & `platypush-1.0.4/platypush/plugins/camera/model/writer/preview/ffplay.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/model/writer/preview/ui.py` & `platypush-1.0.4/platypush/plugins/camera/model/writer/preview/ui.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/model/writer/preview/wx/__init__.py` & `platypush-1.0.4/platypush/plugins/camera/model/writer/preview/wx/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/model/writer/preview/wx/ui.py` & `platypush-1.0.4/platypush/plugins/camera/model/writer/preview/wx/ui.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/pi/__init__.py` & `platypush-1.0.4/platypush/plugins/camera/pi/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/pi/legacy/__init__.py` & `platypush-1.0.4/platypush/plugins/camera/pi/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/pi/legacy/manifest.json` & `platypush-1.0.4/platypush/plugins/camera/pi/legacy/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/pi/legacy/model.py` & `platypush-1.0.4/platypush/plugins/camera/pi/legacy/model.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/pi/manifest.json` & `platypush-1.0.4/platypush/plugins/camera/pi/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/camera/pi/model.py` & `platypush-1.0.4/platypush/plugins/camera/pi/model.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/clipboard/__init__.py` & `platypush-1.0.4/platypush/plugins/clipboard/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/config/__init__.py` & `platypush-1.0.4/platypush/plugins/config/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/csv/__init__.py` & `platypush-1.0.4/platypush/plugins/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/cups/__init__.py` & `platypush-1.0.4/platypush/plugins/cups/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/db/__init__.py` & `platypush-1.0.4/platypush/plugins/db/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/dbus/__init__.py` & `platypush-1.0.4/platypush/plugins/dbus/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/dbus/manifest.json` & `platypush-1.0.4/platypush/plugins/dbus/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/dropbox/__init__.py` & `platypush-1.0.4/platypush/plugins/dropbox/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/entities/__init__.py` & `platypush-1.0.4/platypush/plugins/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/esp/__init__.py` & `platypush-1.0.4/platypush/plugins/esp/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/esp/models/connection.py` & `platypush-1.0.4/platypush/plugins/esp/models/connection.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/esp/models/device.py` & `platypush-1.0.4/platypush/plugins/esp/models/device.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/ffmpeg/__init__.py` & `platypush-1.0.4/platypush/plugins/ffmpeg/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/file/__init__.py` & `platypush-1.0.4/platypush/plugins/file/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/file/monitor/__init__.py` & `platypush-1.0.4/platypush/plugins/file/monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/file/monitor/entities/handlers.py` & `platypush-1.0.4/platypush/plugins/file/monitor/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/file/monitor/entities/resources.py` & `platypush-1.0.4/platypush/plugins/file/monitor/entities/resources.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/file/monitor/manifest.json` & `platypush-1.0.4/platypush/plugins/file/monitor/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/flic/__init__.py` & `platypush-1.0.4/platypush/plugins/flic/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/flic/fliclib.py` & `platypush-1.0.4/platypush/plugins/flic/fliclib.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/foursquare/__init__.py` & `platypush-1.0.4/platypush/plugins/foursquare/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/github/__init__.py` & `platypush-1.0.4/platypush/plugins/github/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/github/manifest.json` & `platypush-1.0.4/platypush/plugins/github/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/google/__init__.py` & `platypush-1.0.4/platypush/plugins/google/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/google/calendar/__init__.py` & `platypush-1.0.4/platypush/plugins/google/calendar/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import datetime
-
 from platypush.plugins import action
 from platypush.plugins.google import GooglePlugin
 from platypush.plugins.calendar import CalendarInterface
+from platypush.utils import utcnow
 
 
 class GoogleCalendarPlugin(GooglePlugin, CalendarInterface):
     r"""
     Google Calendar plugin.
 
     In order to use this plugin:
@@ -68,15 +67,15 @@
     @action
     def get_upcoming_events(self, max_results=10):
         """
         Get the upcoming events. See
         :meth:`platypush.plugins.calendar.CalendarPlugin.get_upcoming_events`.
         """
 
-        now = datetime.datetime.now(datetime.UTC).isoformat() + 'Z'
+        now = utcnow().isoformat() + 'Z'
         service = self.get_service('calendar', 'v3')
         result = (
             service.events()
             .list(
                 calendarId='primary',
                 timeMin=now,
                 maxResults=max_results,
```

### Comparing `platypush-1.0.3/platypush/plugins/google/calendar/manifest.json` & `platypush-1.0.4/platypush/plugins/google/calendar/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/google/credentials.py` & `platypush-1.0.4/platypush/plugins/google/credentials.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/google/drive/__init__.py` & `platypush-1.0.4/platypush/plugins/google/drive/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/google/drive/manifest.json` & `platypush-1.0.4/platypush/plugins/google/drive/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/google/mail/__init__.py` & `platypush-1.0.4/platypush/plugins/google/mail/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/google/mail/manifest.json` & `platypush-1.0.4/platypush/plugins/google/mail/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/google/maps/__init__.py` & `platypush-1.0.4/platypush/plugins/google/maps/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/google/maps/manifest.json` & `platypush-1.0.4/platypush/plugins/google/maps/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/google/pubsub/__init__.py` & `platypush-1.0.4/platypush/plugins/google/pubsub/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/google/pubsub/manifest.json` & `platypush-1.0.4/platypush/plugins/google/pubsub/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/google/translate/__init__.py` & `platypush-1.0.4/platypush/plugins/google/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/google/translate/manifest.json` & `platypush-1.0.4/platypush/plugins/google/translate/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/gotify/__init__.py` & `platypush-1.0.4/platypush/plugins/gotify/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/gpio/__init__.py` & `platypush-1.0.4/platypush/plugins/gpio/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/gpio/zeroborg/__init__.py` & `platypush-1.0.4/platypush/plugins/gpio/zeroborg/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/gpio/zeroborg/lib/__init__.py` & `platypush-1.0.4/platypush/plugins/gpio/zeroborg/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/gps/__init__.py` & `platypush-1.0.4/platypush/plugins/gps/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/gps/_model.py` & `platypush-1.0.4/platypush/plugins/gps/_model.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/gps/manifest.json` & `platypush-1.0.4/platypush/plugins/gps/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/graphite/__init__.py` & `platypush-1.0.4/platypush/plugins/graphite/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/hid/__init__.py` & `platypush-1.0.4/platypush/plugins/hid/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/hid/manifest.json` & `platypush-1.0.4/platypush/plugins/hid/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/http/__init__.py` & `platypush-1.0.4/platypush/plugins/http/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/http/webpage/__init__.py` & `platypush-1.0.4/platypush/plugins/http/webpage/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/http/webpage/manifest.json` & `platypush-1.0.4/platypush/plugins/http/webpage/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/http/webpage/mercury-parser.js` & `platypush-1.0.4/platypush/plugins/http/webpage/mercury-parser.js`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/ifttt/__init__.py` & `platypush-1.0.4/platypush/plugins/ifttt/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/inspect/__init__.py` & `platypush-1.0.4/platypush/plugins/inspect/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/inspect/_cache.py` & `platypush-1.0.4/platypush/plugins/inspect/_cache.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/inspect/_serialize.py` & `platypush-1.0.4/platypush/plugins/inspect/_serialize.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/irc/__init__.py` & `platypush-1.0.4/platypush/plugins/irc/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/irc/_bot.py` & `platypush-1.0.4/platypush/plugins/irc/_bot.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/irc/manifest.json` & `platypush-1.0.4/platypush/plugins/irc/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/joystick/__init__.py` & `platypush-1.0.4/platypush/plugins/joystick/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/joystick/_inputs.py` & `platypush-1.0.4/platypush/plugins/joystick/_inputs.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/joystick/_manager.py` & `platypush-1.0.4/platypush/plugins/joystick/_manager.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/joystick/_state.py` & `platypush-1.0.4/platypush/plugins/joystick/_state.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/kafka/__init__.py` & `platypush-1.0.4/platypush/plugins/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/lastfm/__init__.py` & `platypush-1.0.4/platypush/plugins/lastfm/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/lcd/__init__.py` & `platypush-1.0.4/platypush/plugins/lcd/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/lcd/gpio/__init__.py` & `platypush-1.0.4/platypush/plugins/lcd/gpio/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/lcd/i2c/__init__.py` & `platypush-1.0.4/platypush/plugins/lcd/i2c/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/leap/__init__.py` & `platypush-1.0.4/platypush/plugins/leap/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/light/hue/__init__.py` & `platypush-1.0.4/platypush/plugins/light/hue/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/linode/__init__.py` & `platypush-1.0.4/platypush/plugins/linode/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/log/http/__init__.py` & `platypush-1.0.4/platypush/plugins/log/http/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/logger/__init__.py` & `platypush-1.0.4/platypush/plugins/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/luma/oled/__init__.py` & `platypush-1.0.4/platypush/plugins/luma/oled/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/mail/__init__.py` & `platypush-1.0.4/platypush/plugins/mail/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/mail/_account.py` & `platypush-1.0.4/platypush/plugins/mail/_account.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/mail/_model/_config/_account.py` & `platypush-1.0.4/platypush/plugins/mail/_model/_config/_account.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/mail/_model/_mail.py` & `platypush-1.0.4/platypush/plugins/mail/_model/_mail.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/mail/_model/_transport.py` & `platypush-1.0.4/platypush/plugins/mail/_model/_transport.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/mail/_plugin/_base.py` & `platypush-1.0.4/platypush/plugins/mail/_plugin/_base.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/mail/_plugin/_in.py` & `platypush-1.0.4/platypush/plugins/mail/_plugin/_in.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/mail/_plugin/_out.py` & `platypush-1.0.4/platypush/plugins/mail/_plugin/_out.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/mail/_plugin/_utils.py` & `platypush-1.0.4/platypush/plugins/mail/_plugin/_utils.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/mail/_utils.py` & `platypush-1.0.4/platypush/plugins/mail/_utils.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/mail/imap/__init__.py` & `platypush-1.0.4/platypush/plugins/mail/imap/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/mail/manifest.json` & `platypush-1.0.4/platypush/plugins/mail/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/mail/smtp/__init__.py` & `platypush-1.0.4/platypush/plugins/mail/smtp/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/mailgun/__init__.py` & `platypush-1.0.4/platypush/plugins/mailgun/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/mastodon/__init__.py` & `platypush-1.0.4/platypush/plugins/mastodon/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/matrix/__init__.py` & `platypush-1.0.4/platypush/plugins/matrix/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/matrix/client.py` & `platypush-1.0.4/platypush/plugins/matrix/client.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/matrix/manifest.json` & `platypush-1.0.4/platypush/plugins/matrix/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/__init__.py` & `platypush-1.0.4/platypush/plugins/media/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/chromecast/__init__.py` & `platypush-1.0.4/platypush/plugins/media/chromecast/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/chromecast/_listener.py` & `platypush-1.0.4/platypush/plugins/media/chromecast/_listener.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/chromecast/_subtitles.py` & `platypush-1.0.4/platypush/plugins/media/chromecast/_subtitles.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/chromecast/_utils.py` & `platypush-1.0.4/platypush/plugins/media/chromecast/_utils.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/gstreamer/__init__.py` & `platypush-1.0.4/platypush/plugins/media/gstreamer/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/gstreamer/model.py` & `platypush-1.0.4/platypush/plugins/media/gstreamer/model.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/jellyfin/__init__.py` & `platypush-1.0.4/platypush/plugins/media/jellyfin/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/kodi/__init__.py` & `platypush-1.0.4/platypush/plugins/media/kodi/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/lib/plexcast.py` & `platypush-1.0.4/platypush/plugins/media/lib/plexcast.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/mplayer/__init__.py` & `platypush-1.0.4/platypush/plugins/media/mplayer/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/mpv/__init__.py` & `platypush-1.0.4/platypush/plugins/media/mpv/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/omxplayer/__init__.py` & `platypush-1.0.4/platypush/plugins/media/omxplayer/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/plex/__init__.py` & `platypush-1.0.4/platypush/plugins/media/plex/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/search/__init__.py` & `platypush-1.0.4/platypush/plugins/media/search/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/search/jellyfin.py` & `platypush-1.0.4/platypush/plugins/media/search/jellyfin.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/search/local/__init__.py` & `platypush-1.0.4/platypush/plugins/media/search/local/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/search/local/db.py` & `platypush-1.0.4/platypush/plugins/media/search/local/db.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/search/local/metadata.py` & `platypush-1.0.4/platypush/plugins/media/search/local/metadata.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/search/plex.py` & `platypush-1.0.4/platypush/plugins/media/search/plex.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/search/torrent.py` & `platypush-1.0.4/platypush/plugins/media/search/torrent.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/search/youtube.py` & `platypush-1.0.4/platypush/plugins/media/search/youtube.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/subtitles/__init__.py` & `platypush-1.0.4/platypush/plugins/media/subtitles/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/vlc/__init__.py` & `platypush-1.0.4/platypush/plugins/media/vlc/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/media/webtorrent/__init__.py` & `platypush-1.0.4/platypush/plugins/media/webtorrent/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/midi/__init__.py` & `platypush-1.0.4/platypush/plugins/midi/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/midi/_model.py` & `platypush-1.0.4/platypush/plugins/midi/_model.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/midi/manifest.json` & `platypush-1.0.4/platypush/plugins/midi/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/ml/cv/__init__.py` & `platypush-1.0.4/platypush/plugins/ml/cv/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/mobile/join/__init__.py` & `platypush-1.0.4/platypush/plugins/mobile/join/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/mqtt/__init__.py` & `platypush-1.0.4/platypush/plugins/mqtt/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/mqtt/_client.py` & `platypush-1.0.4/platypush/plugins/mqtt/_client.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/music/__init__.py` & `platypush-1.0.4/platypush/plugins/music/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/music/mopidy/__init__.py` & `platypush-1.0.4/platypush/plugins/music/mopidy/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/music/mopidy/_client.py` & `platypush-1.0.4/platypush/plugins/music/mopidy/_client.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/music/mopidy/_playlist.py` & `platypush-1.0.4/platypush/plugins/music/mopidy/_playlist.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/music/mopidy/_status.py` & `platypush-1.0.4/platypush/plugins/music/mopidy/_status.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/music/mopidy/_sync.py` & `platypush-1.0.4/platypush/plugins/music/mopidy/_sync.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/music/mopidy/_task.py` & `platypush-1.0.4/platypush/plugins/music/mopidy/_task.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/music/mopidy/_track.py` & `platypush-1.0.4/platypush/plugins/music/mopidy/_track.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/music/mopidy/manifest.json` & `platypush-1.0.4/platypush/plugins/music/mopidy/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/music/mpd/__init__.py` & `platypush-1.0.4/platypush/plugins/music/mpd/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/music/mpd/_listener.py` & `platypush-1.0.4/platypush/plugins/music/mpd/_listener.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/music/mpd/manifest.json` & `platypush-1.0.4/platypush/plugins/music/mpd/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/music/snapcast/__init__.py` & `platypush-1.0.4/platypush/plugins/music/snapcast/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/music/spotify/__init__.py` & `platypush-1.0.4/platypush/plugins/music/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/music/tidal/__init__.py` & `platypush-1.0.4/platypush/plugins/music/tidal/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/music/tidal/workers.py` & `platypush-1.0.4/platypush/plugins/music/tidal/workers.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/nextcloud/__init__.py` & `platypush-1.0.4/platypush/plugins/nextcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/nfc/__init__.py` & `platypush-1.0.4/platypush/plugins/nfc/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/ngrok/__init__.py` & `platypush-1.0.4/platypush/plugins/ngrok/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/ngrok/manifest.json` & `platypush-1.0.4/platypush/plugins/ngrok/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/nmap/__init__.py` & `platypush-1.0.4/platypush/plugins/nmap/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/ntfy/__init__.py` & `platypush-1.0.4/platypush/plugins/ntfy/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/openai/__init__.py` & `platypush-1.0.4/platypush/plugins/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/otp/__init__.py` & `platypush-1.0.4/platypush/plugins/otp/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/pihole/__init__.py` & `platypush-1.0.4/platypush/plugins/pihole/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/ping/__init__.py` & `platypush-1.0.4/platypush/plugins/ping/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/pushbullet/__init__.py` & `platypush-1.0.4/platypush/plugins/pushbullet/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/pushbullet/listener.py` & `platypush-1.0.4/platypush/plugins/pushbullet/listener.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/pushbullet/manifest.json` & `platypush-1.0.4/platypush/plugins/pushbullet/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/pwm/pca9685/__init__.py` & `platypush-1.0.4/platypush/plugins/pwm/pca9685/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/qrcode/__init__.py` & `platypush-1.0.4/platypush/plugins/qrcode/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/qrcode/manifest.json` & `platypush-1.0.4/platypush/plugins/qrcode/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/redis/__init__.py` & `platypush-1.0.4/platypush/plugins/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/rss/__init__.py` & `platypush-1.0.4/platypush/plugins/rss/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import requests
 
 from platypush.context import get_bus, get_plugin
 from platypush.message.event.rss import NewFeedEntryEvent
 from platypush.plugins import RunnablePlugin, action
 from platypush.plugins.variable import VariablePlugin
 from platypush.schemas.rss import RssFeedEntrySchema
+from platypush.utils import utcnow
 
 
 def _variable() -> VariablePlugin:
     var = get_plugin(VariablePlugin)
     assert var, 'Could not load the variable plugin'
     return var
 
@@ -285,15 +286,15 @@
         """
         root = ElementTree.Element('opml', {'version': '2.0'})
 
         head = ElementTree.Element('head')
         title = ElementTree.Element('title')
         title.text = 'Platypush feed subscriptions'
         created = ElementTree.Element('dateCreated')
-        created.text = self._datetime_to_string(datetime.datetime.now(datetime.UTC))
+        created.text = self._datetime_to_string(utcnow())
         head.append(title)
         head.append(created)
 
         body = ElementTree.Element('body')
         feeds = ElementTree.Element('outline', {'text': 'Feeds'})
 
         for sub in self.subscriptions:
```

### Comparing `platypush-1.0.3/platypush/plugins/rss/manifest.json` & `platypush-1.0.4/platypush/plugins/rss/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/rtorrent/__init__.py` & `platypush-1.0.4/platypush/plugins/rtorrent/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/rtorrent/manifest.json` & `platypush-1.0.4/platypush/plugins/rtorrent/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sensor/__init__.py` & `platypush-1.0.4/platypush/plugins/sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sensor/bme280/__init__.py` & `platypush-1.0.4/platypush/plugins/sensor/bme280/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sensor/dht/__init__.py` & `platypush-1.0.4/platypush/plugins/sensor/dht/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sensor/distance/vl53l1x/__init__.py` & `platypush-1.0.4/platypush/plugins/sensor/distance/vl53l1x/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sensor/envirophat/__init__.py` & `platypush-1.0.4/platypush/plugins/sensor/envirophat/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sensor/hcsr04/__init__.py` & `platypush-1.0.4/platypush/plugins/sensor/hcsr04/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sensor/lis3dh/__init__.py` & `platypush-1.0.4/platypush/plugins/sensor/lis3dh/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sensor/lis3dh/lib/LIS3DH.py` & `platypush-1.0.4/platypush/plugins/sensor/lis3dh/lib/LIS3DH.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sensor/ltr559/__init__.py` & `platypush-1.0.4/platypush/plugins/sensor/ltr559/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sensor/mcp3008/__init__.py` & `platypush-1.0.4/platypush/plugins/sensor/mcp3008/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sensor/pmw3901/__init__.py` & `platypush-1.0.4/platypush/plugins/sensor/pmw3901/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/serial/__init__.py` & `platypush-1.0.4/platypush/plugins/serial/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/shell/__init__.py` & `platypush-1.0.4/platypush/plugins/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/slack/__init__.py` & `platypush-1.0.4/platypush/plugins/slack/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/slack/manifest.json` & `platypush-1.0.4/platypush/plugins/slack/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/smartthings/__init__.py` & `platypush-1.0.4/platypush/plugins/smartthings/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/smartthings/_mappers.py` & `platypush-1.0.4/platypush/plugins/smartthings/_mappers.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sound/__init__.py` & `platypush-1.0.4/platypush/plugins/sound/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sound/_converters/_base.py` & `platypush-1.0.4/platypush/plugins/sound/_converters/_base.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sound/_converters/_from_raw.py` & `platypush-1.0.4/platypush/plugins/sound/_converters/_from_raw.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sound/_converters/_to_raw.py` & `platypush-1.0.4/platypush/plugins/sound/_converters/_to_raw.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sound/_manager/_device.py` & `platypush-1.0.4/platypush/plugins/sound/_manager/_device.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sound/_manager/_main.py` & `platypush-1.0.4/platypush/plugins/sound/_manager/_main.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sound/_manager/_stream.py` & `platypush-1.0.4/platypush/plugins/sound/_manager/_stream.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sound/_model.py` & `platypush-1.0.4/platypush/plugins/sound/_model.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sound/_streams/_base.py` & `platypush-1.0.4/platypush/plugins/sound/_streams/_base.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sound/_streams/_player/_base.py` & `platypush-1.0.4/platypush/plugins/sound/_streams/_player/_base.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sound/_streams/_player/_resource.py` & `platypush-1.0.4/platypush/plugins/sound/_streams/_player/_resource.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sound/_streams/_player/_synth/_base.py` & `platypush-1.0.4/platypush/plugins/sound/_streams/_player/_synth/_base.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sound/_streams/_player/_synth/_generator.py` & `platypush-1.0.4/platypush/plugins/sound/_streams/_player/_synth/_generator.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sound/_streams/_player/_synth/_mix.py` & `platypush-1.0.4/platypush/plugins/sound/_streams/_player/_synth/_mix.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sound/_streams/_player/_synth/_output.py` & `platypush-1.0.4/platypush/plugins/sound/_streams/_player/_synth/_output.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sound/_streams/_player/_synth/_parser.py` & `platypush-1.0.4/platypush/plugins/sound/_streams/_player/_synth/_parser.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sound/_streams/_player/_synth/_player.py` & `platypush-1.0.4/platypush/plugins/sound/_streams/_player/_synth/_player.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sound/_streams/_player/_synth/_sound.py` & `platypush-1.0.4/platypush/plugins/sound/_streams/_player/_synth/_sound.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sound/_streams/_recorder.py` & `platypush-1.0.4/platypush/plugins/sound/_streams/_recorder.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sound/_utils/_convert.py` & `platypush-1.0.4/platypush/plugins/sound/_utils/_convert.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sound/manifest.json` & `platypush-1.0.4/platypush/plugins/sound/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/ssh/__init__.py` & `platypush-1.0.4/platypush/plugins/ssh/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/ssh/tunnel/forward.py` & `platypush-1.0.4/platypush/plugins/ssh/tunnel/forward.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/ssh/tunnel/reverse.py` & `platypush-1.0.4/platypush/plugins/ssh/tunnel/reverse.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/sun/__init__.py` & `platypush-1.0.4/platypush/plugins/sun/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import requests
 from dateutil.tz import gettz
 
 from platypush.message.event.sun import SunriseEvent, SunsetEvent
 from platypush.plugins import RunnablePlugin, action
 from platypush.schemas.sun import SunEventsSchema
+from platypush.utils import utcnow
 
 
 class SunPlugin(RunnablePlugin):
     """
     Plugin to get sunset/sunrise events and info for a certain location.
     """
 
@@ -59,15 +60,15 @@
 
             if not self.should_stop():
                 self._bus.post(next_event)
                 self.wait_stop(2)
 
     @staticmethod
     def _convert_time(t: str) -> datetime.datetime:
-        now = datetime.datetime.now(datetime.UTC).replace(microsecond=0)
+        now = utcnow().replace(microsecond=0)
         dt = datetime.datetime.strptime(
             f'{now.year}-{now.month:02d}-{now.day:02d} {t}',
             '%Y-%m-%d %I:%M:%S %p',
         ).replace(tzinfo=datetime.UTC)
 
         if dt < now:
             dt += datetime.timedelta(days=1)
```

### Comparing `platypush-1.0.3/platypush/plugins/switch/tplink/__init__.py` & `platypush-1.0.4/platypush/plugins/switch/tplink/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/switch/wemo/__init__.py` & `platypush-1.0.4/platypush/plugins/switch/wemo/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/switch/wemo/lib.py` & `platypush-1.0.4/platypush/plugins/switch/wemo/lib.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/switch/wemo/scanner.py` & `platypush-1.0.4/platypush/plugins/switch/wemo/scanner.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/switchbot/__init__.py` & `platypush-1.0.4/platypush/plugins/switchbot/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/switchbot/_constants.py` & `platypush-1.0.4/platypush/plugins/switchbot/_constants.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/switchbot/_setters.py` & `platypush-1.0.4/platypush/plugins/switchbot/_setters.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/system/__init__.py` & `platypush-1.0.4/platypush/plugins/system/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/tcp/__init__.py` & `platypush-1.0.4/platypush/plugins/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/telegram/__init__.py` & `platypush-1.0.4/platypush/plugins/telegram/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/telegram/_bridge.py` & `platypush-1.0.4/platypush/plugins/telegram/_bridge.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/telegram/_model.py` & `platypush-1.0.4/platypush/plugins/telegram/_model.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/telegram/_service.py` & `platypush-1.0.4/platypush/plugins/telegram/_service.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/telegram/manifest.json` & `platypush-1.0.4/platypush/plugins/telegram/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/tensorflow/__init__.py` & `platypush-1.0.4/platypush/plugins/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/tensorflow/manifest.json` & `platypush-1.0.4/platypush/plugins/tensorflow/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/todoist/__init__.py` & `platypush-1.0.4/platypush/plugins/todoist/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/torrent/__init__.py` & `platypush-1.0.4/platypush/plugins/torrent/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/trello/__init__.py` & `platypush-1.0.4/platypush/plugins/trello/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/trello/_model.py` & `platypush-1.0.4/platypush/plugins/trello/_model.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/tts/__init__.py` & `platypush-1.0.4/platypush/plugins/tts/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/tts/google/__init__.py` & `platypush-1.0.4/platypush/plugins/tts/google/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/tts/google/manifest.json` & `platypush-1.0.4/platypush/plugins/tts/google/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/tts/manifest.json` & `platypush-1.0.4/platypush/plugins/tts/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/tts/mimic3/__init__.py` & `platypush-1.0.4/platypush/plugins/tts/mimic3/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/tts/mimic3/manifest.json` & `platypush-1.0.4/platypush/plugins/tts/mimic3/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/tts/picovoice/__init__.py` & `platypush-1.0.4/platypush/plugins/tts/picovoice/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/tv/samsung/ws/__init__.py` & `platypush-1.0.4/platypush/plugins/tv/samsung/ws/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/twilio/__init__.py` & `platypush-1.0.4/platypush/plugins/twilio/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/udp/__init__.py` & `platypush-1.0.4/platypush/plugins/udp/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/user/__init__.py` & `platypush-1.0.4/platypush/plugins/user/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/utils/__init__.py` & `platypush-1.0.4/platypush/plugins/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/variable/__init__.py` & `platypush-1.0.4/platypush/plugins/variable/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/wallabag/__init__.py` & `platypush-1.0.4/platypush/plugins/wallabag/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/weather/__init__.py` & `platypush-1.0.4/platypush/plugins/weather/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/weather/buienradar/__init__.py` & `platypush-1.0.4/platypush/plugins/weather/buienradar/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/weather/openweathermap/__init__.py` & `platypush-1.0.4/platypush/plugins/weather/openweathermap/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/websocket/__init__.py` & `platypush-1.0.4/platypush/plugins/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/xmpp/__init__.py` & `platypush-1.0.4/platypush/plugins/xmpp/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/xmpp/_config.py` & `platypush-1.0.4/platypush/plugins/xmpp/_config.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/xmpp/_handlers/__init__.py` & `platypush-1.0.4/platypush/plugins/xmpp/_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/xmpp/_handlers/_connection.py` & `platypush-1.0.4/platypush/plugins/xmpp/_handlers/_connection.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/xmpp/_handlers/_conversation.py` & `platypush-1.0.4/platypush/plugins/xmpp/_handlers/_conversation.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/xmpp/_handlers/_discover.py` & `platypush-1.0.4/platypush/plugins/xmpp/_handlers/_discover.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/xmpp/_handlers/_message.py` & `platypush-1.0.4/platypush/plugins/xmpp/_handlers/_message.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/xmpp/_handlers/_presence.py` & `platypush-1.0.4/platypush/plugins/xmpp/_handlers/_presence.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/xmpp/_handlers/_room.py` & `platypush-1.0.4/platypush/plugins/xmpp/_handlers/_room.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/xmpp/_handlers/_roster.py` & `platypush-1.0.4/platypush/plugins/xmpp/_handlers/_roster.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/xmpp/_mixins/_async.py` & `platypush-1.0.4/platypush/plugins/xmpp/_mixins/_async.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/xmpp/_mixins/_base.py` & `platypush-1.0.4/platypush/plugins/xmpp/_mixins/_base.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/xmpp/_mixins/_event_state.py` & `platypush-1.0.4/platypush/plugins/xmpp/_mixins/_event_state.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/xmpp/_mixins/_events.py` & `platypush-1.0.4/platypush/plugins/xmpp/_mixins/_events.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/xmpp/_mixins/_state.py` & `platypush-1.0.4/platypush/plugins/xmpp/_mixins/_state.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/xmpp/_state/_model.py` & `platypush-1.0.4/platypush/plugins/xmpp/_state/_model.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/xmpp/_state/_serializer.py` & `platypush-1.0.4/platypush/plugins/xmpp/_state/_serializer.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/xmpp/_types/_errors.py` & `platypush-1.0.4/platypush/plugins/xmpp/_types/_errors.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/xmpp/_types/_invite.py` & `platypush-1.0.4/platypush/plugins/xmpp/_types/_invite.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/xmpp/manifest.json` & `platypush-1.0.4/platypush/plugins/xmpp/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/youtube/__init__.py` & `platypush-1.0.4/platypush/plugins/youtube/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/zeroconf/__init__.py` & `platypush-1.0.4/platypush/plugins/zeroconf/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/zigbee/mqtt/__init__.py` & `platypush-1.0.4/platypush/plugins/zigbee/mqtt/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/zigbee/mqtt/_state.py` & `platypush-1.0.4/platypush/plugins/zigbee/mqtt/_state.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/zigbee/mqtt/manifest.json` & `platypush-1.0.4/platypush/plugins/zigbee/mqtt/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/zwave/_constants.py` & `platypush-1.0.4/platypush/plugins/zwave/_constants.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/zwave/mqtt/__init__.py` & `platypush-1.0.4/platypush/plugins/zwave/mqtt/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/zwave/mqtt/_state.py` & `platypush-1.0.4/platypush/plugins/zwave/mqtt/_state.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/plugins/zwave/mqtt/manifest.json` & `platypush-1.0.4/platypush/plugins/zwave/mqtt/manifest.json`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/procedure/__init__.py` & `platypush-1.0.4/platypush/procedure/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/process/__init__.py` & `platypush-1.0.4/platypush/process/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/runner/_app.py` & `platypush-1.0.4/platypush/runner/_app.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/runner/_runner.py` & `platypush-1.0.4/platypush/runner/_runner.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/__init__.py` & `platypush-1.0.4/platypush/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/cups.py` & `platypush-1.0.4/platypush/schemas/cups.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/dataclasses/__init__.py` & `platypush-1.0.4/platypush/schemas/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/dbus.py` & `platypush-1.0.4/platypush/schemas/dbus.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/esp.py` & `platypush-1.0.4/platypush/schemas/esp.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/gotify.py` & `platypush-1.0.4/platypush/schemas/gotify.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/gps.py` & `platypush-1.0.4/platypush/schemas/gps.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/hid.py` & `platypush-1.0.4/platypush/schemas/hid.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/irc.py` & `platypush-1.0.4/platypush/schemas/irc.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/joystick.py` & `platypush-1.0.4/platypush/schemas/joystick.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/linode.py` & `platypush-1.0.4/platypush/schemas/linode.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/maps.py` & `platypush-1.0.4/platypush/schemas/maps.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/mastodon.py` & `platypush-1.0.4/platypush/schemas/mastodon.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/matrix.py` & `platypush-1.0.4/platypush/schemas/matrix.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/media/__init__.py` & `platypush-1.0.4/platypush/schemas/media/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/media/jellyfin.py` & `platypush-1.0.4/platypush/schemas/media/jellyfin.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/mopidy.py` & `platypush-1.0.4/platypush/schemas/mopidy.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/ngrok.py` & `platypush-1.0.4/platypush/schemas/ngrok.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/pihole.py` & `platypush-1.0.4/platypush/schemas/pihole.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/ping.py` & `platypush-1.0.4/platypush/schemas/ping.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/piped.py` & `platypush-1.0.4/platypush/schemas/piped.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/pushbullet.py` & `platypush-1.0.4/platypush/schemas/pushbullet.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/qrcode.py` & `platypush-1.0.4/platypush/schemas/qrcode.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/rss.py` & `platypush-1.0.4/platypush/schemas/rss.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/slack.py` & `platypush-1.0.4/platypush/schemas/slack.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/spotify.py` & `platypush-1.0.4/platypush/schemas/spotify.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/sun.py` & `platypush-1.0.4/platypush/schemas/sun.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/switchbot.py` & `platypush-1.0.4/platypush/schemas/switchbot.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/system/__init__.py` & `platypush-1.0.4/platypush/schemas/system/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/system/_battery/_base.py` & `platypush-1.0.4/platypush/schemas/system/_battery/_base.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/system/_battery/_model.py` & `platypush-1.0.4/platypush/schemas/system/_battery/_model.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/system/_connection/_base.py` & `platypush-1.0.4/platypush/schemas/system/_connection/_base.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/system/_connection/_model.py` & `platypush-1.0.4/platypush/schemas/system/_connection/_model.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/system/_cpu/_base.py` & `platypush-1.0.4/platypush/schemas/system/_cpu/_base.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/system/_cpu/_model.py` & `platypush-1.0.4/platypush/schemas/system/_cpu/_model.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/system/_disk/_base.py` & `platypush-1.0.4/platypush/schemas/system/_disk/_base.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/system/_disk/_model.py` & `platypush-1.0.4/platypush/schemas/system/_disk/_model.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/system/_fan/_model.py` & `platypush-1.0.4/platypush/schemas/system/_fan/_model.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/system/_memory/_model.py` & `platypush-1.0.4/platypush/schemas/system/_memory/_model.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/system/_model.py` & `platypush-1.0.4/platypush/schemas/system/_model.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/system/_network/_base.py` & `platypush-1.0.4/platypush/schemas/system/_network/_base.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/system/_network/_model.py` & `platypush-1.0.4/platypush/schemas/system/_network/_model.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/system/_process/_base.py` & `platypush-1.0.4/platypush/schemas/system/_process/_base.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/system/_process/_model.py` & `platypush-1.0.4/platypush/schemas/system/_process/_model.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/system/_temperature/_model.py` & `platypush-1.0.4/platypush/schemas/system/_temperature/_model.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/system/_user/_base.py` & `platypush-1.0.4/platypush/schemas/system/_user/_base.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/system/_user/_model.py` & `platypush-1.0.4/platypush/schemas/system/_user/_model.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/telegram.py` & `platypush-1.0.4/platypush/schemas/telegram.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/tensorflow.py` & `platypush-1.0.4/platypush/schemas/tensorflow.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/tidal.py` & `platypush-1.0.4/platypush/schemas/tidal.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/todoist.py` & `platypush-1.0.4/platypush/schemas/todoist.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/trello.py` & `platypush-1.0.4/platypush/schemas/trello.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/tts/mimic3.py` & `platypush-1.0.4/platypush/schemas/tts/mimic3.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/wallabag.py` & `platypush-1.0.4/platypush/schemas/wallabag.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/weather/buienradar.py` & `platypush-1.0.4/platypush/schemas/weather/buienradar.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/schemas/weather/openweathermap.py` & `platypush-1.0.4/platypush/schemas/weather/openweathermap.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/user/__init__.py` & `platypush-1.0.4/platypush/user/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from platypush.common.db import Base
 from platypush.context import get_plugin
 from platypush.exceptions.user import (
     InvalidJWTTokenException,
     InvalidCredentialsException,
 )
-from platypush.utils import get_or_generate_jwt_rsa_key_pair
+from platypush.utils import get_or_generate_jwt_rsa_key_pair, utcnow
 
 
 class UserManager:
     """
     Main class for managing platform users
     """
 
@@ -74,15 +74,15 @@
             record = User(
                 username=username,
                 password=self._encrypt_password(
                     password, password_salt, hmac_iterations
                 ),
                 password_salt=password_salt.hex(),
                 hmac_iterations=hmac_iterations,
-                created_at=datetime.datetime.now(datetime.UTC),
+                created_at=utcnow(),
                 **kwargs,
             )
 
             session.add(record)
             session.commit()
             user = self._get_user(session, username)
 
@@ -112,16 +112,15 @@
             user_session = (
                 session.query(UserSession)
                 .filter_by(session_token=session_token)
                 .first()
             )
 
             if not user_session or (
-                user_session.expires_at
-                and user_session.expires_at < datetime.datetime.now(datetime.UTC)
+                user_session.expires_at and user_session.expires_at < utcnow()
             ):
                 return None, None
 
             user = session.query(User).filter_by(user_id=user_session.user_id).first()
             return self._mask_password(user), user_session
 
     def delete_user(self, username):
@@ -167,15 +166,15 @@
                 elif isinstance(expires_at, str):
                     expires_at = datetime.datetime.fromisoformat(expires_at)
 
             user_session = UserSession(
                 user_id=user.user_id,
                 session_token=self.generate_session_token(),
                 csrf_token=self.generate_session_token(),
-                created_at=datetime.datetime.now(datetime.UTC),
+                created_at=utcnow(),
                 expires_at=expires_at,
             )
 
             session.add(user_session)
             session.commit()
             return user_session
```

### Comparing `platypush-1.0.3/platypush/utils/__init__.py` & `platypush-1.0.4/platypush/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -810,8 +810,20 @@
     :param cls: The class to be used for the event. Default: threading.Event.
     """
     from .threads import OrEvent
 
     return OrEvent(*events, cls=cls).wait(timeout=timeout)
 
 
+def utcnow():
+    """
+    A workaround util to maintain compatibility both with Python >= 3.12 (which
+    deprecated datetime.utcnow) and Python < 3.12 (which doesn't have
+    datetime.UTC).
+    """
+    if hasattr(datetime, 'UTC'):
+        return datetime.datetime.now(datetime.UTC)
+
+    return datetime.datetime.utcnow()
+
+
 # vim:sw=4:ts=4:et:
```

### Comparing `platypush-1.0.3/platypush/utils/manifest.py` & `platypush-1.0.4/platypush/utils/manifest.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/utils/media.py` & `platypush-1.0.4/platypush/utils/media.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/utils/mock/__init__.py` & `platypush-1.0.4/platypush/utils/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/utils/mock/modules.py` & `platypush-1.0.4/platypush/utils/mock/modules.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/utils/ngrok.py` & `platypush-1.0.4/platypush/utils/ngrok.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/utils/threads.py` & `platypush-1.0.4/platypush/utils/threads.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush/utils/workers.py` & `platypush-1.0.4/platypush/utils/workers.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush.egg-info/PKG-INFO` & `platypush-1.0.4/platypush.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platypush
-Version: 1.0.3
+Version: 1.0.4
 Summary: Platypush service
 Home-page: https://platypush.tech
 Author: Fabio Manganiello
 Author-email: fabio@manganiello.tech
 License: MIT
 Keywords: home-automation automation iot mqtt websockets redis dashboard notifications
 Classifier: Topic :: Utilities
```

### Comparing `platypush-1.0.3/platypush.egg-info/SOURCES.txt` & `platypush-1.0.4/platypush.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/platypush.egg-info/requires.txt` & `platypush-1.0.4/platypush.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/setup.py` & `platypush-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 
 plugins = pkg_files('platypush/plugins')
 backend = pkg_files('platypush/backend')
 
 setup(
     name="platypush",
-    version="1.0.3",
+    version="1.0.4",
     author="Fabio Manganiello",
     author_email="fabio@manganiello.tech",
     description="Platypush service",
     license="MIT",
     python_requires='>= 3.6',
     keywords="home-automation automation iot mqtt websockets redis dashboard notifications",
     url="https://platypush.tech",
```

### Comparing `platypush-1.0.3/tests/test_cron.py` & `platypush-1.0.4/tests/test_cron.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/tests/test_event_parse.py` & `platypush-1.0.4/tests/test_event_parse.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/tests/test_http.py` & `platypush-1.0.4/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `platypush-1.0.3/tests/test_procedure.py` & `platypush-1.0.4/tests/test_procedure.py`

 * *Files identical despite different names*

