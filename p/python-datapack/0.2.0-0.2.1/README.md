# Comparing `tmp/python_datapack-0.2.0.tar.gz` & `tmp/python_datapack-0.2.1.tar.gz`

## Comparing `python_datapack-0.2.0.tar` & `python_datapack-0.2.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.2.0/1_upgrades.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.2.0/2_build.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.2.0/3_upload.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.2.0/build_all_in_one.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 python_datapack-0.2.0/copy_in_local.py
--rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/__init__.py
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/constants.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/enhance_config.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/finalyze.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/initialize.py
--rw-r--r--   0        0        0    11273 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/verify_database.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/datapack/basic_structure.py
--rw-r--r--   0        0        0    15298 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/datapack/custom_blocks.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/datapack/headers.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/datapack/lang.py
--rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/datapack/loading.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/datapack/loot_tables.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/datapack/main.py
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/datapack/recipes.py
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/book_optimizer.py
--rw-r--r--   0        0        0    23667 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/main.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/shared_import.py
--rw-r--r--   0        0        0    30172 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/utils.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/furnace.png
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/invisible_item.png
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/invisible_item_release.png
--rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/minecraft_font.ttf
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/none.png
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/none_release.png
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/shaped_2x2.png
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/shaped_3x3.png
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/simple_case_no_border.png
--rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/wiki_information.png
--rw-r--r--   0        0        0    17129 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
--rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
--rw-r--r--   0        0        0    16198 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/wiki_result_of_craft.png
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/resource_pack/check_unused_textures.py
--rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/resource_pack/item_models.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/resource_pack/main.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/resource_pack/sounds.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/resource_pack/vanilla_models.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/utils/cache.py
--rw-r--r--   0        0        0    28462 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/utils/database_helper.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/utils/ingredients.py
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/utils/io.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/utils/multiprocessing.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/utils/print.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/utils/weld.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.2.0/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.2.0/LICENSE
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.2.0/README.md
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_datapack-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.2.1/1_upgrades.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.2.1/2_build.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.2.1/3_upload.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.2.1/build_all_in_one.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 python_datapack-0.2.1/copy_in_local.py
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/__init__.py
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/constants.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/enhance_config.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/finalyze.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/initialize.py
+-rw-r--r--   0        0        0    11273 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/verify_database.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/datapack/basic_structure.py
+-rw-r--r--   0        0        0    15298 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/datapack/custom_blocks.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/datapack/headers.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/datapack/lang.py
+-rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/datapack/loading.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/datapack/loot_tables.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/datapack/main.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/datapack/recipes.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/book_optimizer.py
+-rw-r--r--   0        0        0    23739 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/main.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/shared_import.py
+-rw-r--r--   0        0        0    30296 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/utils.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/furnace.png
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/invisible_item.png
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/invisible_item_release.png
+-rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/minecraft_font.ttf
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/none.png
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/none_release.png
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/shaped_2x2.png
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/shaped_3x3.png
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/simple_case_no_border.png
+-rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/wiki_information.png
+-rw-r--r--   0        0        0    17129 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
+-rw-r--r--   0        0        0    16198 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/wiki_result_of_craft.png
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/resource_pack/check_unused_textures.py
+-rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/resource_pack/item_models.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/resource_pack/main.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/resource_pack/sounds.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/resource_pack/vanilla_models.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/utils/cache.py
+-rw-r--r--   0        0        0    28462 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/utils/database_helper.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/utils/ingredients.py
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/utils/io.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/utils/multiprocessing.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/utils/print.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/utils/weld.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.2.1/LICENSE
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.2.1/README.md
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_datapack-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.2.1/PKG-INFO
```

### Comparing `python_datapack-0.2.0/src/python_datapack/__init__.py` & `python_datapack-0.2.1/src/python_datapack/__init__.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/constants.py` & `python_datapack-0.2.1/src/python_datapack/constants.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/enhance_config.py` & `python_datapack-0.2.1/src/python_datapack/enhance_config.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/finalyze.py` & `python_datapack-0.2.1/src/python_datapack/finalyze.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/initialize.py` & `python_datapack-0.2.1/src/python_datapack/initialize.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/verify_database.py` & `python_datapack-0.2.1/src/python_datapack/verify_database.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/datapack/basic_structure.py` & `python_datapack-0.2.1/src/python_datapack/datapack/basic_structure.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/datapack/custom_blocks.py` & `python_datapack-0.2.1/src/python_datapack/datapack/custom_blocks.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/datapack/headers.py` & `python_datapack-0.2.1/src/python_datapack/datapack/headers.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/datapack/lang.py` & `python_datapack-0.2.1/src/python_datapack/datapack/lang.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/datapack/loading.py` & `python_datapack-0.2.1/src/python_datapack/datapack/loading.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/datapack/loot_tables.py` & `python_datapack-0.2.1/src/python_datapack/datapack/loot_tables.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/datapack/main.py` & `python_datapack-0.2.1/src/python_datapack/datapack/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/datapack/recipes.py` & `python_datapack-0.2.1/src/python_datapack/datapack/recipes.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/manual/book_optimizer.py` & `python_datapack-0.2.1/src/python_datapack/manual/book_optimizer.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/manual/main.py` & `python_datapack-0.2.1/src/python_datapack/manual/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from copy import deepcopy
 
 def main(config: dict):
 
 	# Prework
 	os.makedirs(f"{config['manual_path']}/font/page", exist_ok=True)
 	os.makedirs(f"{config['manual_path']}/font/wiki_icons", exist_ok = True)
+	os.makedirs(f"{config['manual_path']}/font/high_res", exist_ok = True)
 	generate_all_iso_renders(config)
 
 	# Constants
 	FONT = config['namespace'] + ':' + FONT_FILE
 	MAX_ITEMS_PER_PAGE = config['max_items_per_row'] * config['max_rows_per_page'] # (for showing up all items in the categories pages)
 
 	# Calculate left padding for categories pages depending on config['max_items_per_row']: higher the value, lower the padding
@@ -423,15 +424,15 @@
 		font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/wiki_result_of_craft.png", "ascent": 8, "height": 16, "chars": [WIKI_RESULT_OF_CRAFT_FONT]})
 		font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/wiki_ingredient_of_craft.png", "ascent": 8, "height": 16, "chars": [WIKI_INGR_OF_CRAFT_FONT]})
 		if config['manual_high_resolution']:
 			font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/shaped_3x3.png", "ascent": 1, "height": 58, "chars": [SHAPED_3X3_FONT]})
 			font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/shaped_2x2.png", "ascent": 1, "height": 58, "chars": [SHAPED_2X2_FONT]})
 			font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/furnace.png", "ascent": 1, "height": 58, "chars": [FURNACE_FONT]})
 			font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/shaped_3x3.png", "ascent": -4, "height": 58, "chars": [HOVER_SHAPED_3X3_FONT]})
-			font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/shaped_2x2.png", "ascent": -1, "height": 58, "chars": [HOVER_SHAPED_2X2_FONT]})
+			font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/shaped_2x2.png", "ascent": -2, "height": 58, "chars": [HOVER_SHAPED_2X2_FONT]})
 			font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/furnace.png", "ascent": -3, "height": 58, "chars": [HOVER_FURNACE_FONT]})
 		fonts = {"providers": font_providers}
 		with super_open(f"{config['manual_path']}/font/manual.json", "w") as f:
 			f.write(super_json_dump(fonts).replace("\\\\", "\\"))
 				
 		# Debug book_content
 		with super_open(config['manual_debug'], "w") as f:
```

### Comparing `python_datapack-0.2.0/src/python_datapack/manual/shared_import.py` & `python_datapack-0.2.1/src/python_datapack/manual/shared_import.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/manual/utils.py` & `python_datapack-0.2.1/src/python_datapack/manual/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -471,15 +471,18 @@
 	content.append(SMALL_NONE_FONT + page_font + "\n")
 	
 	# Generate the image for the page
 	generate_page_font(config, name, page_font, craft)
 
 	# Get result component
 	result_count = craft.get("result_count", 1)
-	result_component = get_item_component(config, name, count = result_count)
+	if not craft.get("result"):
+		result_component = get_item_component(config, name, count = result_count)
+	else:
+		result_component = get_item_component(config, craft["result"], count = result_count)
 	if result_component.get("clickEvent"):
 		del result_component["clickEvent"]	# Remove clickEvent for result item (as we already are on the page)
 	result_component["text"] = MICRO_NONE_FONT + result_component["text"]	# Left adjustment
 
 	# If the craft is shaped
 	if craft_type == "crafting_shaped":
```

### Comparing `python_datapack-0.2.0/src/python_datapack/manual/assets/furnace.png` & `python_datapack-0.2.1/src/python_datapack/manual/assets/furnace.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/manual/assets/invisible_item.png` & `python_datapack-0.2.1/src/python_datapack/manual/assets/invisible_item.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/manual/assets/invisible_item_release.png` & `python_datapack-0.2.1/src/python_datapack/manual/assets/invisible_item_release.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/manual/assets/minecraft_font.ttf` & `python_datapack-0.2.1/src/python_datapack/manual/assets/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/manual/assets/shaped_2x2.png` & `python_datapack-0.2.1/src/python_datapack/manual/assets/shaped_2x2.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/manual/assets/shaped_3x3.png` & `python_datapack-0.2.1/src/python_datapack/manual/assets/shaped_3x3.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/manual/assets/simple_case_no_border.png` & `python_datapack-0.2.1/src/python_datapack/manual/assets/simple_case_no_border.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/manual/assets/wiki_information.png` & `python_datapack-0.2.1/src/python_datapack/manual/assets/wiki_information.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png` & `python_datapack-0.2.1/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png` & `python_datapack-0.2.1/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/manual/assets/wiki_result_of_craft.png` & `python_datapack-0.2.1/src/python_datapack/manual/assets/wiki_result_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/resource_pack/check_unused_textures.py` & `python_datapack-0.2.1/src/python_datapack/resource_pack/check_unused_textures.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/resource_pack/item_models.py` & `python_datapack-0.2.1/src/python_datapack/resource_pack/item_models.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/resource_pack/main.py` & `python_datapack-0.2.1/src/python_datapack/resource_pack/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/resource_pack/sounds.py` & `python_datapack-0.2.1/src/python_datapack/resource_pack/sounds.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/resource_pack/vanilla_models.py` & `python_datapack-0.2.1/src/python_datapack/resource_pack/vanilla_models.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/utils/database_helper.py` & `python_datapack-0.2.1/src/python_datapack/utils/database_helper.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/utils/ingredients.py` & `python_datapack-0.2.1/src/python_datapack/utils/ingredients.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/utils/io.py` & `python_datapack-0.2.1/src/python_datapack/utils/io.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/utils/multiprocessing.py` & `python_datapack-0.2.1/src/python_datapack/utils/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/utils/print.py` & `python_datapack-0.2.1/src/python_datapack/utils/print.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/src/python_datapack/utils/weld.py` & `python_datapack-0.2.1/src/python_datapack/utils/weld.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/LICENSE` & `python_datapack-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.0/pyproject.toml` & `python_datapack-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["hatchling", "pillow", "smithed", "model_resolver"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python_datapack"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
 	{ name="Stoupy51", email="stoupy51@gmail.com" },
 ]
 description = "Python package to help generating advanced Minecraft datapack contents"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `python_datapack-0.2.0/PKG-INFO` & `python_datapack-0.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python_datapack
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python package to help generating advanced Minecraft datapack contents
 Project-URL: Homepage, https://github.com/Stoupy51/python_datapack
 Project-URL: Issues, https://github.com/Stoupy51/python_datapack/issues
 Author-email: Stoupy51 <stoupy51@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

