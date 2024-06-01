# Comparing `tmp/rwmapeditor_exgcdwu-1.4.2.tar.gz` & `tmp/rwmapeditor_exgcdwu-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwmapeditor_exgcdwu-1.4.2.tar", last modified: Sun May  5 06:28:23 2024, max compression
+gzip compressed data, was "rwmapeditor_exgcdwu-1.4.3.tar", last modified: Sat Jun  1 05:48:31 2024, max compression
```

## Comparing `rwmapeditor_exgcdwu-1.4.2.tar` & `rwmapeditor_exgcdwu-1.4.3.tar`

### file list

```diff
@@ -1,321 +1,330 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.607302 rwmapeditor_exgcdwu-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    42254 2024-05-05 06:28:23.607302 rwmapeditor_exgcdwu-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.551302 rwmapeditor_exgcdwu-1.4.2/rwmap/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.551302 rwmapeditor_exgcdwu-1.4.2/rwmap/_case/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_case/_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_case/_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_case/_objectgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    10270 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_case/_tileset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15395 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.551302 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.551302 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_credit.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_mapText.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_mapinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_unitAdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_unitDetect.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_unitRemove.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.551302 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.555302 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14198 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/_city.py
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/_city_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/_city_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/_city_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/_normal_unit_add.py
--rw-r--r--   0 runner    (1001) docker     (127)    15130 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/_refresh_building.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.555302 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_count/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_count/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_count/_flash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.555302 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_troop/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_troop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_troop/_troop_add.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.555302 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_victory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_victory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_victory/_victory_co.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.555302 rwmapeditor_exgcdwu-1.4.2/rwmap/_frame/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_frame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_frame/_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_frame/_element_ori.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_frame/_element_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.559302 rwmapeditor_exgcdwu-1.4.2/rwmap/_object/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_object/_object_global.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_object/_object_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_object/_object_one_and_acti.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_object/_object_pos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_object/_object_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_object/_object_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.559302 rwmapeditor_exgcdwu-1.4.2/rwmap/_otgroup/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_otgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_otgroup/_object_tile_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.559302 rwmapeditor_exgcdwu-1.4.2/rwmap/_tile/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_tile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7448 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_tile/_tile_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.559302 rwmapeditor_exgcdwu-1.4.2/rwmap/_util/
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_add_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_class_rel.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_coo_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_dict_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_etElement_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_list_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_matrix_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_png_rel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_str_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.559302 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.559302 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.591302 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/
--rw-r--r--   0 runner    (1001) docker     (127)    66356 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/bridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/decoration.png
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/deepwater.png
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt.png
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    11405 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt_details.png
--rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dust.png
--rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/fauna.png
--rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/fauna_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    21273 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/fauna_highland.png
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice.png
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/lava.png
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/lava2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/lava2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    22847 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass.png
--rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16002 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16661 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)    15956 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    17103 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16817 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    17019 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/misc.png
--rw-r--r--   0 runner    (1001) docker     (127)    14082 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain.png
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13512 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9946 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    14341 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13230 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/nothing2road_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand.png
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2.png
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2_old.png
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    19617 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2lava_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10227 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2sand_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2stone_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    23903 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater.png
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shortgrass.png
--rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow.png
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2snow_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone.png
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2lava.png
--rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2snow.png
--rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)   111877 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/units.png
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/water.png
--rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/decoration.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/misc.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.603302 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Dirt Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Dirt ShalowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Ice Ice - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Ice ShallowWater - Broken.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Ice ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/LongGrass Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/LongGrass Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/LongGrass LongGrass - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/LongGrass ShortGrass - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain LongGrass - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Mountain - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Mountain - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Nothing - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Sand - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Snow - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Stone - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Nothing Dust - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Nothing Road - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Nothing Sand - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Sand Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Sand Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Sand LandGrass - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Sand Nothing - Flat - 2.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Sand Nothing - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Sand Sand - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Sand ShallowWater - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Sand ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/ShallowWater Water - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Snow Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Snow Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Snow Ice - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Snow Snow - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Snow Snow - ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Stone Sand - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Stone ShallowWater - ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Stone Snow - ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Water DeepWater - Flat.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.603302 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Deep Water.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Dirt.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Dirt_Details.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Dust.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Ice.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Lava.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Long Grass.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Mountain.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Sand.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Shallow Water.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Short Grass.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Snow.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Stone.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Water.tsx
--rw-r--r--   0 runner    (1001) docker     (127)    22727 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/units.tsx
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:28:23.607302 rwmapeditor_exgcdwu-1.4.2/rwmapeditor_exgcdwu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42254 2024-05-05 06:28:23.000000 rwmapeditor_exgcdwu-1.4.2/rwmapeditor_exgcdwu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14028 2024-05-05 06:28:23.000000 rwmapeditor_exgcdwu-1.4.2/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 06:28:23.000000 rwmapeditor_exgcdwu-1.4.2/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-05 06:28:23.000000 rwmapeditor_exgcdwu-1.4.2/rwmapeditor_exgcdwu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 06:28:23.000000 rwmapeditor_exgcdwu-1.4.2/rwmapeditor_exgcdwu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-05 06:28:23.607302 rwmapeditor_exgcdwu-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-05 06:28:15.000000 rwmapeditor_exgcdwu-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:31.295586 rwmapeditor_exgcdwu-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    42254 2024-06-01 05:48:31.295586 rwmapeditor_exgcdwu-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:31.235587 rwmapeditor_exgcdwu-1.4.3/hexrwmap/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/hexrwmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/hexrwmap/_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/hexrwmap/_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:31.235587 rwmapeditor_exgcdwu-1.4.3/hexrwmap/_util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/hexrwmap/_util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:31.235587 rwmapeditor_exgcdwu-1.4.3/rwmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:31.239586 rwmapeditor_exgcdwu-1.4.3/rwmap/_case/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_case/_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_case/_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_case/_objectgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11025 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_case/_tileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15724 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:31.239586 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:31.239586 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject/_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject/_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject/_mapText.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject/_mapinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject/_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject/_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject/_unitAdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject/_unitDetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject/_unitRemove.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:31.239586 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:31.239586 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_city/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_city/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14198 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_city/_city.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_city/_city_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_city/_city_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_city/_city_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_city/_normal_unit_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15130 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_city/_refresh_building.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:31.243586 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_count/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_count/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_count/_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_count/_flash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_count/_score_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_count/_time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:31.243586 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_troop/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_troop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_troop/_troop_add.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:31.243586 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_victory/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_victory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_victory/_victory_co.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:31.243586 rwmapeditor_exgcdwu-1.4.3/rwmap/_frame/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_frame/_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_frame/_element_ori.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_frame/_element_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:31.243586 rwmapeditor_exgcdwu-1.4.3/rwmap/_object/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_object/_object_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_object/_object_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_object/_object_one_and_acti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_object/_object_pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_object/_object_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_object/_object_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:31.243586 rwmapeditor_exgcdwu-1.4.3/rwmap/_otgroup/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_otgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_otgroup/_object_tile_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:31.243586 rwmapeditor_exgcdwu-1.4.3/rwmap/_tile/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_tile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7608 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_tile/_tile_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:31.247587 rwmapeditor_exgcdwu-1.4.3/rwmap/_util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_util/_add_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_util/_class_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_util/_coo_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_util/_dict_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_util/_etElement_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_util/_list_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_util/_matrix_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_util/_png_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/_util/_str_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:31.247587 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:31.247587 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:31.279586 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/
+-rw-r--r--   0 runner    (1001) docker     (127)    66356 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/bridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/decoration.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/deepwater.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11405 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt_details.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dust.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/fauna.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/fauna_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21273 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/fauna_highland.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/lava.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/lava2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/lava2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22847 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16002 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16661 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15956 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17103 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16817 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17019 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/misc.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14082 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13512 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9946 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14341 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13230 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/nothing2road_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2_old.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19617 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10227 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2sand_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23903 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/shallowwater.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/shortgrass.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2snow_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2lava.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2snow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)   111877 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/units.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/water.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/decoration.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/misc.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:31.291586 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Dirt Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Dirt ShalowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Ice Ice - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Ice ShallowWater - Broken.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Ice ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/LongGrass Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/LongGrass Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/LongGrass LongGrass - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/LongGrass ShortGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Mountain Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Mountain Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Mountain LongGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Mountain Mountain - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Mountain Mountain - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Mountain Nothing - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Mountain Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Mountain ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Mountain Snow - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Mountain Stone - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Nothing Dust - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Nothing Road - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Nothing Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Sand Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Sand Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Sand LandGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Sand Nothing - Flat - 2.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Sand Nothing - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Sand Sand - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Sand ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Sand ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/ShallowWater Water - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Snow Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Snow Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Snow Ice - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Snow Snow - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Snow Snow - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Stone Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Stone ShallowWater - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Stone Snow - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Water DeepWater - Flat.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:31.291586 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/terrain/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/terrain/Deep Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/terrain/Dirt.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/terrain/Dirt_Details.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/terrain/Dust.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/terrain/Ice.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/terrain/Lava.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/terrain/Long Grass.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/terrain/Mountain.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/terrain/Sand.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/terrain/Shallow Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/terrain/Short Grass.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/terrain/Snow.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/terrain/Stone.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/terrain/Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)    22727 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/units.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:48:31.295586 rwmapeditor_exgcdwu-1.4.3/rwmapeditor_exgcdwu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42254 2024-06-01 05:48:31.000000 rwmapeditor_exgcdwu-1.4.3/rwmapeditor_exgcdwu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14246 2024-06-01 05:48:31.000000 rwmapeditor_exgcdwu-1.4.3/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 05:48:31.000000 rwmapeditor_exgcdwu-1.4.3/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-01 05:48:31.000000 rwmapeditor_exgcdwu-1.4.3/rwmapeditor_exgcdwu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-01 05:48:31.000000 rwmapeditor_exgcdwu-1.4.3/rwmapeditor_exgcdwu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-01 05:48:31.295586 rwmapeditor_exgcdwu-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-06-01 05:48:24.000000 rwmapeditor_exgcdwu-1.4.3/setup.py
```

### Comparing `rwmapeditor_exgcdwu-1.4.2/LICENSE` & `rwmapeditor_exgcdwu-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/PKG-INFO` & `rwmapeditor_exgcdwu-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwmapeditor_exgcdwu
-Version: 1.4.2
+Version: 1.4.3
 Home-page: https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-
 Author: exgcdwu
 Author-email: 1006605318@qq.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `rwmapeditor_exgcdwu-1.4.2/README.md` & `rwmapeditor_exgcdwu-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_case/_layer.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_case/_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,16 +45,16 @@
         root.append(utility.get_etElement_from_text_packed(self._tilematrix, self._encoding, self._compression))
         return root
     
     def name(self)->str:
         return self._properties.returnDefaultProperty("name")
     
     def size(self)->frame.Coordinate:
-        return frame.Coordinate(int(self._properties.returnDefaultProperty("width")), 
-                                int(self._properties.returnDefaultProperty("height")))
+        return frame.Coordinate(int(self._properties.returnDefaultProperty("height")), 
+                                int(self._properties.returnDefaultProperty("width")))
 
     def __repr__(self)->str:
         return self.output_str()
 
     def id(self)->int:
         return int(self._properties.returnDefaultProperty("id"))
```

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_case/_object.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_case/_object.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_case/_objectgroup.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_case/_objectgroup.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_case/_tileset.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_case/_tileset.py`

 * *Files 13% similar despite different names*

```diff
@@ -157,14 +157,28 @@
     
     def name(self)->str:
         tileset_name = self._properties.returnDefaultProperty("name")
         if tileset_name == None:
             tileset_name = self._properties.returnDefaultProperty("source")
             tileset_name = utility.str_slash_to_dot(tileset_name)
         return tileset_name
+
+    def change_name(self, new_name:str)->None:
+        tileset_name = self._properties.returnDefaultProperty("name")
+        if tileset_name != None:
+            self._properties.assignDefaultProperty("name", new_name)
+
+        tileset_name = self._properties.returnDefaultProperty("source")
+        if tileset_name != None:
+            tileset_name_len = len(utility.str_slash_to_dot(tileset_name))
+            self._properties.assignDefaultProperty("source", tileset_name[0:-tileset_name_len-4] + new_name + ".tmx")
+
+        tileset_name = self._image_properties.returnDefaultProperty("source")
+        if tileset_name != None:
+            self._image_properties.assignDefaultProperty("source", tileset_name[0:-tileset_name_len-4] + new_name + ".png")
     
     def totalgid(self)->int:
         return self._size.x() * self._size.y()
 
     def firstgid(self)->int:
         return int(self._properties.returnDefaultProperty("firstgid"))
```

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_core.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,14 +73,21 @@
         return frame.Coordinate(int(self._properties.returnDefaultProperty("width")), 
                                 int(self._properties.returnDefaultProperty("height")))
     
     def tile_size(self)->frame.Coordinate:
         return frame.Coordinate(int(self._properties.returnDefaultProperty("tilewidth")), 
                                 int(self._properties.returnDefaultProperty("tileheight")))
     
+    def end_point_layer(self)->frame.Coordinate:
+        return frame.Coordinate(int(self._properties.returnDefaultProperty("height")), 
+                                int(self._properties.returnDefaultProperty("width")))
+    
+    def end_point_object(self)->frame.Coordinate:
+        return self.size() * self.tile_size()
+    
     def nextlayerid(self)->int:
         return int(self._properties.returnDefaultProperty("nextlayerid"))
     
     def changenextlayerid(self, layerid:int)->None:
         self._properties.assignDefaultProperty("nextlayerid", str(layerid))
 
     def nextobjectid(self)->int:
```

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_credit.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject/_credit.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_mapText.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject/_mapText.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_mapinfo.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject/_mapinfo.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_message.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject/_message.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_node.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject/_node.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_unitDetect.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject/_unitDetect.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 from rwmap._object._object_time import _make_tobject_time
 
 class UnitDetect(object.TObject_One):
     def __init__(self, pos:frame.Coordinate, size:frame.Coordinate, name:str = None,
                  team:int = None, minUnits:int = None, maxUnits:int = None, 
                  unitType:str = None, onlyList:list[str] = [], warmup:int = -1, reset:int = -1, 
                  isdelay:bool = False, isrepeat:bool = False, 
-                 id:str = None, alsoacti_s:list[object.TObject_One] = []):
+                 id:str = None, alsoacti_s:list[object.TObject_One] = [], issecond:bool = True):
         upos = frame.Rectangle(pos, size)
         object.TObject_One.__init__(self, object.TObject_Type.init_unitDetect(team = team, minUnits = minUnits, maxUnits = maxUnits, 
                                                                               unitType = unitType, onlyList = onlyList), 
                                     object.TObject_Pos.init_rectangle(upos), 
                                     name, object.TObject_Acti.init_acti(id = id, alsoacti_s = alsoacti_s), 
-                                    _make_tobject_time(warmup = warmup, reset = reset, isdelay = isdelay, isrepeat = isrepeat))
+                                    _make_tobject_time(warmup = warmup, reset = reset, isdelay = isdelay, isrepeat = isrepeat, issecond = issecond))
```

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject/_unitRemove.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject/_unitRemove.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/__init__.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from rwmap._data.tobject_group._city._city import City, CityNoTeam, CityAllTeam, CityAllTeamGroup
 from rwmap._data.tobject_group._city._refresh_building import RefreshBuilding, RefreshBuildingNoTeam, RefreshBuildingAllTeam, RefreshBuildingAllTeamGroup
 from rwmap._data.tobject_group._city._city_detect import BuildingDetect, BuildingDetectNoTeam, BuildingDetectAllTeam, BuildingDetectAllTeamGroup
 from rwmap._data.tobject_group._city._city_text import CityText, CityTextNoTeam, CityTextAllTeam
 from rwmap._data.tobject_group._city._normal_unit_add import NormalUnitAdd, NormalUnitAddInstant
 from rwmap._data.tobject_group._city._city_remove import unitRemoveAllTeam
 from rwmap._data.tobject_group._troop._troop_add import RefreshTroop
-from rwmap._data.tobject_group._count._flash import Flash
+from rwmap._data.tobject_group._count import *
+from rwmap._data.tobject_group._victory import *
```

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/_city.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_city/_city.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/_city_detect.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_city/_city_detect.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/_city_remove.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_city/_city_remove.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/_city_text.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_city/_city_text.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/_normal_unit_add.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_city/_normal_unit_add.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_city/_refresh_building.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_city/_refresh_building.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_count/_flash.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_count/_flash.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 import rwmap._util as utility
 
 class Flash(object.TObject_Group):
     def __init__(self, pos: frame.Coordinate, delay:Union[int, float], 
                  pre_period:Union[int, float], period:Union[int, float], 
                  id:str, issecond:bool = True, 
-                 size:frame.Coordinate = const.COO.SIZE_STANDARD, 
+                 size:frame.Coordinate = const.COO.SIZE_STANDARD * 2, 
                  name_add:str = None, name_detect:str = None, name_remove:str = None, 
-                 units:str = "antiAirTurret", delayisdetect:bool = True, reset_detect = 0.25):
+                 units:str = const.UNIT.c_antiAirTurretT3, delayisdetect:bool = True, reset_detect = 0.25):
         uadd_s = tobject.UnitAdd(pos, -2, spawnUnits = units, size = size, 
                                  name = name_add, warmup = delay, reset = period, 
                                  isdelay = True, isrepeat = True)
         minUnits = -1 if delayisdetect else 1
         maxUnits = 0 if delayisdetect else -1
         udetect_s = tobject.UnitDetect(pos, size, name = name_detect, team = -2, 
                                        minUnits = minUnits, maxUnits = maxUnits, 
@@ -36,10 +36,10 @@
     
     def unitRemove_s(self)->tobject.UnitRemove:
         return self._TObject_One_list[1]
     
     def unitDetect_s(self)->tobject.UnitDetect:
         return self._TObject_One_list[2]
 
-    def idTObject_s(self)->list[object.TObject_One]:
+    def idTObject_s(self)->object.TObject_One:
         return self.unitDetect_s().idTObject_s()
```

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_troop/_troop_add.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_troop/_troop_add.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_data/tobject_group/_victory/_victory_co.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_data/tobject_group/_victory/_victory_co.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,34 +19,43 @@
         size:frame.Coordinate = const.COO.SIZE_STANDARD
         uadd_s = []
         size_x = frame.Coordinate(size.x(), 0)
         size_y = frame.Coordinate(0, size.y())
         for index, team in enumerate(team_list):
             name_l = name_add_l_list[index] if index < len(name_add_l_list) else None
             name_b = name_add_b_list[index] if index < len(name_add_b_list) else None
-            pos_l = 2 * index * size_x + pos
-            pos_b = 2 * index * size_x + pos + 2 * size_y
+            pos_l = size_x * 2 * index + pos
+            pos_b = size_x * 2 * index + pos + size_y * 2
             uadd_s.append(NormalUnitAddInstant(pos_l, team, "landFactory", size = size, name = name_l))
             uadd_s.append(NormalUnitAddInstant(pos_b, team, "builder", size = size, name = name_b))
-        uremove_s = tobject.UnitRemove(pos, (2 * len(team_list) - 1) * size_x + 3 * size_y, name = name_remove, actiBy_s = actiBy_s, 
+        uremove_s = tobject.UnitRemove(pos, size_x * (2 * len(team_list) - 1) + size_y * 3, name = name_remove, actiBy_s = actiBy_s, 
                                        deactiBy_s = deactiBy_s, isalltoacti = isalltoacti)
-        object.TObject_Group.__init__(self, [], uadd_s + [uremove_s])
+        object.TObject_Group.__init__(self, [uremove_s], uadd_s)
 
     def unitRemove_s(self)->tobject.UnitRemove:
-        return self._TObject_Group_list[-1]
+        return self._TObject_One_list[0]
 
     def add_actiBy_s(self, actiBy_s:Union[list[object.TObject_One], object.TObject_One]):
         actiBy_s_list = deepcopy(utility.list_variable_s(actiBy_s))
         self.unitRemove_s().add_actiBy_s(actiBy_s_list)
 
     def add_deactiBy_s(self, deactiBy_s:Union[list[object.TObject_One], object.TObject_One]):
         deactiBy_s_list = deepcopy(utility.list_variable_s(deactiBy_s))
         self.unitRemove_s().add_deactiBy_s(deactiBy_s_list)
 
     def add_twoactiBy_s(self, add_TObject_One_two_s:tuple[list[object.TObject_One], 
                                                           list[object.TObject_One]] = ([], [])):
         self.unitRemove_s().add_twoactiBy_s(add_TObject_One_two_s)
 
+    def actiBy_s(self)->list[object.TObject_One]:
+        return self.unitRemove_s()._acti._actiBy_s
+
+    def deactiBy_s(self)->list[object.TObject_One]:
+        return self.unitRemove_s()._acti._deactiBy_s
+
+    def twoactiBy_s(self)->tuple[list[object.TObject_One], list[object.TObject_One]]:
+        return [self.actiBy_s(), self.deactiBy_s()]
+
```

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_frame/_coordinate.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_frame/_coordinate.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,17 @@
     
     def id(self, width:int)->int:
         return int(self.x() * width + self.y())
     
     def transpose(self)->Coordinate:
         return Coordinate(self.y(), self.x(), self._content.dtype)
 
+    def changetype(self, dtype)->Coordinate:
+        return Coordinate(self.x(), self.y(), dtype)
+
     def __add__(self, other):
         if isinstance(other, Coordinate):
             return Coordinate(self.x() + other.x(), self.y() + other.y(), self._content.dtype)
         else:
             return Coordinate(other + self.x(), other + self.y(), self._content.dtype)
 
     def __mul__(self, other):
```

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_frame/_element_ori.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_frame/_element_ori.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_frame/_element_property.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_frame/_element_property.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_object/_object_global.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_object/_object_global.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 
     def output_optional_properties(self):
         return deepcopy(self._optional_properties)
     
     @classmethod
     def init_global(cls, message:str, delayPerChar:int = -1, textColor:str = None, issecond:bool = True):
         op_dict = {}
-        op_dict.update({"globalMessage", message})
+        op_dict.update({"globalMessage": message})
         op_dict.update(utility.add_time_pro("globalMessage_delayPerChar", delayPerChar, issecond))
         op_dict.update(utility.add_str_pro("globalMessage_textColor", textColor))
         return cls(op_dict)
```

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_object/_object_group.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_object/_object_group.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_object/_object_one_and_acti.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_object/_object_one_and_acti.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         return self._idTObject_One_s
 
     def output_optional_properties(self)->dict[str, str]:
         op_dict = {}
         if self._idTObject_One_s != None:
             op_dict.update({"id": self._idTObject_One_s._name}) 
         if self._isalltoacti:
-            op_dict.update({"allToActivate": "1"}) 
+            op_dict.update({"allToActivate": {"type": "bool", "value": "true"}}) 
         op_dict.update(utility.add_acti_pro("alsoactivate", self._alsoacti_s))
         op_dict.update(utility.add_acti_pro("activatedBy", self._actiBy_s))
         op_dict.update(utility.add_acti_pro("deactivatedBy", self._deactiBy_s))
         return op_dict
 
 class TObject_One:
     def __init__(self, otype:TObject_Type, pos:TObject_Pos = TObject_Pos({}), name:str = None,
```

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_object/_object_pos.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_object/_object_pos.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 class TObject_Pos:
     def __init__(self, default_properties:dict[str, str], other_properties:list[et.Element] = {}):
         self._default_properties = deepcopy(default_properties)
         self._other_properties = deepcopy(other_properties)
 
     @classmethod
     def init_rectangle(cls, rect:frame.Rectangle):
-        default_properties = {"x": f"{rect.i().x():.0f}", "y": f"{rect.i().y():.0f}", 
-                              "width": f"{rect.a().x():.0f}", "height": f"{rect.a().y():.0f}"}
+        default_properties = {"x": f"{rect.i().x():.2f}", "y": f"{rect.i().y():.2f}", 
+                              "width": f"{rect.a().x():.2f}", "height": f"{rect.a().y():.2f}"}
         return cls(default_properties)
     
     @classmethod
     def init_polygon(cls, point_list:list[frame.Coordinate], midpos:frame.Coordinate):
-        default_properties = {"x": f"{midpos.x():.0f}", "y": f"{midpos.y():.0f}"}
+        default_properties = {"x": f"{midpos.x():.2f}", "y": f"{midpos.y():.2f}"}
         point_list_str = utility.point_list_to_str(point_list)
         other_properties = [et.Element("polygon", {"points": point_list_str})]
         return cls(default_properties, other_properties)
 
     def size(self)->frame.Coordinate:
         return frame.Coordinate(int(self._default_properties["width"]),
                                 int(self._default_properties["height"]))
@@ -41,12 +41,12 @@
     
     def output_other_properties(self):
         return deepcopy(self._other_properties)
     
     def offset(self, offset:frame.Coordinate)->TObject_Pos:
         newtp = deepcopy(self)
         try:
-            newtp._default_properties["x"] = f"{float(self._default_properties["x"]) + offset.x():.0f}"
-            newtp._default_properties["y"] = f"{float(self._default_properties["y"]) + offset.y():.0f}"
+            newtp._default_properties["x"] = f"{float(self._default_properties["x"]) + offset.x():.2f}"
+            newtp._default_properties["y"] = f"{float(self._default_properties["y"]) + offset.y():.2f}"
         except KeyError:
             raise KeyError("Position: uninitialized")
         return newtp
```

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_object/_object_time.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_object/_object_time.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_object/_object_type.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_object/_object_type.py`

 * *Files 21% similar despite different names*

```diff
@@ -30,14 +30,16 @@
         return otype
     
     @classmethod
     def init_unitDetect(cls, team:int = None, minUnits:int = None, maxUnits:int = None, unitType:str = None, onlyList:list[str] = []):
         otype = cls({"type": "unitDetect"}, {})
         otype._add_optional("team", team)
         otype._add_optional("unitType", unitType)
+        minUnits = None if minUnits == -1 else minUnits
+        maxUnits = None if maxUnits == -1 else maxUnits
         otype._add_optional("minUnits", minUnits)
         otype._add_optional("maxUnits", maxUnits)
         for only in onlyList:
             if only[0:13] == "onlyTechLevel":
                 otype._add_optional(only[0:13], only[13])
             else:
                 otype._optional_properties.update({only:{"type": "bool", "value": "true"}})
```

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_tile/_tile_group.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_tile/_tile_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import numpy as np
 from copy import deepcopy
 from typing import Union
 
 import rwmap._frame as frame
 import rwmap._data.const as const
 import rwmap._util as utility
-from rwmap._exceptions import KeyConflictError
+from rwmap._exceptions import KeyConflictError, TileGroupMatrixListOfListError
 from rwmap._data.const import TYPE
 
 tilestate_type = "S20"
 
 class TileGroup_Matrix:
     pass
 
 class TileGroup_Matrix:
     def __init__(self, tilename_matrix:list[list]):
         self._tilematrix = deepcopy(np.array(tilename_matrix, tilestate_type))
+        if len(self._tilematrix.shape) == 1:
+            self._tilematrix = self._tilematrix.reshape((1, len(tilename_matrix)))
         self._size = frame.Coordinate(self._tilematrix.shape[0], self._tilematrix.shape[1])
         self._acce_dict = {}
 
     def tilematrix(self):
         return self._tilematrix
 
     def size(self)->frame.Coordinate:
```

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_util/__init__.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_util/__init__.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_add_dict.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_util/_add_dict.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_etElement_process.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_util/_etElement_process.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_matrix_util.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_util/_matrix_util.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/_util/_str_util.py` & `rwmapeditor_exgcdwu-1.4.3/rwmap/_util/_str_util.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/bridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/bridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/decoration.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/decoration.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/deepwater.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/deepwater.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dirt_details.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dirt_details.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/dust.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/dust.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/fauna.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/fauna.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/fauna_dark.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/fauna_dark.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/fauna_highland.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/fauna_highland.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2ice_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/lava.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/lava.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/lava2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/lava2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/lava2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/lava2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/misc.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/misc.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/nothing2road_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/nothing2road_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2_old.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2_old.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2ice_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2lava_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2lava_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2sand_hill.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2sand_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2stone_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2stone_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sand_dark.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sand_dark.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/shallowwater.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/shortgrass.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/shortgrass.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2snow_hill.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2snow_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2lava.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2lava.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2sand_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2snow.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2snow.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2snow_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/units.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/units.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/water.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/water.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/misc.tsx` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/misc.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/terrain/Lava.tsx` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/terrain/Lava.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmap/other_data/maps/units.tsx` & `rwmapeditor_exgcdwu-1.4.3/rwmap/other_data/maps/units.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmapeditor_exgcdwu.egg-info/PKG-INFO` & `rwmapeditor_exgcdwu-1.4.3/rwmapeditor_exgcdwu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwmapeditor_exgcdwu
-Version: 1.4.2
+Version: 1.4.3
 Home-page: https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-
 Author: exgcdwu
 Author-email: 1006605318@qq.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `rwmapeditor_exgcdwu-1.4.2/rwmapeditor_exgcdwu.egg-info/SOURCES.txt` & `rwmapeditor_exgcdwu-1.4.3/rwmapeditor_exgcdwu.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
+hexrwmap/__init__.py
+hexrwmap/_const.py
+hexrwmap/_core.py
+hexrwmap/_util/__init__.py
 rwmap/__init__.py
 rwmap/_core.py
 rwmap/_exceptions.py
 rwmap/_case/__init__.py
 rwmap/_case/_layer.py
 rwmap/_case/_object.py
 rwmap/_case/_objectgroup.py
@@ -27,15 +31,18 @@
 rwmap/_data/tobject_group/_city/_city.py
 rwmap/_data/tobject_group/_city/_city_detect.py
 rwmap/_data/tobject_group/_city/_city_remove.py
 rwmap/_data/tobject_group/_city/_city_text.py
 rwmap/_data/tobject_group/_city/_normal_unit_add.py
 rwmap/_data/tobject_group/_city/_refresh_building.py
 rwmap/_data/tobject_group/_count/__init__.py
+rwmap/_data/tobject_group/_count/_count.py
 rwmap/_data/tobject_group/_count/_flash.py
+rwmap/_data/tobject_group/_count/_score_text.py
+rwmap/_data/tobject_group/_count/_time.py
 rwmap/_data/tobject_group/_troop/__init__.py
 rwmap/_data/tobject_group/_troop/_troop_add.py
 rwmap/_data/tobject_group/_victory/__init__.py
 rwmap/_data/tobject_group/_victory/_victory_co.py
 rwmap/_frame/__init__.py
 rwmap/_frame/_coordinate.py
 rwmap/_frame/_element_ori.py
```

### Comparing `rwmapeditor_exgcdwu-1.4.2/setup.py` & `rwmapeditor_exgcdwu-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 
 import os
 from setuptools import setup, find_packages
 
-__version__ = '1.4.2'
+__version__ = '1.4.3'
 
 def read_file(file:str):
     with open(file) as file:
         return file.read()
 
 def readline_file(file:str):
     with open(file) as file:
```

