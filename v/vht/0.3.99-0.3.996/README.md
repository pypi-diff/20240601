# Comparing `tmp/vht-0.3.99.tar.gz` & `tmp/vht-0.3.996.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vht-0.3.99.tar", last modified: Fri May 31 20:55:30 2024, max compression
+gzip compressed data, was "vht-0.3.996.tar", last modified: Sat Jun  1 08:02:32 2024, max compression
```

## Comparing `vht-0.3.99.tar` & `vht-0.3.996.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 20:55:30.298117 vht-0.3.99/
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    35148 2024-05-08 12:01:32.000000 vht-0.3.99/LICENSE
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       49 2024-05-08 12:01:32.000000 vht-0.3.99/MANIFEST.in
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1894 2024-05-31 20:55:30.298117 vht-0.3.99/PKG-INFO
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1147 2024-05-28 20:35:49.000000 vht-0.3.99/README.md
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 20:55:30.286117 vht-0.3.99/data/
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 20:55:30.286117 vht-0.3.99/data/bank/
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2430 2024-05-08 12:01:32.000000 vht-0.3.99/data/bank/10-gm1
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4875 2024-05-08 12:01:32.000000 vht-0.3.99/data/bank/20-gm2
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 20:55:30.286117 vht-0.3.99/data/ctrl/
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      294 2024-05-08 12:01:32.000000 vht-0.3.99/data/ctrl/10-gm
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      166 2024-05-08 12:01:32.000000 vht-0.3.99/data/ctrl/20-zyn
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      310 2024-05-31 18:57:53.000000 vht-0.3.99/data/io.github.rdybka.vht.desktop
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2930 2024-05-31 19:00:17.000000 vht-0.3.99/data/io.github.rdybka.vht.metainfo.xml
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    23161 2024-05-31 20:40:19.000000 vht-0.3.99/data/io.github.rdybka.vht.png
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4550 2024-05-08 12:01:32.000000 vht-0.3.99/data/mandy.png
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1246 2024-05-08 12:01:32.000000 vht-0.3.99/data/menu.ui
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1112 2024-05-31 14:19:09.000000 vht-0.3.99/data/menu_norend.ui
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    23161 2024-05-31 20:40:19.000000 vht-0.3.99/data/vht.png
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4458 2024-05-08 12:01:32.000000 vht-0.3.99/data/vht.svg
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 20:55:30.286117 vht-0.3.99/doc/
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2362 2024-05-31 20:55:17.000000 vht-0.3.99/doc/vht.1.gz
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4641 2024-05-31 20:33:17.000000 vht-0.3.99/doc/vht.1.md
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 20:55:30.290117 vht-0.3.99/libvht/
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       75 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/__init__.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1538 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/ctrlrow.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1416 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/ctrlrow.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7088 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/envelope.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1612 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/envelope.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2121 2024-05-29 20:50:11.000000 vht-0.3.99/libvht/jack_process.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1212 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/jack_process.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    19982 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/libcvht.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    32223 2024-05-31 20:55:17.000000 vht-0.3.99/libvht/libcvht.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)   481702 2024-05-31 20:55:17.000000 vht-0.3.99/libvht/libcvht_wrap.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7542 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/libvht.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    34594 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/mandy.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6088 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/mandy.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2354 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/mandy_pix_scan.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1001 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/mandy_pix_scan.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7405 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/mandy_trk_disp.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      986 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/mandy_trk_disp.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    17045 2024-05-27 12:13:59.000000 vht-0.3.99/libvht/midi_client.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4531 2024-05-27 12:12:54.000000 vht-0.3.99/libvht/midi_client.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3496 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/midi_event.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1540 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/midi_event.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    15996 2024-05-27 12:02:48.000000 vht-0.3.99/libvht/module.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3256 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/module.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3029 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/row.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1670 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/row.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    28972 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/sequence.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4503 2024-05-15 11:24:39.000000 vht-0.3.99/libvht/sequence.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6493 2024-05-08 12:02:30.000000 vht-0.3.99/libvht/smf.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1680 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/smf.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2912 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/stolen.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    29373 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/timeline.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4538 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/timeline.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    41038 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/track.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4153 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/track.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4675 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/tracy.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2370 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/tracy.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1882 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/vhtcolumn.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2639 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/vhtctrl.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2012 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/vhtctrllist.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3639 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/vhtctrlrow.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1973 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/vhtextras.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6566 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/vhtmandy.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    21144 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/vhtmodule.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3432 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/vhtport.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2404 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/vhtports.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1922 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/vhtquicklist.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5623 2024-05-27 12:45:52.000000 vht-0.3.99/libvht/vhtrow.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    10975 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/vhtsequence.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3751 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/vhttimeline.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1887 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/vhttimelinechange.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2204 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/vhttimelinechanges.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1686 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/vhttimelineloop.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1913 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/vhttimelineslices.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5262 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/vhttimelinestrip.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3637 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/vhttimelinestrips.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1454 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/vhttimelineticks.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     9143 2024-05-27 13:05:52.000000 vht-0.3.99/libvht/vhttrack.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2270 2024-05-08 12:01:32.000000 vht-0.3.99/libvht/vhttracy.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1913 2024-05-31 20:45:00.000000 vht-0.3.99/pyproject.toml
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       70 2024-05-31 20:55:30.298117 vht-0.3.99/setup.cfg
--rwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)     1973 2024-05-31 20:44:43.000000 vht-0.3.99/setup.py
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 20:55:30.298117 vht-0.3.99/vht/
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      124 2024-05-08 12:01:32.000000 vht-0.3.99/vht/__init__.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1088 2024-05-08 12:01:32.000000 vht-0.3.99/vht/autoexec.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3531 2024-05-08 12:01:32.000000 vht-0.3.99/vht/bankcfg.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1688 2024-05-08 12:01:32.000000 vht-0.3.99/vht/capturebutton.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3834 2024-05-08 12:01:32.000000 vht-0.3.99/vht/codedaemon.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    24274 2024-05-08 12:01:32.000000 vht-0.3.99/vht/configuration.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5836 2024-05-08 12:01:32.000000 vht-0.3.99/vht/console.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    55124 2024-05-09 10:48:54.000000 vht-0.3.99/vht/controllereditor.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6976 2024-05-08 12:01:32.000000 vht-0.3.99/vht/controllersview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5707 2024-05-08 12:01:32.000000 vht-0.3.99/vht/controllersviewrow.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4560 2024-05-08 12:01:32.000000 vht-0.3.99/vht/controllerundobuffer.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2909 2024-05-08 12:01:32.000000 vht-0.3.99/vht/ctrlcfg.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1910 2024-05-08 12:01:32.000000 vht-0.3.99/vht/extras.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1298 2024-05-08 12:01:32.000000 vht-0.3.99/vht/filerotator.py
--rwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)    11519 2024-05-31 14:34:24.000000 vht-0.3.99/vht/main.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    18736 2024-05-31 14:20:00.000000 vht-0.3.99/vht/mainwin.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    14192 2024-05-08 12:01:32.000000 vht-0.3.99/vht/mandymenu.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    18144 2024-05-08 12:01:32.000000 vht-0.3.99/vht/mandyview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2401 2024-05-08 12:01:32.000000 vht-0.3.99/vht/midimapview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4176 2024-05-08 12:01:32.000000 vht-0.3.99/vht/midimapviewrow.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1299 2024-05-08 12:01:32.000000 vht-0.3.99/vht/notebooklabel.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4721 2024-05-08 12:01:32.000000 vht-0.3.99/vht/poormanspiano.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2677 2024-05-08 12:01:32.000000 vht-0.3.99/vht/portconfig.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3547 2024-05-08 12:01:32.000000 vht-0.3.99/vht/portconfigpopover.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7770 2024-05-28 19:34:11.000000 vht-0.3.99/vht/portconfigview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    24678 2024-05-28 18:53:13.000000 vht-0.3.99/vht/preferenceswin.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6623 2024-05-08 12:01:32.000000 vht-0.3.99/vht/probeditor.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4996 2024-05-08 12:01:32.000000 vht-0.3.99/vht/propview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1035 2024-05-08 12:01:32.000000 vht-0.3.99/vht/pulsar.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1100 2024-05-08 12:01:32.000000 vht-0.3.99/vht/randomcomposer.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     8188 2024-05-28 20:16:35.000000 vht-0.3.99/vht/renderer.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     9640 2024-05-27 12:29:20.000000 vht-0.3.99/vht/renderwin.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    15715 2024-05-08 12:01:32.000000 vht-0.3.99/vht/sequencelistview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    13404 2024-05-29 20:09:20.000000 vht-0.3.99/vht/sequencelistviewpopover.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    11262 2024-05-08 12:01:32.000000 vht-0.3.99/vht/sequencepropviewpopover.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    12223 2024-05-08 12:01:32.000000 vht-0.3.99/vht/sequencetriggersview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    37321 2024-05-08 12:01:32.000000 vht-0.3.99/vht/sequenceview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6644 2024-05-29 18:59:49.000000 vht-0.3.99/vht/shortcutmayhem.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    20316 2024-05-08 12:01:32.000000 vht-0.3.99/vht/sidetrackview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    19612 2024-05-08 12:01:32.000000 vht-0.3.99/vht/statusbar.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2879 2024-05-08 12:01:32.000000 vht-0.3.99/vht/thumbmanager.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    51601 2024-05-08 12:01:32.000000 vht-0.3.99/vht/timelineview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6308 2024-05-08 12:01:32.000000 vht-0.3.99/vht/timeshifteditor.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    22027 2024-05-08 12:01:32.000000 vht-0.3.99/vht/trackpropview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    31965 2024-05-08 12:01:32.000000 vht-0.3.99/vht/trackpropviewpopover.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3229 2024-05-08 12:01:32.000000 vht-0.3.99/vht/trackundobuffer.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    96428 2024-05-15 11:23:14.000000 vht-0.3.99/vht/trackview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     9212 2024-05-08 12:01:32.000000 vht-0.3.99/vht/trackviewpointer.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     8127 2024-05-08 12:01:32.000000 vht-0.3.99/vht/velocityeditor.py
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 20:55:30.298117 vht-0.3.99/vht.egg-info/
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1894 2024-05-31 20:55:30.000000 vht-0.3.99/vht.egg-info/PKG-INFO
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2606 2024-05-31 20:55:30.000000 vht-0.3.99/vht.egg-info/SOURCES.txt
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)        1 2024-05-31 20:55:30.000000 vht-0.3.99/vht.egg-info/dependency_links.txt
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       38 2024-05-31 20:55:30.000000 vht-0.3.99/vht.egg-info/entry_points.txt
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       27 2024-05-31 20:55:30.000000 vht-0.3.99/vht.egg-info/top_level.txt
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-06-01 08:02:32.873083 vht-0.3.996/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    35148 2024-05-08 12:01:32.000000 vht-0.3.996/LICENSE
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       49 2024-05-08 12:01:32.000000 vht-0.3.996/MANIFEST.in
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1895 2024-06-01 08:02:32.873083 vht-0.3.996/PKG-INFO
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1147 2024-05-28 20:35:49.000000 vht-0.3.996/README.md
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-06-01 08:02:32.857083 vht-0.3.996/data/
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-06-01 08:02:32.857083 vht-0.3.996/data/bank/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2430 2024-05-08 12:01:32.000000 vht-0.3.996/data/bank/10-gm1
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4875 2024-05-08 12:01:32.000000 vht-0.3.996/data/bank/20-gm2
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-06-01 08:02:32.857083 vht-0.3.996/data/ctrl/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      294 2024-05-08 12:01:32.000000 vht-0.3.996/data/ctrl/10-gm
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      166 2024-05-08 12:01:32.000000 vht-0.3.996/data/ctrl/20-zyn
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      310 2024-05-31 18:57:53.000000 vht-0.3.996/data/io.github.rdybka.vht.desktop
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2930 2024-05-31 19:00:17.000000 vht-0.3.996/data/io.github.rdybka.vht.metainfo.xml
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    23161 2024-05-31 20:40:19.000000 vht-0.3.996/data/io.github.rdybka.vht.png
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4550 2024-05-08 12:01:32.000000 vht-0.3.996/data/mandy.png
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1246 2024-05-08 12:01:32.000000 vht-0.3.996/data/menu.ui
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1112 2024-05-31 14:19:09.000000 vht-0.3.996/data/menu_norend.ui
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    23161 2024-05-31 20:40:19.000000 vht-0.3.996/data/vht.png
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4458 2024-05-08 12:01:32.000000 vht-0.3.996/data/vht.svg
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-06-01 08:02:32.857083 vht-0.3.996/doc/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2364 2024-06-01 07:49:40.000000 vht-0.3.996/doc/vht.1.gz
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4642 2024-06-01 07:47:23.000000 vht-0.3.996/doc/vht.1.md
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-06-01 08:02:32.865083 vht-0.3.996/libvht/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       75 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/__init__.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1538 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/ctrlrow.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1416 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/ctrlrow.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7088 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/envelope.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1612 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/envelope.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2121 2024-05-29 20:50:11.000000 vht-0.3.996/libvht/jack_process.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1212 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/jack_process.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    19982 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/libcvht.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    32223 2024-06-01 07:49:40.000000 vht-0.3.996/libvht/libcvht.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)   481702 2024-06-01 07:49:40.000000 vht-0.3.996/libvht/libcvht_wrap.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7542 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/libvht.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    34594 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/mandy.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6088 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/mandy.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2354 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/mandy_pix_scan.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1001 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/mandy_pix_scan.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7405 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/mandy_trk_disp.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      986 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/mandy_trk_disp.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    17045 2024-05-27 12:13:59.000000 vht-0.3.996/libvht/midi_client.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4531 2024-05-27 12:12:54.000000 vht-0.3.996/libvht/midi_client.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3496 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/midi_event.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1540 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/midi_event.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    15996 2024-05-27 12:02:48.000000 vht-0.3.996/libvht/module.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3256 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/module.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3029 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/row.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1670 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/row.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    28972 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/sequence.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4503 2024-05-15 11:24:39.000000 vht-0.3.996/libvht/sequence.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6493 2024-05-08 12:02:30.000000 vht-0.3.996/libvht/smf.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1680 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/smf.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2912 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/stolen.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    29373 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/timeline.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4538 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/timeline.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    41038 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/track.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4153 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/track.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4675 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/tracy.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2370 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/tracy.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1882 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/vhtcolumn.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2639 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/vhtctrl.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2012 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/vhtctrllist.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3639 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/vhtctrlrow.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1973 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/vhtextras.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6566 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/vhtmandy.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    21144 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/vhtmodule.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3432 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/vhtport.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2404 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/vhtports.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1922 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/vhtquicklist.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5623 2024-05-27 12:45:52.000000 vht-0.3.996/libvht/vhtrow.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    10975 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/vhtsequence.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3751 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/vhttimeline.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1887 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/vhttimelinechange.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2204 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/vhttimelinechanges.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1686 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/vhttimelineloop.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1913 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/vhttimelineslices.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5262 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/vhttimelinestrip.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3637 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/vhttimelinestrips.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1454 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/vhttimelineticks.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     9143 2024-05-27 13:05:52.000000 vht-0.3.996/libvht/vhttrack.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2270 2024-05-08 12:01:32.000000 vht-0.3.996/libvht/vhttracy.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1914 2024-06-01 07:47:31.000000 vht-0.3.996/pyproject.toml
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       70 2024-06-01 08:02:32.873083 vht-0.3.996/setup.cfg
+-rwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)     1974 2024-06-01 07:47:25.000000 vht-0.3.996/setup.py
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-06-01 08:02:32.873083 vht-0.3.996/vht/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      124 2024-05-08 12:01:32.000000 vht-0.3.996/vht/__init__.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1088 2024-05-08 12:01:32.000000 vht-0.3.996/vht/autoexec.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3531 2024-05-08 12:01:32.000000 vht-0.3.996/vht/bankcfg.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1688 2024-05-08 12:01:32.000000 vht-0.3.996/vht/capturebutton.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3834 2024-05-08 12:01:32.000000 vht-0.3.996/vht/codedaemon.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    24274 2024-05-08 12:01:32.000000 vht-0.3.996/vht/configuration.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5836 2024-05-08 12:01:32.000000 vht-0.3.996/vht/console.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    55124 2024-05-09 10:48:54.000000 vht-0.3.996/vht/controllereditor.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6976 2024-05-08 12:01:32.000000 vht-0.3.996/vht/controllersview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5707 2024-05-08 12:01:32.000000 vht-0.3.996/vht/controllersviewrow.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4560 2024-05-08 12:01:32.000000 vht-0.3.996/vht/controllerundobuffer.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2909 2024-05-08 12:01:32.000000 vht-0.3.996/vht/ctrlcfg.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1910 2024-05-08 12:01:32.000000 vht-0.3.996/vht/extras.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1298 2024-05-08 12:01:32.000000 vht-0.3.996/vht/filerotator.py
+-rwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)    11508 2024-06-01 07:46:37.000000 vht-0.3.996/vht/main.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    18736 2024-05-31 14:20:00.000000 vht-0.3.996/vht/mainwin.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    14192 2024-05-08 12:01:32.000000 vht-0.3.996/vht/mandymenu.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    18144 2024-05-08 12:01:32.000000 vht-0.3.996/vht/mandyview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2401 2024-05-08 12:01:32.000000 vht-0.3.996/vht/midimapview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4176 2024-05-08 12:01:32.000000 vht-0.3.996/vht/midimapviewrow.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1299 2024-05-08 12:01:32.000000 vht-0.3.996/vht/notebooklabel.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4721 2024-05-08 12:01:32.000000 vht-0.3.996/vht/poormanspiano.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2677 2024-05-08 12:01:32.000000 vht-0.3.996/vht/portconfig.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3547 2024-05-08 12:01:32.000000 vht-0.3.996/vht/portconfigpopover.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7770 2024-05-28 19:34:11.000000 vht-0.3.996/vht/portconfigview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    24678 2024-05-28 18:53:13.000000 vht-0.3.996/vht/preferenceswin.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6623 2024-05-08 12:01:32.000000 vht-0.3.996/vht/probeditor.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4996 2024-05-08 12:01:32.000000 vht-0.3.996/vht/propview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1035 2024-05-08 12:01:32.000000 vht-0.3.996/vht/pulsar.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1100 2024-05-08 12:01:32.000000 vht-0.3.996/vht/randomcomposer.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     8188 2024-05-28 20:16:35.000000 vht-0.3.996/vht/renderer.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     9640 2024-05-27 12:29:20.000000 vht-0.3.996/vht/renderwin.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    15715 2024-05-08 12:01:32.000000 vht-0.3.996/vht/sequencelistview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    13404 2024-05-29 20:09:20.000000 vht-0.3.996/vht/sequencelistviewpopover.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    11262 2024-05-08 12:01:32.000000 vht-0.3.996/vht/sequencepropviewpopover.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    12223 2024-05-08 12:01:32.000000 vht-0.3.996/vht/sequencetriggersview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    37321 2024-05-08 12:01:32.000000 vht-0.3.996/vht/sequenceview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6644 2024-05-29 18:59:49.000000 vht-0.3.996/vht/shortcutmayhem.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    20316 2024-05-08 12:01:32.000000 vht-0.3.996/vht/sidetrackview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    19612 2024-05-08 12:01:32.000000 vht-0.3.996/vht/statusbar.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2879 2024-05-08 12:01:32.000000 vht-0.3.996/vht/thumbmanager.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    51601 2024-05-08 12:01:32.000000 vht-0.3.996/vht/timelineview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6308 2024-05-08 12:01:32.000000 vht-0.3.996/vht/timeshifteditor.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    22027 2024-05-08 12:01:32.000000 vht-0.3.996/vht/trackpropview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    31965 2024-05-08 12:01:32.000000 vht-0.3.996/vht/trackpropviewpopover.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3229 2024-05-08 12:01:32.000000 vht-0.3.996/vht/trackundobuffer.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    96428 2024-05-15 11:23:14.000000 vht-0.3.996/vht/trackview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     9212 2024-05-08 12:01:32.000000 vht-0.3.996/vht/trackviewpointer.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     8127 2024-05-08 12:01:32.000000 vht-0.3.996/vht/velocityeditor.py
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-06-01 08:02:32.873083 vht-0.3.996/vht.egg-info/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1895 2024-06-01 08:02:32.000000 vht-0.3.996/vht.egg-info/PKG-INFO
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2606 2024-06-01 08:02:32.000000 vht-0.3.996/vht.egg-info/SOURCES.txt
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)        1 2024-06-01 08:02:32.000000 vht-0.3.996/vht.egg-info/dependency_links.txt
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       38 2024-06-01 08:02:32.000000 vht-0.3.996/vht.egg-info/entry_points.txt
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       27 2024-06-01 08:02:32.000000 vht-0.3.996/vht.egg-info/top_level.txt
```

### Comparing `vht-0.3.99/LICENSE` & `vht-0.3.996/LICENSE`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/PKG-INFO` & `vht-0.3.996/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vht
-Version: 0.3.99
+Version: 0.3.996
 Summary: vahatraker - a live MIDI sequencer for pipewire/JACK
 Home-page: https://github.com/rdybka/vht
 Author: Remigiusz Dybka
 Author-email: remigiusz.dybka@gmail.com
 License: GPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vht-0.3.99/README.md` & `vht-0.3.996/README.md`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/data/bank/10-gm1` & `vht-0.3.996/data/bank/10-gm1`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/data/bank/20-gm2` & `vht-0.3.996/data/bank/20-gm2`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/data/io.github.rdybka.vht.metainfo.xml` & `vht-0.3.996/data/io.github.rdybka.vht.metainfo.xml`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/data/io.github.rdybka.vht.png` & `vht-0.3.996/data/io.github.rdybka.vht.png`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/data/mandy.png` & `vht-0.3.996/data/mandy.png`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/data/menu.ui` & `vht-0.3.996/data/menu.ui`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/data/menu_norend.ui` & `vht-0.3.996/data/menu_norend.ui`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/data/vht.png` & `vht-0.3.996/data/vht.png`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/data/vht.svg` & `vht-0.3.996/data/vht.svg`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/doc/vht.1.md` & `vht-0.3.996/doc/vht.1.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-% VHT(1) vht 0.3.99
+% VHT(1) vht 0.3.996
 % Remigiusz Dybka
 % May 2024
 
 # NAME
 **vht** - a minimalistic MIDI sequencer for JACK/GNOME
 
 # SYNOPSIS
```

### Comparing `vht-0.3.99/libvht/ctrlrow.c` & `vht-0.3.996/libvht/ctrlrow.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/ctrlrow.h` & `vht-0.3.996/libvht/ctrlrow.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/envelope.c` & `vht-0.3.996/libvht/envelope.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/envelope.h` & `vht-0.3.996/libvht/envelope.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/jack_process.c` & `vht-0.3.996/libvht/jack_process.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/jack_process.h` & `vht-0.3.996/libvht/jack_process.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/libcvht.h` & `vht-0.3.996/libvht/libcvht.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/libcvht.py` & `vht-0.3.996/libvht/libcvht.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/libcvht_wrap.c` & `vht-0.3.996/libvht/libcvht_wrap.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/libvht.c` & `vht-0.3.996/libvht/libvht.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/mandy.c` & `vht-0.3.996/libvht/mandy.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/mandy.h` & `vht-0.3.996/libvht/mandy.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/mandy_pix_scan.c` & `vht-0.3.996/libvht/mandy_pix_scan.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/mandy_pix_scan.h` & `vht-0.3.996/libvht/mandy_pix_scan.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/mandy_trk_disp.c` & `vht-0.3.996/libvht/mandy_trk_disp.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/mandy_trk_disp.h` & `vht-0.3.996/libvht/mandy_trk_disp.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/midi_client.c` & `vht-0.3.996/libvht/midi_client.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/midi_client.h` & `vht-0.3.996/libvht/midi_client.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/midi_event.c` & `vht-0.3.996/libvht/midi_event.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/midi_event.h` & `vht-0.3.996/libvht/midi_event.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/module.c` & `vht-0.3.996/libvht/module.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/module.h` & `vht-0.3.996/libvht/module.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/row.c` & `vht-0.3.996/libvht/row.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/row.h` & `vht-0.3.996/libvht/row.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/sequence.c` & `vht-0.3.996/libvht/sequence.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/sequence.h` & `vht-0.3.996/libvht/sequence.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/smf.c` & `vht-0.3.996/libvht/smf.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/smf.h` & `vht-0.3.996/libvht/smf.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/stolen.c` & `vht-0.3.996/libvht/stolen.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/timeline.c` & `vht-0.3.996/libvht/timeline.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/timeline.h` & `vht-0.3.996/libvht/timeline.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/track.c` & `vht-0.3.996/libvht/track.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/track.h` & `vht-0.3.996/libvht/track.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/tracy.c` & `vht-0.3.996/libvht/tracy.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/tracy.h` & `vht-0.3.996/libvht/tracy.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/vhtcolumn.py` & `vht-0.3.996/libvht/vhtcolumn.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/vhtctrl.py` & `vht-0.3.996/libvht/vhtctrl.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/vhtctrllist.py` & `vht-0.3.996/libvht/vhtctrllist.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/vhtctrlrow.py` & `vht-0.3.996/libvht/vhtctrlrow.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/vhtextras.py` & `vht-0.3.996/libvht/vhtextras.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/vhtmandy.py` & `vht-0.3.996/libvht/vhtmandy.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/vhtmodule.py` & `vht-0.3.996/libvht/vhtmodule.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/vhtport.py` & `vht-0.3.996/libvht/vhtport.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/vhtports.py` & `vht-0.3.996/libvht/vhtports.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/vhtquicklist.py` & `vht-0.3.996/libvht/vhtquicklist.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/vhtrow.py` & `vht-0.3.996/libvht/vhtrow.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/vhtsequence.py` & `vht-0.3.996/libvht/vhtsequence.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/vhttimeline.py` & `vht-0.3.996/libvht/vhttimeline.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/vhttimelinechange.py` & `vht-0.3.996/libvht/vhttimelinechange.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/vhttimelinechanges.py` & `vht-0.3.996/libvht/vhttimelinechanges.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/vhttimelineloop.py` & `vht-0.3.996/libvht/vhttimelineloop.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/vhttimelineslices.py` & `vht-0.3.996/libvht/vhttimelineslices.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/vhttimelinestrip.py` & `vht-0.3.996/libvht/vhttimelinestrip.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/vhttimelinestrips.py` & `vht-0.3.996/libvht/vhttimelinestrips.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/vhttimelineticks.py` & `vht-0.3.996/libvht/vhttimelineticks.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/vhttrack.py` & `vht-0.3.996/libvht/vhttrack.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/libvht/vhttracy.py` & `vht-0.3.996/libvht/vhttracy.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/pyproject.toml` & `vht-0.3.996/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = 'setuptools.build_meta'
 requires = ["setuptools>=61.0"]
 [metadata]
 name = "vht"
-version = "0.3.99"
+version = "0.3.996"
 description = "vahatraker - a live MIDI sequencer for pipewire/JACK"
 author = "Remigiusz Dybka"
 author_email = "remigiusz.dybka@gmail.com"
 url = "https://github.com/rdybka/vht"
 long_description = "file: README.md"
 long_description_content_type = "text/markdown"
 classifiers = [
```

### Comparing `vht-0.3.99/setup.py` & `vht-0.3.996/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, Extension
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name = "vht",
-	version = "0.3.99",
+	version = "0.3.996",
 	description = "vahatraker - a live MIDI sequencer for pipewire/JACK",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	author = "Remigiusz Dybka",
 	author_email = "remigiusz.dybka@gmail.com",
 	url = "https://github.com/rdybka/vht",
 	license = 'GPLv3+',
```

### Comparing `vht-0.3.99/vht/autoexec.py` & `vht-0.3.996/vht/autoexec.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/bankcfg.py` & `vht-0.3.996/vht/bankcfg.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/capturebutton.py` & `vht-0.3.996/vht/capturebutton.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/codedaemon.py` & `vht-0.3.996/vht/codedaemon.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/configuration.py` & `vht-0.3.996/vht/configuration.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/console.py` & `vht-0.3.996/vht/console.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/controllereditor.py` & `vht-0.3.996/vht/controllereditor.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/controllersview.py` & `vht-0.3.996/vht/controllersview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/controllersviewrow.py` & `vht-0.3.996/vht/controllersviewrow.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/controllerundobuffer.py` & `vht-0.3.996/vht/controllerundobuffer.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/ctrlcfg.py` & `vht-0.3.996/vht/ctrlcfg.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/extras.py` & `vht-0.3.996/vht/extras.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/filerotator.py` & `vht-0.3.996/vht/filerotator.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/main.py` & `vht-0.3.996/vht/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 # I hereby testify,
-# on Sweetmorn, the 5nd day of Confusion in the YOLD 3190,
+# on Boomtime, the 6nd day of Confusion in the YOLD 3190,
 # that everything in this program checks out with The Law of Fives
 
 # [^^^intentionally left blank]
 
 import gi
 
 gi.require_version("Gtk", "3.0")
@@ -309,15 +309,15 @@
     print("vahatraker %s" % (pkg.version))
 
     mod.start_error = None
     if mod.midi_start() != 0:
         mod.start_error = "you will need JACK for this"
 
     # fix local config path
-    mod.cfg_path = os.path.expanduser("~/.config/vht")
+    mod.cfg_path = GLib.get_user_config_dir()
     if not os.path.exists(mod.cfg_path):
         print("creating", mod.cfg_path)
         os.mkdir(mod.cfg_path)
 
     cfg.load(os.path.join(mod.cfg_path, "config.ini"))
 
     mod.ctrlpr = cfg.controller_resolution
@@ -330,15 +330,14 @@
 
     vht.extras.register(mod)
     mod.set_midi_record_ignore(midig)
     randomcomposer.muzakize()
     mod.cdaemon = CodeDaemon()
     # fix data path
     paths2try = []
-
     paths2try.append(os.path.normpath(os.path.join(pkg.module_path, "data")))
     paths2try.append(os.path.normpath(os.path.join(pkg.module_path, "share/vht")))
 
     p = pkg.module_path
     pf = p.find("/lib")
     if pf:
         p = p[:pf]
```

### Comparing `vht-0.3.99/vht/mainwin.py` & `vht-0.3.996/vht/mainwin.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/mandymenu.py` & `vht-0.3.996/vht/mandymenu.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/mandyview.py` & `vht-0.3.996/vht/mandyview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/midimapview.py` & `vht-0.3.996/vht/midimapview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/midimapviewrow.py` & `vht-0.3.996/vht/midimapviewrow.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/notebooklabel.py` & `vht-0.3.996/vht/notebooklabel.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/poormanspiano.py` & `vht-0.3.996/vht/poormanspiano.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/portconfig.py` & `vht-0.3.996/vht/portconfig.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/portconfigpopover.py` & `vht-0.3.996/vht/portconfigpopover.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/portconfigview.py` & `vht-0.3.996/vht/portconfigview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/preferenceswin.py` & `vht-0.3.996/vht/preferenceswin.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/probeditor.py` & `vht-0.3.996/vht/probeditor.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/propview.py` & `vht-0.3.996/vht/propview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/pulsar.py` & `vht-0.3.996/vht/pulsar.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/randomcomposer.py` & `vht-0.3.996/vht/randomcomposer.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/renderer.py` & `vht-0.3.996/vht/renderer.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/renderwin.py` & `vht-0.3.996/vht/renderwin.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/sequencelistview.py` & `vht-0.3.996/vht/sequencelistview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/sequencelistviewpopover.py` & `vht-0.3.996/vht/sequencelistviewpopover.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/sequencepropviewpopover.py` & `vht-0.3.996/vht/sequencepropviewpopover.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/sequencetriggersview.py` & `vht-0.3.996/vht/sequencetriggersview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/sequenceview.py` & `vht-0.3.996/vht/sequenceview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/shortcutmayhem.py` & `vht-0.3.996/vht/shortcutmayhem.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/sidetrackview.py` & `vht-0.3.996/vht/sidetrackview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/statusbar.py` & `vht-0.3.996/vht/statusbar.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/thumbmanager.py` & `vht-0.3.996/vht/thumbmanager.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/timelineview.py` & `vht-0.3.996/vht/timelineview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/timeshifteditor.py` & `vht-0.3.996/vht/timeshifteditor.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/trackpropview.py` & `vht-0.3.996/vht/trackpropview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/trackpropviewpopover.py` & `vht-0.3.996/vht/trackpropviewpopover.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/trackundobuffer.py` & `vht-0.3.996/vht/trackundobuffer.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/trackview.py` & `vht-0.3.996/vht/trackview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/trackviewpointer.py` & `vht-0.3.996/vht/trackviewpointer.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht/velocityeditor.py` & `vht-0.3.996/vht/velocityeditor.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.99/vht.egg-info/PKG-INFO` & `vht-0.3.996/vht.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vht
-Version: 0.3.99
+Version: 0.3.996
 Summary: vahatraker - a live MIDI sequencer for pipewire/JACK
 Home-page: https://github.com/rdybka/vht
 Author: Remigiusz Dybka
 Author-email: remigiusz.dybka@gmail.com
 License: GPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vht-0.3.99/vht.egg-info/SOURCES.txt` & `vht-0.3.996/vht.egg-info/SOURCES.txt`

 * *Files identical despite different names*

