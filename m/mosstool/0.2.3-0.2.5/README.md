# Comparing `tmp/mosstool-0.2.3.tar.gz` & `tmp/mosstool-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosstool-0.2.3.tar", max compression
+gzip compressed data, was "mosstool-0.2.5.tar", max compression
```

## Comparing `mosstool-0.2.3.tar` & `mosstool-0.2.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0      106 2024-05-29 02:24:00.137560 mosstool-0.2.3/README.md
--rw-r--r--   0        0        0      268 2024-05-29 02:24:00.789557 mosstool-0.2.3/mosstool/map/__init__.py
--rw-r--r--   0        0        0    16340 2024-05-29 02:24:00.789557 mosstool-0.2.3/mosstool/map/_map_util/add_aoi_pop.py
--rw-r--r--   0        0        0    70708 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/_map_util/aoi_matcher.py
--rw-r--r--   0        0        0    16237 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/_map_util/aoiutils.py
--rw-r--r--   0        0        0     2978 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/_map_util/const.py
--rw-r--r--   0        0        0    11404 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/_map_util/convert_aoi.py
--rw-r--r--   0        0        0    16617 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/_map_util/format_checker.py
--rw-r--r--   0        0        0    21033 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/_map_util/gen_traffic_light.py
--rw-r--r--   0        0        0     2045 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/_map_util/map_aois_matchers.py
--rw-r--r--   0        0        0     1155 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/_map_util/osm_const.py
--rw-r--r--   0        0        0        0 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/_util/__init__.py
--rw-r--r--   0        0        0      444 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/_util/angle.py
--rw-r--r--   0        0        0     3626 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/_util/bezier.py
--rw-r--r--   0        0        0    12436 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/_util/line.py
--rw-r--r--   0        0        0      100 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/builder/__init__.py
--rw-r--r--   0        0        0   206166 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/builder/builder.py
--rw-r--r--   0        0        0      185 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/osm/__init__.py
--rw-r--r--   0        0        0     7162 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/osm/_motif.py
--rw-r--r--   0        0        0     2643 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/osm/_wayutil.py
--rw-r--r--   0        0        0    14567 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/osm/building.py
--rw-r--r--   0        0        0    28323 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/osm/roadnet.py
--rw-r--r--   0        0        0      373 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/public_transport/__init__.py
--rw-r--r--   0        0        0    12458 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/public_transport/get_bus.py
--rw-r--r--   0        0        0    12224 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/public_transport/get_subway.py
--rw-r--r--   0        0        0    21211 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/public_transport/get_transitland.py
--rw-r--r--   0        0        0    16145 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/public_transport/public_transport_post.py
--rw-r--r--   0        0        0       92 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/sumo/__init__.py
--rw-r--r--   0        0        0    37747 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/sumo/map.py
--rw-r--r--   0        0        0       79 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/vis/__init__.py
--rw-r--r--   0        0        0     9999 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/map/vis/map.py
--rw-r--r--   0        0        0       36 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/trip/__init__.py
--rw-r--r--   0        0        0      758 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/trip/generator/AIGC.py
--rw-r--r--   0        0        0      347 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/trip/generator/__init__.py
--rw-r--r--   0        0        0      688 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/trip/generator/_util/const.py
--rw-r--r--   0        0        0      406 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/trip/generator/_util/utils.py
--rw-r--r--   0        0        0    19820 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/trip/generator/generate_from_od.py
--rw-r--r--   0        0        0     3774 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/trip/generator/gravity.py
--rw-r--r--   0        0        0     5190 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/trip/generator/random.py
--rw-r--r--   0        0        0      702 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/trip/generator/template.py
--rw-r--r--   0        0        0      119 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/trip/route/__init__.py
--rw-r--r--   0        0        0     2105 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/trip/route/client.py
--rw-r--r--   0        0        0     3398 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/trip/route/preroute.py
--rw-r--r--   0        0        0      100 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/trip/sumo/__init__.py
--rw-r--r--   0        0        0    37589 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/trip/sumo/route.py
--rw-r--r--   0        0        0       78 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/trip/vis/__init__.py
--rw-r--r--   0        0        0     8307 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/trip/vis/trip.py
--rw-r--r--   0        0        0      783 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/type/__init__.py
--rw-r--r--   0        0        0       22 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/util/__init__.py
--rw-r--r--   0        0        0      481 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/util/color.py
--rw-r--r--   0        0        0     4519 2024-05-29 02:24:00.793557 mosstool-0.2.3/mosstool/util/format_converter.py
--rw-r--r--   0        0        0    14922 2024-05-29 02:24:00.797556 mosstool-0.2.3/mosstool/util/geo_match_pop.py
--rw-r--r--   0        0        0     2039 2024-05-29 02:24:00.797556 mosstool-0.2.3/mosstool/util/map_merger.py
--rw-r--r--   0        0        0     6538 2024-05-29 02:24:00.797556 mosstool-0.2.3/mosstool/util/map_splitter.py
--rw-r--r--   0        0        0        0 2024-05-29 02:24:00.797556 mosstool-0.2.3/mosstool/util/test/__init__.py
--rw-r--r--   0        0        0      194 2024-05-29 02:24:00.797556 mosstool-0.2.3/mosstool/util/test/test_color.py
--rw-r--r--   0        0        0     1150 2024-05-29 02:24:00.797556 mosstool-0.2.3/mosstool/util/test/test_format_conveter.py
--rw-r--r--   0        0        0      853 2024-05-29 02:24:00.797556 mosstool-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 mosstool-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-06-01 03:30:52.493486 mosstool-0.2.5/README.md
+-rw-r--r--   0        0        0      268 2024-06-01 03:30:53.173486 mosstool-0.2.5/mosstool/map/__init__.py
+-rw-r--r--   0        0        0    16340 2024-06-01 03:30:53.173486 mosstool-0.2.5/mosstool/map/_map_util/add_aoi_pop.py
+-rw-r--r--   0        0        0    70708 2024-06-01 03:30:53.173486 mosstool-0.2.5/mosstool/map/_map_util/aoi_matcher.py
+-rw-r--r--   0        0        0    16237 2024-06-01 03:30:53.173486 mosstool-0.2.5/mosstool/map/_map_util/aoiutils.py
+-rw-r--r--   0        0        0     2978 2024-06-01 03:30:53.173486 mosstool-0.2.5/mosstool/map/_map_util/const.py
+-rw-r--r--   0        0        0    11404 2024-06-01 03:30:53.173486 mosstool-0.2.5/mosstool/map/_map_util/convert_aoi.py
+-rw-r--r--   0        0        0    16617 2024-06-01 03:30:53.173486 mosstool-0.2.5/mosstool/map/_map_util/format_checker.py
+-rw-r--r--   0        0        0    21033 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/map/_map_util/gen_traffic_light.py
+-rw-r--r--   0        0        0     2045 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/map/_map_util/map_aois_matchers.py
+-rw-r--r--   0        0        0     1155 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/map/_map_util/osm_const.py
+-rw-r--r--   0        0        0        0 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/map/_util/__init__.py
+-rw-r--r--   0        0        0      444 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/map/_util/angle.py
+-rw-r--r--   0        0        0     3626 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/map/_util/bezier.py
+-rw-r--r--   0        0        0    12436 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/map/_util/line.py
+-rw-r--r--   0        0        0      100 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/map/builder/__init__.py
+-rw-r--r--   0        0        0   206166 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/map/builder/builder.py
+-rw-r--r--   0        0        0      185 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/map/osm/__init__.py
+-rw-r--r--   0        0        0     7162 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/map/osm/_motif.py
+-rw-r--r--   0        0        0     2643 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/map/osm/_wayutil.py
+-rw-r--r--   0        0        0    14567 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/map/osm/building.py
+-rw-r--r--   0        0        0    28323 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/map/osm/roadnet.py
+-rw-r--r--   0        0        0      373 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/map/public_transport/__init__.py
+-rw-r--r--   0        0        0    12458 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/map/public_transport/get_bus.py
+-rw-r--r--   0        0        0    12224 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/map/public_transport/get_subway.py
+-rw-r--r--   0        0        0    21211 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/map/public_transport/get_transitland.py
+-rw-r--r--   0        0        0    16145 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/map/public_transport/public_transport_post.py
+-rw-r--r--   0        0        0       92 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/map/sumo/__init__.py
+-rw-r--r--   0        0        0    37747 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/map/sumo/map.py
+-rw-r--r--   0        0        0       79 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/map/vis/__init__.py
+-rw-r--r--   0        0        0     9999 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/map/vis/map.py
+-rw-r--r--   0        0        0       36 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/trip/__init__.py
+-rw-r--r--   0        0        0      758 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/trip/generator/AIGC.py
+-rw-r--r--   0        0        0      347 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/trip/generator/__init__.py
+-rw-r--r--   0        0        0      688 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/trip/generator/_util/const.py
+-rw-r--r--   0        0        0      406 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/trip/generator/_util/utils.py
+-rw-r--r--   0        0        0    19820 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/trip/generator/generate_from_od.py
+-rw-r--r--   0        0        0     3774 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/trip/generator/gravity.py
+-rw-r--r--   0        0        0     5190 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/trip/generator/random.py
+-rw-r--r--   0        0        0      702 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/trip/generator/template.py
+-rw-r--r--   0        0        0      119 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/trip/route/__init__.py
+-rw-r--r--   0        0        0     2105 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/trip/route/client.py
+-rw-r--r--   0        0        0     3398 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/trip/route/preroute.py
+-rw-r--r--   0        0        0      100 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/trip/sumo/__init__.py
+-rw-r--r--   0        0        0    37589 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/trip/sumo/route.py
+-rw-r--r--   0        0        0       78 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/trip/vis/__init__.py
+-rw-r--r--   0        0        0     8307 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/trip/vis/trip.py
+-rw-r--r--   0        0        0      783 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/type/__init__.py
+-rw-r--r--   0        0        0       22 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/util/__init__.py
+-rw-r--r--   0        0        0      481 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/util/color.py
+-rw-r--r--   0        0        0     4519 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/util/format_converter.py
+-rw-r--r--   0        0        0    14922 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/util/geo_match_pop.py
+-rw-r--r--   0        0        0     2039 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/util/map_merger.py
+-rw-r--r--   0        0        0     6538 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/util/map_splitter.py
+-rw-r--r--   0        0        0        0 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/util/test/__init__.py
+-rw-r--r--   0        0        0      194 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/util/test/test_color.py
+-rw-r--r--   0        0        0     1150 2024-06-01 03:30:53.177486 mosstool-0.2.5/mosstool/util/test/test_format_conveter.py
+-rw-r--r--   0        0        0      854 2024-06-01 03:30:53.181486 mosstool-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1510 1970-01-01 00:00:00.000000 mosstool-0.2.5/PKG-INFO
```

### Comparing `mosstool-0.2.3/mosstool/map/_map_util/add_aoi_pop.py` & `mosstool-0.2.5/mosstool/map/_map_util/add_aoi_pop.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/map/_map_util/aoi_matcher.py` & `mosstool-0.2.5/mosstool/map/_map_util/aoi_matcher.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/map/_map_util/aoiutils.py` & `mosstool-0.2.5/mosstool/map/_map_util/aoiutils.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/map/_map_util/const.py` & `mosstool-0.2.5/mosstool/map/_map_util/const.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/map/_map_util/convert_aoi.py` & `mosstool-0.2.5/mosstool/map/_map_util/convert_aoi.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/map/_map_util/format_checker.py` & `mosstool-0.2.5/mosstool/map/_map_util/format_checker.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/map/_map_util/gen_traffic_light.py` & `mosstool-0.2.5/mosstool/map/_map_util/gen_traffic_light.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/map/_map_util/map_aois_matchers.py` & `mosstool-0.2.5/mosstool/map/_map_util/map_aois_matchers.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/map/_map_util/osm_const.py` & `mosstool-0.2.5/mosstool/map/_map_util/osm_const.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/map/_util/bezier.py` & `mosstool-0.2.5/mosstool/map/_util/bezier.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/map/_util/line.py` & `mosstool-0.2.5/mosstool/map/_util/line.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/map/builder/builder.py` & `mosstool-0.2.5/mosstool/map/builder/builder.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/map/osm/_motif.py` & `mosstool-0.2.5/mosstool/map/osm/_motif.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/map/osm/_wayutil.py` & `mosstool-0.2.5/mosstool/map/osm/_wayutil.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/map/osm/building.py` & `mosstool-0.2.5/mosstool/map/osm/building.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/map/osm/roadnet.py` & `mosstool-0.2.5/mosstool/map/osm/roadnet.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/map/public_transport/get_bus.py` & `mosstool-0.2.5/mosstool/map/public_transport/get_bus.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/map/public_transport/get_subway.py` & `mosstool-0.2.5/mosstool/map/public_transport/get_subway.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/map/public_transport/get_transitland.py` & `mosstool-0.2.5/mosstool/map/public_transport/get_transitland.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/map/public_transport/public_transport_post.py` & `mosstool-0.2.5/mosstool/map/public_transport/public_transport_post.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/map/sumo/map.py` & `mosstool-0.2.5/mosstool/map/sumo/map.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/map/vis/map.py` & `mosstool-0.2.5/mosstool/map/vis/map.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/trip/generator/AIGC.py` & `mosstool-0.2.5/mosstool/trip/generator/AIGC.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/trip/generator/_util/const.py` & `mosstool-0.2.5/mosstool/trip/generator/_util/const.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/trip/generator/generate_from_od.py` & `mosstool-0.2.5/mosstool/trip/generator/generate_from_od.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/trip/generator/gravity.py` & `mosstool-0.2.5/mosstool/trip/generator/gravity.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/trip/generator/random.py` & `mosstool-0.2.5/mosstool/trip/generator/random.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/trip/generator/template.py` & `mosstool-0.2.5/mosstool/trip/generator/template.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/trip/route/client.py` & `mosstool-0.2.5/mosstool/trip/route/client.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/trip/route/preroute.py` & `mosstool-0.2.5/mosstool/trip/route/preroute.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/trip/sumo/route.py` & `mosstool-0.2.5/mosstool/trip/sumo/route.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/trip/vis/trip.py` & `mosstool-0.2.5/mosstool/trip/vis/trip.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/type/__init__.py` & `mosstool-0.2.5/mosstool/type/__init__.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/util/format_converter.py` & `mosstool-0.2.5/mosstool/util/format_converter.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/util/geo_match_pop.py` & `mosstool-0.2.5/mosstool/util/geo_match_pop.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/util/map_merger.py` & `mosstool-0.2.5/mosstool/util/map_merger.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/util/map_splitter.py` & `mosstool-0.2.5/mosstool/util/map_splitter.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/mosstool/util/test/test_format_conveter.py` & `mosstool-0.2.5/mosstool/util/test/test_format_conveter.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.2.3/pyproject.toml` & `mosstool-0.2.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mosstool"
-version = "0.2.3"
+version = "0.2.5"
 description = "MObility Simulation System toolbox "
 authors = ["Jun Zhang <zhangjun990222@qq.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -16,17 +16,17 @@
 pymongo = "^4.6.2"
 pytest-coverage = "^0.0"
 pyproj = "^3.6.1"
 scipy = "^1.12.0"
 scikit-learn = "^1.4.1.post1"
 numpy = "^1.26.4"
 geopandas = "^0.14.3"
-requests = "^2.31.0"
+requests = "^2.32.3"
 rasterio = "1.3.9"
-pycityproto = "1.13.1"
+pycityproto = "^1.13.1"
 lxml = "^5.1.0"
 coord-convert = "^0.2.1"
 levenshtein = "^0.25.0"
 bs4 = "^0.0.2"
 matplotlib = "^3.8.3"
 generate-od = "^0.1"
```

### Comparing `mosstool-0.2.3/PKG-INFO` & `mosstool-0.2.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosstool
-Version: 0.2.3
+Version: 0.2.5
 Summary: MObility Simulation System toolbox 
 License: MIT
 Author: Jun Zhang
 Author-email: zhangjun990222@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,21 +18,21 @@
 Requires-Dist: geojson (>=3.1.0,<4.0.0)
 Requires-Dist: geopandas (>=0.14.3,<0.15.0)
 Requires-Dist: levenshtein (>=0.25.0,<0.26.0)
 Requires-Dist: lxml (>=5.1.0,<6.0.0)
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: networkx (>=3.2.1,<4.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Requires-Dist: pycityproto (==1.13.1)
+Requires-Dist: pycityproto (>=1.13.1,<2.0.0)
 Requires-Dist: pydeck (>=0.8.0,<0.9.0)
 Requires-Dist: pymongo (>=4.6.2,<5.0.0)
 Requires-Dist: pyproj (>=3.6.1,<4.0.0)
 Requires-Dist: pytest-coverage (>=0.0,<0.1)
 Requires-Dist: rasterio (==1.3.9)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests (>=2.32.3,<3.0.0)
 Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0)
 Requires-Dist: scipy (>=1.12.0,<2.0.0)
 Requires-Dist: shapely (>=2.0.3,<3.0.0)
 Requires-Dist: stringcase (>=1.2.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # mosstool
```

