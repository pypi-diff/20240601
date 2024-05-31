# Comparing `tmp/python_datapack-0.1.7.tar.gz` & `tmp/python_datapack-0.2.0.tar.gz`

## Comparing `python_datapack-0.1.7.tar` & `python_datapack-0.2.0.tar`

### file list

```diff
@@ -1,51 +1,53 @@
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.7/1_upgrades.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.1.7/2_build.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.7/3_upload.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.1.7/build_all_in_one.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 python_datapack-0.1.7/copy_in_local.py
--rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/__init__.py
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/constants.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/enhance_config.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/finalyze.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/initialize.py
--rw-r--r--   0        0        0    11273 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/verify_database.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/datapack/basic_structure.py
--rw-r--r--   0        0        0    15298 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/datapack/custom_blocks.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/datapack/headers.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/datapack/lang.py
--rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/datapack/loading.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/datapack/loot_tables.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/datapack/main.py
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/datapack/recipes.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/book_optimizer.py
--rw-r--r--   0        0        0    21133 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/main.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/shared_import.py
--rw-r--r--   0        0        0    26767 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/utils.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/assets/furnace.png
--rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/assets/minecraft_font.ttf
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/assets/none.png
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/assets/none_release.png
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/assets/shaped_2x2.png
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/assets/shaped_3x3.png
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/assets/simple_case_no_border.png
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/assets/wiki_information.png
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/assets/wiki_result_of_craft.png
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/resource_pack/check_unused_textures.py
--rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/resource_pack/item_models.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/resource_pack/main.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/resource_pack/sounds.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/resource_pack/vanilla_models.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/utils/cache.py
--rw-r--r--   0        0        0    28462 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/utils/database_helper.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/utils/ingredients.py
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/utils/io.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/utils/multiprocessing.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/utils/print.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/utils/weld.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.1.7/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.1.7/LICENSE
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.1.7/README.md
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_datapack-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.2.0/1_upgrades.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.2.0/2_build.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.2.0/3_upload.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.2.0/build_all_in_one.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 python_datapack-0.2.0/copy_in_local.py
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/__init__.py
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/constants.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/enhance_config.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/finalyze.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/initialize.py
+-rw-r--r--   0        0        0    11273 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/verify_database.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/datapack/basic_structure.py
+-rw-r--r--   0        0        0    15298 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/datapack/custom_blocks.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/datapack/headers.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/datapack/lang.py
+-rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/datapack/loading.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/datapack/loot_tables.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/datapack/main.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/datapack/recipes.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/book_optimizer.py
+-rw-r--r--   0        0        0    23667 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/main.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/shared_import.py
+-rw-r--r--   0        0        0    30172 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/utils.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/furnace.png
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/invisible_item.png
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/invisible_item_release.png
+-rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/minecraft_font.ttf
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/none.png
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/none_release.png
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/shaped_2x2.png
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/shaped_3x3.png
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/simple_case_no_border.png
+-rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/wiki_information.png
+-rw-r--r--   0        0        0    17129 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
+-rw-r--r--   0        0        0    16198 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/manual/assets/wiki_result_of_craft.png
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/resource_pack/check_unused_textures.py
+-rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/resource_pack/item_models.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/resource_pack/main.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/resource_pack/sounds.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/resource_pack/vanilla_models.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/utils/cache.py
+-rw-r--r--   0        0        0    28462 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/utils/database_helper.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/utils/ingredients.py
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/utils/io.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/utils/multiprocessing.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/utils/print.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.2.0/src/python_datapack/utils/weld.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.2.0/LICENSE
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.2.0/README.md
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_datapack-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.2.0/PKG-INFO
```

### Comparing `python_datapack-0.1.7/src/python_datapack/__init__.py` & `python_datapack-0.2.0/src/python_datapack/__init__.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/constants.py` & `python_datapack-0.2.0/src/python_datapack/constants.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/enhance_config.py` & `python_datapack-0.2.0/src/python_datapack/enhance_config.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/finalyze.py` & `python_datapack-0.2.0/src/python_datapack/finalyze.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/initialize.py` & `python_datapack-0.2.0/src/python_datapack/initialize.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/verify_database.py` & `python_datapack-0.2.0/src/python_datapack/verify_database.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/datapack/basic_structure.py` & `python_datapack-0.2.0/src/python_datapack/datapack/basic_structure.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/datapack/custom_blocks.py` & `python_datapack-0.2.0/src/python_datapack/datapack/custom_blocks.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/datapack/headers.py` & `python_datapack-0.2.0/src/python_datapack/datapack/headers.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/datapack/lang.py` & `python_datapack-0.2.0/src/python_datapack/datapack/lang.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/datapack/loading.py` & `python_datapack-0.2.0/src/python_datapack/datapack/loading.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/datapack/loot_tables.py` & `python_datapack-0.2.0/src/python_datapack/datapack/loot_tables.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/datapack/main.py` & `python_datapack-0.2.0/src/python_datapack/datapack/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/datapack/recipes.py` & `python_datapack-0.2.0/src/python_datapack/datapack/recipes.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/manual/main.py` & `python_datapack-0.2.0/src/python_datapack/manual/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,16 +21,18 @@
 
 	# Calculate left padding for categories pages depending on config['max_items_per_row']: higher the value, lower the padding
 	LEFT_PADDING = 6 - config['max_items_per_row']
 
 	# Copy assets in the resource pack
 	if not config['debug_mode']:
 		super_copy(f"{TEMPLATES_PATH}/none_release.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/none.png")
+		super_copy(f"{TEMPLATES_PATH}/invisible_item_release.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/invisible_item.png")
 	else:
 		super_copy(f"{TEMPLATES_PATH}/none.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/none.png")
+		super_copy(f"{TEMPLATES_PATH}/invisible_item.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/invisible_item.png")
 	super_copy(f"{TEMPLATES_PATH}/wiki_information.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/wiki_information.png")
 	super_copy(f"{TEMPLATES_PATH}/wiki_result_of_craft.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/wiki_result_of_craft.png")
 	super_copy(f"{TEMPLATES_PATH}/wiki_ingredient_of_craft.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/wiki_ingredient_of_craft.png")
 	if config['manual_high_resolution']:
 		super_copy(f"{TEMPLATES_PATH}/furnace.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/furnace.png")
 		super_copy(f"{TEMPLATES_PATH}/shaped_2x2.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/shaped_2x2.png")
 		super_copy(f"{TEMPLATES_PATH}/shaped_3x3.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/shaped_3x3.png")
@@ -96,22 +98,25 @@
 		# Encode pages
 		book_content = []
 		os.makedirs(f"{config['manual_path']}/font/category", exist_ok=True)
 		simple_case = load_simple_case_no_border(config['manual_high_resolution'])	# Load the simple case image for later use in categories pages
 		for page in manual_pages:
 			content = []
 			number = page["number"]
-			page_font = get_page_font(number)
+			raw_data: dict = page["raw_data"]
+			page_font = ""
+			if not config['manual_high_resolution']:
+				page_font = get_page_font(number)
 			name = str(page["name"])
-			raw_data = page["raw_data"]
 			titled = name.replace("_", " ").title() + "\n"
 
 			# Encode categories {'number': 2, 'name': 'Material #1', 'raw_data': ['adamantium_block', 'adamantium_fragment', ...]}
 			if page["type"] == CATEGORY:
 				file_name = name.replace(" ", "_").replace("#", "").lower()
+				page_font = get_page_font(number)
 				font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/category/{file_name}.png", "ascent": 0, "height": 130, "chars": [page_font]})
 				content.append({"text": "", "font": FONT, "color": "white"})	# Make default font for every next component
 				content.append({"text": "➤ ", "font": "minecraft:default", "color": "black"})
 				content.append({"text": titled, "font": "minecraft:default", "color": "black", "underlined": True})
 				content.append(SMALL_NONE_FONT * LEFT_PADDING + page_font + "\n")
 
 				# Prepare image and line list
@@ -178,16 +183,19 @@
 					first_craft = raw_data[RESULT_OF_CRAFTING][0]
 					l = generate_craft_content(config, first_craft, name, page_font)
 					if l:
 						content += l
 				
 				# Else, generate the content for the single item in a big box
 				else:
+					if not page_font:
+						page_font = get_page_font(number)
 					generate_page_font(config, name, page_font, craft = None)
 					component = get_item_component(config, name)
+					component["text"] = NONE_FONT
 					component["text"] *= 2
 					content.append({"text": "", "font": FONT, "color": "white"})	# Make default font for every next component
 					content.append({"text": titled, "font": "minecraft:default", "color": "black", "underlined": True})
 					content.append(MEDIUM_NONE_FONT * 2 + page_font + "\n")
 					for _ in range(4):
 						content.append(MEDIUM_NONE_FONT * 2)
 						content.append(component)
@@ -207,23 +215,33 @@
 				crafts += generate_otherside_crafts(config, name)
 				crafts = [craft for craft in crafts if craft["type"] not in ["blasting", "smoking", "campfire_cooking"]]	# Remove smelting dupes
 				crafts = unique_crafts(crafts)
 
 				for i, craft in enumerate(crafts):
 					if craft["type"] == "crafting_shapeless":
 						craft = convert_shapeless_to_shaped(craft)
-					craft_font = get_next_font()	# Unique used font for the craft
-					generate_page_font(config, name, craft_font, craft, output_name = f"{name}_{i+1}")
-					hover_text = [""]
 
-					# Append the craft font and breaklines
+					# Get breaklines
 					breaklines = 3
 					if "shape" in craft:
 						breaklines = max(2, max(len(craft["shape"]), len(craft["shape"][0])))
-					hover_text.append({"text": craft_font + "\n\n" * breaklines, "font": FONT, "color": "white"})
+
+					if not config['manual_high_resolution']:
+						craft_font = get_next_font()	# Unique used font for the craft
+						generate_page_font(config, name, craft_font, craft, output_name = f"{name}_{i+1}")
+						hover_text = [""]
+						hover_text.append({"text": craft_font + "\n\n" * breaklines, "font": FONT, "color": "white"})
+					else:
+						l = generate_craft_content(config, craft, name, "")
+						l = [l[0]] + l[2:]	# Remove craft title
+						remove_events(l)
+						replaces = {SHAPED_2X2_FONT: HOVER_SHAPED_2X2_FONT, SHAPED_3X3_FONT: HOVER_SHAPED_3X3_FONT, FURNACE_FONT: HOVER_FURNACE_FONT}
+						for k, v in replaces.items():
+							l[1] = l[1].replace(k, v)
+						hover_text = ["", l]
 
 					# Append ingredients
 					if craft.get("ingredient"):
 						id = ingr_to_id(craft["ingredient"], False).replace("_", " ").title()
 						hover_text.append({"text": f"\n- x1 ", "color": "gray"})
 						hover_text.append({"text": id, "color": "gray"})
 					elif craft.get("ingredients"):
@@ -308,56 +326,60 @@
 		x, y = 2, 2	# Prevision for global border and implicit border
 		line = []
 
 		# For each item in the category, get its page number and texture, then add it to the image
 		for page in manual_pages:
 			if page["type"] == CATEGORY:
 				item = page["raw_data"][0]
-				texture_path = f"{config['manual_path']}/items/{config['namespace']}/{item}.png"
-				item_image = Image.open(texture_path)
-				item_image = careful_resize(item_image, 32)
 
-				# Get item texture
+				# Get item texture TODO
 				texture_path = f"{config['manual_path']}/items/{config['namespace']}/{item}.png"
 				if os.path.exists(texture_path):
 					item_image = Image.open(texture_path)
 				else:
 					warning(f"Missing texture at '{texture_path}', using empty texture")
 					item_image = Image.new("RGBA", (1, 1), (0, 0, 0, 0))
 				if not config['manual_high_resolution']:
 					resized = careful_resize(item_image, 32)
 				else:
 					resized = Image.new("RGBA", (1, 1), (0, 0, 0, 0))	# Empty texture to use for category page
 					high_res_font = generate_high_res_font(config, item, item_image)
 
 				# Paste the simple case and the item_image
 				page_image.paste(simple_case, (x, y))
-				mask = item_image.convert("RGBA").split()[3]
-				page_image.paste(item_image, (x + 2, y + 2), mask)
+				mask = resized.convert("RGBA").split()[3]
+				page_image.paste(resized, (x + 2, y + 2), mask)
 				x += simple_case.size[0]
 
 				# Add the clickEvent part to the line and add the 2 times the line if enough items
 				component = get_item_component(config, item, ["custom_model_data"])
 				component["hoverEvent"]["contents"]["components"]["item_name"] = str({"text": page["name"], "color": "white"})
 				component["clickEvent"]["value"] = str(page["number"])
-				component["text"] = MEDIUM_NONE_FONT
+				if not config['manual_high_resolution']:
+					component["text"] = MEDIUM_NONE_FONT
+				else:
+					component["text"] = high_res_font
 				line.append(component)
 				if len(line) == config['max_items_per_row']:
-					line[-1]["text"] += "\n"
-					line[0]["text"] = SMALL_NONE_FONT * LEFT_PADDING + line[0]["text"]
-					content += line * 2
+					line.insert(0, SMALL_NONE_FONT * LEFT_PADDING)
+					content += deepcopy(line) + ["\n"]
+					for i in range(1, len(line)):
+						line[-i]["text"] = MEDIUM_NONE_FONT
+					content += line + ["\n"]
 					line = []
 					x = 2
 					y += simple_case.size[1]
 		
 		# If remaining items in the line, add them
 		if len(line) > 0:
-			line[-1]["text"] += "\n"
-			line[0]["text"] = SMALL_NONE_FONT * LEFT_PADDING + line[0]["text"]
-			content += line * 2
+			line.insert(0, SMALL_NONE_FONT * LEFT_PADDING)
+			content += deepcopy(line) + ["\n"]
+			for i in range(1, len(line)):
+				line[-i]["text"] = MEDIUM_NONE_FONT
+			content += line + ["\n"]
 		
 		# Add the 2 pixels border
 		is_rectangle_shape = len(raw_data) % config['max_items_per_row'] == 0
 		page_image = add_border(page_image, BORDER_COLOR, BORDER_SIZE, is_rectangle_shape)
 		
 		# Save the image and add the page to the book
 		page_image.save(f"{config['manual_path']}/font/category/{file_name}.png")
@@ -392,17 +414,25 @@
 		# Add fonts
 		font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/none.png", "ascent": 8, "height": 20, "chars": [NONE_FONT]})
 		font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/none.png", "ascent": 8, "height": 18, "chars": [MEDIUM_NONE_FONT]})
 		font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/none.png", "ascent": 7, "height": 7, "chars": [SMALL_NONE_FONT]})
 		font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/none.png", "ascent": 0, "height": 2, "chars": [VERY_SMALL_NONE_FONT]})
 		font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/none.png", "ascent": 0, "height": 1, "chars": [MICRO_NONE_FONT]})
 		font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/none.png", "ascent": 7, "height": 16, "chars": [WIKI_NONE_FONT]})
+		font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/invisible_item.png", "ascent": 7, "height": 16, "chars": [INVISIBLE_ITEM_FONT]})
 		font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/wiki_information.png", "ascent": 8, "height": 16, "chars": [WIKI_INFO_FONT]})
 		font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/wiki_result_of_craft.png", "ascent": 8, "height": 16, "chars": [WIKI_RESULT_OF_CRAFT_FONT]})
 		font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/wiki_ingredient_of_craft.png", "ascent": 8, "height": 16, "chars": [WIKI_INGR_OF_CRAFT_FONT]})
+		if config['manual_high_resolution']:
+			font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/shaped_3x3.png", "ascent": 1, "height": 58, "chars": [SHAPED_3X3_FONT]})
+			font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/shaped_2x2.png", "ascent": 1, "height": 58, "chars": [SHAPED_2X2_FONT]})
+			font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/furnace.png", "ascent": 1, "height": 58, "chars": [FURNACE_FONT]})
+			font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/shaped_3x3.png", "ascent": -4, "height": 58, "chars": [HOVER_SHAPED_3X3_FONT]})
+			font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/shaped_2x2.png", "ascent": -1, "height": 58, "chars": [HOVER_SHAPED_2X2_FONT]})
+			font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/furnace.png", "ascent": -3, "height": 58, "chars": [HOVER_FURNACE_FONT]})
 		fonts = {"providers": font_providers}
 		with super_open(f"{config['manual_path']}/font/manual.json", "w") as f:
 			f.write(super_json_dump(fonts).replace("\\\\", "\\"))
 				
 		# Debug book_content
 		with super_open(config['manual_debug'], "w") as f:
 			f.write(super_json_dump(book_content).replace("\\\\", "\\"))
@@ -413,14 +443,23 @@
 	super_copy(f"{config['manual_path']}/font/manual.json", f"{config['build_resource_pack']}/assets/{config['namespace']}/font/manual.json")
 	super_copy(f"{config['manual_path']}/font/category/", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/category/")
 	super_copy(f"{config['manual_path']}/font/page/", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/page/")
 	super_copy(f"{config['manual_path']}/font/wiki_icons/", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/wiki_icons/")
 	if config['manual_high_resolution']:
 		super_copy(f"{config['manual_path']}/font/high_res/", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/high_res/")
 
+	# Verify font providers and textures
+	for fp in font_providers:
+		if "file" in fp:
+			path: str = fp["file"]
+			path = path.replace(config['namespace'] + ':', f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/")
+			if not os.path.exists(path):
+				error(f"Missing font provider at '{path}' for {fp})")
+			if len(fp["chars"]) < 1 or (len(fp["chars"]) == 1 and not fp["chars"][0]):
+				error(f"Font provider '{path}' has no chars")
 
 	# Finally, prepend the manual to the database
 	manual_cmd = min(x["custom_model_data"] for x in config['database'].values() if x.get("custom_model_data")) - 1		# First custom_model_data minus 1
 	manual_database = {"manual":
 		{
 			"id": "minecraft:written_book",
 			"written_book_content": {
```

### Comparing `python_datapack-0.1.7/src/python_datapack/manual/utils.py` & `python_datapack-0.2.0/src/python_datapack/manual/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -219,28 +219,29 @@
 	# If recipe result is specified, take the right texture
 	if craft and craft.get("result"):
 		result_id = ingr_to_id(craft["result"])
 		result_id = result_id.replace(":", "/")
 		image_path = f"{config['manual_path']}/items/{result_id}.png"
 		result_texture = Image.open(image_path)
 
-	# Resize the texture and get the mask
-	result_texture = careful_resize(result_texture, SQUARE_SIZE)
-	result_mask = result_texture.convert("RGBA").split()[3]
-	
 	# Check if there is a craft
 	if craft:
 
+		# Resize the texture and get the mask
+		result_texture = careful_resize(result_texture, SQUARE_SIZE)
+		result_mask = result_texture.convert("RGBA").split()[3]
+
 		# Shaped craft
 		if craft["type"] in "crafting_shaped":
 
 			# Get the image template and append the provider
 			shaped_size = max(2, max(len(craft["shape"]), len(craft["shape"][0])))
 			template = Image.open(f"{TEMPLATES_PATH}/shaped_{shaped_size}x{shaped_size}.png")
-			font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/page/{output_filename}.png", "ascent": 0 if not output_name else 6, "height": 60, "chars": [page_font]})
+			if not config['manual_high_resolution']:
+				font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/page/{output_filename}.png", "ascent": 0 if not output_name else 6, "height": 60, "chars": [page_font]})
 
 			# Loop the shape matrix
 			STARTING_PIXEL = (4, 4)
 			CASE_OFFSETS = (4, 4)
 			for i, row in enumerate(craft["shape"]):
 				for j, symbol in enumerate(row):
 					if symbol != " ":
@@ -271,22 +272,24 @@
 
 			# Place count if the result is greater than 1
 			if craft["result_count"] > 1:
 				count_img = image_count(craft["result_count"])
 				template.paste(count_img, [x + 2 for x in coords], count_img)
 
 			# Save the image
-			template.save(f"{config['manual_path']}/font/page/{output_filename}.png")
+			if not config['manual_high_resolution']:
+				template.save(f"{config['manual_path']}/font/page/{output_filename}.png")
 
 		# Smelting craft
 		elif craft["type"] in FURNACES_RECIPES_TYPES:
 			
 			# Get the image template and append the provider
 			template = Image.open(f"{TEMPLATES_PATH}/furnace.png")
-			font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/page/{output_filename}.png", "ascent": 0 if not output_name else 6, "height": 60, "chars": [page_font]})
+			if not config['manual_high_resolution']:
+				font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/page/{output_filename}.png", "ascent": 0 if not output_name else 6, "height": 60, "chars": [page_font]})
 
 			# Place input item
 			input_item = ingr_to_id(craft["ingredient"])
 			input_item = input_item.replace(":", "/")
 			image_path = f"{config['manual_path']}/items/{input_item}.png"
 			if not os.path.exists(image_path):
 				error(f"Missing item texture at '{image_path}'")
@@ -299,24 +302,35 @@
 			coords = (124, 40)
 			template.paste(result_texture, coords, result_mask)
 			if craft["result_count"] > 1:
 				count_img = image_count(craft["result_count"])
 				template.paste(count_img, [x + 2 for x in coords], count_img)
 			
 			# Save the image
-			template.save(f"{config['manual_path']}/font/page/{output_filename}.png")
+			if not config['manual_high_resolution']:
+				template.save(f"{config['manual_path']}/font/page/{output_filename}.png")
 	
 	# Else, there is no craft, just put the item in a box
 	else:
 		# Get the image template and append the provider
 		template = Image.open(f"{TEMPLATES_PATH}/simple_case_no_border.png")
+		factor = 1
+		if config['manual_high_resolution']:
+			factor = 256 // template.size[0]
+			result_texture = careful_resize(result_texture, SQUARE_SIZE * factor)
+			template = careful_resize(template, 256)
+			result_mask = result_texture.convert("RGBA").split()[3]
+		else:
+			# Resize the texture and get the mask
+			result_texture = careful_resize(result_texture, SQUARE_SIZE)
+			result_mask = result_texture.convert("RGBA").split()[3]
 		font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/page/{output_filename}.png", "ascent": 0 if not output_name else 6, "height": 40, "chars": [page_font]})
 
 		# Place the result item
-		template.paste(result_texture, (2, 2), result_mask)
+		template.paste(result_texture, (2 * factor, 2 * factor), result_mask)
 		template = add_border(template, BORDER_COLOR, BORDER_SIZE, is_rectangle_shape = True)
 		template.save(f"{config['manual_path']}/font/page/{output_filename}.png")
 	return
 
 # Convert craft function
 @simple_cache
 def convert_shapeless_to_shaped(craft: dict) -> dict:
@@ -364,16 +378,16 @@
 		new_craft["shape"] = ["".join(new_craft["shape"][i:i + col_size]) for i in ranged]
 	
 	# Return the shaped craft
 	return new_craft
 
 
 # Convert ingredient to formatted JSON for book
-COMPONENTS_TO_IGNORE = NOT_COMPONENTS + ["custom_data", "count"]
-def get_item_component(config: dict, ingredient: dict|str, only_those_components: list[str] = None) -> dict:
+COMPONENTS_TO_IGNORE = NOT_COMPONENTS + ["custom_data", "count", "profile", "dyed_color", "container"]
+def get_item_component(config: dict, ingredient: dict|str, only_those_components: list[str] = None, count: int = 1) -> dict:
 	""" Generate item hover text for a craft ingredient
 	Args:
 		ingredient (dict|str): The ingredient
 			ex: {'components': {'custom_data': {'iyc': {'adamantium_fragment': True}}}}
 			ex: {'item': 'minecraft:stick'}
 			ex: "adamantium_fragment"	# Only available for the datapack items
 	Returns:
@@ -387,15 +401,15 @@
 		formatted["hoverEvent"]["contents"]["id"] = ingredient["item"]
 	else:
 		# Get the item in the database
 		if isinstance(ingredient, str):
 			id = ingredient
 			item = config['database'][ingredient]
 		else:
-			custom_data = ingredient["components"]["custom_data"]
+			custom_data: dict = ingredient["components"]["custom_data"]
 			id = ingr_to_id(ingredient, add_namespace = False)
 			if custom_data.get(config['namespace']):
 				item = config['database'].get(id)
 			else:
 				for data in custom_data.values():
 					item = config['external_database'].get(list(data.keys())[0])
 					if item:
@@ -417,14 +431,18 @@
 		formatted["hoverEvent"]["contents"]["components"] = components
 
 		# If item is from my datapack, get its page number
 		page_number = get_page_number(id)
 		if page_number != -1:
 			formatted["clickEvent"] = {"action":"change_page","value":str(page_number)}
 	
+	# High resolution
+	if config['manual_high_resolution']:
+		formatted["text"] = high_res_font_from_ingredient(config, ingredient, count)
+
 	# Return
 	return formatted
 
 
 # Generate all craft types content
 def generate_craft_content(config: dict, craft: dict, name: str, page_font: str) -> list:
 	""" Generate the content for the craft type
@@ -433,94 +451,109 @@
 		name		(str):	The name of the item, ex: "adamantium_pickaxe"
 		page_font	(str):	The font for the page, ex: "\u0002"
 	Returns:
 		list:	The content of the craft, ex: [{"text": ...}]
 	"""
 	craft_type = craft["type"]
 	content = [{"text": "", "font": config['namespace'] + ':' + FONT_FILE, "color": "white"}]	# Make default font for every next component
-	
-	# Show up item title and page font
-	titled = name.replace("_", " ").title() + "\n"
-	content.append({"text": titled, "font": "minecraft:default", "color": "black", "underlined": True})
-	content.append(SMALL_NONE_FONT + page_font + "\n")
 
 	# Convert shapeless crafting to shaped crafting
 	if craft_type == "crafting_shapeless":
 		craft = convert_shapeless_to_shaped(craft)
 		craft_type = "crafting_shaped"
 	
+	# If high resolution, get proper page font
+	if config['manual_high_resolution']:
+		page_font = high_res_font_from_craft(craft)
+	
+	# Show up item title and page font
+	titled = name.replace("_", " ").title() + "\n"
+	content.append({"text": titled, "font": "minecraft:default", "color": "black", "underlined": True})
+	content.append(SMALL_NONE_FONT + page_font + "\n")
+	
 	# Generate the image for the page
 	generate_page_font(config, name, page_font, craft)
 
 	# Get result component
-	result_component = get_item_component(config, name)
+	result_count = craft.get("result_count", 1)
+	result_component = get_item_component(config, name, count = result_count)
 	if result_component.get("clickEvent"):
 		del result_component["clickEvent"]	# Remove clickEvent for result item (as we already are on the page)
+	result_component["text"] = MICRO_NONE_FONT + result_component["text"]	# Left adjustment
 
 	# If the craft is shaped
 	if craft_type == "crafting_shaped":
 
 		# Convert each ingredients to its text component
-		formatted_ingredients = {}
+		formatted_ingredients: dict[str, dict] = {}
 		for k, v in craft["ingredients"].items():
 			formatted_ingredients[k] = get_item_component(config, v)
 
 		# Add each ingredient to the craft
 		for line in craft["shape"]:
-			for _ in range(2):	# We need two lines to make a square, otherwise it will be a rectangle
+			for i in range(2):	# We need two lines to make a square, otherwise it will be a rectangle
 				content.append(SMALL_NONE_FONT)
 				for k in line:
 					if k == " ":
-						content.append(NONE_FONT)
+						content.append(INVISIBLE_ITEM_WIDTH)
 					else:
-						content.append(formatted_ingredients[k])
+						if i == 0:
+							content.append(formatted_ingredients[k])
+						else:
+							copy = formatted_ingredients[k].copy()
+							copy["text"] = INVISIBLE_ITEM_WIDTH
+							content.append(copy)
 				content.append("\n")
 		if len(craft["shape"]) == 1 and len(craft["shape"][0]) < 3:
 			content.append("\n")
 			pass
 		
 		# Add the result to the craft
 		if len(craft["shape"]) <= 2 and len(craft["shape"][0]) <= 2:
 
 			# First layer of the square
 			len_1 = len(craft["shape"][0])
 			offset_1 = 3 - len_1
 			break_line_pos = content.index("\n", content.index("\n") + 1)	# Find the second line break
-			content.insert(break_line_pos, NONE_FONT * offset_1)
+			content.insert(break_line_pos, (INVISIBLE_ITEM_WIDTH * offset_1))
 			content.insert(break_line_pos + 1, result_component)
 			
 			# Second layer of the square
 			len_2 = len(craft["shape"][1]) if len(craft["shape"]) > 1 else 0
 			offset_2 = 3 - len_2
 			if len_2 == 0:
 				content.insert(break_line_pos + 2, "\n" + SMALL_NONE_FONT)
 			break_line_pos = content.index("\n", break_line_pos + 3)	# Find the third line break
-			content.insert(break_line_pos, NONE_FONT * offset_2)
-			content.insert(break_line_pos + 1, result_component)
+			content.insert(break_line_pos, (INVISIBLE_ITEM_WIDTH * offset_2))
+			copy = result_component.copy()
+			copy["text"] = INVISIBLE_ITEM_WIDTH
+			content.insert(break_line_pos + 1, copy)
 		else:
 			# First layer of the square
 			len_line = len(craft["shape"][1]) if len(craft["shape"]) > 1 else 0
 			offset = 4 - len_line
 			break_line_pos = content.index("\n", content.index("\n") + 1)	# Find the second line break
 			try:
 				break_line_pos = content.index("\n", break_line_pos + 1) # Find the third line break
 			except:
 				content.append(SMALL_NONE_FONT)
 				break_line_pos = len(content)
-			content.insert(break_line_pos, NONE_FONT * (offset - 1) + SMALL_NONE_FONT * 2)
+			content.insert(break_line_pos, (INVISIBLE_ITEM_WIDTH * (offset - 1) + SMALL_NONE_FONT * 2))
 			content.insert(break_line_pos + 1, result_component)
 
 			# Second layer of the square
 			try:
 				break_line_pos = content.index("\n", break_line_pos + 3)	# Find the fourth line break
 			except:
 				content.append("\n" + SMALL_NONE_FONT)
 				break_line_pos = len(content)
-			content.insert(break_line_pos, NONE_FONT * (offset - 1) + SMALL_NONE_FONT * 2)
-			content.insert(break_line_pos + 1, result_component)
+			content.insert(break_line_pos, (INVISIBLE_ITEM_WIDTH * (offset - 1) + SMALL_NONE_FONT * 2))
+			copy = result_component.copy()
+			copy["text"] = INVISIBLE_ITEM_WIDTH
+			content.insert(break_line_pos + 1, copy)
 
 			# Add break lines for the third layer of a 3x3 craft
 			if len(craft["shape"]) < 3 and len(craft["shape"][0]) == 3:
 				content.append("\n\n")
 				if len(craft["shape"]) < 2:
 					content.append("\n")
 		
@@ -528,23 +561,33 @@
 	# If the type is furnace type,
 	elif craft_type in FURNACES_RECIPES_TYPES:
 		
 		# Convert ingredient to its text component
 		formatted_ingredient = get_item_component(config, craft["ingredient"])
 
 		# Add the ingredient to the craft
-		for _ in range(2):
+		for i in range(2):
 			content.append(SMALL_NONE_FONT)
-			content.append(formatted_ingredient)
+			if i == 0:
+				content.append(formatted_ingredient)
+			else:
+				copy = formatted_ingredient.copy()
+				copy["text"] = INVISIBLE_ITEM_WIDTH
+				content.append(copy)
 			content.append("\n")
 		
 		# Add the result to the craft
-		for _ in range(2):
-			content.append(SMALL_NONE_FONT * 4 + NONE_FONT * 2)
-			content.append(result_component)
+		for i in range(2):
+			content.append(SMALL_NONE_FONT * 4 + INVISIBLE_ITEM_WIDTH * 2)
+			if i == 0:
+				content.append(result_component)
+			else:
+				copy = result_component.copy()
+				copy["text"] = INVISIBLE_ITEM_WIDTH
+				content.append(copy)
 			content.append("\n")
 		content.append("\n\n")
 
 	return content
 
 # Extract unique crafts from a craft list
 def unique_crafts(crafts: list[dict]) -> list[dict]:
@@ -571,14 +614,15 @@
 		list[dict]: ex: [{"type": "crafting_shaped","result_count": 1,"category": "equipment","shape": ["XXX","X X"],"ingredients": {"X": {"components": {"custom_data": {"iyc": {"chainmail": true}}}}},"result": {"item": "minecraft:chainmail_helmet","count": 1}}, ...]
 	"""
 	# Get all crafts that use the item
 	crafts = []
 	for key, value in config['database'].items():
 		if key != item and value.get(RESULT_OF_CRAFTING):
 			for craft in value[RESULT_OF_CRAFTING]:
+				craft: dict = craft
 				if ("ingredient" in craft and item == ingr_to_id(craft["ingredient"], False)) or \
 					("ingredients" in craft and isinstance(craft["ingredients"], dict) and item in [ingr_to_id(x, False) for x in craft["ingredients"].values()]) or \
 					("ingredients" in craft and isinstance(craft["ingredients"], list) and item in [ingr_to_id(x, False) for x in craft["ingredients"]]):
 					# Convert craft, ex:
 					# before:	chainmail_helmet	{"type": "crafting_shaped","result_count": 1,"category": "equipment","shape": ["XXX","X X"],"ingredients": {"X": {"components": {"custom_data": {"iyc": {"chainmail": true}}}}}}}
 					# after:	chainmail			{"type": "crafting_shaped","result_count": 1,"category": "equipment","shape": ["XXX","X X"],"ingredients": {"X": {"components": {"custom_data": {"iyc": {"chainmail": true}}}}},"result": {"item": "minecraft:chainmail_helmet","count": 1}}
 					craft_copy = craft.copy()
@@ -606,27 +650,30 @@
 	
 	# Get result item texture and paste it on the wiki_ingredient_of_craft_template
 	try:
 		result_item = ingr_to_id(craft["result"]).replace(":", "/")
 		texture_path = f"{config['manual_path']}/items/{result_item}.png"
 		result_item = result_item.replace("/", "_")
 		dest_path = f"{config['manual_path']}/font/wiki_icons/{result_item}.png"
-		if not os.path.exists(dest_path):
 
-			# Load texture and resize it
-			item_texture = Image.open(texture_path)
-			item_texture = careful_resize(item_texture, 42)
-			item_texture = item_texture.convert("RGBA")
-
-			# Load the template and paste the texture on it
-			template = Image.open(f"{TEMPLATES_PATH}/wiki_ingredient_of_craft_template.png")
-			template.paste(item_texture, (11, 11), item_texture)
-			
-			# Save the result
-			template.save(dest_path)
+		# Load texture and resize it
+		item_texture = Image.open(texture_path)
+		item_res = 64 if not config["manual_high_resolution"] else 256
+		item_res_adjusted = int(item_res * 0.75)
+		item_texture = careful_resize(item_texture, item_res_adjusted)
+		item_texture = item_texture.convert("RGBA")
+
+		# Load the template and paste the texture on it
+		template = Image.open(f"{TEMPLATES_PATH}/wiki_ingredient_of_craft_template.png")
+		template = careful_resize(template, item_res)
+		offset = (item_res - item_res_adjusted) // 2
+		template.paste(item_texture, (offset, offset), item_texture)
+
+		# Save the result
+		template.save(dest_path)
 
 		# Prepare provider
 		font = get_next_font()
 		font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/wiki_icons/{result_item}.png", "ascent": 8, "height": 16, "chars": [font]})
 
 	except Exception as e:
 		warning(f"Failed to generate craft icon for {name}: {e}\nreturning default font...")
@@ -649,15 +696,15 @@
 	item = f"{item}_{count}" if count > 1 else item
 	
 	# Get output path
 	path = f"{config['manual_path']}/font/high_res/{item}.png"
 	provider_path = f"{config['namespace']}:font/high_res/{item}.png"
 	for p in font_providers:	# Check if it already exists
 		if p["file"] == provider_path:
-			return p["chars"][0]
+			return MICRO_NONE_FONT + p["chars"][0]
 	font_providers.append({"type":"bitmap","file": provider_path, "ascent": 7, "height": 16, "chars": [font]})
 
 
 	# Generate high res font
 	os.makedirs(os.path.dirname(path), exist_ok = True)
 	high_res: int = 256
 	resized = careful_resize(item_image, high_res)
@@ -675,8 +722,46 @@
 	angles = [(0, 0), (total_width, 0), (0, total_height), (total_width, total_height)]
 	for angle in angles:
 		resized.putpixel(angle, (0, 0, 0, 100))
 
 	# Save the result and return the font
 	resized.save(path)
 	return MICRO_NONE_FONT + font
+
+# Call the previous function
+def high_res_font_from_ingredient(config: dict, ingredient: str|dict, count: int = 1) -> str:
+	""" Generate the high res font to display in the manual for the ingredient
+	Args:
+		ingredient	(str|dict):	The ingredient, ex: "adamantium_fragment" or {"item": "minecraft:stick"} or {"components": {"custom_data": {"iyc": {"adamantium_fragment": true}}}}
+		count		(int):		The count of the item
+	Returns:
+		str: The font to the generated texture
+	"""
+	# Decode the ingredient
+	if isinstance(ingredient, dict):
+		ingredient = ingr_to_id(ingredient, add_namespace = True)
+	if ':' in ingredient:
+		image_path = f"{config['manual_path']}/items/{ingredient.replace(':', '/')}.png"
+		if not os.path.exists(image_path):
+			error(f"Missing item texture at '{image_path}'")
+		item_image = Image.open(image_path)
+		ingredient = ingredient.split(":")[1]
+	else:
+		item_image = Image.open(f"{config['manual_path']}/items/{config['namespace']}/{ingredient}.png")
 	
+	# Generate the high res font
+	return generate_high_res_font(config, ingredient, item_image, count)
+
+# Util function
+@simple_cache
+def high_res_font_from_craft(craft: dict) -> str:
+	if craft["type"] in FURNACES_RECIPES_TYPES:
+		return FURNACE_FONT
+	elif craft["type"] == "crafting_shaped":
+		if len(craft["shape"]) == 3 or len(craft["shape"][0]) == 3:
+			return SHAPED_3X3_FONT
+		else:
+			return SHAPED_2X2_FONT
+	else:
+		error(f"Unknown craft type '{craft['type']}'")
+		return ""
+
```

### Comparing `python_datapack-0.1.7/src/python_datapack/manual/assets/furnace.png` & `python_datapack-0.2.0/src/python_datapack/manual/assets/furnace.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/manual/assets/minecraft_font.ttf` & `python_datapack-0.2.0/src/python_datapack/manual/assets/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/manual/assets/shaped_2x2.png` & `python_datapack-0.2.0/src/python_datapack/manual/assets/shaped_2x2.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/manual/assets/shaped_3x3.png` & `python_datapack-0.2.0/src/python_datapack/manual/assets/shaped_3x3.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/manual/assets/simple_case_no_border.png` & `python_datapack-0.2.0/src/python_datapack/manual/assets/simple_case_no_border.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/resource_pack/check_unused_textures.py` & `python_datapack-0.2.0/src/python_datapack/resource_pack/check_unused_textures.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/resource_pack/item_models.py` & `python_datapack-0.2.0/src/python_datapack/resource_pack/item_models.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/resource_pack/main.py` & `python_datapack-0.2.0/src/python_datapack/resource_pack/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/resource_pack/sounds.py` & `python_datapack-0.2.0/src/python_datapack/resource_pack/sounds.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/resource_pack/vanilla_models.py` & `python_datapack-0.2.0/src/python_datapack/resource_pack/vanilla_models.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/utils/database_helper.py` & `python_datapack-0.2.0/src/python_datapack/utils/database_helper.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/utils/ingredients.py` & `python_datapack-0.2.0/src/python_datapack/utils/ingredients.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/utils/io.py` & `python_datapack-0.2.0/src/python_datapack/utils/io.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/utils/multiprocessing.py` & `python_datapack-0.2.0/src/python_datapack/utils/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/utils/print.py` & `python_datapack-0.2.0/src/python_datapack/utils/print.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/src/python_datapack/utils/weld.py` & `python_datapack-0.2.0/src/python_datapack/utils/weld.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/LICENSE` & `python_datapack-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.7/pyproject.toml` & `python_datapack-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["hatchling", "pillow", "smithed", "model_resolver"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python_datapack"
-version = "0.1.7"
+version = "0.2.0"
 authors = [
 	{ name="Stoupy51", email="stoupy51@gmail.com" },
 ]
 description = "Python package to help generating advanced Minecraft datapack contents"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `python_datapack-0.1.7/PKG-INFO` & `python_datapack-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python_datapack
-Version: 0.1.7
+Version: 0.2.0
 Summary: Python package to help generating advanced Minecraft datapack contents
 Project-URL: Homepage, https://github.com/Stoupy51/python_datapack
 Project-URL: Issues, https://github.com/Stoupy51/python_datapack/issues
 Author-email: Stoupy51 <stoupy51@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

