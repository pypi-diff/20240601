# Comparing `tmp/ezdxf-1.3.1b0.zip` & `tmp/ezdxf-1.3.1b1.zip`

## zipinfo {}

```diff
@@ -1,870 +1,870 @@
-Zip file size: 2210198 bytes, number of entries: 868
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/integration_tests/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/
--rw-rw-rw-  2.0 fat     1092 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/LICENSE
--rw-rw-rw-  2.0 fat      329 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/MANIFEST.in
--rw-rw-rw-  2.0 fat    10110 b- defN 24-May-28 12:38 ezdxf-1.3.1b0/PKG-INFO
--rw-rw-rw-  2.0 fat     2527 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/pyproject.toml
--rw-rw-rw-  2.0 fat     7479 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/README.md
--rw-rw-rw-  2.0 fat       74 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/requirements.txt
--rw-rw-rw-  2.0 fat       42 b- defN 24-May-28 12:38 ezdxf-1.3.1b0/setup.cfg
--rw-rw-rw-  2.0 fat     2140 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/setup.py
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/integration_tests/data/
--rw-rw-rw-  2.0 fat      567 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/check_disable_c_ext_by_config_file.py
--rw-rw-rw-  2.0 fat      541 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/check_disable_c_ext_by_env_var.py
--rw-rw-rw-  2.0 fat      410 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/conftest.py
--rw-rw-rw-  2.0 fat     1054 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_acad_table.py
--rw-rw-rw-  2.0 fat     1339 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_acis_entites.py
--rw-rw-rw-  2.0 fat     4686 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_all_dimline_styles.py
--rw-rw-rw-  2.0 fat     4153 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_all_ellipse_transformations.py
--rw-rw-rw-  2.0 fat     1064 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_anonymous_blocks.py
--rw-rw-rw-  2.0 fat      577 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_appsettings.py
--rw-rw-rw-  2.0 fat      871 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_audit_critical_dxf_files.py
--rw-rw-rw-  2.0 fat     1603 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_audit_layouts.py
--rw-rw-rw-  2.0 fat     1726 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_complex_line_type_2.py
--rw-rw-rw-  2.0 fat     1003 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_create_basic_graphics.py
--rw-rw-rw-  2.0 fat     1921 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_document_guid.py
--rw-rw-rw-  2.0 fat     1832 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_document_page_setup.py
--rw-rw-rw-  2.0 fat      998 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_dxf_info_scanning.py
--rw-rw-rw-  2.0 fat     1299 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_dynblkhelper.py
--rw-rw-rw-  2.0 fat     1558 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_entities_iterator.py
--rw-rw-rw-  2.0 fat      934 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_fix_dulicate_handles.py
--rw-rw-rw-  2.0 fat     1901 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_geo.py
--rw-rw-rw-  2.0 fat     1250 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_groups.py
--rw-rw-rw-  2.0 fat      905 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_hpgl2_addon.py
--rw-rw-rw-  2.0 fat      630 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_ignore_junk_beyond_EOF.py
--rw-rw-rw-  2.0 fat     1155 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_launcher.py
--rw-rw-rw-  2.0 fat      631 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_leica_disto_r12.py
--rw-rw-rw-  2.0 fat      737 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_load_dxf_unicode_notation.py
--rw-rw-rw-  2.0 fat     2931 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_mapbox_earcut.py
--rw-rw-rw-  2.0 fat     2230 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_mtext_columns.py
--rw-rw-rw-  2.0 fat     2392 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_mtext_explode_addon.py
--rw-rw-rw-  2.0 fat     1846 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_mtext_text_frame.py
--rw-rw-rw-  2.0 fat     1053 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_new_table_entries.py
--rw-rw-rw-  2.0 fat      887 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_none_ascii_read_write.py
--rw-rw-rw-  2.0 fat     3435 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_odafc.py
--rw-rw-rw-  2.0 fat     1737 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_open_binary_DXF_files.py
--rw-rw-rw-  2.0 fat      751 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_open_coord_order_issue.py
--rw-rw-rw-  2.0 fat     3842 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_open_exotic_dxf_files.py
--rw-rw-rw-  2.0 fat      879 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_open_R13_R14.py
--rw-rw-rw-  2.0 fat     3152 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_polyline_entity.py
--rw-rw-rw-  2.0 fat     1749 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_preserve_binary_data_in_xrecords.py
--rw-rw-rw-  2.0 fat     6944 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_r12export.py
--rw-rw-rw-  2.0 fat     6256 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_r12strict.py
--rw-rw-rw-  2.0 fat     3410 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_r12writer.py
--rw-rw-rw-  2.0 fat      567 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_read_file_without_handles.py
--rw-rw-rw-  2.0 fat     1121 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_read_write_modern_entites.py
--rw-rw-rw-  2.0 fat     7747 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_recover.py
--rw-rw-rw-  2.0 fat     1959 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_redraw_order.py
--rw-rw-rw-  2.0 fat     1819 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_rotated_block_attributes.py
--rw-rw-rw-  2.0 fat      774 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_surface_entities.py
--rw-rw-rw-  2.0 fat      928 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_write_fixed_meta_data.py
--rw-rw-rw-  2.0 fat     1806 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_write_without_handles.py
--rw-rw-rw-  2.0 fat     3638 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_xref_detach.py
--rw-rw-rw-  2.0 fat     2347 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/test_xref_load_acis.py
--rw-rw-rw-  2.0 fat     3060 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/AC1003_LINE_Example.dxf
--rw-rw-rw-  2.0 fat   179505 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/acad_table_with_blk_ref.dxf
--rw-rw-rw-  2.0 fat     7956 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/ASCII_R12.dxf
--rw-rw-rw-  2.0 fat     3761 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r12.dxf
--rw-rw-rw-  2.0 fat    20914 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r13.dxf
--rw-rw-rw-  2.0 fat    21137 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r14.dxf
--rw-rw-rw-  2.0 fat    11564 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r2000.dxf
--rw-rw-rw-  2.0 fat     6424 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/cc_dxflib.dxf
--rw-rw-rw-  2.0 fat   173753 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/custom_blocks.dxf
--rw-rw-rw-  2.0 fat    32203 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/duplicate_handles.dxf
--rw-rw-rw-  2.0 fat    18554 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/dxf_unicode.dxf
--rw-rw-rw-  2.0 fat    56494 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/dynblks.zip
--rw-rw-rw-  2.0 fat     1592 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/empty_handles.dxf
--rw-rw-rw-  2.0 fat    97103 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/groups.dxf
--rw-rw-rw-  2.0 fat    19533 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/layout_broken_links.dxf
--rw-rw-rw-  2.0 fat    19506 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/layout_broken_links_2.dxf
--rw-rw-rw-  2.0 fat    19291 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/layout_missing_block_definition.dxf
--rw-rw-rw-  2.0 fat    19383 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/layout_missing_block_record.dxf
--rw-rw-rw-  2.0 fat     9146 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/Leica_Disto_S910.dxf
--rw-rw-rw-  2.0 fat    17986 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/MODEL.dxf
--rw-rw-rw-  2.0 fat    25799 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/mtext_columns_R2007.dxf
--rw-rw-rw-  2.0 fat    23927 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/mtext_columns_R2018.dxf
--rw-rw-rw-  2.0 fat    98230 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/mtext_framed_columns.dxf
--rw-rw-rw-  2.0 fat   106574 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/mtext_text_frame.dxf
--rw-rw-rw-  2.0 fat    12001 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/no_layouts.dxf
--rw-rw-rw-  2.0 fat    16295 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/PLOTFILE.plt
--rw-rw-rw-  2.0 fat    28788 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/POLI-ALL210_12.DXF
--rw-rw-rw-  2.0 fat      144 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/R12_with_trash_beyond_EOF.dxf
--rw-rw-rw-  2.0 fat   212407 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/recover01.dxf
--rw-rw-rw-  2.0 fat   115423 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/recover02.dxf
--rw-rw-rw-  2.0 fat    21178 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/small_r13.dxf
--rw-rw-rw-  2.0 fat    10326 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/small_r14.dxf
--rw-rw-rw-  2.0 fat    11286 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/XRECORD_0.bin
--rw-rw-rw-  2.0 fat    11662 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/XRECORD_1.bin
--rw-rw-rw-  2.0 fat    15337 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/integration_tests/data/XRECORD_2.bin
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf.egg-info/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/acc/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/acis/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/addons/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/entities/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/fonts/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/layouts/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/lldxf/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/math/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/path/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/render/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/resources/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/sections/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/tools/
--rw-rw-rw-  2.0 fat     4841 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/appsettings.py
--rw-rw-rw-  2.0 fat    19976 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/audit.py
--rw-rw-rw-  2.0 fat     5324 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/bbox.py
--rw-rw-rw-  2.0 fat     7872 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/blkrefs.py
--rw-rw-rw-  2.0 fat    17062 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/colors.py
--rw-rw-rw-  2.0 fat    33508 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/commands.py
--rw-rw-rw-  2.0 fat     1549 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/comments.py
--rw-rw-rw-  2.0 fat    22334 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/disassemble.py
--rw-rw-rw-  2.0 fat    55248 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/document.py
--rw-rw-rw-  2.0 fat      832 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/dwginfo.py
--rw-rw-rw-  2.0 fat     2475 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/dynblkhelper.py
--rw-rw-rw-  2.0 fat    21292 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/edgeminer.py
--rw-rw-rw-  2.0 fat     5441 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/edgesmith.py
--rw-rw-rw-  2.0 fat    16254 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entitydb.py
--rw-rw-rw-  2.0 fat     7495 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/enums.py
--rw-rw-rw-  2.0 fat    14519 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/explode.py
--rw-rw-rw-  2.0 fat     1653 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/eztypes.py
--rw-rw-rw-  2.0 fat    10366 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/filemanagement.py
--rw-rw-rw-  2.0 fat    12157 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/gfxattribs.py
--rw-rw-rw-  2.0 fat   107519 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/graphicsfactory.py
--rw-rw-rw-  2.0 fat     3416 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/groupby.py
--rw-rw-rw-  2.0 fat      658 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/messenger.py
--rw-rw-rw-  2.0 fat      272 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/msgtypes.py
--rw-rw-rw-  2.0 fat    20554 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/npshapes.py
--rw-rw-rw-  2.0 fat     3030 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/protocols.py
--rw-rw-rw-  2.0 fat    35308 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/proxygraphic.py
--rw-rw-rw-  2.0 fat       95 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/py.typed
--rw-rw-rw-  2.0 fat    22499 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/query.py
--rw-rw-rw-  2.0 fat     2780 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/queryparser.py
--rw-rw-rw-  2.0 fat     9564 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/r12strict.py
--rw-rw-rw-  2.0 fat    31442 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/recover.py
--rw-rw-rw-  2.0 fat     3515 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/reorder.py
--rw-rw-rw-  2.0 fat     3926 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/revcloud.py
--rw-rw-rw-  2.0 fat    11250 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/select.py
--rw-rw-rw-  2.0 fat    12848 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/transform.py
--rw-rw-rw-  2.0 fat     5750 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/units.py
--rw-rw-rw-  2.0 fat     8280 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/upright.py
--rw-rw-rw-  2.0 fat     9875 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/urecord.py
--rw-rw-rw-  2.0 fat     1024 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/version.py
--rw-rw-rw-  2.0 fat    18280 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/xclip.py
--rw-rw-rw-  2.0 fat    65739 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/xref.py
--rw-rw-rw-  2.0 fat     2853 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/zoom.py
--rw-rw-rw-  2.0 fat    10898 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/_options.py
--rw-rw-rw-  2.0 fat     3138 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/__init__.py
--rw-rw-rw-  2.0 fat     3259 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/__main__.py
--rw-rw-rw-  2.0 fat     6788 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/bezier3p.pyx
--rw-rw-rw-  2.0 fat    11502 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/bezier4p.pyx
--rw-rw-rw-  2.0 fat    14048 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/bspline.pyx
--rw-rw-rw-  2.0 fat      252 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/constants.h
--rw-rw-rw-  2.0 fat    11844 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/construct.pyx
--rw-rw-rw-  2.0 fat     3161 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/linetypes.pyx
--rw-rw-rw-  2.0 fat    23976 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/mapbox_earcut.pyx
--rw-rw-rw-  2.0 fat      385 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/matrix44.pxd
--rw-rw-rw-  2.0 fat    23703 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/matrix44.pyx
--rw-rw-rw-  2.0 fat     4705 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/np_support.pyx
--rw-rw-rw-  2.0 fat     1719 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/vector.pxd
--rw-rw-rw-  2.0 fat    23377 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/vector.pyx
--rw-rw-rw-  2.0 fat     1265 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acc/__init__.py
--rw-rw-rw-  2.0 fat     6398 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/abstract.py
--rw-rw-rw-  2.0 fat      938 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/api.py
--rw-rw-rw-  2.0 fat     1792 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/cache.py
--rw-rw-rw-  2.0 fat     5489 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/const.py
--rw-rw-rw-  2.0 fat     6731 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/dbg.py
--rw-rw-rw-  2.0 fat     2985 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/dxf.py
--rw-rw-rw-  2.0 fat    28750 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/entities.py
--rw-rw-rw-  2.0 fat     4093 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/hdr.py
--rw-rw-rw-  2.0 fat    15566 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/mesh.py
--rw-rw-rw-  2.0 fat    18695 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/sab.py
--rw-rw-rw-  2.0 fat    13189 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/sat.py
--rw-rw-rw-  2.0 fat      247 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/type_hints.py
--rw-rw-rw-  2.0 fat      120 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/acis/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/addons/acisbrowser/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/addons/browser/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/addons/dwg/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/
--rw-rw-rw-  2.0 fat    26766 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/acadctb.py
--rw-rw-rw-  2.0 fat    22229 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/binpacking.py
--rw-rw-rw-  2.0 fat    27692 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/dimlines.py
--rw-rw-rw-  2.0 fat    31464 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/dxf2code.py
--rw-rw-rw-  2.0 fat    22005 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/genetic_algorithm.py
--rw-rw-rw-  2.0 fat    38393 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/geo.py
--rw-rw-rw-  2.0 fat     2674 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/gerber_D6673.py
--rw-rw-rw-  2.0 fat    25472 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/importer.py
--rw-rw-rw-  2.0 fat    17355 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/iterdxf.py
--rw-rw-rw-  2.0 fat     8946 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/menger_sponge.py
--rw-rw-rw-  2.0 fat    24787 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/meshex.py
--rw-rw-rw-  2.0 fat      492 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/mixins.py
--rw-rw-rw-  2.0 fat     6203 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/mtextsurrogate.py
--rw-rw-rw-  2.0 fat    13528 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/mtxpl.py
--rw-rw-rw-  2.0 fat    16364 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/odafc.py
--rw-rw-rw-  2.0 fat     9456 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/openscad.py
--rw-rw-rw-  2.0 fat    15878 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/pycsg.py
--rw-rw-rw-  2.0 fat    22301 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/r12export.py
--rw-rw-rw-  2.0 fat    27191 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/r12writer.py
--rw-rw-rw-  2.0 fat     7605 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/sierpinski_pyramid.py
--rw-rw-rw-  2.0 fat    33167 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/tablepainter.py
--rw-rw-rw-  2.0 fat    12768 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/text2path.py
--rw-rw-rw-  2.0 fat     3335 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/xplayer.py
--rw-rw-rw-  2.0 fat     2312 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/xqt.py
--rw-rw-rw-  2.0 fat      453 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/__init__.py
--rw-rw-rw-  2.0 fat     9975 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/acisbrowser/browser.py
--rw-rw-rw-  2.0 fat     1907 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/acisbrowser/data.py
--rw-rw-rw-  2.0 fat       64 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/acisbrowser/__init__.py
--rw-rw-rw-  2.0 fat      820 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/browser/bookmarks.py
--rw-rw-rw-  2.0 fat    29347 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/browser/browser.py
--rw-rw-rw-  2.0 fat    14891 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/browser/data.py
--rw-rw-rw-  2.0 fat    10993 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/browser/find_dialog.py
--rw-rw-rw-  2.0 fat     1249 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/browser/loader.py
--rw-rw-rw-  2.0 fat    21111 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/browser/model.py
--rw-rw-rw-  2.0 fat     6896 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/browser/reflinks.py
--rw-rw-rw-  2.0 fat     2214 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/browser/tags.py
--rw-rw-rw-  2.0 fat     1366 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/browser/views.py
--rw-rw-rw-  2.0 fat      133 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/browser/__init__.py
--rw-rw-rw-  2.0 fat     9265 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/backend.py
--rw-rw-rw-  2.0 fat    11113 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/config.py
--rw-rw-rw-  2.0 fat     1756 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/debug_backend.py
--rw-rw-rw-  2.0 fat      514 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/debug_utils.py
--rw-rw-rw-  2.0 fat     7391 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/dxf.py
--rw-rw-rw-  2.0 fat     7753 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/file_output.py
--rw-rw-rw-  2.0 fat    44576 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/frontend.py
--rw-rw-rw-  2.0 fat     1877 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/gfxproxy.py
--rw-rw-rw-  2.0 fat    20834 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/hpgl2.py
--rw-rw-rw-  2.0 fat    20101 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/json.py
--rw-rw-rw-  2.0 fat    18871 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/layout.py
--rw-rw-rw-  2.0 fat    13209 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/matplotlib.py
--rw-rw-rw-  2.0 fat     9862 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/mtext_complex.py
--rw-rw-rw-  2.0 fat    32445 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/pipeline.py
--rw-rw-rw-  2.0 fat    40194 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/properties.py
--rw-rw-rw-  2.0 fat    18036 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/pymupdf.py
--rw-rw-rw-  2.0 fat    11577 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/pyqt.py
--rw-rw-rw-  2.0 fat    22713 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/qtviewer.py
--rw-rw-rw-  2.0 fat    16434 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/recorder.py
--rw-rw-rw-  2.0 fat    16222 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/svg.py
--rw-rw-rw-  2.0 fat    13023 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/text.py
--rw-rw-rw-  2.0 fat     1194 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/text_renderer.py
--rw-rw-rw-  2.0 fat      314 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/type_hints.py
--rw-rw-rw-  2.0 fat     2559 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/unified_text_renderer.py
--rw-rw-rw-  2.0 fat      171 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/drawing/__init__.py
--rw-rw-rw-  2.0 fat     3112 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/dwg/classes_section.py
--rw-rw-rw-  2.0 fat      763 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/dwg/const.py
--rw-rw-rw-  2.0 fat     6091 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/dwg/crc.py
--rw-rw-rw-  2.0 fat     3160 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/dwg/fileheader.py
--rw-rw-rw-  2.0 fat    14851 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/dwg/header_section.py
--rw-rw-rw-  2.0 fat     2976 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/dwg/loader.py
--rw-rw-rw-  2.0 fat      141 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/dwg/__init__.py
--rw-rw-rw-  2.0 fat    13443 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/api.py
--rw-rw-rw-  2.0 fat     8554 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/backend.py
--rw-rw-rw-  2.0 fat      561 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/deps.py
--rw-rw-rw-  2.0 fat    16079 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/interpreter.py
--rw-rw-rw-  2.0 fat     4836 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/page.py
--rw-rw-rw-  2.0 fat    11766 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/plotter.py
--rw-rw-rw-  2.0 fat     1698 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/polygon_buffer.py
--rw-rw-rw-  2.0 fat     5615 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/properties.py
--rw-rw-rw-  2.0 fat     6222 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/tokenizer.py
--rw-rw-rw-  2.0 fat    19435 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/viewer.py
--rw-rw-rw-  2.0 fat      164 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/__init__.py
--rw-rw-rw-  2.0 fat     5710 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/acad_proxy_entity.py
--rw-rw-rw-  2.0 fat    21579 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/acad_table.py
--rw-rw-rw-  2.0 fat     2850 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/acad_xrec_roundtrip.py
--rw-rw-rw-  2.0 fat    30267 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/acis.py
--rw-rw-rw-  2.0 fat     4996 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/appdata.py
--rw-rw-rw-  2.0 fat     1954 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/appid.py
--rw-rw-rw-  2.0 fat     4942 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/arc.py
--rw-rw-rw-  2.0 fat    27092 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/attrib.py
--rw-rw-rw-  2.0 fat     8881 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/block.py
--rw-rw-rw-  2.0 fat    10586 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/blockrecord.py
--rw-rw-rw-  2.0 fat    51025 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/boundary_paths.py
--rw-rw-rw-  2.0 fat     7929 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/circle.py
--rw-rw-rw-  2.0 fat     3214 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/copy.py
--rw-rw-rw-  2.0 fat    24981 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/dictionary.py
--rw-rw-rw-  2.0 fat    48717 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/dimension.py
--rw-rw-rw-  2.0 fat    35043 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/dimstyle.py
--rw-rw-rw-  2.0 fat    23813 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/dimstyleoverride.py
--rw-rw-rw-  2.0 fat     4399 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/dxfclass.py
--rw-rw-rw-  2.0 fat    40587 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/dxfentity.py
--rw-rw-rw-  2.0 fat    27114 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/dxfgfx.py
--rw-rw-rw-  2.0 fat    16471 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/dxfgroups.py
--rw-rw-rw-  2.0 fat    23679 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/dxfns.py
--rw-rw-rw-  2.0 fat    13910 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/dxfobj.py
--rw-rw-rw-  2.0 fat    11186 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/ellipse.py
--rw-rw-rw-  2.0 fat     4138 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/factory.py
--rw-rw-rw-  2.0 fat    23747 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/geodata.py
--rw-rw-rw-  2.0 fat     4026 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/gradient.py
--rw-rw-rw-  2.0 fat    12263 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/hatch.py
--rw-rw-rw-  2.0 fat     3944 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/helix.py
--rw-rw-rw-  2.0 fat     4838 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/idbuffer.py
--rw-rw-rw-  2.0 fat    27125 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/image.py
--rw-rw-rw-  2.0 fat    28148 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/insert.py
--rw-rw-rw-  2.0 fat    28698 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/layer.py
--rw-rw-rw-  2.0 fat    14358 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/layout.py
--rw-rw-rw-  2.0 fat    13070 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/leader.py
--rw-rw-rw-  2.0 fat     4718 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/light.py
--rw-rw-rw-  2.0 fat     3718 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/line.py
--rw-rw-rw-  2.0 fat     9763 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/ltype.py
--rw-rw-rw-  2.0 fat    19055 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/lwpolyline.py
--rw-rw-rw-  2.0 fat    19352 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/material.py
--rw-rw-rw-  2.0 fat    17444 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/mesh.py
--rw-rw-rw-  2.0 fat    57437 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/mleader.py
--rw-rw-rw-  2.0 fat    37229 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/mline.py
--rw-rw-rw-  2.0 fat     8385 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/mpolygon.py
--rw-rw-rw-  2.0 fat    48239 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/mtext.py
--rw-rw-rw-  2.0 fat     4351 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/mtext_columns.py
--rw-rw-rw-  2.0 fat     6230 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/objectcollection.py
--rw-rw-rw-  2.0 fat     2151 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/oleframe.py
--rw-rw-rw-  2.0 fat     4332 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/pattern.py
--rw-rw-rw-  2.0 fat     5238 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/point.py
--rw-rw-rw-  2.0 fat    16978 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/polygon.py
--rw-rw-rw-  2.0 fat    40126 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/polyline.py
--rw-rw-rw-  2.0 fat     4822 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/shape.py
--rw-rw-rw-  2.0 fat    10485 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/solid.py
--rw-rw-rw-  2.0 fat     7990 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/spatial_filter.py
--rw-rw-rw-  2.0 fat    23810 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/spline.py
--rw-rw-rw-  2.0 fat     8382 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/subentity.py
--rw-rw-rw-  2.0 fat     5196 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/sun.py
--rw-rw-rw-  2.0 fat     2449 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/table.py
--rw-rw-rw-  2.0 fat     1341 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/temporary_transform.py
--rw-rw-rw-  2.0 fat    17633 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/text.py
--rw-rw-rw-  2.0 fat     9053 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/textstyle.py
--rw-rw-rw-  2.0 fat     3617 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/tolerance.py
--rw-rw-rw-  2.0 fat     2703 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/ucs.py
--rw-rw-rw-  2.0 fat    14452 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/underlay.py
--rw-rw-rw-  2.0 fat     6040 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/view.py
--rw-rw-rw-  2.0 fat    28360 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/viewport.py
--rw-rw-rw-  2.0 fat     7958 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/visualstyle.py
--rw-rw-rw-  2.0 fat     9970 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/vport.py
--rw-rw-rw-  2.0 fat    17024 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/xdata.py
--rw-rw-rw-  2.0 fat     8531 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/xdict.py
--rw-rw-rw-  2.0 fat     3062 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/xline.py
--rw-rw-rw-  2.0 fat     3191 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/entities/__init__.py
--rw-rw-rw-  2.0 fat    26337 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/fonts/fonts.py
--rw-rw-rw-  2.0 fat     2242 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/fonts/font_face.py
--rw-rw-rw-  2.0 fat    18620 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/fonts/font_manager.py
--rw-rw-rw-  2.0 fat     1702 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/fonts/font_measurements.py
--rw-rw-rw-  2.0 fat      288 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/fonts/font_synonyms.py
--rw-rw-rw-  2.0 fat     1175 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/fonts/glyphs.py
--rw-rw-rw-  2.0 fat    10763 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/fonts/lff.py
--rw-rw-rw-  2.0 fat    35414 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/fonts/shapefile.py
--rw-rw-rw-  2.0 fat     7244 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/fonts/ttfonts.py
--rw-rw-rw-  2.0 fat       64 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/fonts/__init__.py
--rw-rw-rw-  2.0 fat    16964 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/layouts/base.py
--rw-rw-rw-  2.0 fat     4343 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/layouts/blocklayout.py
--rw-rw-rw-  2.0 fat    32460 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/layouts/layout.py
--rw-rw-rw-  2.0 fat    15314 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/layouts/layouts.py
--rw-rw-rw-  2.0 fat      232 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/layouts/__init__.py
--rw-rw-rw-  2.0 fat     8327 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/attributes.py
--rw-rw-rw-  2.0 fat    16560 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/const.py
--rw-rw-rw-  2.0 fat     2715 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/encoding.py
--rw-rw-rw-  2.0 fat    16997 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/extendedtags.py
--rw-rw-rw-  2.0 fat     5363 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/fileindex.py
--rw-rw-rw-  2.0 fat      727 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/hdrvars.py
--rw-rw-rw-  2.0 fat     5469 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/loader.py
--rw-rw-rw-  2.0 fat     7152 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/packedtags.py
--rw-rw-rw-  2.0 fat     6355 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/repair.py
--rw-rw-rw-  2.0 fat    14509 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/tagger.py
--rw-rw-rw-  2.0 fat    14325 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/tags.py
--rw-rw-rw-  2.0 fat    11054 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/tagwriter.py
--rw-rw-rw-  2.0 fat    12000 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/types.py
--rw-rw-rw-  2.0 fat    17303 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/validator.py
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/lldxf/__init__.py
--rw-rw-rw-  2.0 fat    19209 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/arc.py
--rw-rw-rw-  2.0 fat    15532 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/bbox.py
--rw-rw-rw-  2.0 fat     9310 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/bezier.py
--rw-rw-rw-  2.0 fat     2458 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/bezier_interpolation.py
--rw-rw-rw-  2.0 fat     8730 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/box.py
--rw-rw-rw-  2.0 fat    53170 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/bspline.py
--rw-rw-rw-  2.0 fat     5608 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/bulge.py
--rw-rw-rw-  2.0 fat     9135 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/circle.py
--rw-rw-rw-  2.0 fat    33170 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/clipping.py
--rw-rw-rw-  2.0 fat     4319 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/clustering.py
--rw-rw-rw-  2.0 fat    11618 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/construct2d.py
--rw-rw-rw-  2.0 fat    26176 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/construct3d.py
--rw-rw-rw-  2.0 fat     1273 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/cspline.py
--rw-rw-rw-  2.0 fat     9114 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/curvetools.py
--rw-rw-rw-  2.0 fat    21723 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/ellipse.py
--rw-rw-rw-  2.0 fat     4406 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/eulerspiral.py
--rw-rw-rw-  2.0 fat    13190 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/legacy.py
--rw-rw-rw-  2.0 fat    27210 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/linalg.py
--rw-rw-rw-  2.0 fat    10213 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/line.py
--rw-rw-rw-  2.0 fat     3053 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/offset2d.py
--rw-rw-rw-  2.0 fat     8171 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/parametrize.py
--rw-rw-rw-  2.0 fat    15602 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/perlin.py
--rw-rw-rw-  2.0 fat    15934 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/polyline.py
--rw-rw-rw-  2.0 fat    11703 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/rtree.py
--rw-rw-rw-  2.0 fat     4815 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/shape.py
--rw-rw-rw-  2.0 fat    12135 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/transformtools.py
--rw-rw-rw-  2.0 fat     3539 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/triangulation.py
--rw-rw-rw-  2.0 fat    17116 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/ucs.py
--rw-rw-rw-  2.0 fat     6710 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/_bezier3p.py
--rw-rw-rw-  2.0 fat    11876 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/_bezier4p.py
--rw-rw-rw-  2.0 fat     9440 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/_bspline.py
--rw-rw-rw-  2.0 fat    12477 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/_construct.py
--rw-rw-rw-  2.0 fat     2548 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/_ctypes.py
--rw-rw-rw-  2.0 fat    24812 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/_mapbox_earcut.py
--rw-rw-rw-  2.0 fat    22757 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/_matrix44.py
--rw-rw-rw-  2.0 fat    25882 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/_vector.py
--rw-rw-rw-  2.0 fat     1978 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/math/__init__.py
--rw-rw-rw-  2.0 fat     1306 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/path/commands.py
--rw-rw-rw-  2.0 fat    31293 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/path/converter.py
--rw-rw-rw-  2.0 fat     5868 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/path/nesting.py
--rw-rw-rw-  2.0 fat    18224 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/path/path.py
--rw-rw-rw-  2.0 fat    10129 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/path/shapes.py
--rw-rw-rw-  2.0 fat    34213 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/path/tools.py
--rw-rw-rw-  2.0 fat      385 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/path/__init__.py
--rw-rw-rw-  2.0 fat    10125 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/abstract_mtext_renderer.py
--rw-rw-rw-  2.0 fat    20495 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/arrows.py
--rw-rw-rw-  2.0 fat    17745 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/curves.py
--rw-rw-rw-  2.0 fat     4041 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/dimension.py
--rw-rw-rw-  2.0 fat    51443 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/dim_base.py
--rw-rw-rw-  2.0 fat    35702 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/dim_curved.py
--rw-rw-rw-  2.0 fat     6894 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/dim_diameter.py
--rw-rw-rw-  2.0 fat    24751 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/dim_linear.py
--rw-rw-rw-  2.0 fat     8084 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/dim_ordinate.py
--rw-rw-rw-  2.0 fat    20295 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/dim_radius.py
--rw-rw-rw-  2.0 fat    47170 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/forms.py
--rw-rw-rw-  2.0 fat    25780 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/hatching.py
--rw-rw-rw-  2.0 fat     4728 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/leader.py
--rw-rw-rw-  2.0 fat      664 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/linetypes.py
--rw-rw-rw-  2.0 fat    65258 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/mesh.py
--rw-rw-rw-  2.0 fat    60907 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/mleader.py
--rw-rw-rw-  2.0 fat     8437 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/mline.py
--rw-rw-rw-  2.0 fat     2964 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/point.py
--rw-rw-rw-  2.0 fat     8736 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/polyline.py
--rw-rw-rw-  2.0 fat     7886 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/r12spline.py
--rw-rw-rw-  2.0 fat    22287 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/trace.py
--rw-rw-rw-  2.0 fat     2881 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/_linetypes.py
--rw-rw-rw-  2.0 fat      778 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/render/__init__.py
--rw-rw-rw-  2.0 fat     1050 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/16x16.png
--rw-rw-rw-  2.0 fat     1420 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/24x24.png
--rw-rw-rw-  2.0 fat    10638 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/256x256.png
--rw-rw-rw-  2.0 fat     1758 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/32x32.png
--rw-rw-rw-  2.0 fat     2335 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/48x48.png
--rw-rw-rw-  2.0 fat     3050 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/64x64.png
--rw-rw-rw-  2.0 fat     2090 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/icon-copy-64px.png
--rw-rw-rw-  2.0 fat     3109 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/icon-find-64px.png
--rw-rw-rw-  2.0 fat     2388 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/icon-goto-bookmark-64px.png
--rw-rw-rw-  2.0 fat     2519 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/icon-goto-handle-64px.png
--rw-rw-rw-  2.0 fat     2409 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/icon-goto-line-64px.png
--rw-rw-rw-  2.0 fat     2231 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/icon-left-arrow-64px.png
--rw-rw-rw-  2.0 fat     2322 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/icon-next-entity-64px.png
--rw-rw-rw-  2.0 fat     2320 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/icon-prev-entity-64px.png
--rw-rw-rw-  2.0 fat     2244 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/icon-right-arrow-64px.png
--rw-rw-rw-  2.0 fat     2553 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/icon-show-in-tree-64px.png
--rw-rw-rw-  2.0 fat     2373 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/resources/icon-store-bookmark-64px.png
--rw-rw-rw-  2.0 fat    10650 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/sections/acdsdata.py
--rw-rw-rw-  2.0 fat    17369 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/sections/blocks.py
--rw-rw-rw-  2.0 fat    11639 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/sections/classes.py
--rw-rw-rw-  2.0 fat     4137 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/sections/entities.py
--rw-rw-rw-  2.0 fat    11937 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/sections/header.py
--rw-rw-rw-  2.0 fat    61373 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/sections/headervars.py
--rw-rw-rw-  2.0 fat    27009 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/sections/objects.py
--rw-rw-rw-  2.0 fat    26565 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/sections/table.py
--rw-rw-rw-  2.0 fat     5270 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/sections/tables.py
--rw-rw-rw-  2.0 fat       67 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/sections/__init__.py
--rw-rw-rw-  2.0 fat    19711 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/analyze.py
--rw-rw-rw-  2.0 fat    20440 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/binarydata.py
--rw-rw-rw-  2.0 fat    15737 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/clipping_portal.py
--rw-rw-rw-  2.0 fat     2931 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/codepage.py
--rw-rw-rw-  2.0 fat     7613 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/complex_ltype.py
--rw-rw-rw-  2.0 fat     1782 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/crypt.py
--rw-rw-rw-  2.0 fat     1511 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/debug.py
--rw-rw-rw-  2.0 fat     2325 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/difftags.py
--rw-rw-rw-  2.0 fat     1235 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/handle.py
--rw-rw-rw-  2.0 fat      780 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/indexing.py
--rw-rw-rw-  2.0 fat     2145 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/juliandate.py
--rw-rw-rw-  2.0 fat     6166 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/pattern.py
--rw-rw-rw-  2.0 fat     1224 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/rawloader.py
--rw-rw-rw-  2.0 fat   129174 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/standards.py
--rw-rw-rw-  2.0 fat     6187 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/strip.py
--rw-rw-rw-  2.0 fat     1466 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/test.py
--rw-rw-rw-  2.0 fat    66061 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/text.py
--rw-rw-rw-  2.0 fat    54140 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/text_layout.py
--rw-rw-rw-  2.0 fat     6893 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/text_size.py
--rw-rw-rw-  2.0 fat     3116 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/zipmanager.py
--rw-rw-rw-  2.0 fat   142734 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/_iso_pattern.py
--rw-rw-rw-  2.0 fat     4413 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/src/ezdxf/tools/__init__.py
--rw-rw-rw-  2.0 fat        1 b- defN 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat       46 b- defN 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf.egg-info/entry_points.txt
--rw-rw-rw-  2.0 fat        2 b- defN 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf.egg-info/not-zip-safe
--rw-rw-rw-  2.0 fat    10110 b- defN 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat      316 b- defN 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf.egg-info/requires.txt
--rw-rw-rw-  2.0 fat    33328 b- defN 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat        6 b- defN 24-May-28 12:38 ezdxf-1.3.1b0/src/ezdxf.egg-info/top_level.txt
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/test_01_dxf_entities/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/test_05_tools/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/test_06_math/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/test_07_render/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/test_08_addons/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/test_09_cython_acceleration/
-drwxrwxrwx  2.0 fat        0 b- stor 24-May-28 12:38 ezdxf-1.3.1b0/tests/test_10_issues/
--rw-rw-rw-  2.0 fat      410 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/conftest.py
--rw-rw-rw-  2.0 fat     2336 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
--rw-rw-rw-  2.0 fat      780 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
--rw-rw-rw-  2.0 fat     2599 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
--rw-rw-rw-  2.0 fat     1124 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
--rw-rw-rw-  2.0 fat     5667 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
--rw-rw-rw-  2.0 fat      582 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
--rw-rw-rw-  2.0 fat      473 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_011_codepage.py
--rw-rw-rw-  2.0 fat    11593 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_012_crypt.py
--rw-rw-rw-  2.0 fat     1191 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
--rw-rw-rw-  2.0 fat     1033 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
--rw-rw-rw-  2.0 fat     4792 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
--rw-rw-rw-  2.0 fat      989 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_016_encoding.py
--rw-rw-rw-  2.0 fat     1383 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_018_handle.py
--rw-rw-rw-  2.0 fat     5518 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
--rw-rw-rw-  2.0 fat     8688 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
--rw-rw-rw-  2.0 fat     3787 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
--rw-rw-rw-  2.0 fat      401 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
--rw-rw-rw-  2.0 fat      539 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
--rw-rw-rw-  2.0 fat     2092 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
--rw-rw-rw-  2.0 fat    10917 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_040_tags.py
--rw-rw-rw-  2.0 fat     3073 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
--rw-rw-rw-  2.0 fat     6419 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
--rw-rw-rw-  2.0 fat     1632 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
--rw-rw-rw-  2.0 fat    11265 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
--rw-rw-rw-  2.0 fat     3363 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
--rw-rw-rw-  2.0 fat     1974 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
--rw-rw-rw-  2.0 fat     2321 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
--rw-rw-rw-  2.0 fat      568 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
--rw-rw-rw-  2.0 fat     8797 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
--rw-rw-rw-  2.0 fat     2581 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_056_special_string_decoding.py
--rw-rw-rw-  2.0 fat     1500 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
--rw-rw-rw-  2.0 fat     1947 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_058_json_tags.py
--rw-rw-rw-  2.0 fat    11689 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_101_dxfnamespace.py
--rw-rw-rw-  2.0 fat     2893 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_102_appdata.py
--rw-rw-rw-  2.0 fat     2622 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_103_reactors.py
--rw-rw-rw-  2.0 fat     4679 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_104_extension_dict.py
--rw-rw-rw-  2.0 fat    20860 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_105_xdata.py
--rw-rw-rw-  2.0 fat    14169 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_110_dxfentity.py
--rw-rw-rw-  2.0 fat     2433 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
--rw-rw-rw-  2.0 fat     6781 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_112a_dxfgfx.py
--rw-rw-rw-  2.0 fat      695 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_112b_dxfobj.py
--rw-rw-rw-  2.0 fat     2431 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_113_dxfclass.py
--rw-rw-rw-  2.0 fat     4044 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_114_factory.py
--rw-rw-rw-  2.0 fat     2256 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
--rw-rw-rw-  2.0 fat    15794 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_116_dictionary.py
--rw-rw-rw-  2.0 fat     4999 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_117_layer_table_entry.py
--rw-rw-rw-  2.0 fat      385 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_118_appid_table_entry.py
--rw-rw-rw-  2.0 fat     1058 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
--rw-rw-rw-  2.0 fat     3003 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_120_style_table_entry.py
--rw-rw-rw-  2.0 fat     2943 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
--rw-rw-rw-  2.0 fat      379 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_122_vport_table_entry.py
--rw-rw-rw-  2.0 fat     1113 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_123_view_table_entry.py
--rw-rw-rw-  2.0 fat     8757 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
--rw-rw-rw-  2.0 fat     1698 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_125_image_def.py
--rw-rw-rw-  2.0 fat     1312 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_126_image_def_reactor.py
--rw-rw-rw-  2.0 fat     1430 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_127_raster_variables.py
--rw-rw-rw-  2.0 fat     1540 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_128_pdf_definition.py
--rw-rw-rw-  2.0 fat     2778 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_129_xrecord.py
--rw-rw-rw-  2.0 fat     2423 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_130_id_buffer.py
--rw-rw-rw-  2.0 fat     2470 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_131_field_list.py
--rw-rw-rw-  2.0 fat     2435 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_132_layer_filter.py
--rw-rw-rw-  2.0 fat     2153 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_133_sun.py
--rw-rw-rw-  2.0 fat      852 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_134_material.py
--rw-rw-rw-  2.0 fat    11497 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_135_geo_data.py
--rw-rw-rw-  2.0 fat     1087 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_136_vba_project.py
--rw-rw-rw-  2.0 fat     3099 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_137_sortentstable.py
--rw-rw-rw-  2.0 fat      704 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
--rw-rw-rw-  2.0 fat     7570 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_139_user_record.py
--rw-rw-rw-  2.0 fat      714 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_140_block_record.py
--rw-rw-rw-  2.0 fat     9199 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_141_layer_vp_override.py
--rw-rw-rw-  2.0 fat     1876 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_142_copy_strategy.py
--rw-rw-rw-  2.0 fat     2268 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_143_spatial_filter.py
--rw-rw-rw-  2.0 fat     2141 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_144_roundtrip_xrecord.py
--rw-rw-rw-  2.0 fat     2231 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/conftest.py
--rw-rw-rw-  2.0 fat     6532 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_200_line.py
--rw-rw-rw-  2.0 fat     4273 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_201_point.py
--rw-rw-rw-  2.0 fat     6827 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_202_circle.py
--rw-rw-rw-  2.0 fat     8949 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_203_arc.py
--rw-rw-rw-  2.0 fat     2852 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_204_shape.py
--rw-rw-rw-  2.0 fat     8274 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_205_solid.py
--rw-rw-rw-  2.0 fat     8476 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_206_text.py
--rw-rw-rw-  2.0 fat     6487 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_207_attdef.py
--rw-rw-rw-  2.0 fat     8628 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_208_attrib.py
--rw-rw-rw-  2.0 fat     2671 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_209_vertex.py
--rw-rw-rw-  2.0 fat     5916 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_1.py
--rw-rw-rw-  2.0 fat    13489 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_2.py
--rw-rw-rw-  2.0 fat     6650 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_explode.py
--rw-rw-rw-  2.0 fat     1780 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
--rw-rw-rw-  2.0 fat     7847 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_211_viewport.py
--rw-rw-rw-  2.0 fat    12629 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_212_insert.py
--rw-rw-rw-  2.0 fat     6024 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_213_minsert.py
--rw-rw-rw-  2.0 fat     3284 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_214_block.py
--rw-rw-rw-  2.0 fat     6914 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_215_dimension.py
--rw-rw-rw-  2.0 fat     4907 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
--rw-rw-rw-  2.0 fat    13186 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
--rw-rw-rw-  2.0 fat     6471 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
--rw-rw-rw-  2.0 fat     5535 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
--rw-rw-rw-  2.0 fat     3056 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
--rw-rw-rw-  2.0 fat     7345 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
--rw-rw-rw-  2.0 fat     2066 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
--rw-rw-rw-  2.0 fat     3615 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
--rw-rw-rw-  2.0 fat     6919 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_221_ellipse.py
--rw-rw-rw-  2.0 fat     2223 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_222_xline.py
--rw-rw-rw-  2.0 fat     1493 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_223_ray.py
--rw-rw-rw-  2.0 fat     3104 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_224_group.py
--rw-rw-rw-  2.0 fat    10917 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_225_mtext.py
--rw-rw-rw-  2.0 fat    12226 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_226_spline.py
--rw-rw-rw-  2.0 fat     5529 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
--rw-rw-rw-  2.0 fat    10893 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
--rw-rw-rw-  2.0 fat    15284 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_228_mesh.py
--rw-rw-rw-  2.0 fat     2695 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
--rw-rw-rw-  2.0 fat    21421 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
--rw-rw-rw-  2.0 fat     6587 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
--rw-rw-rw-  2.0 fat     3140 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
--rw-rw-rw-  2.0 fat    12486 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
--rw-rw-rw-  2.0 fat     2274 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_231_underlay.py
--rw-rw-rw-  2.0 fat     5243 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_231_underlay_2.py
--rw-rw-rw-  2.0 fat     2294 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232a_add_acis.py
--rw-rw-rw-  2.0 fat     7614 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232b_acis_export.py
--rw-rw-rw-  2.0 fat     1854 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232c_acis_surface.py
--rw-rw-rw-  2.0 fat     4215 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232d_acis_copy.py
--rw-rw-rw-  2.0 fat     1936 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232e_acis_transform.py
--rw-rw-rw-  2.0 fat     2695 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_233_helix.py
--rw-rw-rw-  2.0 fat     2040 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_234_light.py
--rw-rw-rw-  2.0 fat     3806 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_235_leader.py
--rw-rw-rw-  2.0 fat    20392 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_236_multileader.py
--rw-rw-rw-  2.0 fat    10992 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_237_mline.py
--rw-rw-rw-  2.0 fat     2356 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_238_tolerance.py
--rw-rw-rw-  2.0 fat    27392 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
--rw-rw-rw-  2.0 fat     4347 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_240_arc_dimension.py
--rw-rw-rw-  2.0 fat     1069 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_241_hyperlink.py
--rw-rw-rw-  2.0 fat    11333 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_242_random_transform.py
--rw-rw-rw-  2.0 fat     3725 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_243_replace_entity.py
--rw-rw-rw-  2.0 fat     1445 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
--rw-rw-rw-  2.0 fat     4456 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_245_wipeout.py
--rw-rw-rw-  2.0 fat     6175 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_246_spline_audit.py
--rw-rw-rw-  2.0 fat     8165 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
--rw-rw-rw-  2.0 fat     6003 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_248_mpolygon.py
--rw-rw-rw-  2.0 fat    13682 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
--rw-rw-rw-  2.0 fat     7274 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_249_boundary_paths.py
--rw-rw-rw-  2.0 fat     8331 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
--rw-rw-rw-  2.0 fat     7331 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_251_upright.py
--rw-rw-rw-  2.0 fat     4850 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
--rw-rw-rw-  2.0 fat     2082 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_253_ole2frame.py
--rw-rw-rw-  2.0 fat     1039 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_254_get_font_name.py
--rw-rw-rw-  2.0 fat     5149 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_300_layout.py
--rw-rw-rw-  2.0 fat     4274 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
--rw-rw-rw-  2.0 fat     5582 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_302_block_references.py
--rw-rw-rw-  2.0 fat     2695 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_303_auto_block_references.py
--rw-rw-rw-  2.0 fat      913 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_304_new_entity_space.py
--rw-rw-rw-  2.0 fat     3279 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
--rw-rw-rw-  2.0 fat     2609 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
--rw-rw-rw-  2.0 fat     2343 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_307_groupby.py
--rw-rw-rw-  2.0 fat    17748 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_308_query.py
--rw-rw-rw-  2.0 fat     6382 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_309_query_parser.py
--rw-rw-rw-  2.0 fat     5031 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
--rw-rw-rw-  2.0 fat     5782 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_312_virtual_layout.py
--rw-rw-rw-  2.0 fat      647 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_313_redraw_order.py
--rw-rw-rw-  2.0 fat     6128 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_401_headersection.py
--rw-rw-rw-  2.0 fat     2750 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_402_classessection.py
--rw-rw-rw-  2.0 fat     5208 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
--rw-rw-rw-  2.0 fat     6795 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_404a_tables.py
--rw-rw-rw-  2.0 fat     4981 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
--rw-rw-rw-  2.0 fat     2450 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_405_classes.py
--rw-rw-rw-  2.0 fat     9094 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
--rw-rw-rw-  2.0 fat      848 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
--rw-rw-rw-  2.0 fat     3375 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
--rw-rw-rw-  2.0 fat     1433 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
--rw-rw-rw-  2.0 fat     5736 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_410_table.py
--rw-rw-rw-  2.0 fat     6607 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
--rw-rw-rw-  2.0 fat     1058 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
--rw-rw-rw-  2.0 fat     2340 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
--rw-rw-rw-  2.0 fat    18072 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
--rw-rw-rw-  2.0 fat     4638 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
--rw-rw-rw-  2.0 fat    12327 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
--rw-rw-rw-  2.0 fat     6509 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
--rw-rw-rw-  2.0 fat     5656 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_417_bbox.py
--rw-rw-rw-  2.0 fat     5434 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
--rw-rw-rw-  2.0 fat      733 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
--rw-rw-rw-  2.0 fat     1240 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
--rw-rw-rw-  2.0 fat     5007 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
--rw-rw-rw-  2.0 fat      769 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
--rw-rw-rw-  2.0 fat     8058 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_424_audit.py
--rw-rw-rw-  2.0 fat     3737 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
--rw-rw-rw-  2.0 fat     2981 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
--rw-rw-rw-  2.0 fat     2416 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
--rw-rw-rw-  2.0 fat     2533 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
--rw-rw-rw-  2.0 fat     7813 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_429_xclip.py
--rw-rw-rw-  2.0 fat   112800 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/conftest.py
--rw-rw-rw-  2.0 fat     5510 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_500_units.py
--rw-rw-rw-  2.0 fat     2665 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_501_truecolor.py
--rw-rw-rw-  2.0 fat     1021 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_502_raw_color.py
--rw-rw-rw-  2.0 fat     1695 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_503_indexing.py
--rw-rw-rw-  2.0 fat     1442 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_504_suppress_zeros.py
--rw-rw-rw-  2.0 fat      216 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_506_version.py
--rw-rw-rw-  2.0 fat      657 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_508_read_zip.py
--rw-rw-rw-  2.0 fat     1445 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_509_comments.py
--rw-rw-rw-  2.0 fat     1185 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_510_byte_stream.py
--rw-rw-rw-  2.0 fat     4239 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_511_bit_stream.py
--rw-rw-rw-  2.0 fat     5595 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_512_pattern.py
--rw-rw-rw-  2.0 fat     2372 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_513_reorder_entities.py
--rw-rw-rw-  2.0 fat    18181 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_514_text.py
--rw-rw-rw-  2.0 fat     9361 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_515a_fonts_truetype.py
--rw-rw-rw-  2.0 fat     4752 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_515b_fonts_shapefiles.py
--rw-rw-rw-  2.0 fat     2469 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_515c_fonts_lff.py
--rw-rw-rw-  2.0 fat     4002 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_516_zoom.py
--rw-rw-rw-  2.0 fat    34209 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_517_text_layout.py
--rw-rw-rw-  2.0 fat      474 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_518_header_guid.py
--rw-rw-rw-  2.0 fat     3716 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_519_mtext_editor.py
--rw-rw-rw-  2.0 fat     3205 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_520_mtext_context.py
--rw-rw-rw-  2.0 fat    24496 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_521_mtext_parser.py
--rw-rw-rw-  2.0 fat     3863 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_522_text_scanner.py
--rw-rw-rw-  2.0 fat     5564 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_523_text_size.py
--rw-rw-rw-  2.0 fat     5063 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_524_block_reference_manager.py
--rw-rw-rw-  2.0 fat      773 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_525_transparency.py
--rw-rw-rw-  2.0 fat     2133 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_526_explode.py
--rw-rw-rw-  2.0 fat    13521 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_527_gfxattribs.py
--rw-rw-rw-  2.0 fat     2748 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_528_difftags.py
--rw-rw-rw-  2.0 fat     6700 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_529_acis_sat.py
--rw-rw-rw-  2.0 fat     2062 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_530_acis_sab.py
--rw-rw-rw-  2.0 fat    12357 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_531_acis_entities.py
--rw-rw-rw-  2.0 fat     7858 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_532_acis_mesh.py
--rw-rw-rw-  2.0 fat    43259 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_533_shapefiles.py
--rw-rw-rw-  2.0 fat     1034 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_534_dwg_info.py
--rw-rw-rw-  2.0 fat    48174 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_535_xref_basic.py
--rw-rw-rw-  2.0 fat    27614 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_536_xref_conflict.py
--rw-rw-rw-  2.0 fat     7186 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_537_transform.py
--rw-rw-rw-  2.0 fat     2246 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
--rw-rw-rw-  2.0 fat    17771 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_539_npshapes.py
--rw-rw-rw-  2.0 fat     2605 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_540_lff_parser.py
--rw-rw-rw-  2.0 fat     1206 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_541_clipping_portal.py
--rw-rw-rw-  2.0 fat     1400 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_542_itertools.py
--rw-rw-rw-  2.0 fat    11705 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_543_select.py
--rw-rw-rw-  2.0 fat     1264 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_544_revcloud.py
--rw-rw-rw-  2.0 fat     2567 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_545_acis_cache.py
--rw-rw-rw-  2.0 fat    13061 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_546_edgeminer.py
--rw-rw-rw-  2.0 fat     3413 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_05_tools/test_547_edgesmith.py
--rw-rw-rw-  2.0 fat     4026 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/conftest.py
--rw-rw-rw-  2.0 fat     7503 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_600_base.py
--rw-rw-rw-  2.0 fat     2098 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_601_bulge.py
--rw-rw-rw-  2.0 fat    14661 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_602_vec3.py
--rw-rw-rw-  2.0 fat     8956 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_603_vec2.py
--rw-rw-rw-  2.0 fat     2829 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_604_banded_matrix.py
--rw-rw-rw-  2.0 fat     9709 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_604_linalg.py
--rw-rw-rw-  2.0 fat    14118 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_605_matrix44.py
--rw-rw-rw-  2.0 fat     5888 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_606_convexhull.py
--rw-rw-rw-  2.0 fat     1010 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_607_perlin_noise.py
--rw-rw-rw-  2.0 fat     3833 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_608_intersection_line_line_2d.py
--rw-rw-rw-  2.0 fat     1676 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_609_point_on_line.py
--rw-rw-rw-  2.0 fat     3171 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_610_ocs.py
--rw-rw-rw-  2.0 fat     7529 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_611_ucs.py
--rw-rw-rw-  2.0 fat     1831 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_612_ucs_pass_trough.py
--rw-rw-rw-  2.0 fat     6332 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_613_is_point_in_polygon_2d.py
--rw-rw-rw-  2.0 fat    10913 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_614_construct_3d.py
--rw-rw-rw-  2.0 fat      602 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_615_rytz_axis.py
--rw-rw-rw-  2.0 fat     5215 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_616_plane.py
--rw-rw-rw-  2.0 fat      772 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_617_clockwise_orientation.py
--rw-rw-rw-  2.0 fat     7712 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_618_clipping.py
--rw-rw-rw-  2.0 fat    10108 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_619_greiner_hormann.py
--rw-rw-rw-  2.0 fat     2669 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_620_knot.py
--rw-rw-rw-  2.0 fat    18834 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_621_bspline.py
--rw-rw-rw-  2.0 fat     7652 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_622_bsplineu.py
--rw-rw-rw-  2.0 fat    11314 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_623_rbspline.py
--rw-rw-rw-  2.0 fat    10869 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_624_global_bspline_interpolation.py
--rw-rw-rw-  2.0 fat     1247 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_626_local_bspline_interpolation.py
--rw-rw-rw-  2.0 fat     1967 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_627_bspline_basis.py
--rw-rw-rw-  2.0 fat    10545 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_629_bezier.py
--rw-rw-rw-  2.0 fat    10900 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_630a_bezier4p_base.py
--rw-rw-rw-  2.0 fat    10354 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_630b_bezier4p_functions.py
--rw-rw-rw-  2.0 fat     1683 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_631_euler_spiral.py
--rw-rw-rw-  2.0 fat     4054 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_632_bezier3p.py
--rw-rw-rw-  2.0 fat    20154 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_640_bbox.py
--rw-rw-rw-  2.0 fat     5393 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_641_construction_ray.py
--rw-rw-rw-  2.0 fat     3673 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_642_construction_line.py
--rw-rw-rw-  2.0 fat     9459 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_643_construction_box.py
--rw-rw-rw-  2.0 fat    11561 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_644_construction_circle.py
--rw-rw-rw-  2.0 fat    10988 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_645_construction_arc.py
--rw-rw-rw-  2.0 fat     3422 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_646_offset_vertices_2d.py
--rw-rw-rw-  2.0 fat     7672 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_647_transform_tools.py
--rw-rw-rw-  2.0 fat     9001 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_648_construction_ellipse.py
--rw-rw-rw-  2.0 fat     4243 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_650_elliptic_arc_span.py
--rw-rw-rw-  2.0 fat     9024 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_651_construction_polyline.py
--rw-rw-rw-  2.0 fat     3212 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_652_approx_param_t.py
--rw-rw-rw-  2.0 fat     5806 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_653_polyline_intersection.py
--rw-rw-rw-  2.0 fat     5193 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_654_rtree.py
--rw-rw-rw-  2.0 fat      788 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_655_dbscan.py
--rw-rw-rw-  2.0 fat      834 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_656_k_means.py
--rw-rw-rw-  2.0 fat     4654 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_657_mapbox_earcut.py
--rw-rw-rw-  2.0 fat    11654 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_658_bevel_tools.py
--rw-rw-rw-  2.0 fat     1875 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_659_intersection_line_polygon_3d.py
--rw-rw-rw-  2.0 fat     1428 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
--rw-rw-rw-  2.0 fat     1741 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
--rw-rw-rw-  2.0 fat     3307 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_662_is_convex_polygon_2d.py
--rw-rw-rw-  2.0 fat     1266 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_663_is_axes_aligned_rectange.py
--rw-rw-rw-  2.0 fat    17333 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_664_concave_clipping_polygon.py
--rw-rw-rw-  2.0 fat     7980 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_665_inverted_clipping_polygon.py
--rw-rw-rw-  2.0 fat     1553 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_06_math/test_666_wgs84_transform.py
--rw-rw-rw-  2.0 fat     1466 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_701_arrows.py
--rw-rw-rw-  2.0 fat    17245 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_702_render_forms.py
--rw-rw-rw-  2.0 fat    34554 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_703_mesh_builder.py
--rw-rw-rw-  2.0 fat     4459 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_704_render_linear_dimension.py
--rw-rw-rw-  2.0 fat     1345 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_705_shape.py
--rw-rw-rw-  2.0 fat      483 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_706_random_path.py
--rw-rw-rw-  2.0 fat     5603 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_707_trace.py
--rw-rw-rw-  2.0 fat    34121 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_708a_path.py
--rw-rw-rw-  2.0 fat    27365 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_708b_path_tools.py
--rw-rw-rw-  2.0 fat     3352 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_708c_matplotlib_path_tools.py
--rw-rw-rw-  2.0 fat     3278 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_708d_qpainter_path_tools.py
--rw-rw-rw-  2.0 fat     4589 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_708e_path_shapes.py
--rw-rw-rw-  2.0 fat     4121 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_708f_path_nesting.py
--rw-rw-rw-  2.0 fat     1308 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_709_linetype_renderer.py
--rw-rw-rw-  2.0 fat     2815 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_711_points.py
--rw-rw-rw-  2.0 fat     6594 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_712_render_curved_dimension.py
--rw-rw-rw-  2.0 fat     1472 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_713_mleader_builder.py
--rw-rw-rw-  2.0 fat     1091 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_714_mleader_render_engine.py
--rw-rw-rw-  2.0 fat    11887 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_715_hatching.py
--rw-rw-rw-  2.0 fat     2626 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
--rw-rw-rw-  2.0 fat     4771 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_800_mtext_surrogate.py
--rw-rw-rw-  2.0 fat     1352 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_801_r12spline.py
--rw-rw-rw-  2.0 fat     7881 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_802_table_painter.py
--rw-rw-rw-  2.0 fat    13038 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_803_entities_to_code.py
--rw-rw-rw-  2.0 fat     6844 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_804_importer.py
--rw-rw-rw-  2.0 fat     2362 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_805_pycsg.py
--rw-rw-rw-  2.0 fat    16011 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_806_acadctb.py
--rw-rw-rw-  2.0 fat     4860 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_807_dwg_loader_basics.py
--rw-rw-rw-  2.0 fat    11204 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_810_drawing_properties.py
--rw-rw-rw-  2.0 fat    12549 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_811a_drawing_frontend.py
--rw-rw-rw-  2.0 fat     9101 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_811b_drawing_recorder.py
--rw-rw-rw-  2.0 fat     2898 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_811c_viewport_processing.py
--rw-rw-rw-  2.0 fat     4229 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_812_drawing_graphic_proxy.py
--rw-rw-rw-  2.0 fat    13751 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_813_geo_interface.py
--rw-rw-rw-  2.0 fat    14853 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_814_text2path.py
--rw-rw-rw-  2.0 fat    16239 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_815_dxf_browser.py
--rw-rw-rw-  2.0 fat    11275 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_816_bin_packing.py
--rw-rw-rw-  2.0 fat    12554 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_817_genetic_algorithm.py
--rw-rw-rw-  2.0 fat     9008 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_818_meshex.py
--rw-rw-rw-  2.0 fat     1003 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_819_menger_sponge.py
--rw-rw-rw-  2.0 fat     4433 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_820_openscad.py
--rw-rw-rw-  2.0 fat    15655 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_821_hpgl2.py
--rw-rw-rw-  2.0 fat     1376 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
--rw-rw-rw-  2.0 fat     5284 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_823_drawing_layout.py
--rw-rw-rw-  2.0 fat     3312 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_824_svg_drawing_backend.py
--rw-rw-rw-  2.0 fat     2014 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_825_hpgl2_drawing_backend.py
--rw-rw-rw-  2.0 fat     3158 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_826_custom_json_backend.py
--rw-rw-rw-  2.0 fat     3388 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_08_addons/test_827_geojson_backend.py
--rw-rw-rw-  2.0 fat     2527 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_901_acc_vec2.py
--rw-rw-rw-  2.0 fat     2199 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_902_acc_vec3.py
--rw-rw-rw-  2.0 fat     2142 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
--rw-rw-rw-  2.0 fat     3175 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
--rw-rw-rw-  2.0 fat     1463 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
--rw-rw-rw-  2.0 fat     4773 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_906_acc_bspline.py
--rw-rw-rw-  2.0 fat     1666 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_10_issues/test_issue_1078_bbox_calculation.py
--rw-rw-rw-  2.0 fat     2656 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_10_issues/test_issue_414_bbox_calculation.py
--rw-rw-rw-  2.0 fat     1213 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
--rw-rw-rw-  2.0 fat     2268 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_10_issues/test_issue_574_flattening_error.py
--rw-rw-rw-  2.0 fat     1754 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
--rw-rw-rw-  2.0 fat      682 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_10_issues/test_issue_749_text_layout.py
--rw-rw-rw-  2.0 fat    11094 b- defN 24-May-28 12:37 ezdxf-1.3.1b0/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
-868 files, 8966146 bytes uncompressed, 2053454 bytes compressed:  77.1%
+Zip file size: 2214246 bytes, number of entries: 868
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/integration_tests/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/src/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/tests/
+-rw-rw-rw-  2.0 fat     1092 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/LICENSE
+-rw-rw-rw-  2.0 fat      329 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/MANIFEST.in
+-rw-rw-rw-  2.0 fat    10110 b- defN 24-Jun-01 13:14 ezdxf-1.3.1b1/PKG-INFO
+-rw-rw-rw-  2.0 fat     2527 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/pyproject.toml
+-rw-rw-rw-  2.0 fat     7479 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/README.md
+-rw-rw-rw-  2.0 fat       74 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/requirements.txt
+-rw-rw-rw-  2.0 fat       42 b- defN 24-Jun-01 13:14 ezdxf-1.3.1b1/setup.cfg
+-rw-rw-rw-  2.0 fat     2140 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/setup.py
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/integration_tests/data/
+-rw-rw-rw-  2.0 fat      567 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/check_disable_c_ext_by_config_file.py
+-rw-rw-rw-  2.0 fat      541 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/check_disable_c_ext_by_env_var.py
+-rw-rw-rw-  2.0 fat      410 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/conftest.py
+-rw-rw-rw-  2.0 fat     1054 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_acad_table.py
+-rw-rw-rw-  2.0 fat     1339 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_acis_entites.py
+-rw-rw-rw-  2.0 fat     4686 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_all_dimline_styles.py
+-rw-rw-rw-  2.0 fat     4153 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_all_ellipse_transformations.py
+-rw-rw-rw-  2.0 fat     1064 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_anonymous_blocks.py
+-rw-rw-rw-  2.0 fat      577 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_appsettings.py
+-rw-rw-rw-  2.0 fat      871 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_audit_critical_dxf_files.py
+-rw-rw-rw-  2.0 fat     1603 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_audit_layouts.py
+-rw-rw-rw-  2.0 fat     1726 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_complex_line_type_2.py
+-rw-rw-rw-  2.0 fat     1003 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_create_basic_graphics.py
+-rw-rw-rw-  2.0 fat     1921 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_document_guid.py
+-rw-rw-rw-  2.0 fat     1832 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_document_page_setup.py
+-rw-rw-rw-  2.0 fat      998 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_dxf_info_scanning.py
+-rw-rw-rw-  2.0 fat     1299 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_dynblkhelper.py
+-rw-rw-rw-  2.0 fat     1558 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_entities_iterator.py
+-rw-rw-rw-  2.0 fat      934 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_fix_dulicate_handles.py
+-rw-rw-rw-  2.0 fat     1901 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_geo.py
+-rw-rw-rw-  2.0 fat     1250 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_groups.py
+-rw-rw-rw-  2.0 fat      905 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_hpgl2_addon.py
+-rw-rw-rw-  2.0 fat      630 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_ignore_junk_beyond_EOF.py
+-rw-rw-rw-  2.0 fat     1155 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_launcher.py
+-rw-rw-rw-  2.0 fat      631 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_leica_disto_r12.py
+-rw-rw-rw-  2.0 fat      737 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_load_dxf_unicode_notation.py
+-rw-rw-rw-  2.0 fat     2931 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat     2230 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_mtext_columns.py
+-rw-rw-rw-  2.0 fat     2392 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_mtext_explode_addon.py
+-rw-rw-rw-  2.0 fat     1846 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_mtext_text_frame.py
+-rw-rw-rw-  2.0 fat     1053 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_new_table_entries.py
+-rw-rw-rw-  2.0 fat      887 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_none_ascii_read_write.py
+-rw-rw-rw-  2.0 fat     3435 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_odafc.py
+-rw-rw-rw-  2.0 fat     1737 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_open_binary_DXF_files.py
+-rw-rw-rw-  2.0 fat      751 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_open_coord_order_issue.py
+-rw-rw-rw-  2.0 fat     3842 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_open_exotic_dxf_files.py
+-rw-rw-rw-  2.0 fat      879 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_open_R13_R14.py
+-rw-rw-rw-  2.0 fat     3152 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_polyline_entity.py
+-rw-rw-rw-  2.0 fat     1749 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_preserve_binary_data_in_xrecords.py
+-rw-rw-rw-  2.0 fat     6944 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_r12export.py
+-rw-rw-rw-  2.0 fat     6256 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_r12strict.py
+-rw-rw-rw-  2.0 fat     3410 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_r12writer.py
+-rw-rw-rw-  2.0 fat      567 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_read_file_without_handles.py
+-rw-rw-rw-  2.0 fat     1121 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_read_write_modern_entites.py
+-rw-rw-rw-  2.0 fat     7747 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_recover.py
+-rw-rw-rw-  2.0 fat     1959 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_redraw_order.py
+-rw-rw-rw-  2.0 fat     1819 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_rotated_block_attributes.py
+-rw-rw-rw-  2.0 fat      774 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_surface_entities.py
+-rw-rw-rw-  2.0 fat      928 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_write_fixed_meta_data.py
+-rw-rw-rw-  2.0 fat     1806 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_write_without_handles.py
+-rw-rw-rw-  2.0 fat     3638 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_xref_detach.py
+-rw-rw-rw-  2.0 fat     2347 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/test_xref_load_acis.py
+-rw-rw-rw-  2.0 fat     3060 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/AC1003_LINE_Example.dxf
+-rw-rw-rw-  2.0 fat   179505 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/acad_table_with_blk_ref.dxf
+-rw-rw-rw-  2.0 fat     7956 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/ASCII_R12.dxf
+-rw-rw-rw-  2.0 fat     3761 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/bin_dxf_r12.dxf
+-rw-rw-rw-  2.0 fat    20914 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/bin_dxf_r13.dxf
+-rw-rw-rw-  2.0 fat    21137 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/bin_dxf_r14.dxf
+-rw-rw-rw-  2.0 fat    11564 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/bin_dxf_r2000.dxf
+-rw-rw-rw-  2.0 fat     6424 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/cc_dxflib.dxf
+-rw-rw-rw-  2.0 fat   173753 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/custom_blocks.dxf
+-rw-rw-rw-  2.0 fat    32203 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/duplicate_handles.dxf
+-rw-rw-rw-  2.0 fat    18554 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/dxf_unicode.dxf
+-rw-rw-rw-  2.0 fat    56494 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/dynblks.zip
+-rw-rw-rw-  2.0 fat     1592 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/empty_handles.dxf
+-rw-rw-rw-  2.0 fat    97103 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/groups.dxf
+-rw-rw-rw-  2.0 fat    19533 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/layout_broken_links.dxf
+-rw-rw-rw-  2.0 fat    19506 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/layout_broken_links_2.dxf
+-rw-rw-rw-  2.0 fat    19291 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/layout_missing_block_definition.dxf
+-rw-rw-rw-  2.0 fat    19383 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/layout_missing_block_record.dxf
+-rw-rw-rw-  2.0 fat     9146 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/Leica_Disto_S910.dxf
+-rw-rw-rw-  2.0 fat    17986 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/MODEL.dxf
+-rw-rw-rw-  2.0 fat    25799 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/mtext_columns_R2007.dxf
+-rw-rw-rw-  2.0 fat    23927 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/mtext_columns_R2018.dxf
+-rw-rw-rw-  2.0 fat    98230 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/mtext_framed_columns.dxf
+-rw-rw-rw-  2.0 fat   106574 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/mtext_text_frame.dxf
+-rw-rw-rw-  2.0 fat    12001 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/no_layouts.dxf
+-rw-rw-rw-  2.0 fat    16295 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/PLOTFILE.plt
+-rw-rw-rw-  2.0 fat    28788 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/POLI-ALL210_12.DXF
+-rw-rw-rw-  2.0 fat      144 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/R12_with_trash_beyond_EOF.dxf
+-rw-rw-rw-  2.0 fat   212407 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/recover01.dxf
+-rw-rw-rw-  2.0 fat   115423 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/recover02.dxf
+-rw-rw-rw-  2.0 fat    21178 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/small_r13.dxf
+-rw-rw-rw-  2.0 fat    10326 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/small_r14.dxf
+-rw-rw-rw-  2.0 fat    11286 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/XRECORD_0.bin
+-rw-rw-rw-  2.0 fat    11662 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/XRECORD_1.bin
+-rw-rw-rw-  2.0 fat    15337 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/integration_tests/data/XRECORD_2.bin
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf.egg-info/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf/acc/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf/acis/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf/addons/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf/entities/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf/fonts/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf/layouts/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf/lldxf/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf/math/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf/path/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf/render/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf/resources/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf/sections/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf/tools/
+-rw-rw-rw-  2.0 fat     4841 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/appsettings.py
+-rw-rw-rw-  2.0 fat    19976 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/audit.py
+-rw-rw-rw-  2.0 fat     5324 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/bbox.py
+-rw-rw-rw-  2.0 fat     7872 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/blkrefs.py
+-rw-rw-rw-  2.0 fat    17062 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/colors.py
+-rw-rw-rw-  2.0 fat    33508 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/commands.py
+-rw-rw-rw-  2.0 fat     1549 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/comments.py
+-rw-rw-rw-  2.0 fat    22334 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/disassemble.py
+-rw-rw-rw-  2.0 fat    55248 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/document.py
+-rw-rw-rw-  2.0 fat      832 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/dwginfo.py
+-rw-rw-rw-  2.0 fat     2475 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/dynblkhelper.py
+-rw-rw-rw-  2.0 fat    31758 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/edgeminer.py
+-rw-rw-rw-  2.0 fat     8158 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/edgesmith.py
+-rw-rw-rw-  2.0 fat    16254 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entitydb.py
+-rw-rw-rw-  2.0 fat     7495 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/enums.py
+-rw-rw-rw-  2.0 fat    14519 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/explode.py
+-rw-rw-rw-  2.0 fat     1653 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/eztypes.py
+-rw-rw-rw-  2.0 fat    10366 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/filemanagement.py
+-rw-rw-rw-  2.0 fat    12157 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/gfxattribs.py
+-rw-rw-rw-  2.0 fat   107519 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/graphicsfactory.py
+-rw-rw-rw-  2.0 fat     3416 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/groupby.py
+-rw-rw-rw-  2.0 fat      658 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/messenger.py
+-rw-rw-rw-  2.0 fat      272 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/msgtypes.py
+-rw-rw-rw-  2.0 fat    20554 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/npshapes.py
+-rw-rw-rw-  2.0 fat     3030 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/protocols.py
+-rw-rw-rw-  2.0 fat    35308 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/proxygraphic.py
+-rw-rw-rw-  2.0 fat       95 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/py.typed
+-rw-rw-rw-  2.0 fat    22499 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/query.py
+-rw-rw-rw-  2.0 fat     2780 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/queryparser.py
+-rw-rw-rw-  2.0 fat     9564 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/r12strict.py
+-rw-rw-rw-  2.0 fat    31442 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/recover.py
+-rw-rw-rw-  2.0 fat     3515 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/reorder.py
+-rw-rw-rw-  2.0 fat     3926 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/revcloud.py
+-rw-rw-rw-  2.0 fat    11250 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/select.py
+-rw-rw-rw-  2.0 fat    12848 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/transform.py
+-rw-rw-rw-  2.0 fat     5750 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/units.py
+-rw-rw-rw-  2.0 fat     8280 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/upright.py
+-rw-rw-rw-  2.0 fat     9875 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/urecord.py
+-rw-rw-rw-  2.0 fat     1024 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/version.py
+-rw-rw-rw-  2.0 fat    18280 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/xclip.py
+-rw-rw-rw-  2.0 fat    65739 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/xref.py
+-rw-rw-rw-  2.0 fat     2853 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/zoom.py
+-rw-rw-rw-  2.0 fat    10898 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/_options.py
+-rw-rw-rw-  2.0 fat     3138 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/__init__.py
+-rw-rw-rw-  2.0 fat     3259 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/__main__.py
+-rw-rw-rw-  2.0 fat     6788 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acc/bezier3p.pyx
+-rw-rw-rw-  2.0 fat    11502 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acc/bezier4p.pyx
+-rw-rw-rw-  2.0 fat    14048 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acc/bspline.pyx
+-rw-rw-rw-  2.0 fat      252 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acc/constants.h
+-rw-rw-rw-  2.0 fat    11844 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acc/construct.pyx
+-rw-rw-rw-  2.0 fat     3161 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acc/linetypes.pyx
+-rw-rw-rw-  2.0 fat    23976 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acc/mapbox_earcut.pyx
+-rw-rw-rw-  2.0 fat      385 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acc/matrix44.pxd
+-rw-rw-rw-  2.0 fat    23703 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acc/matrix44.pyx
+-rw-rw-rw-  2.0 fat     4705 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acc/np_support.pyx
+-rw-rw-rw-  2.0 fat     1719 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acc/vector.pxd
+-rw-rw-rw-  2.0 fat    23377 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acc/vector.pyx
+-rw-rw-rw-  2.0 fat     1265 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acc/__init__.py
+-rw-rw-rw-  2.0 fat     6398 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acis/abstract.py
+-rw-rw-rw-  2.0 fat      938 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acis/api.py
+-rw-rw-rw-  2.0 fat     1792 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acis/cache.py
+-rw-rw-rw-  2.0 fat     5489 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acis/const.py
+-rw-rw-rw-  2.0 fat     6731 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acis/dbg.py
+-rw-rw-rw-  2.0 fat     2985 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acis/dxf.py
+-rw-rw-rw-  2.0 fat    28750 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acis/entities.py
+-rw-rw-rw-  2.0 fat     4093 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acis/hdr.py
+-rw-rw-rw-  2.0 fat    15566 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acis/mesh.py
+-rw-rw-rw-  2.0 fat    18695 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acis/sab.py
+-rw-rw-rw-  2.0 fat    13189 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acis/sat.py
+-rw-rw-rw-  2.0 fat      247 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acis/type_hints.py
+-rw-rw-rw-  2.0 fat      120 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/acis/__init__.py
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf/addons/acisbrowser/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf/addons/browser/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf/addons/dwg/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/
+-rw-rw-rw-  2.0 fat    26766 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/acadctb.py
+-rw-rw-rw-  2.0 fat    22229 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/binpacking.py
+-rw-rw-rw-  2.0 fat    27692 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/dimlines.py
+-rw-rw-rw-  2.0 fat    31464 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/dxf2code.py
+-rw-rw-rw-  2.0 fat    22005 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/genetic_algorithm.py
+-rw-rw-rw-  2.0 fat    38393 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/geo.py
+-rw-rw-rw-  2.0 fat     2674 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/gerber_D6673.py
+-rw-rw-rw-  2.0 fat    25472 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/importer.py
+-rw-rw-rw-  2.0 fat    17355 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/iterdxf.py
+-rw-rw-rw-  2.0 fat     8946 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/menger_sponge.py
+-rw-rw-rw-  2.0 fat    24787 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/meshex.py
+-rw-rw-rw-  2.0 fat      492 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/mixins.py
+-rw-rw-rw-  2.0 fat     6203 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/mtextsurrogate.py
+-rw-rw-rw-  2.0 fat    13528 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/mtxpl.py
+-rw-rw-rw-  2.0 fat    16364 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/odafc.py
+-rw-rw-rw-  2.0 fat     9456 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/openscad.py
+-rw-rw-rw-  2.0 fat    15878 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/pycsg.py
+-rw-rw-rw-  2.0 fat    22301 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/r12export.py
+-rw-rw-rw-  2.0 fat    27191 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/r12writer.py
+-rw-rw-rw-  2.0 fat     7605 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/sierpinski_pyramid.py
+-rw-rw-rw-  2.0 fat    33167 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/tablepainter.py
+-rw-rw-rw-  2.0 fat    12768 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/text2path.py
+-rw-rw-rw-  2.0 fat     3335 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/xplayer.py
+-rw-rw-rw-  2.0 fat     2312 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/xqt.py
+-rw-rw-rw-  2.0 fat      453 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/__init__.py
+-rw-rw-rw-  2.0 fat     9975 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/acisbrowser/browser.py
+-rw-rw-rw-  2.0 fat     1907 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/acisbrowser/data.py
+-rw-rw-rw-  2.0 fat       64 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/acisbrowser/__init__.py
+-rw-rw-rw-  2.0 fat      820 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/browser/bookmarks.py
+-rw-rw-rw-  2.0 fat    29347 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/browser/browser.py
+-rw-rw-rw-  2.0 fat    14891 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/browser/data.py
+-rw-rw-rw-  2.0 fat    10993 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/browser/find_dialog.py
+-rw-rw-rw-  2.0 fat     1249 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/browser/loader.py
+-rw-rw-rw-  2.0 fat    21111 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/browser/model.py
+-rw-rw-rw-  2.0 fat     6896 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/browser/reflinks.py
+-rw-rw-rw-  2.0 fat     2214 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/browser/tags.py
+-rw-rw-rw-  2.0 fat     1366 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/browser/views.py
+-rw-rw-rw-  2.0 fat      133 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/browser/__init__.py
+-rw-rw-rw-  2.0 fat     9265 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/backend.py
+-rw-rw-rw-  2.0 fat    11113 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/config.py
+-rw-rw-rw-  2.0 fat     1756 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/debug_backend.py
+-rw-rw-rw-  2.0 fat      514 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/debug_utils.py
+-rw-rw-rw-  2.0 fat     7391 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/dxf.py
+-rw-rw-rw-  2.0 fat     7753 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/file_output.py
+-rw-rw-rw-  2.0 fat    44717 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/frontend.py
+-rw-rw-rw-  2.0 fat     1877 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/gfxproxy.py
+-rw-rw-rw-  2.0 fat    20834 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/hpgl2.py
+-rw-rw-rw-  2.0 fat    20101 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/json.py
+-rw-rw-rw-  2.0 fat    18871 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/layout.py
+-rw-rw-rw-  2.0 fat    13209 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/matplotlib.py
+-rw-rw-rw-  2.0 fat     9862 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/mtext_complex.py
+-rw-rw-rw-  2.0 fat    32445 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/pipeline.py
+-rw-rw-rw-  2.0 fat    40194 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/properties.py
+-rw-rw-rw-  2.0 fat    18036 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/pymupdf.py
+-rw-rw-rw-  2.0 fat    11577 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/pyqt.py
+-rw-rw-rw-  2.0 fat    22713 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/qtviewer.py
+-rw-rw-rw-  2.0 fat    16434 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/recorder.py
+-rw-rw-rw-  2.0 fat    16222 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/svg.py
+-rw-rw-rw-  2.0 fat    13023 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/text.py
+-rw-rw-rw-  2.0 fat     1194 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/text_renderer.py
+-rw-rw-rw-  2.0 fat      314 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/type_hints.py
+-rw-rw-rw-  2.0 fat     2559 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/unified_text_renderer.py
+-rw-rw-rw-  2.0 fat      171 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/drawing/__init__.py
+-rw-rw-rw-  2.0 fat     3112 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/dwg/classes_section.py
+-rw-rw-rw-  2.0 fat      763 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/dwg/const.py
+-rw-rw-rw-  2.0 fat     6091 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/dwg/crc.py
+-rw-rw-rw-  2.0 fat     3160 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/dwg/fileheader.py
+-rw-rw-rw-  2.0 fat    14851 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/dwg/header_section.py
+-rw-rw-rw-  2.0 fat     2976 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/dwg/loader.py
+-rw-rw-rw-  2.0 fat      141 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/dwg/__init__.py
+-rw-rw-rw-  2.0 fat    13443 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/api.py
+-rw-rw-rw-  2.0 fat     8554 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/backend.py
+-rw-rw-rw-  2.0 fat      561 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/deps.py
+-rw-rw-rw-  2.0 fat    16079 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/interpreter.py
+-rw-rw-rw-  2.0 fat     4836 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/page.py
+-rw-rw-rw-  2.0 fat    11766 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/plotter.py
+-rw-rw-rw-  2.0 fat     1698 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/polygon_buffer.py
+-rw-rw-rw-  2.0 fat     5615 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/properties.py
+-rw-rw-rw-  2.0 fat     6222 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/tokenizer.py
+-rw-rw-rw-  2.0 fat    19435 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/viewer.py
+-rw-rw-rw-  2.0 fat      164 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/__init__.py
+-rw-rw-rw-  2.0 fat     5710 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/acad_proxy_entity.py
+-rw-rw-rw-  2.0 fat    21579 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/acad_table.py
+-rw-rw-rw-  2.0 fat     2850 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/acad_xrec_roundtrip.py
+-rw-rw-rw-  2.0 fat    30267 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/acis.py
+-rw-rw-rw-  2.0 fat     4996 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/appdata.py
+-rw-rw-rw-  2.0 fat     1954 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/appid.py
+-rw-rw-rw-  2.0 fat     4942 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/arc.py
+-rw-rw-rw-  2.0 fat    27092 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/attrib.py
+-rw-rw-rw-  2.0 fat     8881 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/block.py
+-rw-rw-rw-  2.0 fat    10586 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/blockrecord.py
+-rw-rw-rw-  2.0 fat    51025 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/boundary_paths.py
+-rw-rw-rw-  2.0 fat     7929 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/circle.py
+-rw-rw-rw-  2.0 fat     3214 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/copy.py
+-rw-rw-rw-  2.0 fat    24981 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/dictionary.py
+-rw-rw-rw-  2.0 fat    48717 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/dimension.py
+-rw-rw-rw-  2.0 fat    35043 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/dimstyle.py
+-rw-rw-rw-  2.0 fat    23813 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/dimstyleoverride.py
+-rw-rw-rw-  2.0 fat     4399 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/dxfclass.py
+-rw-rw-rw-  2.0 fat    40587 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/dxfentity.py
+-rw-rw-rw-  2.0 fat    27114 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/dxfgfx.py
+-rw-rw-rw-  2.0 fat    16471 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/dxfgroups.py
+-rw-rw-rw-  2.0 fat    23679 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/dxfns.py
+-rw-rw-rw-  2.0 fat    13910 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/dxfobj.py
+-rw-rw-rw-  2.0 fat    11186 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/ellipse.py
+-rw-rw-rw-  2.0 fat     4138 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/factory.py
+-rw-rw-rw-  2.0 fat    23747 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/geodata.py
+-rw-rw-rw-  2.0 fat     4026 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/gradient.py
+-rw-rw-rw-  2.0 fat    12263 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/hatch.py
+-rw-rw-rw-  2.0 fat     3944 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/helix.py
+-rw-rw-rw-  2.0 fat     4838 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/idbuffer.py
+-rw-rw-rw-  2.0 fat    27125 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/image.py
+-rw-rw-rw-  2.0 fat    28148 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/insert.py
+-rw-rw-rw-  2.0 fat    28698 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/layer.py
+-rw-rw-rw-  2.0 fat    14358 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/layout.py
+-rw-rw-rw-  2.0 fat    13070 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/leader.py
+-rw-rw-rw-  2.0 fat     4718 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/light.py
+-rw-rw-rw-  2.0 fat     3718 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/line.py
+-rw-rw-rw-  2.0 fat     9763 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/ltype.py
+-rw-rw-rw-  2.0 fat    19055 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/lwpolyline.py
+-rw-rw-rw-  2.0 fat    19352 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/material.py
+-rw-rw-rw-  2.0 fat    17444 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/mesh.py
+-rw-rw-rw-  2.0 fat    57437 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/mleader.py
+-rw-rw-rw-  2.0 fat    37229 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/mline.py
+-rw-rw-rw-  2.0 fat     8385 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/mpolygon.py
+-rw-rw-rw-  2.0 fat    48239 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/mtext.py
+-rw-rw-rw-  2.0 fat     4351 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/mtext_columns.py
+-rw-rw-rw-  2.0 fat     6230 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/objectcollection.py
+-rw-rw-rw-  2.0 fat     2151 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/oleframe.py
+-rw-rw-rw-  2.0 fat     4332 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/pattern.py
+-rw-rw-rw-  2.0 fat     5238 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/point.py
+-rw-rw-rw-  2.0 fat    16978 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/polygon.py
+-rw-rw-rw-  2.0 fat    40126 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/polyline.py
+-rw-rw-rw-  2.0 fat     4822 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/shape.py
+-rw-rw-rw-  2.0 fat    10485 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/solid.py
+-rw-rw-rw-  2.0 fat     7990 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/spatial_filter.py
+-rw-rw-rw-  2.0 fat    23810 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/spline.py
+-rw-rw-rw-  2.0 fat     8382 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/subentity.py
+-rw-rw-rw-  2.0 fat     5196 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/sun.py
+-rw-rw-rw-  2.0 fat     2449 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/table.py
+-rw-rw-rw-  2.0 fat     1341 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/temporary_transform.py
+-rw-rw-rw-  2.0 fat    17633 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/text.py
+-rw-rw-rw-  2.0 fat     9053 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/textstyle.py
+-rw-rw-rw-  2.0 fat     3617 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/tolerance.py
+-rw-rw-rw-  2.0 fat     2703 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/ucs.py
+-rw-rw-rw-  2.0 fat    14452 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/underlay.py
+-rw-rw-rw-  2.0 fat     6040 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/view.py
+-rw-rw-rw-  2.0 fat    28360 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/viewport.py
+-rw-rw-rw-  2.0 fat     7958 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/visualstyle.py
+-rw-rw-rw-  2.0 fat     9970 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/vport.py
+-rw-rw-rw-  2.0 fat    17024 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/xdata.py
+-rw-rw-rw-  2.0 fat     8531 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/xdict.py
+-rw-rw-rw-  2.0 fat     3062 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/xline.py
+-rw-rw-rw-  2.0 fat     3191 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/entities/__init__.py
+-rw-rw-rw-  2.0 fat    26337 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/fonts/fonts.py
+-rw-rw-rw-  2.0 fat     2242 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/fonts/font_face.py
+-rw-rw-rw-  2.0 fat    18620 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/fonts/font_manager.py
+-rw-rw-rw-  2.0 fat     1702 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/fonts/font_measurements.py
+-rw-rw-rw-  2.0 fat      288 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/fonts/font_synonyms.py
+-rw-rw-rw-  2.0 fat     1175 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/fonts/glyphs.py
+-rw-rw-rw-  2.0 fat    10763 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/fonts/lff.py
+-rw-rw-rw-  2.0 fat    35414 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/fonts/shapefile.py
+-rw-rw-rw-  2.0 fat     7244 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/fonts/ttfonts.py
+-rw-rw-rw-  2.0 fat       64 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/fonts/__init__.py
+-rw-rw-rw-  2.0 fat    16964 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/layouts/base.py
+-rw-rw-rw-  2.0 fat     4343 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/layouts/blocklayout.py
+-rw-rw-rw-  2.0 fat    32460 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/layouts/layout.py
+-rw-rw-rw-  2.0 fat    15314 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/layouts/layouts.py
+-rw-rw-rw-  2.0 fat      232 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/layouts/__init__.py
+-rw-rw-rw-  2.0 fat     8327 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/lldxf/attributes.py
+-rw-rw-rw-  2.0 fat    16560 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/lldxf/const.py
+-rw-rw-rw-  2.0 fat     2715 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/lldxf/encoding.py
+-rw-rw-rw-  2.0 fat    16997 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/lldxf/extendedtags.py
+-rw-rw-rw-  2.0 fat     5363 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/lldxf/fileindex.py
+-rw-rw-rw-  2.0 fat      727 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/lldxf/hdrvars.py
+-rw-rw-rw-  2.0 fat     5469 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/lldxf/loader.py
+-rw-rw-rw-  2.0 fat     7152 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/lldxf/packedtags.py
+-rw-rw-rw-  2.0 fat     6355 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/lldxf/repair.py
+-rw-rw-rw-  2.0 fat    14509 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/lldxf/tagger.py
+-rw-rw-rw-  2.0 fat    14325 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/lldxf/tags.py
+-rw-rw-rw-  2.0 fat    11054 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/lldxf/tagwriter.py
+-rw-rw-rw-  2.0 fat    12000 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/lldxf/types.py
+-rw-rw-rw-  2.0 fat    17303 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/lldxf/validator.py
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/lldxf/__init__.py
+-rw-rw-rw-  2.0 fat    19209 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/arc.py
+-rw-rw-rw-  2.0 fat    15532 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/bbox.py
+-rw-rw-rw-  2.0 fat     9310 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/bezier.py
+-rw-rw-rw-  2.0 fat     2458 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/bezier_interpolation.py
+-rw-rw-rw-  2.0 fat     8730 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/box.py
+-rw-rw-rw-  2.0 fat    53170 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/bspline.py
+-rw-rw-rw-  2.0 fat     5608 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/bulge.py
+-rw-rw-rw-  2.0 fat     9135 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/circle.py
+-rw-rw-rw-  2.0 fat    32584 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/clipping.py
+-rw-rw-rw-  2.0 fat     4319 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/clustering.py
+-rw-rw-rw-  2.0 fat    11618 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/construct2d.py
+-rw-rw-rw-  2.0 fat    26176 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/construct3d.py
+-rw-rw-rw-  2.0 fat     1273 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/cspline.py
+-rw-rw-rw-  2.0 fat     9114 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/curvetools.py
+-rw-rw-rw-  2.0 fat    21723 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/ellipse.py
+-rw-rw-rw-  2.0 fat     4406 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/eulerspiral.py
+-rw-rw-rw-  2.0 fat    13190 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/legacy.py
+-rw-rw-rw-  2.0 fat    27210 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/linalg.py
+-rw-rw-rw-  2.0 fat    10213 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/line.py
+-rw-rw-rw-  2.0 fat     3053 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/offset2d.py
+-rw-rw-rw-  2.0 fat     8171 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/parametrize.py
+-rw-rw-rw-  2.0 fat    15602 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/perlin.py
+-rw-rw-rw-  2.0 fat    15934 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/polyline.py
+-rw-rw-rw-  2.0 fat    11703 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/rtree.py
+-rw-rw-rw-  2.0 fat     4815 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/shape.py
+-rw-rw-rw-  2.0 fat    12135 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/transformtools.py
+-rw-rw-rw-  2.0 fat     3539 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/triangulation.py
+-rw-rw-rw-  2.0 fat    17116 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/ucs.py
+-rw-rw-rw-  2.0 fat     6710 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/_bezier3p.py
+-rw-rw-rw-  2.0 fat    11876 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/_bezier4p.py
+-rw-rw-rw-  2.0 fat     9440 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/_bspline.py
+-rw-rw-rw-  2.0 fat    12477 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/_construct.py
+-rw-rw-rw-  2.0 fat     2548 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/_ctypes.py
+-rw-rw-rw-  2.0 fat    24812 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat    22757 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/_matrix44.py
+-rw-rw-rw-  2.0 fat    25882 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/_vector.py
+-rw-rw-rw-  2.0 fat     1978 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/math/__init__.py
+-rw-rw-rw-  2.0 fat     1306 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/path/commands.py
+-rw-rw-rw-  2.0 fat    31293 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/path/converter.py
+-rw-rw-rw-  2.0 fat     5868 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/path/nesting.py
+-rw-rw-rw-  2.0 fat    18224 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/path/path.py
+-rw-rw-rw-  2.0 fat    10129 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/path/shapes.py
+-rw-rw-rw-  2.0 fat    34213 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/path/tools.py
+-rw-rw-rw-  2.0 fat      385 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/path/__init__.py
+-rw-rw-rw-  2.0 fat    10125 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/render/abstract_mtext_renderer.py
+-rw-rw-rw-  2.0 fat    20495 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/render/arrows.py
+-rw-rw-rw-  2.0 fat    17745 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/render/curves.py
+-rw-rw-rw-  2.0 fat     4041 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/render/dimension.py
+-rw-rw-rw-  2.0 fat    51443 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/render/dim_base.py
+-rw-rw-rw-  2.0 fat    35702 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/render/dim_curved.py
+-rw-rw-rw-  2.0 fat     6894 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/render/dim_diameter.py
+-rw-rw-rw-  2.0 fat    24751 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/render/dim_linear.py
+-rw-rw-rw-  2.0 fat     8084 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/render/dim_ordinate.py
+-rw-rw-rw-  2.0 fat    20295 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/render/dim_radius.py
+-rw-rw-rw-  2.0 fat    47170 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/render/forms.py
+-rw-rw-rw-  2.0 fat    25780 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/render/hatching.py
+-rw-rw-rw-  2.0 fat     4728 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/render/leader.py
+-rw-rw-rw-  2.0 fat      664 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/render/linetypes.py
+-rw-rw-rw-  2.0 fat    65258 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/render/mesh.py
+-rw-rw-rw-  2.0 fat    60907 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/render/mleader.py
+-rw-rw-rw-  2.0 fat     8437 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/render/mline.py
+-rw-rw-rw-  2.0 fat     2964 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/render/point.py
+-rw-rw-rw-  2.0 fat     8736 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/render/polyline.py
+-rw-rw-rw-  2.0 fat     7886 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/render/r12spline.py
+-rw-rw-rw-  2.0 fat    22287 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/render/trace.py
+-rw-rw-rw-  2.0 fat     2881 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/render/_linetypes.py
+-rw-rw-rw-  2.0 fat      778 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/render/__init__.py
+-rw-rw-rw-  2.0 fat     1050 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/resources/16x16.png
+-rw-rw-rw-  2.0 fat     1420 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/resources/24x24.png
+-rw-rw-rw-  2.0 fat    10638 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/resources/256x256.png
+-rw-rw-rw-  2.0 fat     1758 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/resources/32x32.png
+-rw-rw-rw-  2.0 fat     2335 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/resources/48x48.png
+-rw-rw-rw-  2.0 fat     3050 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/resources/64x64.png
+-rw-rw-rw-  2.0 fat     2090 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/resources/icon-copy-64px.png
+-rw-rw-rw-  2.0 fat     3109 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/resources/icon-find-64px.png
+-rw-rw-rw-  2.0 fat     2388 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/resources/icon-goto-bookmark-64px.png
+-rw-rw-rw-  2.0 fat     2519 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/resources/icon-goto-handle-64px.png
+-rw-rw-rw-  2.0 fat     2409 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/resources/icon-goto-line-64px.png
+-rw-rw-rw-  2.0 fat     2231 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/resources/icon-left-arrow-64px.png
+-rw-rw-rw-  2.0 fat     2322 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/resources/icon-next-entity-64px.png
+-rw-rw-rw-  2.0 fat     2320 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/resources/icon-prev-entity-64px.png
+-rw-rw-rw-  2.0 fat     2244 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/resources/icon-right-arrow-64px.png
+-rw-rw-rw-  2.0 fat     2553 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/resources/icon-show-in-tree-64px.png
+-rw-rw-rw-  2.0 fat     2373 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/resources/icon-store-bookmark-64px.png
+-rw-rw-rw-  2.0 fat    10650 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/sections/acdsdata.py
+-rw-rw-rw-  2.0 fat    17369 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/sections/blocks.py
+-rw-rw-rw-  2.0 fat    11639 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/sections/classes.py
+-rw-rw-rw-  2.0 fat     4137 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/sections/entities.py
+-rw-rw-rw-  2.0 fat    11937 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/sections/header.py
+-rw-rw-rw-  2.0 fat    61373 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/sections/headervars.py
+-rw-rw-rw-  2.0 fat    27009 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/sections/objects.py
+-rw-rw-rw-  2.0 fat    26565 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/sections/table.py
+-rw-rw-rw-  2.0 fat     5270 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/sections/tables.py
+-rw-rw-rw-  2.0 fat       67 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/sections/__init__.py
+-rw-rw-rw-  2.0 fat    19711 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/tools/analyze.py
+-rw-rw-rw-  2.0 fat    20440 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/tools/binarydata.py
+-rw-rw-rw-  2.0 fat    15926 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/tools/clipping_portal.py
+-rw-rw-rw-  2.0 fat     2931 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/tools/codepage.py
+-rw-rw-rw-  2.0 fat     7613 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/tools/complex_ltype.py
+-rw-rw-rw-  2.0 fat     1782 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/tools/crypt.py
+-rw-rw-rw-  2.0 fat     1511 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/tools/debug.py
+-rw-rw-rw-  2.0 fat     2325 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/tools/difftags.py
+-rw-rw-rw-  2.0 fat     1235 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/tools/handle.py
+-rw-rw-rw-  2.0 fat      780 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/tools/indexing.py
+-rw-rw-rw-  2.0 fat     2145 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/tools/juliandate.py
+-rw-rw-rw-  2.0 fat     6166 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/tools/pattern.py
+-rw-rw-rw-  2.0 fat     1224 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/tools/rawloader.py
+-rw-rw-rw-  2.0 fat   129174 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/tools/standards.py
+-rw-rw-rw-  2.0 fat     6187 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/tools/strip.py
+-rw-rw-rw-  2.0 fat     1466 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/tools/test.py
+-rw-rw-rw-  2.0 fat    66061 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/tools/text.py
+-rw-rw-rw-  2.0 fat    54140 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/tools/text_layout.py
+-rw-rw-rw-  2.0 fat     6893 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/tools/text_size.py
+-rw-rw-rw-  2.0 fat     3116 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/tools/zipmanager.py
+-rw-rw-rw-  2.0 fat   142734 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/tools/_iso_pattern.py
+-rw-rw-rw-  2.0 fat     4413 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/src/ezdxf/tools/__init__.py
+-rw-rw-rw-  2.0 fat        1 b- defN 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat       46 b- defN 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf.egg-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf.egg-info/not-zip-safe
+-rw-rw-rw-  2.0 fat    10110 b- defN 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat      316 b- defN 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf.egg-info/requires.txt
+-rw-rw-rw-  2.0 fat    33328 b- defN 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Jun-01 13:14 ezdxf-1.3.1b1/src/ezdxf.egg-info/top_level.txt
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/tests/test_01_dxf_entities/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/tests/test_03_dxf_layouts/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/tests/test_05_tools/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/tests/test_06_math/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/tests/test_07_render/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/tests/test_08_addons/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/tests/test_09_cython_acceleration/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-01 13:14 ezdxf-1.3.1b1/tests/test_10_issues/
+-rw-rw-rw-  2.0 fat      410 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/conftest.py
+-rw-rw-rw-  2.0 fat     2336 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
+-rw-rw-rw-  2.0 fat      780 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
+-rw-rw-rw-  2.0 fat     2599 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
+-rw-rw-rw-  2.0 fat     1124 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
+-rw-rw-rw-  2.0 fat     5667 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
+-rw-rw-rw-  2.0 fat      582 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
+-rw-rw-rw-  2.0 fat      473 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_011_codepage.py
+-rw-rw-rw-  2.0 fat    11593 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_012_crypt.py
+-rw-rw-rw-  2.0 fat     1191 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
+-rw-rw-rw-  2.0 fat     1033 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
+-rw-rw-rw-  2.0 fat     4792 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
+-rw-rw-rw-  2.0 fat      989 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_016_encoding.py
+-rw-rw-rw-  2.0 fat     1383 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_018_handle.py
+-rw-rw-rw-  2.0 fat     5518 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
+-rw-rw-rw-  2.0 fat     8688 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
+-rw-rw-rw-  2.0 fat     3787 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
+-rw-rw-rw-  2.0 fat      401 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
+-rw-rw-rw-  2.0 fat      539 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
+-rw-rw-rw-  2.0 fat     2092 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
+-rw-rw-rw-  2.0 fat    10917 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_040_tags.py
+-rw-rw-rw-  2.0 fat     3073 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
+-rw-rw-rw-  2.0 fat     6419 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
+-rw-rw-rw-  2.0 fat     1632 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
+-rw-rw-rw-  2.0 fat    11265 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
+-rw-rw-rw-  2.0 fat     3363 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
+-rw-rw-rw-  2.0 fat     1974 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
+-rw-rw-rw-  2.0 fat     2321 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
+-rw-rw-rw-  2.0 fat      568 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
+-rw-rw-rw-  2.0 fat     8797 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
+-rw-rw-rw-  2.0 fat     2581 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_056_special_string_decoding.py
+-rw-rw-rw-  2.0 fat     1500 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
+-rw-rw-rw-  2.0 fat     1947 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_058_json_tags.py
+-rw-rw-rw-  2.0 fat    11689 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_101_dxfnamespace.py
+-rw-rw-rw-  2.0 fat     2893 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_102_appdata.py
+-rw-rw-rw-  2.0 fat     2622 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_103_reactors.py
+-rw-rw-rw-  2.0 fat     4679 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_104_extension_dict.py
+-rw-rw-rw-  2.0 fat    20860 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_105_xdata.py
+-rw-rw-rw-  2.0 fat    14169 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_110_dxfentity.py
+-rw-rw-rw-  2.0 fat     2433 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
+-rw-rw-rw-  2.0 fat     6781 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_112a_dxfgfx.py
+-rw-rw-rw-  2.0 fat      695 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_112b_dxfobj.py
+-rw-rw-rw-  2.0 fat     2431 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_113_dxfclass.py
+-rw-rw-rw-  2.0 fat     4044 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_114_factory.py
+-rw-rw-rw-  2.0 fat     2256 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
+-rw-rw-rw-  2.0 fat    15794 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_116_dictionary.py
+-rw-rw-rw-  2.0 fat     4999 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_117_layer_table_entry.py
+-rw-rw-rw-  2.0 fat      385 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_118_appid_table_entry.py
+-rw-rw-rw-  2.0 fat     1058 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
+-rw-rw-rw-  2.0 fat     3003 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_120_style_table_entry.py
+-rw-rw-rw-  2.0 fat     2943 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
+-rw-rw-rw-  2.0 fat      379 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_122_vport_table_entry.py
+-rw-rw-rw-  2.0 fat     1113 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_123_view_table_entry.py
+-rw-rw-rw-  2.0 fat     8757 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
+-rw-rw-rw-  2.0 fat     1698 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_125_image_def.py
+-rw-rw-rw-  2.0 fat     1312 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_126_image_def_reactor.py
+-rw-rw-rw-  2.0 fat     1430 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_127_raster_variables.py
+-rw-rw-rw-  2.0 fat     1540 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_128_pdf_definition.py
+-rw-rw-rw-  2.0 fat     2778 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_129_xrecord.py
+-rw-rw-rw-  2.0 fat     2423 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_130_id_buffer.py
+-rw-rw-rw-  2.0 fat     2470 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_131_field_list.py
+-rw-rw-rw-  2.0 fat     2435 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_132_layer_filter.py
+-rw-rw-rw-  2.0 fat     2153 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_133_sun.py
+-rw-rw-rw-  2.0 fat      852 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_134_material.py
+-rw-rw-rw-  2.0 fat    11497 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_135_geo_data.py
+-rw-rw-rw-  2.0 fat     1087 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_136_vba_project.py
+-rw-rw-rw-  2.0 fat     3099 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_137_sortentstable.py
+-rw-rw-rw-  2.0 fat      704 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
+-rw-rw-rw-  2.0 fat     7570 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_139_user_record.py
+-rw-rw-rw-  2.0 fat      714 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_140_block_record.py
+-rw-rw-rw-  2.0 fat     9199 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_141_layer_vp_override.py
+-rw-rw-rw-  2.0 fat     1876 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_142_copy_strategy.py
+-rw-rw-rw-  2.0 fat     2268 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_143_spatial_filter.py
+-rw-rw-rw-  2.0 fat     2141 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_144_roundtrip_xrecord.py
+-rw-rw-rw-  2.0 fat     2231 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/conftest.py
+-rw-rw-rw-  2.0 fat     6532 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_200_line.py
+-rw-rw-rw-  2.0 fat     4273 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_201_point.py
+-rw-rw-rw-  2.0 fat     6827 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_202_circle.py
+-rw-rw-rw-  2.0 fat     8949 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_203_arc.py
+-rw-rw-rw-  2.0 fat     2852 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_204_shape.py
+-rw-rw-rw-  2.0 fat     8274 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_205_solid.py
+-rw-rw-rw-  2.0 fat     8476 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_206_text.py
+-rw-rw-rw-  2.0 fat     6487 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_207_attdef.py
+-rw-rw-rw-  2.0 fat     8628 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_208_attrib.py
+-rw-rw-rw-  2.0 fat     2671 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_209_vertex.py
+-rw-rw-rw-  2.0 fat     5916 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_210_polyline_1.py
+-rw-rw-rw-  2.0 fat    13489 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_210_polyline_2.py
+-rw-rw-rw-  2.0 fat     6650 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_210_polyline_explode.py
+-rw-rw-rw-  2.0 fat     1780 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
+-rw-rw-rw-  2.0 fat     7847 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_211_viewport.py
+-rw-rw-rw-  2.0 fat    12629 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_212_insert.py
+-rw-rw-rw-  2.0 fat     6024 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_213_minsert.py
+-rw-rw-rw-  2.0 fat     3284 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_214_block.py
+-rw-rw-rw-  2.0 fat     6914 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_215_dimension.py
+-rw-rw-rw-  2.0 fat     4907 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
+-rw-rw-rw-  2.0 fat    13186 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
+-rw-rw-rw-  2.0 fat     6471 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
+-rw-rw-rw-  2.0 fat     5535 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
+-rw-rw-rw-  2.0 fat     3056 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
+-rw-rw-rw-  2.0 fat     7345 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
+-rw-rw-rw-  2.0 fat     2066 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
+-rw-rw-rw-  2.0 fat     3615 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
+-rw-rw-rw-  2.0 fat     6919 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_221_ellipse.py
+-rw-rw-rw-  2.0 fat     2223 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_222_xline.py
+-rw-rw-rw-  2.0 fat     1493 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_223_ray.py
+-rw-rw-rw-  2.0 fat     3104 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_224_group.py
+-rw-rw-rw-  2.0 fat    10917 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_225_mtext.py
+-rw-rw-rw-  2.0 fat    12226 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_226_spline.py
+-rw-rw-rw-  2.0 fat     5529 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
+-rw-rw-rw-  2.0 fat    10893 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
+-rw-rw-rw-  2.0 fat    15284 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_228_mesh.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
+-rw-rw-rw-  2.0 fat    21421 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
+-rw-rw-rw-  2.0 fat     6587 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
+-rw-rw-rw-  2.0 fat     3140 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
+-rw-rw-rw-  2.0 fat    12486 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
+-rw-rw-rw-  2.0 fat     2274 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_231_underlay.py
+-rw-rw-rw-  2.0 fat     5243 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_231_underlay_2.py
+-rw-rw-rw-  2.0 fat     2294 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_232a_add_acis.py
+-rw-rw-rw-  2.0 fat     7614 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_232b_acis_export.py
+-rw-rw-rw-  2.0 fat     1854 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_232c_acis_surface.py
+-rw-rw-rw-  2.0 fat     4215 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_232d_acis_copy.py
+-rw-rw-rw-  2.0 fat     1936 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_232e_acis_transform.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_233_helix.py
+-rw-rw-rw-  2.0 fat     2040 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_234_light.py
+-rw-rw-rw-  2.0 fat     3806 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_235_leader.py
+-rw-rw-rw-  2.0 fat    20392 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_236_multileader.py
+-rw-rw-rw-  2.0 fat    10992 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_237_mline.py
+-rw-rw-rw-  2.0 fat     2356 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_238_tolerance.py
+-rw-rw-rw-  2.0 fat    27392 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
+-rw-rw-rw-  2.0 fat     4347 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_240_arc_dimension.py
+-rw-rw-rw-  2.0 fat     1069 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_241_hyperlink.py
+-rw-rw-rw-  2.0 fat    11333 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_242_random_transform.py
+-rw-rw-rw-  2.0 fat     3725 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_243_replace_entity.py
+-rw-rw-rw-  2.0 fat     1445 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
+-rw-rw-rw-  2.0 fat     4456 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_245_wipeout.py
+-rw-rw-rw-  2.0 fat     6175 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_246_spline_audit.py
+-rw-rw-rw-  2.0 fat     8165 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
+-rw-rw-rw-  2.0 fat     6003 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_248_mpolygon.py
+-rw-rw-rw-  2.0 fat    13682 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
+-rw-rw-rw-  2.0 fat     7274 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_249_boundary_paths.py
+-rw-rw-rw-  2.0 fat     8331 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
+-rw-rw-rw-  2.0 fat     7331 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_251_upright.py
+-rw-rw-rw-  2.0 fat     4850 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
+-rw-rw-rw-  2.0 fat     2082 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_253_ole2frame.py
+-rw-rw-rw-  2.0 fat     1039 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_254_get_font_name.py
+-rw-rw-rw-  2.0 fat     5149 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_300_layout.py
+-rw-rw-rw-  2.0 fat     4274 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
+-rw-rw-rw-  2.0 fat     5582 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_302_block_references.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_303_auto_block_references.py
+-rw-rw-rw-  2.0 fat      913 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_304_new_entity_space.py
+-rw-rw-rw-  2.0 fat     3279 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
+-rw-rw-rw-  2.0 fat     2609 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
+-rw-rw-rw-  2.0 fat     2343 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_307_groupby.py
+-rw-rw-rw-  2.0 fat    17748 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_308_query.py
+-rw-rw-rw-  2.0 fat     6382 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_309_query_parser.py
+-rw-rw-rw-  2.0 fat     5031 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
+-rw-rw-rw-  2.0 fat     5782 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_312_virtual_layout.py
+-rw-rw-rw-  2.0 fat      647 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_313_redraw_order.py
+-rw-rw-rw-  2.0 fat     6128 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_401_headersection.py
+-rw-rw-rw-  2.0 fat     2750 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_402_classessection.py
+-rw-rw-rw-  2.0 fat     5208 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
+-rw-rw-rw-  2.0 fat     6795 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_404a_tables.py
+-rw-rw-rw-  2.0 fat     4981 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
+-rw-rw-rw-  2.0 fat     2450 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_405_classes.py
+-rw-rw-rw-  2.0 fat     9094 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
+-rw-rw-rw-  2.0 fat      848 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
+-rw-rw-rw-  2.0 fat     3375 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
+-rw-rw-rw-  2.0 fat     1433 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
+-rw-rw-rw-  2.0 fat     5736 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_410_table.py
+-rw-rw-rw-  2.0 fat     6607 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
+-rw-rw-rw-  2.0 fat     1058 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
+-rw-rw-rw-  2.0 fat     2340 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
+-rw-rw-rw-  2.0 fat    18072 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
+-rw-rw-rw-  2.0 fat     4638 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
+-rw-rw-rw-  2.0 fat    12327 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
+-rw-rw-rw-  2.0 fat     6509 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
+-rw-rw-rw-  2.0 fat     5656 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_417_bbox.py
+-rw-rw-rw-  2.0 fat     5434 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
+-rw-rw-rw-  2.0 fat      733 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
+-rw-rw-rw-  2.0 fat     1240 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
+-rw-rw-rw-  2.0 fat     5007 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
+-rw-rw-rw-  2.0 fat      769 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
+-rw-rw-rw-  2.0 fat     8058 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_424_audit.py
+-rw-rw-rw-  2.0 fat     3737 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
+-rw-rw-rw-  2.0 fat     2981 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
+-rw-rw-rw-  2.0 fat     2416 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
+-rw-rw-rw-  2.0 fat     2533 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
+-rw-rw-rw-  2.0 fat     7813 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_429_xclip.py
+-rw-rw-rw-  2.0 fat   112800 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/conftest.py
+-rw-rw-rw-  2.0 fat     5510 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_500_units.py
+-rw-rw-rw-  2.0 fat     2665 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_501_truecolor.py
+-rw-rw-rw-  2.0 fat     1021 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_502_raw_color.py
+-rw-rw-rw-  2.0 fat     1695 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_503_indexing.py
+-rw-rw-rw-  2.0 fat     1442 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_504_suppress_zeros.py
+-rw-rw-rw-  2.0 fat      216 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_506_version.py
+-rw-rw-rw-  2.0 fat      657 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_508_read_zip.py
+-rw-rw-rw-  2.0 fat     1445 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_509_comments.py
+-rw-rw-rw-  2.0 fat     1185 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_510_byte_stream.py
+-rw-rw-rw-  2.0 fat     4239 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_511_bit_stream.py
+-rw-rw-rw-  2.0 fat     5595 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_512_pattern.py
+-rw-rw-rw-  2.0 fat     2372 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_513_reorder_entities.py
+-rw-rw-rw-  2.0 fat    18181 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_514_text.py
+-rw-rw-rw-  2.0 fat     9361 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_515a_fonts_truetype.py
+-rw-rw-rw-  2.0 fat     4752 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_515b_fonts_shapefiles.py
+-rw-rw-rw-  2.0 fat     2469 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_515c_fonts_lff.py
+-rw-rw-rw-  2.0 fat     4002 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_516_zoom.py
+-rw-rw-rw-  2.0 fat    34209 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_517_text_layout.py
+-rw-rw-rw-  2.0 fat      474 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_518_header_guid.py
+-rw-rw-rw-  2.0 fat     3716 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_519_mtext_editor.py
+-rw-rw-rw-  2.0 fat     3205 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_520_mtext_context.py
+-rw-rw-rw-  2.0 fat    24496 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_521_mtext_parser.py
+-rw-rw-rw-  2.0 fat     3863 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_522_text_scanner.py
+-rw-rw-rw-  2.0 fat     5564 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_523_text_size.py
+-rw-rw-rw-  2.0 fat     5063 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_524_block_reference_manager.py
+-rw-rw-rw-  2.0 fat      773 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_525_transparency.py
+-rw-rw-rw-  2.0 fat     2133 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_526_explode.py
+-rw-rw-rw-  2.0 fat    13521 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_527_gfxattribs.py
+-rw-rw-rw-  2.0 fat     2748 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_528_difftags.py
+-rw-rw-rw-  2.0 fat     6700 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_529_acis_sat.py
+-rw-rw-rw-  2.0 fat     2062 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_530_acis_sab.py
+-rw-rw-rw-  2.0 fat    12357 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_531_acis_entities.py
+-rw-rw-rw-  2.0 fat     7858 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_532_acis_mesh.py
+-rw-rw-rw-  2.0 fat    43259 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_533_shapefiles.py
+-rw-rw-rw-  2.0 fat     1034 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_534_dwg_info.py
+-rw-rw-rw-  2.0 fat    48174 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_535_xref_basic.py
+-rw-rw-rw-  2.0 fat    27614 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_536_xref_conflict.py
+-rw-rw-rw-  2.0 fat     7186 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_537_transform.py
+-rw-rw-rw-  2.0 fat     2246 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
+-rw-rw-rw-  2.0 fat    17771 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_539_npshapes.py
+-rw-rw-rw-  2.0 fat     2605 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_540_lff_parser.py
+-rw-rw-rw-  2.0 fat     1206 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_541_clipping_portal.py
+-rw-rw-rw-  2.0 fat     1400 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_542_itertools.py
+-rw-rw-rw-  2.0 fat    11705 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_543_select.py
+-rw-rw-rw-  2.0 fat     1264 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_544_revcloud.py
+-rw-rw-rw-  2.0 fat     2567 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_545_acis_cache.py
+-rw-rw-rw-  2.0 fat    19698 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_546_edgeminer.py
+-rw-rw-rw-  2.0 fat     3413 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_05_tools/test_547_edgesmith.py
+-rw-rw-rw-  2.0 fat     4026 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/conftest.py
+-rw-rw-rw-  2.0 fat     7503 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_600_base.py
+-rw-rw-rw-  2.0 fat     2098 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_601_bulge.py
+-rw-rw-rw-  2.0 fat    14661 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_602_vec3.py
+-rw-rw-rw-  2.0 fat     8956 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_603_vec2.py
+-rw-rw-rw-  2.0 fat     2829 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_604_banded_matrix.py
+-rw-rw-rw-  2.0 fat     9709 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_604_linalg.py
+-rw-rw-rw-  2.0 fat    14118 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_605_matrix44.py
+-rw-rw-rw-  2.0 fat     5888 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_606_convexhull.py
+-rw-rw-rw-  2.0 fat     1010 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_607_perlin_noise.py
+-rw-rw-rw-  2.0 fat     3833 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_608_intersection_line_line_2d.py
+-rw-rw-rw-  2.0 fat     1676 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_609_point_on_line.py
+-rw-rw-rw-  2.0 fat     3171 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_610_ocs.py
+-rw-rw-rw-  2.0 fat     7529 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_611_ucs.py
+-rw-rw-rw-  2.0 fat     1831 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_612_ucs_pass_trough.py
+-rw-rw-rw-  2.0 fat     6332 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_613_is_point_in_polygon_2d.py
+-rw-rw-rw-  2.0 fat    10913 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_614_construct_3d.py
+-rw-rw-rw-  2.0 fat      602 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_615_rytz_axis.py
+-rw-rw-rw-  2.0 fat     5215 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_616_plane.py
+-rw-rw-rw-  2.0 fat      772 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_617_clockwise_orientation.py
+-rw-rw-rw-  2.0 fat     7712 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_618_clipping.py
+-rw-rw-rw-  2.0 fat    14372 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_619_greiner_hormann.py
+-rw-rw-rw-  2.0 fat     2669 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_620_knot.py
+-rw-rw-rw-  2.0 fat    18834 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_621_bspline.py
+-rw-rw-rw-  2.0 fat     7652 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_622_bsplineu.py
+-rw-rw-rw-  2.0 fat    11314 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_623_rbspline.py
+-rw-rw-rw-  2.0 fat    10869 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_624_global_bspline_interpolation.py
+-rw-rw-rw-  2.0 fat     1247 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_626_local_bspline_interpolation.py
+-rw-rw-rw-  2.0 fat     1967 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_627_bspline_basis.py
+-rw-rw-rw-  2.0 fat    10545 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_629_bezier.py
+-rw-rw-rw-  2.0 fat    10900 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_630a_bezier4p_base.py
+-rw-rw-rw-  2.0 fat    10354 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_630b_bezier4p_functions.py
+-rw-rw-rw-  2.0 fat     1683 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_631_euler_spiral.py
+-rw-rw-rw-  2.0 fat     4054 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_632_bezier3p.py
+-rw-rw-rw-  2.0 fat    20154 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_640_bbox.py
+-rw-rw-rw-  2.0 fat     5393 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_641_construction_ray.py
+-rw-rw-rw-  2.0 fat     3673 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_642_construction_line.py
+-rw-rw-rw-  2.0 fat     9459 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_643_construction_box.py
+-rw-rw-rw-  2.0 fat    11561 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_644_construction_circle.py
+-rw-rw-rw-  2.0 fat    10988 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_645_construction_arc.py
+-rw-rw-rw-  2.0 fat     3422 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_646_offset_vertices_2d.py
+-rw-rw-rw-  2.0 fat     7672 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_647_transform_tools.py
+-rw-rw-rw-  2.0 fat     9001 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_648_construction_ellipse.py
+-rw-rw-rw-  2.0 fat     4243 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_650_elliptic_arc_span.py
+-rw-rw-rw-  2.0 fat     9024 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_651_construction_polyline.py
+-rw-rw-rw-  2.0 fat     3212 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_652_approx_param_t.py
+-rw-rw-rw-  2.0 fat     5806 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_653_polyline_intersection.py
+-rw-rw-rw-  2.0 fat     5193 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_654_rtree.py
+-rw-rw-rw-  2.0 fat      788 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_655_dbscan.py
+-rw-rw-rw-  2.0 fat      834 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_656_k_means.py
+-rw-rw-rw-  2.0 fat     4654 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_657_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat    11654 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_658_bevel_tools.py
+-rw-rw-rw-  2.0 fat     1875 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_659_intersection_line_polygon_3d.py
+-rw-rw-rw-  2.0 fat     1428 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
+-rw-rw-rw-  2.0 fat     1741 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
+-rw-rw-rw-  2.0 fat     3307 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_662_is_convex_polygon_2d.py
+-rw-rw-rw-  2.0 fat     1266 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_663_is_axes_aligned_rectange.py
+-rw-rw-rw-  2.0 fat    17333 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_664_concave_clipping_polygon.py
+-rw-rw-rw-  2.0 fat     7980 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_665_inverted_clipping_polygon.py
+-rw-rw-rw-  2.0 fat     1553 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_06_math/test_666_wgs84_transform.py
+-rw-rw-rw-  2.0 fat     1466 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_07_render/test_701_arrows.py
+-rw-rw-rw-  2.0 fat    17245 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_07_render/test_702_render_forms.py
+-rw-rw-rw-  2.0 fat    34554 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_07_render/test_703_mesh_builder.py
+-rw-rw-rw-  2.0 fat     4459 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_07_render/test_704_render_linear_dimension.py
+-rw-rw-rw-  2.0 fat     1345 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_07_render/test_705_shape.py
+-rw-rw-rw-  2.0 fat      483 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_07_render/test_706_random_path.py
+-rw-rw-rw-  2.0 fat     5603 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_07_render/test_707_trace.py
+-rw-rw-rw-  2.0 fat    34121 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_07_render/test_708a_path.py
+-rw-rw-rw-  2.0 fat    27365 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_07_render/test_708b_path_tools.py
+-rw-rw-rw-  2.0 fat     3352 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_07_render/test_708c_matplotlib_path_tools.py
+-rw-rw-rw-  2.0 fat     3278 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_07_render/test_708d_qpainter_path_tools.py
+-rw-rw-rw-  2.0 fat     4589 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_07_render/test_708e_path_shapes.py
+-rw-rw-rw-  2.0 fat     4121 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_07_render/test_708f_path_nesting.py
+-rw-rw-rw-  2.0 fat     1308 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_07_render/test_709_linetype_renderer.py
+-rw-rw-rw-  2.0 fat     2815 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_07_render/test_711_points.py
+-rw-rw-rw-  2.0 fat     6594 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_07_render/test_712_render_curved_dimension.py
+-rw-rw-rw-  2.0 fat     1472 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_07_render/test_713_mleader_builder.py
+-rw-rw-rw-  2.0 fat     1091 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_07_render/test_714_mleader_render_engine.py
+-rw-rw-rw-  2.0 fat    11887 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_07_render/test_715_hatching.py
+-rw-rw-rw-  2.0 fat     2626 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
+-rw-rw-rw-  2.0 fat     4771 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_800_mtext_surrogate.py
+-rw-rw-rw-  2.0 fat     1352 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_801_r12spline.py
+-rw-rw-rw-  2.0 fat     7881 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_802_table_painter.py
+-rw-rw-rw-  2.0 fat    13038 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_803_entities_to_code.py
+-rw-rw-rw-  2.0 fat     6844 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_804_importer.py
+-rw-rw-rw-  2.0 fat     2362 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_805_pycsg.py
+-rw-rw-rw-  2.0 fat    16011 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_806_acadctb.py
+-rw-rw-rw-  2.0 fat     4860 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_807_dwg_loader_basics.py
+-rw-rw-rw-  2.0 fat    11204 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_810_drawing_properties.py
+-rw-rw-rw-  2.0 fat    12549 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_811a_drawing_frontend.py
+-rw-rw-rw-  2.0 fat     9101 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_811b_drawing_recorder.py
+-rw-rw-rw-  2.0 fat     2898 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_811c_viewport_processing.py
+-rw-rw-rw-  2.0 fat     4229 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_812_drawing_graphic_proxy.py
+-rw-rw-rw-  2.0 fat    13751 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_813_geo_interface.py
+-rw-rw-rw-  2.0 fat    14853 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_814_text2path.py
+-rw-rw-rw-  2.0 fat    16239 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_815_dxf_browser.py
+-rw-rw-rw-  2.0 fat    11275 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_816_bin_packing.py
+-rw-rw-rw-  2.0 fat    12554 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_817_genetic_algorithm.py
+-rw-rw-rw-  2.0 fat     9008 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_818_meshex.py
+-rw-rw-rw-  2.0 fat     1003 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_819_menger_sponge.py
+-rw-rw-rw-  2.0 fat     4433 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_820_openscad.py
+-rw-rw-rw-  2.0 fat    15655 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_821_hpgl2.py
+-rw-rw-rw-  2.0 fat     1376 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
+-rw-rw-rw-  2.0 fat     5284 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_823_drawing_layout.py
+-rw-rw-rw-  2.0 fat     3312 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_824_svg_drawing_backend.py
+-rw-rw-rw-  2.0 fat     2014 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_825_hpgl2_drawing_backend.py
+-rw-rw-rw-  2.0 fat     3158 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_826_custom_json_backend.py
+-rw-rw-rw-  2.0 fat     3388 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_08_addons/test_827_geojson_backend.py
+-rw-rw-rw-  2.0 fat     2527 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_09_cython_acceleration/test_901_acc_vec2.py
+-rw-rw-rw-  2.0 fat     2199 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_09_cython_acceleration/test_902_acc_vec3.py
+-rw-rw-rw-  2.0 fat     2142 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+-rw-rw-rw-  2.0 fat     3175 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+-rw-rw-rw-  2.0 fat     1463 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+-rw-rw-rw-  2.0 fat     4773 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+-rw-rw-rw-  2.0 fat     1666 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_10_issues/test_issue_1078_bbox_calculation.py
+-rw-rw-rw-  2.0 fat     2656 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_10_issues/test_issue_414_bbox_calculation.py
+-rw-rw-rw-  2.0 fat     1213 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+-rw-rw-rw-  2.0 fat     2268 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_10_issues/test_issue_574_flattening_error.py
+-rw-rw-rw-  2.0 fat     1754 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+-rw-rw-rw-  2.0 fat      682 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_10_issues/test_issue_749_text_layout.py
+-rw-rw-rw-  2.0 fat    11094 b- defN 24-Jun-01 13:13 ezdxf-1.3.1b1/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
+868 files, 8989974 bytes uncompressed, 2057502 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -1,2605 +1,2605 @@
-Filename: ezdxf-1.3.1b0/
+Filename: ezdxf-1.3.1b1/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/
+Filename: ezdxf-1.3.1b1/integration_tests/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/
+Filename: ezdxf-1.3.1b1/src/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/
+Filename: ezdxf-1.3.1b1/tests/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/LICENSE
+Filename: ezdxf-1.3.1b1/LICENSE
 Comment: 
 
-Filename: ezdxf-1.3.1b0/MANIFEST.in
+Filename: ezdxf-1.3.1b1/MANIFEST.in
 Comment: 
 
-Filename: ezdxf-1.3.1b0/PKG-INFO
+Filename: ezdxf-1.3.1b1/PKG-INFO
 Comment: 
 
-Filename: ezdxf-1.3.1b0/pyproject.toml
+Filename: ezdxf-1.3.1b1/pyproject.toml
 Comment: 
 
-Filename: ezdxf-1.3.1b0/README.md
+Filename: ezdxf-1.3.1b1/README.md
 Comment: 
 
-Filename: ezdxf-1.3.1b0/requirements.txt
+Filename: ezdxf-1.3.1b1/requirements.txt
 Comment: 
 
-Filename: ezdxf-1.3.1b0/setup.cfg
+Filename: ezdxf-1.3.1b1/setup.cfg
 Comment: 
 
-Filename: ezdxf-1.3.1b0/setup.py
+Filename: ezdxf-1.3.1b1/setup.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/
+Filename: ezdxf-1.3.1b1/integration_tests/data/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/check_disable_c_ext_by_config_file.py
+Filename: ezdxf-1.3.1b1/integration_tests/check_disable_c_ext_by_config_file.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/check_disable_c_ext_by_env_var.py
+Filename: ezdxf-1.3.1b1/integration_tests/check_disable_c_ext_by_env_var.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/conftest.py
+Filename: ezdxf-1.3.1b1/integration_tests/conftest.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_acad_table.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_acad_table.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_acis_entites.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_acis_entites.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_all_dimline_styles.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_all_dimline_styles.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_all_ellipse_transformations.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_all_ellipse_transformations.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_anonymous_blocks.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_anonymous_blocks.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_appsettings.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_appsettings.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_audit_critical_dxf_files.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_audit_critical_dxf_files.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_audit_layouts.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_audit_layouts.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_complex_line_type_2.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_complex_line_type_2.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_create_basic_graphics.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_create_basic_graphics.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_document_guid.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_document_guid.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_document_page_setup.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_document_page_setup.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_dxf_info_scanning.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_dxf_info_scanning.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_dynblkhelper.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_dynblkhelper.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_entities_iterator.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_entities_iterator.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_fix_dulicate_handles.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_fix_dulicate_handles.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_geo.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_geo.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_groups.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_groups.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_hpgl2_addon.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_hpgl2_addon.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_ignore_junk_beyond_EOF.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_ignore_junk_beyond_EOF.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_launcher.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_launcher.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_leica_disto_r12.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_leica_disto_r12.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_load_dxf_unicode_notation.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_load_dxf_unicode_notation.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_mapbox_earcut.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_mtext_columns.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_mtext_columns.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_mtext_explode_addon.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_mtext_explode_addon.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_mtext_text_frame.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_mtext_text_frame.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_new_table_entries.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_new_table_entries.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_none_ascii_read_write.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_none_ascii_read_write.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_odafc.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_odafc.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_open_binary_DXF_files.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_open_binary_DXF_files.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_open_coord_order_issue.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_open_coord_order_issue.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_open_exotic_dxf_files.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_open_exotic_dxf_files.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_open_R13_R14.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_open_R13_R14.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_polyline_entity.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_polyline_entity.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_preserve_binary_data_in_xrecords.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_preserve_binary_data_in_xrecords.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_r12export.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_r12export.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_r12strict.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_r12strict.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_r12writer.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_r12writer.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_read_file_without_handles.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_read_file_without_handles.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_read_write_modern_entites.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_read_write_modern_entites.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_recover.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_recover.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_redraw_order.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_redraw_order.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_rotated_block_attributes.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_rotated_block_attributes.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_surface_entities.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_surface_entities.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_write_fixed_meta_data.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_write_fixed_meta_data.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_write_without_handles.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_write_without_handles.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_xref_detach.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_xref_detach.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/test_xref_load_acis.py
+Filename: ezdxf-1.3.1b1/integration_tests/test_xref_load_acis.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/AC1003_LINE_Example.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/AC1003_LINE_Example.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/acad_table_with_blk_ref.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/acad_table_with_blk_ref.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/ASCII_R12.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/ASCII_R12.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r12.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/bin_dxf_r12.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r13.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/bin_dxf_r13.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r14.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/bin_dxf_r14.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r2000.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/bin_dxf_r2000.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/cc_dxflib.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/cc_dxflib.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/custom_blocks.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/custom_blocks.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/duplicate_handles.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/duplicate_handles.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/dxf_unicode.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/dxf_unicode.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/dynblks.zip
+Filename: ezdxf-1.3.1b1/integration_tests/data/dynblks.zip
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/empty_handles.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/empty_handles.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/groups.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/groups.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/layout_broken_links.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/layout_broken_links.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/layout_broken_links_2.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/layout_broken_links_2.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/layout_missing_block_definition.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/layout_missing_block_definition.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/layout_missing_block_record.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/layout_missing_block_record.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/Leica_Disto_S910.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/Leica_Disto_S910.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/MODEL.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/MODEL.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/mtext_columns_R2007.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/mtext_columns_R2007.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/mtext_columns_R2018.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/mtext_columns_R2018.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/mtext_framed_columns.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/mtext_framed_columns.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/mtext_text_frame.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/mtext_text_frame.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/no_layouts.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/no_layouts.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/PLOTFILE.plt
+Filename: ezdxf-1.3.1b1/integration_tests/data/PLOTFILE.plt
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/POLI-ALL210_12.DXF
+Filename: ezdxf-1.3.1b1/integration_tests/data/POLI-ALL210_12.DXF
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/R12_with_trash_beyond_EOF.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/R12_with_trash_beyond_EOF.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/recover01.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/recover01.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/recover02.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/recover02.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/small_r13.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/small_r13.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/small_r14.dxf
+Filename: ezdxf-1.3.1b1/integration_tests/data/small_r14.dxf
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/XRECORD_0.bin
+Filename: ezdxf-1.3.1b1/integration_tests/data/XRECORD_0.bin
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/XRECORD_1.bin
+Filename: ezdxf-1.3.1b1/integration_tests/data/XRECORD_1.bin
 Comment: 
 
-Filename: ezdxf-1.3.1b0/integration_tests/data/XRECORD_2.bin
+Filename: ezdxf-1.3.1b1/integration_tests/data/XRECORD_2.bin
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/
+Filename: ezdxf-1.3.1b1/src/ezdxf/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf.egg-info/
+Filename: ezdxf-1.3.1b1/src/ezdxf.egg-info/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acc/
+Filename: ezdxf-1.3.1b1/src/ezdxf/acc/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acis/
+Filename: ezdxf-1.3.1b1/src/ezdxf/acis/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/fonts/
+Filename: ezdxf-1.3.1b1/src/ezdxf/fonts/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/layouts/
+Filename: ezdxf-1.3.1b1/src/ezdxf/layouts/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/
+Filename: ezdxf-1.3.1b1/src/ezdxf/lldxf/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/path/
+Filename: ezdxf-1.3.1b1/src/ezdxf/path/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/resources/
+Filename: ezdxf-1.3.1b1/src/ezdxf/resources/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/sections/
+Filename: ezdxf-1.3.1b1/src/ezdxf/sections/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/tools/
+Filename: ezdxf-1.3.1b1/src/ezdxf/tools/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/appsettings.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/appsettings.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/audit.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/audit.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/bbox.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/bbox.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/blkrefs.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/blkrefs.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/colors.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/colors.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/commands.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/commands.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/comments.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/comments.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/disassemble.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/disassemble.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/document.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/document.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/dwginfo.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/dwginfo.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/dynblkhelper.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/dynblkhelper.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/edgeminer.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/edgeminer.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/edgesmith.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/edgesmith.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entitydb.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entitydb.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/enums.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/enums.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/explode.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/explode.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/eztypes.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/eztypes.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/filemanagement.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/filemanagement.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/gfxattribs.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/gfxattribs.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/graphicsfactory.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/graphicsfactory.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/groupby.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/groupby.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/messenger.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/messenger.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/msgtypes.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/msgtypes.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/npshapes.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/npshapes.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/protocols.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/protocols.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/proxygraphic.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/proxygraphic.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/py.typed
+Filename: ezdxf-1.3.1b1/src/ezdxf/py.typed
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/query.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/query.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/queryparser.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/queryparser.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/r12strict.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/r12strict.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/recover.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/recover.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/reorder.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/reorder.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/revcloud.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/revcloud.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/select.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/select.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/transform.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/transform.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/units.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/units.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/upright.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/upright.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/urecord.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/urecord.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/version.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/version.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/xclip.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/xclip.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/xref.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/xref.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/zoom.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/zoom.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/_options.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/_options.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/__init__.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/__main__.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/__main__.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acc/bezier3p.pyx
+Filename: ezdxf-1.3.1b1/src/ezdxf/acc/bezier3p.pyx
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acc/bezier4p.pyx
+Filename: ezdxf-1.3.1b1/src/ezdxf/acc/bezier4p.pyx
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acc/bspline.pyx
+Filename: ezdxf-1.3.1b1/src/ezdxf/acc/bspline.pyx
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acc/constants.h
+Filename: ezdxf-1.3.1b1/src/ezdxf/acc/constants.h
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acc/construct.pyx
+Filename: ezdxf-1.3.1b1/src/ezdxf/acc/construct.pyx
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acc/linetypes.pyx
+Filename: ezdxf-1.3.1b1/src/ezdxf/acc/linetypes.pyx
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acc/mapbox_earcut.pyx
+Filename: ezdxf-1.3.1b1/src/ezdxf/acc/mapbox_earcut.pyx
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acc/matrix44.pxd
+Filename: ezdxf-1.3.1b1/src/ezdxf/acc/matrix44.pxd
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acc/matrix44.pyx
+Filename: ezdxf-1.3.1b1/src/ezdxf/acc/matrix44.pyx
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acc/np_support.pyx
+Filename: ezdxf-1.3.1b1/src/ezdxf/acc/np_support.pyx
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acc/vector.pxd
+Filename: ezdxf-1.3.1b1/src/ezdxf/acc/vector.pxd
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acc/vector.pyx
+Filename: ezdxf-1.3.1b1/src/ezdxf/acc/vector.pyx
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acc/__init__.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/acc/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acis/abstract.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/acis/abstract.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acis/api.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/acis/api.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acis/cache.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/acis/cache.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acis/const.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/acis/const.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acis/dbg.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/acis/dbg.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acis/dxf.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/acis/dxf.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acis/entities.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/acis/entities.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acis/hdr.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/acis/hdr.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acis/mesh.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/acis/mesh.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acis/sab.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/acis/sab.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acis/sat.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/acis/sat.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acis/type_hints.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/acis/type_hints.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/acis/__init__.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/acis/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/acisbrowser/
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/acisbrowser/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/browser/
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/browser/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/dwg/
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/dwg/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/acadctb.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/acadctb.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/binpacking.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/binpacking.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/dimlines.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/dimlines.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/dxf2code.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/dxf2code.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/genetic_algorithm.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/genetic_algorithm.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/geo.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/geo.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/gerber_D6673.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/gerber_D6673.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/importer.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/importer.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/iterdxf.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/iterdxf.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/menger_sponge.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/menger_sponge.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/meshex.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/meshex.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/mixins.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/mixins.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/mtextsurrogate.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/mtextsurrogate.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/mtxpl.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/mtxpl.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/odafc.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/odafc.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/openscad.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/openscad.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/pycsg.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/pycsg.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/r12export.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/r12export.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/r12writer.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/r12writer.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/sierpinski_pyramid.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/sierpinski_pyramid.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/tablepainter.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/tablepainter.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/text2path.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/text2path.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/xplayer.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/xplayer.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/xqt.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/xqt.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/__init__.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/acisbrowser/browser.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/acisbrowser/browser.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/acisbrowser/data.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/acisbrowser/data.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/acisbrowser/__init__.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/acisbrowser/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/browser/bookmarks.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/browser/bookmarks.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/browser/browser.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/browser/browser.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/browser/data.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/browser/data.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/browser/find_dialog.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/browser/find_dialog.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/browser/loader.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/browser/loader.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/browser/model.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/browser/model.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/browser/reflinks.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/browser/reflinks.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/browser/tags.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/browser/tags.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/browser/views.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/browser/views.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/browser/__init__.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/browser/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/backend.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/backend.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/config.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/config.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/debug_backend.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/debug_backend.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/debug_utils.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/debug_utils.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/dxf.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/dxf.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/file_output.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/file_output.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/frontend.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/frontend.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/gfxproxy.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/gfxproxy.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/hpgl2.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/hpgl2.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/json.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/json.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/layout.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/layout.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/matplotlib.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/matplotlib.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/mtext_complex.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/mtext_complex.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/pipeline.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/pipeline.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/properties.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/properties.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/pymupdf.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/pymupdf.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/pyqt.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/pyqt.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/qtviewer.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/qtviewer.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/recorder.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/recorder.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/svg.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/svg.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/text.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/text.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/text_renderer.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/text_renderer.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/type_hints.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/type_hints.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/unified_text_renderer.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/unified_text_renderer.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/drawing/__init__.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/drawing/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/dwg/classes_section.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/dwg/classes_section.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/dwg/const.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/dwg/const.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/dwg/crc.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/dwg/crc.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/dwg/fileheader.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/dwg/fileheader.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/dwg/header_section.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/dwg/header_section.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/dwg/loader.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/dwg/loader.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/dwg/__init__.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/dwg/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/api.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/api.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/backend.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/backend.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/deps.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/deps.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/interpreter.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/interpreter.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/page.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/page.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/plotter.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/plotter.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/polygon_buffer.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/polygon_buffer.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/properties.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/properties.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/tokenizer.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/tokenizer.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/viewer.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/viewer.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/__init__.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/acad_proxy_entity.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/acad_proxy_entity.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/acad_table.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/acad_table.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/acad_xrec_roundtrip.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/acad_xrec_roundtrip.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/acis.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/acis.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/appdata.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/appdata.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/appid.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/appid.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/arc.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/arc.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/attrib.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/attrib.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/block.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/block.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/blockrecord.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/blockrecord.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/boundary_paths.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/boundary_paths.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/circle.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/circle.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/copy.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/copy.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/dictionary.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/dictionary.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/dimension.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/dimension.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/dimstyle.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/dimstyle.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/dimstyleoverride.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/dimstyleoverride.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/dxfclass.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/dxfclass.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/dxfentity.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/dxfentity.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/dxfgfx.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/dxfgfx.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/dxfgroups.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/dxfgroups.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/dxfns.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/dxfns.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/dxfobj.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/dxfobj.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/ellipse.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/ellipse.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/factory.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/factory.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/geodata.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/geodata.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/gradient.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/gradient.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/hatch.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/hatch.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/helix.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/helix.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/idbuffer.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/idbuffer.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/image.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/image.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/insert.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/insert.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/layer.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/layer.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/layout.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/layout.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/leader.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/leader.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/light.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/light.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/line.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/line.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/ltype.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/ltype.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/lwpolyline.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/lwpolyline.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/material.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/material.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/mesh.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/mesh.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/mleader.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/mleader.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/mline.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/mline.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/mpolygon.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/mpolygon.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/mtext.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/mtext.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/mtext_columns.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/mtext_columns.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/objectcollection.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/objectcollection.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/oleframe.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/oleframe.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/pattern.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/pattern.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/point.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/point.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/polygon.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/polygon.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/polyline.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/polyline.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/shape.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/shape.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/solid.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/solid.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/spatial_filter.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/spatial_filter.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/spline.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/spline.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/subentity.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/subentity.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/sun.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/sun.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/table.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/table.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/temporary_transform.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/temporary_transform.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/text.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/text.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/textstyle.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/textstyle.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/tolerance.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/tolerance.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/ucs.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/ucs.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/underlay.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/underlay.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/view.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/view.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/viewport.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/viewport.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/visualstyle.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/visualstyle.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/vport.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/vport.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/xdata.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/xdata.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/xdict.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/xdict.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/xline.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/xline.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/entities/__init__.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/entities/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/fonts/fonts.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/fonts/fonts.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/fonts/font_face.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/fonts/font_face.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/fonts/font_manager.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/fonts/font_manager.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/fonts/font_measurements.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/fonts/font_measurements.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/fonts/font_synonyms.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/fonts/font_synonyms.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/fonts/glyphs.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/fonts/glyphs.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/fonts/lff.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/fonts/lff.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/fonts/shapefile.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/fonts/shapefile.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/fonts/ttfonts.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/fonts/ttfonts.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/fonts/__init__.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/fonts/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/layouts/base.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/layouts/base.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/layouts/blocklayout.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/layouts/blocklayout.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/layouts/layout.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/layouts/layout.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/layouts/layouts.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/layouts/layouts.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/layouts/__init__.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/layouts/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/attributes.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/lldxf/attributes.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/const.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/lldxf/const.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/encoding.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/lldxf/encoding.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/extendedtags.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/lldxf/extendedtags.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/fileindex.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/lldxf/fileindex.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/hdrvars.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/lldxf/hdrvars.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/loader.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/lldxf/loader.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/packedtags.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/lldxf/packedtags.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/repair.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/lldxf/repair.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/tagger.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/lldxf/tagger.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/tags.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/lldxf/tags.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/tagwriter.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/lldxf/tagwriter.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/types.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/lldxf/types.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/validator.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/lldxf/validator.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/lldxf/__init__.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/lldxf/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/arc.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/arc.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/bbox.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/bbox.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/bezier.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/bezier.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/bezier_interpolation.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/bezier_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/box.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/box.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/bspline.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/bspline.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/bulge.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/bulge.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/circle.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/circle.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/clipping.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/clipping.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/clustering.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/clustering.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/construct2d.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/construct2d.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/construct3d.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/construct3d.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/cspline.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/cspline.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/curvetools.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/curvetools.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/ellipse.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/ellipse.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/eulerspiral.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/eulerspiral.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/legacy.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/legacy.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/linalg.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/linalg.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/line.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/line.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/offset2d.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/offset2d.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/parametrize.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/parametrize.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/perlin.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/perlin.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/polyline.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/polyline.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/rtree.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/rtree.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/shape.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/shape.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/transformtools.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/transformtools.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/triangulation.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/triangulation.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/ucs.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/ucs.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/_bezier3p.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/_bezier4p.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/_bezier4p.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/_bspline.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/_bspline.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/_construct.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/_construct.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/_ctypes.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/_ctypes.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/_mapbox_earcut.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/_matrix44.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/_vector.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/_vector.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/math/__init__.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/math/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/path/commands.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/path/commands.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/path/converter.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/path/converter.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/path/nesting.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/path/nesting.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/path/path.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/path/path.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/path/shapes.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/path/shapes.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/path/tools.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/path/tools.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/path/__init__.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/path/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/abstract_mtext_renderer.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/abstract_mtext_renderer.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/arrows.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/arrows.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/curves.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/curves.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/dimension.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/dimension.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/dim_base.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/dim_base.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/dim_curved.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/dim_curved.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/dim_diameter.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/dim_diameter.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/dim_linear.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/dim_linear.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/dim_ordinate.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/dim_ordinate.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/dim_radius.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/dim_radius.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/forms.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/forms.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/hatching.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/hatching.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/leader.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/leader.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/linetypes.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/linetypes.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/mesh.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/mesh.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/mleader.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/mleader.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/mline.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/mline.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/point.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/point.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/polyline.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/polyline.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/r12spline.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/r12spline.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/trace.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/trace.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/_linetypes.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/_linetypes.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/render/__init__.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/render/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/resources/16x16.png
+Filename: ezdxf-1.3.1b1/src/ezdxf/resources/16x16.png
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/resources/24x24.png
+Filename: ezdxf-1.3.1b1/src/ezdxf/resources/24x24.png
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/resources/256x256.png
+Filename: ezdxf-1.3.1b1/src/ezdxf/resources/256x256.png
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/resources/32x32.png
+Filename: ezdxf-1.3.1b1/src/ezdxf/resources/32x32.png
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/resources/48x48.png
+Filename: ezdxf-1.3.1b1/src/ezdxf/resources/48x48.png
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/resources/64x64.png
+Filename: ezdxf-1.3.1b1/src/ezdxf/resources/64x64.png
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/resources/icon-copy-64px.png
+Filename: ezdxf-1.3.1b1/src/ezdxf/resources/icon-copy-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/resources/icon-find-64px.png
+Filename: ezdxf-1.3.1b1/src/ezdxf/resources/icon-find-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/resources/icon-goto-bookmark-64px.png
+Filename: ezdxf-1.3.1b1/src/ezdxf/resources/icon-goto-bookmark-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/resources/icon-goto-handle-64px.png
+Filename: ezdxf-1.3.1b1/src/ezdxf/resources/icon-goto-handle-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/resources/icon-goto-line-64px.png
+Filename: ezdxf-1.3.1b1/src/ezdxf/resources/icon-goto-line-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/resources/icon-left-arrow-64px.png
+Filename: ezdxf-1.3.1b1/src/ezdxf/resources/icon-left-arrow-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/resources/icon-next-entity-64px.png
+Filename: ezdxf-1.3.1b1/src/ezdxf/resources/icon-next-entity-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/resources/icon-prev-entity-64px.png
+Filename: ezdxf-1.3.1b1/src/ezdxf/resources/icon-prev-entity-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/resources/icon-right-arrow-64px.png
+Filename: ezdxf-1.3.1b1/src/ezdxf/resources/icon-right-arrow-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/resources/icon-show-in-tree-64px.png
+Filename: ezdxf-1.3.1b1/src/ezdxf/resources/icon-show-in-tree-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/resources/icon-store-bookmark-64px.png
+Filename: ezdxf-1.3.1b1/src/ezdxf/resources/icon-store-bookmark-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/sections/acdsdata.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/sections/acdsdata.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/sections/blocks.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/sections/blocks.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/sections/classes.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/sections/classes.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/sections/entities.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/sections/entities.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/sections/header.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/sections/header.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/sections/headervars.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/sections/headervars.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/sections/objects.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/sections/objects.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/sections/table.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/sections/table.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/sections/tables.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/sections/tables.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/sections/__init__.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/sections/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/tools/analyze.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/tools/analyze.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/tools/binarydata.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/tools/binarydata.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/tools/clipping_portal.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/tools/clipping_portal.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/tools/codepage.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/tools/codepage.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/tools/complex_ltype.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/tools/complex_ltype.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/tools/crypt.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/tools/crypt.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/tools/debug.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/tools/debug.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/tools/difftags.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/tools/difftags.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/tools/handle.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/tools/handle.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/tools/indexing.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/tools/indexing.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/tools/juliandate.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/tools/juliandate.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/tools/pattern.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/tools/pattern.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/tools/rawloader.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/tools/rawloader.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/tools/standards.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/tools/standards.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/tools/strip.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/tools/strip.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/tools/test.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/tools/test.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/tools/text.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/tools/text.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/tools/text_layout.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/tools/text_layout.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/tools/text_size.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/tools/text_size.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/tools/zipmanager.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/tools/zipmanager.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/tools/_iso_pattern.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/tools/_iso_pattern.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf/tools/__init__.py
+Filename: ezdxf-1.3.1b1/src/ezdxf/tools/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf.egg-info/dependency_links.txt
+Filename: ezdxf-1.3.1b1/src/ezdxf.egg-info/dependency_links.txt
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf.egg-info/entry_points.txt
+Filename: ezdxf-1.3.1b1/src/ezdxf.egg-info/entry_points.txt
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf.egg-info/not-zip-safe
+Filename: ezdxf-1.3.1b1/src/ezdxf.egg-info/not-zip-safe
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf.egg-info/PKG-INFO
+Filename: ezdxf-1.3.1b1/src/ezdxf.egg-info/PKG-INFO
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf.egg-info/requires.txt
+Filename: ezdxf-1.3.1b1/src/ezdxf.egg-info/requires.txt
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf.egg-info/SOURCES.txt
+Filename: ezdxf-1.3.1b1/src/ezdxf.egg-info/SOURCES.txt
 Comment: 
 
-Filename: ezdxf-1.3.1b0/src/ezdxf.egg-info/top_level.txt
+Filename: ezdxf-1.3.1b1/src/ezdxf.egg-info/top_level.txt
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/
+Filename: ezdxf-1.3.1b1/tests/test_03_dxf_layouts/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/
+Filename: ezdxf-1.3.1b1/tests/test_06_math/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_07_render/
+Filename: ezdxf-1.3.1b1/tests/test_07_render/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_09_cython_acceleration/
+Filename: ezdxf-1.3.1b1/tests/test_09_cython_acceleration/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_10_issues/
+Filename: ezdxf-1.3.1b1/tests/test_10_issues/
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/conftest.py
+Filename: ezdxf-1.3.1b1/tests/conftest.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_011_codepage.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_011_codepage.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_012_crypt.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_012_crypt.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_016_encoding.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_016_encoding.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_018_handle.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_018_handle.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_040_tags.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_040_tags.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_056_special_string_decoding.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_056_special_string_decoding.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_058_json_tags.py
+Filename: ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_058_json_tags.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_101_dxfnamespace.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_101_dxfnamespace.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_102_appdata.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_102_appdata.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_103_reactors.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_103_reactors.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_104_extension_dict.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_104_extension_dict.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_105_xdata.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_105_xdata.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_110_dxfentity.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_110_dxfentity.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_112a_dxfgfx.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_112a_dxfgfx.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_112b_dxfobj.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_112b_dxfobj.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_113_dxfclass.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_113_dxfclass.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_114_factory.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_114_factory.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_116_dictionary.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_116_dictionary.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_117_layer_table_entry.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_117_layer_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_118_appid_table_entry.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_118_appid_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_120_style_table_entry.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_120_style_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_122_vport_table_entry.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_122_vport_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_123_view_table_entry.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_123_view_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_125_image_def.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_125_image_def.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_126_image_def_reactor.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_126_image_def_reactor.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_127_raster_variables.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_127_raster_variables.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_128_pdf_definition.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_128_pdf_definition.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_129_xrecord.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_129_xrecord.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_130_id_buffer.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_130_id_buffer.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_131_field_list.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_131_field_list.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_132_layer_filter.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_132_layer_filter.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_133_sun.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_133_sun.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_134_material.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_134_material.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_135_geo_data.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_135_geo_data.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_136_vba_project.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_136_vba_project.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_137_sortentstable.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_137_sortentstable.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_139_user_record.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_139_user_record.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_140_block_record.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_140_block_record.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_141_layer_vp_override.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_141_layer_vp_override.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_142_copy_strategy.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_142_copy_strategy.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_143_spatial_filter.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_143_spatial_filter.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_144_roundtrip_xrecord.py
+Filename: ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_144_roundtrip_xrecord.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/conftest.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/conftest.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_200_line.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_200_line.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_201_point.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_201_point.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_202_circle.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_202_circle.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_203_arc.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_203_arc.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_204_shape.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_204_shape.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_205_solid.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_205_solid.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_206_text.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_206_text.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_207_attdef.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_207_attdef.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_208_attrib.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_208_attrib.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_209_vertex.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_209_vertex.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_1.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_210_polyline_1.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_2.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_210_polyline_2.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_explode.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_210_polyline_explode.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_211_viewport.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_211_viewport.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_212_insert.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_212_insert.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_213_minsert.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_213_minsert.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_214_block.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_214_block.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_215_dimension.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_215_dimension.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_221_ellipse.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_221_ellipse.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_222_xline.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_222_xline.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_223_ray.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_223_ray.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_224_group.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_224_group.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_225_mtext.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_225_mtext.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_226_spline.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_226_spline.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_228_mesh.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_228_mesh.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_231_underlay.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_231_underlay.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_231_underlay_2.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_231_underlay_2.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232a_add_acis.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_232a_add_acis.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232b_acis_export.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_232b_acis_export.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232c_acis_surface.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_232c_acis_surface.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232d_acis_copy.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_232d_acis_copy.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232e_acis_transform.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_232e_acis_transform.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_233_helix.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_233_helix.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_234_light.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_234_light.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_235_leader.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_235_leader.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_236_multileader.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_236_multileader.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_237_mline.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_237_mline.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_238_tolerance.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_238_tolerance.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_240_arc_dimension.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_240_arc_dimension.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_241_hyperlink.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_241_hyperlink.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_242_random_transform.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_242_random_transform.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_243_replace_entity.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_243_replace_entity.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_245_wipeout.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_245_wipeout.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_246_spline_audit.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_246_spline_audit.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_248_mpolygon.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_248_mpolygon.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_249_boundary_paths.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_249_boundary_paths.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_251_upright.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_251_upright.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_253_ole2frame.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_253_ole2frame.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_254_get_font_name.py
+Filename: ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_254_get_font_name.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_300_layout.py
+Filename: ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_300_layout.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
+Filename: ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_302_block_references.py
+Filename: ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_302_block_references.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_303_auto_block_references.py
+Filename: ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_303_auto_block_references.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_304_new_entity_space.py
+Filename: ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_304_new_entity_space.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
+Filename: ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
+Filename: ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_307_groupby.py
+Filename: ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_307_groupby.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_308_query.py
+Filename: ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_308_query.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_309_query_parser.py
+Filename: ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_309_query_parser.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
+Filename: ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_312_virtual_layout.py
+Filename: ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_312_virtual_layout.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_313_redraw_order.py
+Filename: ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_313_redraw_order.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_401_headersection.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_401_headersection.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_402_classessection.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_402_classessection.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_404a_tables.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_404a_tables.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_405_classes.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_405_classes.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_410_table.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_410_table.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_417_bbox.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_417_bbox.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_424_audit.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_424_audit.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_429_xclip.py
+Filename: ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_429_xclip.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/conftest.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/conftest.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_500_units.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_500_units.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_501_truecolor.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_501_truecolor.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_502_raw_color.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_502_raw_color.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_503_indexing.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_503_indexing.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_504_suppress_zeros.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_504_suppress_zeros.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_506_version.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_506_version.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_508_read_zip.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_508_read_zip.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_509_comments.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_509_comments.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_510_byte_stream.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_510_byte_stream.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_511_bit_stream.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_511_bit_stream.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_512_pattern.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_512_pattern.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_513_reorder_entities.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_513_reorder_entities.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_514_text.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_514_text.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_515a_fonts_truetype.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_515a_fonts_truetype.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_515b_fonts_shapefiles.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_515b_fonts_shapefiles.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_515c_fonts_lff.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_515c_fonts_lff.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_516_zoom.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_516_zoom.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_517_text_layout.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_517_text_layout.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_518_header_guid.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_518_header_guid.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_519_mtext_editor.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_519_mtext_editor.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_520_mtext_context.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_520_mtext_context.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_521_mtext_parser.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_521_mtext_parser.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_522_text_scanner.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_522_text_scanner.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_523_text_size.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_523_text_size.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_524_block_reference_manager.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_524_block_reference_manager.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_525_transparency.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_525_transparency.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_526_explode.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_526_explode.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_527_gfxattribs.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_527_gfxattribs.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_528_difftags.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_528_difftags.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_529_acis_sat.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_529_acis_sat.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_530_acis_sab.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_530_acis_sab.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_531_acis_entities.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_531_acis_entities.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_532_acis_mesh.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_532_acis_mesh.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_533_shapefiles.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_533_shapefiles.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_534_dwg_info.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_534_dwg_info.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_535_xref_basic.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_535_xref_basic.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_536_xref_conflict.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_536_xref_conflict.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_537_transform.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_537_transform.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_539_npshapes.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_539_npshapes.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_540_lff_parser.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_540_lff_parser.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_541_clipping_portal.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_541_clipping_portal.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_542_itertools.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_542_itertools.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_543_select.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_543_select.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_544_revcloud.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_544_revcloud.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_545_acis_cache.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_545_acis_cache.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_546_edgeminer.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_546_edgeminer.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_05_tools/test_547_edgesmith.py
+Filename: ezdxf-1.3.1b1/tests/test_05_tools/test_547_edgesmith.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/conftest.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/conftest.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_600_base.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_600_base.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_601_bulge.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_601_bulge.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_602_vec3.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_602_vec3.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_603_vec2.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_603_vec2.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_604_banded_matrix.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_604_banded_matrix.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_604_linalg.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_604_linalg.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_605_matrix44.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_605_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_606_convexhull.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_606_convexhull.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_607_perlin_noise.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_607_perlin_noise.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_608_intersection_line_line_2d.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_608_intersection_line_line_2d.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_609_point_on_line.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_609_point_on_line.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_610_ocs.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_610_ocs.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_611_ucs.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_611_ucs.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_612_ucs_pass_trough.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_612_ucs_pass_trough.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_613_is_point_in_polygon_2d.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_613_is_point_in_polygon_2d.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_614_construct_3d.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_614_construct_3d.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_615_rytz_axis.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_615_rytz_axis.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_616_plane.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_616_plane.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_617_clockwise_orientation.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_617_clockwise_orientation.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_618_clipping.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_618_clipping.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_619_greiner_hormann.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_619_greiner_hormann.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_620_knot.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_620_knot.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_621_bspline.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_621_bspline.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_622_bsplineu.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_622_bsplineu.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_623_rbspline.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_623_rbspline.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_624_global_bspline_interpolation.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_624_global_bspline_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_626_local_bspline_interpolation.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_626_local_bspline_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_627_bspline_basis.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_627_bspline_basis.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_629_bezier.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_629_bezier.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_630a_bezier4p_base.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_630a_bezier4p_base.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_630b_bezier4p_functions.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_630b_bezier4p_functions.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_631_euler_spiral.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_631_euler_spiral.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_632_bezier3p.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_632_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_640_bbox.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_640_bbox.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_641_construction_ray.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_641_construction_ray.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_642_construction_line.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_642_construction_line.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_643_construction_box.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_643_construction_box.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_644_construction_circle.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_644_construction_circle.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_645_construction_arc.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_645_construction_arc.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_646_offset_vertices_2d.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_646_offset_vertices_2d.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_647_transform_tools.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_647_transform_tools.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_648_construction_ellipse.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_648_construction_ellipse.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_650_elliptic_arc_span.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_650_elliptic_arc_span.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_651_construction_polyline.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_651_construction_polyline.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_652_approx_param_t.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_652_approx_param_t.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_653_polyline_intersection.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_653_polyline_intersection.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_654_rtree.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_654_rtree.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_655_dbscan.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_655_dbscan.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_656_k_means.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_656_k_means.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_657_mapbox_earcut.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_657_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_658_bevel_tools.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_658_bevel_tools.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_659_intersection_line_polygon_3d.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_659_intersection_line_polygon_3d.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_662_is_convex_polygon_2d.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_662_is_convex_polygon_2d.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_663_is_axes_aligned_rectange.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_663_is_axes_aligned_rectange.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_664_concave_clipping_polygon.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_664_concave_clipping_polygon.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_665_inverted_clipping_polygon.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_665_inverted_clipping_polygon.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_06_math/test_666_wgs84_transform.py
+Filename: ezdxf-1.3.1b1/tests/test_06_math/test_666_wgs84_transform.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_07_render/test_701_arrows.py
+Filename: ezdxf-1.3.1b1/tests/test_07_render/test_701_arrows.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_07_render/test_702_render_forms.py
+Filename: ezdxf-1.3.1b1/tests/test_07_render/test_702_render_forms.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_07_render/test_703_mesh_builder.py
+Filename: ezdxf-1.3.1b1/tests/test_07_render/test_703_mesh_builder.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_07_render/test_704_render_linear_dimension.py
+Filename: ezdxf-1.3.1b1/tests/test_07_render/test_704_render_linear_dimension.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_07_render/test_705_shape.py
+Filename: ezdxf-1.3.1b1/tests/test_07_render/test_705_shape.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_07_render/test_706_random_path.py
+Filename: ezdxf-1.3.1b1/tests/test_07_render/test_706_random_path.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_07_render/test_707_trace.py
+Filename: ezdxf-1.3.1b1/tests/test_07_render/test_707_trace.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_07_render/test_708a_path.py
+Filename: ezdxf-1.3.1b1/tests/test_07_render/test_708a_path.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_07_render/test_708b_path_tools.py
+Filename: ezdxf-1.3.1b1/tests/test_07_render/test_708b_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_07_render/test_708c_matplotlib_path_tools.py
+Filename: ezdxf-1.3.1b1/tests/test_07_render/test_708c_matplotlib_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_07_render/test_708d_qpainter_path_tools.py
+Filename: ezdxf-1.3.1b1/tests/test_07_render/test_708d_qpainter_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_07_render/test_708e_path_shapes.py
+Filename: ezdxf-1.3.1b1/tests/test_07_render/test_708e_path_shapes.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_07_render/test_708f_path_nesting.py
+Filename: ezdxf-1.3.1b1/tests/test_07_render/test_708f_path_nesting.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_07_render/test_709_linetype_renderer.py
+Filename: ezdxf-1.3.1b1/tests/test_07_render/test_709_linetype_renderer.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_07_render/test_711_points.py
+Filename: ezdxf-1.3.1b1/tests/test_07_render/test_711_points.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_07_render/test_712_render_curved_dimension.py
+Filename: ezdxf-1.3.1b1/tests/test_07_render/test_712_render_curved_dimension.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_07_render/test_713_mleader_builder.py
+Filename: ezdxf-1.3.1b1/tests/test_07_render/test_713_mleader_builder.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_07_render/test_714_mleader_render_engine.py
+Filename: ezdxf-1.3.1b1/tests/test_07_render/test_714_mleader_render_engine.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_07_render/test_715_hatching.py
+Filename: ezdxf-1.3.1b1/tests/test_07_render/test_715_hatching.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
+Filename: ezdxf-1.3.1b1/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_800_mtext_surrogate.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_800_mtext_surrogate.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_801_r12spline.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_801_r12spline.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_802_table_painter.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_802_table_painter.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_803_entities_to_code.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_803_entities_to_code.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_804_importer.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_804_importer.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_805_pycsg.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_805_pycsg.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_806_acadctb.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_806_acadctb.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_807_dwg_loader_basics.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_807_dwg_loader_basics.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_810_drawing_properties.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_810_drawing_properties.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_811a_drawing_frontend.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_811a_drawing_frontend.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_811b_drawing_recorder.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_811b_drawing_recorder.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_811c_viewport_processing.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_811c_viewport_processing.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_812_drawing_graphic_proxy.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_812_drawing_graphic_proxy.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_813_geo_interface.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_813_geo_interface.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_814_text2path.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_814_text2path.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_815_dxf_browser.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_815_dxf_browser.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_816_bin_packing.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_816_bin_packing.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_817_genetic_algorithm.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_817_genetic_algorithm.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_818_meshex.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_818_meshex.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_819_menger_sponge.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_819_menger_sponge.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_820_openscad.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_820_openscad.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_821_hpgl2.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_821_hpgl2.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_823_drawing_layout.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_823_drawing_layout.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_824_svg_drawing_backend.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_824_svg_drawing_backend.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_825_hpgl2_drawing_backend.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_825_hpgl2_drawing_backend.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_826_custom_json_backend.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_826_custom_json_backend.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_08_addons/test_827_geojson_backend.py
+Filename: ezdxf-1.3.1b1/tests/test_08_addons/test_827_geojson_backend.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_901_acc_vec2.py
+Filename: ezdxf-1.3.1b1/tests/test_09_cython_acceleration/test_901_acc_vec2.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_902_acc_vec3.py
+Filename: ezdxf-1.3.1b1/tests/test_09_cython_acceleration/test_902_acc_vec3.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+Filename: ezdxf-1.3.1b1/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+Filename: ezdxf-1.3.1b1/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+Filename: ezdxf-1.3.1b1/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+Filename: ezdxf-1.3.1b1/tests/test_09_cython_acceleration/test_906_acc_bspline.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_10_issues/test_issue_1078_bbox_calculation.py
+Filename: ezdxf-1.3.1b1/tests/test_10_issues/test_issue_1078_bbox_calculation.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_10_issues/test_issue_414_bbox_calculation.py
+Filename: ezdxf-1.3.1b1/tests/test_10_issues/test_issue_414_bbox_calculation.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+Filename: ezdxf-1.3.1b1/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_10_issues/test_issue_574_flattening_error.py
+Filename: ezdxf-1.3.1b1/tests/test_10_issues/test_issue_574_flattening_error.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+Filename: ezdxf-1.3.1b1/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_10_issues/test_issue_749_text_layout.py
+Filename: ezdxf-1.3.1b1/tests/test_10_issues/test_issue_749_text_layout.py
 Comment: 
 
-Filename: ezdxf-1.3.1b0/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
+Filename: ezdxf-1.3.1b1/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
 Comment: 
 
 Zip file comment:
```

## Comparing `ezdxf-1.3.1b0/LICENSE` & `ezdxf-1.3.1b1/LICENSE`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/PKG-INFO` & `ezdxf-1.3.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdxf
-Version: 1.3.1b0
+Version: 1.3.1b1
 Summary: A Python package to create/manipulate DXF drawings.
 Author-email: Manfred Moitzi <me@mozman.at>
 Project-URL: Repository, https://github.com/mozman/ezdxf
 Project-URL: Documentation, https://ezdxf.readthedocs.io
 Project-URL: Changelog, https://ezdxf.mozman.at/notes/#/page/changelog
 Project-URL: Forum, https://github.com/mozman/ezdxf/discussions
 Project-URL: Issues, https://github.com/mozman/ezdxf/issues
```

## Comparing `ezdxf-1.3.1b0/pyproject.toml` & `ezdxf-1.3.1b1/pyproject.toml`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/README.md` & `ezdxf-1.3.1b1/README.md`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/setup.py` & `ezdxf-1.3.1b1/setup.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/check_disable_c_ext_by_config_file.py` & `ezdxf-1.3.1b1/integration_tests/check_disable_c_ext_by_config_file.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/check_disable_c_ext_by_env_var.py` & `ezdxf-1.3.1b1/integration_tests/check_disable_c_ext_by_env_var.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_acad_table.py` & `ezdxf-1.3.1b1/integration_tests/test_acad_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_acis_entites.py` & `ezdxf-1.3.1b1/integration_tests/test_acis_entites.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_all_dimline_styles.py` & `ezdxf-1.3.1b1/integration_tests/test_all_dimline_styles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_all_ellipse_transformations.py` & `ezdxf-1.3.1b1/integration_tests/test_all_ellipse_transformations.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_anonymous_blocks.py` & `ezdxf-1.3.1b1/integration_tests/test_anonymous_blocks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_appsettings.py` & `ezdxf-1.3.1b1/integration_tests/test_appsettings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_audit_critical_dxf_files.py` & `ezdxf-1.3.1b1/integration_tests/test_audit_critical_dxf_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_audit_layouts.py` & `ezdxf-1.3.1b1/integration_tests/test_audit_layouts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_complex_line_type_2.py` & `ezdxf-1.3.1b1/integration_tests/test_complex_line_type_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_create_basic_graphics.py` & `ezdxf-1.3.1b1/integration_tests/test_create_basic_graphics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_document_guid.py` & `ezdxf-1.3.1b1/integration_tests/test_document_guid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_document_page_setup.py` & `ezdxf-1.3.1b1/integration_tests/test_document_page_setup.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_dxf_info_scanning.py` & `ezdxf-1.3.1b1/integration_tests/test_dxf_info_scanning.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_dynblkhelper.py` & `ezdxf-1.3.1b1/integration_tests/test_dynblkhelper.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_entities_iterator.py` & `ezdxf-1.3.1b1/integration_tests/test_entities_iterator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_fix_dulicate_handles.py` & `ezdxf-1.3.1b1/integration_tests/test_fix_dulicate_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_geo.py` & `ezdxf-1.3.1b1/integration_tests/test_geo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_groups.py` & `ezdxf-1.3.1b1/integration_tests/test_groups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_hpgl2_addon.py` & `ezdxf-1.3.1b1/integration_tests/test_hpgl2_addon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_ignore_junk_beyond_EOF.py` & `ezdxf-1.3.1b1/integration_tests/test_ignore_junk_beyond_EOF.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_launcher.py` & `ezdxf-1.3.1b1/integration_tests/test_launcher.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_leica_disto_r12.py` & `ezdxf-1.3.1b1/integration_tests/test_leica_disto_r12.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_load_dxf_unicode_notation.py` & `ezdxf-1.3.1b1/integration_tests/test_load_dxf_unicode_notation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_mapbox_earcut.py` & `ezdxf-1.3.1b1/integration_tests/test_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_mtext_columns.py` & `ezdxf-1.3.1b1/integration_tests/test_mtext_columns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_mtext_explode_addon.py` & `ezdxf-1.3.1b1/integration_tests/test_mtext_explode_addon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_mtext_text_frame.py` & `ezdxf-1.3.1b1/integration_tests/test_mtext_text_frame.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_new_table_entries.py` & `ezdxf-1.3.1b1/integration_tests/test_new_table_entries.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_none_ascii_read_write.py` & `ezdxf-1.3.1b1/integration_tests/test_none_ascii_read_write.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_odafc.py` & `ezdxf-1.3.1b1/integration_tests/test_odafc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_open_binary_DXF_files.py` & `ezdxf-1.3.1b1/integration_tests/test_open_binary_DXF_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_open_coord_order_issue.py` & `ezdxf-1.3.1b1/integration_tests/test_open_coord_order_issue.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_open_exotic_dxf_files.py` & `ezdxf-1.3.1b1/integration_tests/test_open_exotic_dxf_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_open_R13_R14.py` & `ezdxf-1.3.1b1/integration_tests/test_open_R13_R14.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_polyline_entity.py` & `ezdxf-1.3.1b1/integration_tests/test_polyline_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_preserve_binary_data_in_xrecords.py` & `ezdxf-1.3.1b1/integration_tests/test_preserve_binary_data_in_xrecords.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_r12export.py` & `ezdxf-1.3.1b1/integration_tests/test_r12export.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_r12strict.py` & `ezdxf-1.3.1b1/integration_tests/test_r12strict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_r12writer.py` & `ezdxf-1.3.1b1/integration_tests/test_r12writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_read_file_without_handles.py` & `ezdxf-1.3.1b1/integration_tests/test_read_file_without_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_read_write_modern_entites.py` & `ezdxf-1.3.1b1/integration_tests/test_read_write_modern_entites.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_recover.py` & `ezdxf-1.3.1b1/integration_tests/test_recover.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_redraw_order.py` & `ezdxf-1.3.1b1/integration_tests/test_redraw_order.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_rotated_block_attributes.py` & `ezdxf-1.3.1b1/integration_tests/test_rotated_block_attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_surface_entities.py` & `ezdxf-1.3.1b1/integration_tests/test_surface_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_write_fixed_meta_data.py` & `ezdxf-1.3.1b1/integration_tests/test_write_fixed_meta_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_write_without_handles.py` & `ezdxf-1.3.1b1/integration_tests/test_write_without_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_xref_detach.py` & `ezdxf-1.3.1b1/integration_tests/test_xref_detach.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/test_xref_load_acis.py` & `ezdxf-1.3.1b1/integration_tests/test_xref_load_acis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/AC1003_LINE_Example.dxf` & `ezdxf-1.3.1b1/integration_tests/data/AC1003_LINE_Example.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/acad_table_with_blk_ref.dxf` & `ezdxf-1.3.1b1/integration_tests/data/acad_table_with_blk_ref.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/ASCII_R12.dxf` & `ezdxf-1.3.1b1/integration_tests/data/ASCII_R12.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r12.dxf` & `ezdxf-1.3.1b1/integration_tests/data/bin_dxf_r12.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r13.dxf` & `ezdxf-1.3.1b1/integration_tests/data/bin_dxf_r13.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r14.dxf` & `ezdxf-1.3.1b1/integration_tests/data/bin_dxf_r14.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/bin_dxf_r2000.dxf` & `ezdxf-1.3.1b1/integration_tests/data/bin_dxf_r2000.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/cc_dxflib.dxf` & `ezdxf-1.3.1b1/integration_tests/data/cc_dxflib.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/custom_blocks.dxf` & `ezdxf-1.3.1b1/integration_tests/data/custom_blocks.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/duplicate_handles.dxf` & `ezdxf-1.3.1b1/integration_tests/data/duplicate_handles.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/dxf_unicode.dxf` & `ezdxf-1.3.1b1/integration_tests/data/dxf_unicode.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/dynblks.zip` & `ezdxf-1.3.1b1/integration_tests/data/dynblks.zip`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/empty_handles.dxf` & `ezdxf-1.3.1b1/integration_tests/data/empty_handles.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/groups.dxf` & `ezdxf-1.3.1b1/integration_tests/data/groups.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/layout_broken_links.dxf` & `ezdxf-1.3.1b1/integration_tests/data/layout_broken_links.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/layout_broken_links_2.dxf` & `ezdxf-1.3.1b1/integration_tests/data/layout_broken_links_2.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/layout_missing_block_definition.dxf` & `ezdxf-1.3.1b1/integration_tests/data/layout_missing_block_definition.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/layout_missing_block_record.dxf` & `ezdxf-1.3.1b1/integration_tests/data/layout_missing_block_record.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/Leica_Disto_S910.dxf` & `ezdxf-1.3.1b1/integration_tests/data/Leica_Disto_S910.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/MODEL.dxf` & `ezdxf-1.3.1b1/integration_tests/data/MODEL.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/mtext_columns_R2007.dxf` & `ezdxf-1.3.1b1/integration_tests/data/mtext_columns_R2007.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/mtext_columns_R2018.dxf` & `ezdxf-1.3.1b1/integration_tests/data/mtext_columns_R2018.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/mtext_framed_columns.dxf` & `ezdxf-1.3.1b1/integration_tests/data/mtext_framed_columns.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/mtext_text_frame.dxf` & `ezdxf-1.3.1b1/integration_tests/data/mtext_text_frame.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/no_layouts.dxf` & `ezdxf-1.3.1b1/integration_tests/data/no_layouts.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/PLOTFILE.plt` & `ezdxf-1.3.1b1/integration_tests/data/PLOTFILE.plt`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/POLI-ALL210_12.DXF` & `ezdxf-1.3.1b1/integration_tests/data/POLI-ALL210_12.DXF`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/recover01.dxf` & `ezdxf-1.3.1b1/integration_tests/data/recover01.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/recover02.dxf` & `ezdxf-1.3.1b1/integration_tests/data/recover02.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/small_r13.dxf` & `ezdxf-1.3.1b1/integration_tests/data/small_r13.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/small_r14.dxf` & `ezdxf-1.3.1b1/integration_tests/data/small_r14.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/XRECORD_0.bin` & `ezdxf-1.3.1b1/integration_tests/data/XRECORD_0.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/XRECORD_1.bin` & `ezdxf-1.3.1b1/integration_tests/data/XRECORD_1.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/integration_tests/data/XRECORD_2.bin` & `ezdxf-1.3.1b1/integration_tests/data/XRECORD_2.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/appsettings.py` & `ezdxf-1.3.1b1/src/ezdxf/appsettings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/audit.py` & `ezdxf-1.3.1b1/src/ezdxf/audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/bbox.py` & `ezdxf-1.3.1b1/src/ezdxf/bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/blkrefs.py` & `ezdxf-1.3.1b1/src/ezdxf/blkrefs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/colors.py` & `ezdxf-1.3.1b1/src/ezdxf/colors.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/commands.py` & `ezdxf-1.3.1b1/src/ezdxf/commands.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/comments.py` & `ezdxf-1.3.1b1/src/ezdxf/comments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/disassemble.py` & `ezdxf-1.3.1b1/src/ezdxf/disassemble.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/document.py` & `ezdxf-1.3.1b1/src/ezdxf/document.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/dwginfo.py` & `ezdxf-1.3.1b1/src/ezdxf/dwginfo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/dynblkhelper.py` & `ezdxf-1.3.1b1/src/ezdxf/dynblkhelper.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/edgeminer.py` & `ezdxf-1.3.1b1/src/ezdxf/edgeminer.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,57 +5,117 @@
 =========
 
 A module for detecting linked edges.
 
 The complementary module ezdxf.edgesmith can create entities from the output of this 
 module.
 
+Terminology
+-----------
+
+Edge
+    An edge has:
+        - unique id
+        - 3D start point
+        - 3D end point
+        - optional length
+        - optional payload (arbitrary data)
+
+    The geometry of an edge is not known.
+    Intersection points of edges are not known.
+
+Chain
+    A chain has sequential connected edges. 
+    The end point of an edge is connected to the start point of the following edge. 
+    A chain has unique edges, each edge appears only once in the chain. 
+    A solitary edge is also a chain.
+    Chains are represented as Sequence[Edge].
+
+Open Chain
+    An open chain is a chain with at least one loose end. 
+    A loose end is an edge point without a connection to other edges. 
+    A solitary edge is also an open chain.
+
+Loop
+    A loop is a chain with two or more edges.
+    The end point of the last edge is connected to the start point of the first edge.
+    A solitary edge is not a loop.
+
+Network
+    A network has two or more edges that are directly and indirectly connected. 
+    The edges in a network have no order.
+    A network can have junction points with two or more connected edges.
+    A solitary edge is not a network. 
+    A chain with two or more edges is a network. 
+    Networks are represented as Sequence[Edge].
+
+Gap Tolerance
+    Maximum vertex distance to consider two edges as connected
+
+Forward Connection
+    An edge is forward connected when the end point of the edge is connected to the 
+    start point of the following edge.
+
+Backwards Connection
+    An edge is backwards connected when the start point of the edge is connected to the 
+    end point of the previous edge.
+
 .. versionadded:: 1.4
 
 """
 from __future__ import annotations
 from typing import Any, Sequence, Iterator, Iterable, Dict, Tuple
 from typing_extensions import Self, TypeAlias
-from collections import defaultdict
 import time
 
 from ezdxf.math import UVec, Vec3, distance_point_line_3d
 from ezdxf.math import rtree
 
 
 __all__ = [
     "Edge",
     "EdgeDeposit",
+    "find_all_chains_in_deposit",
+    "find_all_chains",
     "find_all_loops_in_deposit",
     "find_all_loops",
     "find_all_sequential",
-    "find_first_loop_in_deposit",
-    "find_first_loop",
+    "find_chain_in_deposit",
+    "find_loop_in_deposit",
+    "find_loop",
+    "find_open_chains_in_deposit",
+    "find_open_chains",
     "find_sequential",
+    "flatten",
     "is_backwards_connected",
     "is_chain",
     "is_forward_connected",
     "is_loop",
+    "is_wrapped_chain",
     "length",
     "longest_chain",
-    "Network",
     "shortest_chain",
     "TimeoutError",
+    "unwrap_chain",
+    "wrap_chain",
 ]
-ABS_TOL = 1e-12
-GAP_TOL = 1e-12
+GAP_TOL = 1e-9
 TIMEOUT = 60.0  # in seconds
 
 
-class EdgeMinerException(Exception):
-    pass
+class EdgeMinerException(Exception): ...
+
+
+class InternalError(EdgeMinerException): ...
 
 
 class TimeoutError(EdgeMinerException):
-    pass
+    def __init__(self, msg: str, solutions: Sequence[Sequence[Edge]] = tuple()) -> None:
+        super().__init__(msg)
+        self.solutions = solutions
 
 
 class Edge:
     """Represents an edge.
 
     The edge can represent any linear curve (line, arc, spline,...).
     Therefore, the length of the edge must be specified if the length calculation for
@@ -91,18 +151,21 @@
     def __eq__(self, other) -> bool:
         """Return ``True`` if the ids of the edges are equal."""
         if isinstance(other, Edge):
             return self.id == other.id
         return False
 
     def __repr__(self) -> str:
-        if self.payload is None:
+        payload = self.payload
+        if payload is None:
             content = str(self.id)
+        elif isinstance(payload, EdgeWrapper):
+            content = "[" + (",".join(repr(e) for e in payload.edges)) + "]"
         else:
-            content = str(self.payload)
+            content = str(payload)
         return f"Edge({content})"
 
     def __hash__(self) -> int:
         # edges can be used in sets and set-operations
         return self.id
 
     def reversed(self) -> Self:
@@ -152,26 +215,29 @@
     Args:
         edges: sequence of edges
         gap_tol: maximum vertex distance to consider two edges as connected
     """
     return all(is_forward_connected(a, b, gap_tol) for a, b in zip(edges, edges[1:]))
 
 
-def is_loop(edges: Sequence[Edge], gap_tol=GAP_TOL, full=True) -> bool:
+def is_loop(edges: Sequence[Edge], gap_tol=GAP_TOL) -> bool:
     """Return ``True`` if the sequence of edges is a closed loop.
 
     Args:
         edges: sequence of edges
         gap_tol: maximum vertex distance to consider two edges as connected
-        full: does a full check if all edges have a forward connection if ``True``,
-            otherwise checks only if the last edge is connected to the first edge.
     """
-    if full and not is_chain(edges, gap_tol):
+    if not is_chain(edges, gap_tol):
         return False
-    return is_forward_connected(edges[-1], edges[0])
+    return isclose(edges[-1].end, edges[0].start, gap_tol)
+
+
+def is_loop_fast(edges: Sequence[Edge], gap_tol=GAP_TOL) -> bool:
+    """Internal fast loop check."""
+    return isclose(edges[-1].end, edges[0].start, gap_tol)
 
 
 def length(edges: Sequence[Edge]) -> float:
     """Returns the length of a sequence of edges."""
     return sum(e.length for e in edges)
 
 
@@ -202,16 +268,18 @@
         return sorted_chains[-1]
     return tuple()
 
 
 def find_sequential(edges: Sequence[Edge], gap_tol=GAP_TOL) -> Sequence[Edge]:
     """Returns all consecutive connected edges starting from the first edge.
 
-    The search stops at the first edge without a froward connection from the previous
-    edge.
+    The search stops at the first edge without a forward connection from the previous
+    edge. Edges are reversed if necessary to create a forward connection. This means
+    that the :attr:`Edge.reverse` flag is ``True`` ad start and end vertices are swapped,
+    the attached payload is not changed.
 
     Args:
         edges: edges to be examined
         gap_tol: maximum vertex distance to consider two edges as connected
 
     Raises:
         TypeError: invalid data in sequence `edges`
@@ -263,15 +331,15 @@
         self.start_time = time.perf_counter()
 
     @property
     def has_timed_out(self) -> bool:
         return time.perf_counter() - self.start_time > self.timeout
 
 
-def find_first_loop(
+def find_loop(
     edges: Sequence[Edge], gap_tol=GAP_TOL, timeout=TIMEOUT
 ) -> Sequence[Edge]:
     """Returns the first closed loop found in `edges`.
 
     .. note::
 
         Recursive backtracking algorithm with time complexity of O(n!).
@@ -281,21 +349,33 @@
         gap_tol: maximum vertex distance to consider two edges as connected
         timeout: timeout in seconds
 
     Raises:
         TimeoutError: search process has timed out
         TypeError: invalid data in sequence `edges`
     """
-    deposit = EdgeDeposit(edges, gap_tol=gap_tol)
+    chains = find_all_chains(edges, gap_tol)
+    if not chains:
+        return tuple()
+
+    packed_edges: list[Edge] = []
+    for chain in chains:
+        if len(chain) > 1:
+            if is_loop_fast(chain, gap_tol):
+                return chain
+            packed_edges.append(_wrap_chain(chain))
+        else:
+            packed_edges.append(chain[0])
+    deposit = EdgeDeposit(packed_edges, gap_tol)
     if len(deposit.edges) < 2:
         return tuple()
-    return find_first_loop_in_deposit(deposit, timeout=timeout)
+    return tuple(flatten(find_loop_in_deposit(deposit, timeout=timeout)))
 
 
-def find_first_loop_in_deposit(deposit: EdgeDeposit, timeout=TIMEOUT) -> Sequence[Edge]:
+def find_loop_in_deposit(deposit: EdgeDeposit, timeout=TIMEOUT) -> Sequence[Edge]:
     """Returns the first closed loop found in edge `deposit`.
 
     .. note::
 
         Recursive backtracking algorithm with time complexity of O(n!).
 
     Args:
@@ -304,20 +384,19 @@
 
     Raises:
         TimeoutError: search process has timed out
     """
 
     if len(deposit.edges) < 2:
         return tuple()
-    networks = list(deposit.build_all_networks(timeout=timeout))
-    for network in networks:
-        finder = LoopFinder(network, timeout=timeout)
-        loop = finder.find_any_loop()
-        if loop:
-            return loop
+
+    finder = LoopFinder(deposit, timeout=timeout)
+    loop = finder.find_any_loop()
+    if loop:
+        return loop
     return tuple()
 
 
 def find_all_loops(
     edges: Sequence[Edge], gap_tol=GAP_TOL, timeout=TIMEOUT
 ) -> Sequence[Sequence[Edge]]:
     """Returns all unique closed loops and doesn't include reversed solutions.
@@ -331,18 +410,45 @@
         gap_tol: maximum vertex distance to consider two edges as connected
         timeout: timeout in seconds
 
     Raises:
         TimeoutError: search process has timed out
         TypeError: invalid data in sequence `edges`
     """
-    deposit = EdgeDeposit(edges, gap_tol=gap_tol)
+    chains = find_all_chains(edges, gap_tol)
+    if not chains:
+        return tuple()
+
+    solutions: list[Sequence[Edge]] = []
+    packed_edges: list[Edge] = []
+    for chain in chains:
+        if len(chain) > 1:
+            if is_loop_fast(chain, gap_tol):
+                # these loops have no ambiguities (junctions)
+                solutions.append(chain)
+            else:
+                packed_edges.append(_wrap_chain(chain))
+        else:
+            packed_edges.append(chain[0])
+
+    if not packed_edges:
+        return solutions
+
+    deposit = EdgeDeposit(packed_edges, gap_tol)
     if len(deposit.edges) < 2:
         return tuple()
-    return find_all_loops_in_deposit(deposit, timeout=timeout)
+    try:
+        result = find_all_loops_in_deposit(deposit, timeout=timeout)
+    except TimeoutError as err:
+        if err.solutions:
+            solutions.extend(err.solutions)
+            err.solutions = solutions
+        raise
+    solutions.extend(result)
+    return _unwrap_chains(solutions)
 
 
 def find_all_loops_in_deposit(
     deposit: EdgeDeposit, timeout=TIMEOUT
 ) -> Sequence[Sequence[Edge]]:
     """Returns all unique closed loops in found in the edge `deposit` and doesn't
     include reversed solutions.
@@ -354,110 +460,81 @@
     Args:
         deposit: edge deposit
         timeout: timeout in seconds
 
     Raises:
         TimeoutError: search process has timed out
     """
-    gap_tol = deposit.gap_tol
     solutions: list[Sequence[Edge]] = []
-    for network in deposit.build_all_networks(timeout=timeout):
-        finder = LoopFinder(network, gap_tol=gap_tol, timeout=timeout)
-        for edge in network:
-            finder.search(edge)
-        solutions.extend(finder)
+    finder = LoopFinder(deposit, timeout=timeout)
+    for edge in deposit.edges:
+        finder.search(edge)
+    solutions.extend(finder)
     return solutions
 
 
 def type_check(edges: Sequence[Edge]) -> Sequence[Edge]:
     for edge in edges:
         if not isinstance(edge, Edge):
             raise TypeError(f"expected type <Edge>, got {str(type(edge))}")
     return edges
 
 
-class EdgeVertexIndex:
-    """Index of edges referenced by the id of their start- and end vertices.
+class EdgeVertex(Vec3):
+    # for unknown reasons super().__init__(location) doesn't work, therefor no
+    # EdgeVertex.__init__(self, location: Vec3, edge: Edge) constructor
+    edge: Edge
 
-    .. important::
 
-        The id of the vertices is indexed not the location!
-
-    (internal class)
-    """
-
-    def __init__(self, edges: Sequence[Edge]) -> None:
-        index: dict[int, Edge] = {}
-        for edge in edges:
-            index[id(edge.start)] = edge
-            index[id(edge.end)] = edge
-        self._index = index
-
-    def find_edges(self, vertices: Iterable[Vec3]) -> Sequence[Edge]:
-        """Returns all edges referenced by the id of given vertices."""
-        index = self._index
-        edges: list[Edge] = []
-        for vertex in vertices:
-            edge = index.get(id(vertex))
-            if edge:
-                edges.append(edge)
-        return edges
+def make_edge_vertex(location: Vec3, edge: Edge) -> EdgeVertex:
+    edge_vertex = EdgeVertex(location)
+    edge_vertex.edge = edge
+    return edge_vertex
 
 
 class SpatialSearchIndex:
     """Spatial search index of all edge vertices.
 
     (internal class)
     """
 
     def __init__(self, edges: Sequence[Edge]) -> None:
-        vertices: list[Vec3] = []
+        vertices: list[EdgeVertex] = []
         for edge in edges:
-            vertices.append(edge.start)
-            vertices.append(edge.end)
+            vertices.append(make_edge_vertex(edge.start, edge))
+            vertices.append(make_edge_vertex(edge.end, edge))
         self._search_tree = rtree.RTree(vertices)
 
-    def vertices_in_sphere(self, center: Vec3, radius: float) -> Sequence[Vec3]:
+    def vertices_in_sphere(self, center: Vec3, radius: float) -> Sequence[EdgeVertex]:
         """Returns all vertices located around `center` with a max. distance of `radius`."""
-        return tuple(self._search_tree.points_in_sphere(center, radius))  # type: ignore
+        return tuple(self._search_tree.points_in_sphere(center, radius))
 
-    def nearest_vertex(self, location: Vec3) -> Vec3:
+    def nearest_vertex(self, location: Vec3) -> EdgeVertex:
         """Returns the nearest vertex to the given location."""
         vertex, _ = self._search_tree.nearest_neighbor(location)
-        return vertex  # type: ignore
-
-
-def discard_edges(edges: Iterable[Edge], discard: Iterable[Edge]) -> Sequence[Edge]:
-    return discard_ids(edges, ids=set(e.id for e in discard))
-
-
-def discard_ids(edges: Iterable[Edge], ids: set[int]) -> Sequence[Edge]:
-    return tuple(e for e in edges if e.id not in ids)
+        return vertex
 
 
 class EdgeDeposit:
     """The edge deposit stores all available edges for further searches."""
 
     def __init__(self, edges: Sequence[Edge], gap_tol=GAP_TOL) -> None:
         self.gap_tol = gap_tol
         self.edges = type_check(tuple(edges))
-        self.edge_index = EdgeVertexIndex(self.edges)
         self.search_index = SpatialSearchIndex(self.edges)
 
     def edges_linked_to(self, vertex: UVec, radius: float = -1) -> Sequence[Edge]:
         """Returns all edges linked to `vertex` in range of `radius`.
 
         Default radius is :attr:`self.gap_tol`.
         """
         if radius < 0:
             radius = self.gap_tol
         vertices = self.search_index.vertices_in_sphere(Vec3(vertex), radius)
-        if not vertices:
-            return tuple()
-        return self.edge_index.find_edges(vertices)
+        return tuple(v.edge for v in vertices)
 
     def find_nearest_edge(self, vertex: UVec) -> Edge | None:
         """Return the nearest edge to the given vertex.
 
         The distance is measured to the connection line from start to end of the edge.
         This is not correct for edges that represent arcs or splines.
         """
@@ -469,187 +546,147 @@
         si = self.search_index
         nearest_vertex = si.nearest_vertex(vertex)
         edges = self.edges_linked_to(nearest_vertex)
         if edges:
             return min(edges, key=distance)
         return None
 
-    def build_network(self, edge: Edge, timeout=TIMEOUT) -> Network:
+    def find_network(self, edge: Edge) -> set[Edge]:
         """Returns the network of all edges that are directly and indirectly linked to
-        `edge`.
-
-        Raises:
-            TimeoutError: build process has timed out
+        `edge`.  A network has two or more edges, a solitary edge is not a network.
         """
 
         def process(vertex: Vec3) -> None:
-            linked_edges = self.edges_linked_to(vertex)
-            linked_edges = discard_ids(linked_edges, ids=done)
+            linked_edges = set(self.edges_linked_to(vertex)) - network
             if linked_edges:
-                network.add_connections(edge, linked_edges)
+                network.update(linked_edges)
                 todo.extend(linked_edges)
 
-        network = Network()
-        done: set[int] = set()
         todo: list[Edge] = [edge]
-        watchdog = Watchdog(timeout)
-
+        network: set[Edge] = set(todo)
         while todo:
-            if watchdog.has_timed_out:
-                raise TimeoutError("build process has timed out")
             edge = todo.pop()
-            done.add(edge.id)
             process(edge.start)
             process(edge.end)
+        if len(network) > 1:  # a network requires two or more edges
+            return network
+        return set()
 
-        return network
-
-    def build_all_networks(self, timeout=TIMEOUT) -> Sequence[Network]:
+    def find_all_networks(self) -> Sequence[set[Edge]]:
         """Returns all separated networks in this deposit in ascending order of edge
         count.
-
-        Raises:
-            TimeoutError: build process has timed out
         """
-        watchdog = Watchdog(timeout)
         edges = set(self.edges)
-        networks: list[Network] = []
+        networks: list[set[Edge]] = []
         while edges:
-            if watchdog.has_timed_out:
-                raise TimeoutError("search process has timed out")
             edge = edges.pop()
-            network = self.build_network(edge, timeout=timeout)
+            network = self.find_network(edge)
             if len(network):
                 networks.append(network)
-                edges -= set(network)
+                edges -= network
             else:  # solitary edge
                 edges.discard(edge)
 
         networks.sort(key=lambda n: len(n))
         return networks
 
-
-class Network:
-    """The all edges in a network are reachable from every other edge."""
-
-    def __init__(self) -> None:
-        self._edges: dict[int, Edge] = {}
-        self._connections: dict[int, set[int]] = defaultdict(set)
-
-    def __repr__(self) -> str:
-        content = ",".join(str(e) for e in self)
-        return f"Network([{content}])"
-
-    def __len__(self) -> int:
-        return len(self._edges)
-
-    def __iter__(self) -> Iterator[Edge]:
-        return iter(self._edges.values())
-
-    def __contains__(self, edge: Edge) -> bool:
-        return edge.id in self._edges
-
-    def add_connection(self, base: Edge, target: Edge) -> None:
-        if base.id == target.id:
-            return
-        self._edges[base.id] = base
-        self._edges[target.id] = target
-        self._connections[base.id].add(target.id)
-        self._connections[target.id].add(base.id)
-
-    def add_connections(self, base: Edge, targets: Iterable[Edge]) -> None:
-        for target in targets:
-            self.add_connection(base, target)
-
-    def edges_linked_to(self, edge: Edge) -> Sequence[Edge]:
-        return tuple(self._edges[eid] for eid in self._connections[edge.id])
+    def find_loose_ends(self) -> Iterator[Edge]:
+        """Yields all edges that have at least one end point without connection to other
+        edges.
+        """
+        for edge in self.edges:
+            if len(self.edges_linked_to(edge.start)) == 1:
+                yield edge
+            elif len(self.edges_linked_to(edge.end)) == 1:
+                yield edge
 
 
 SearchSolutions: TypeAlias = Dict[Tuple[int, ...], Sequence[Edge]]
 
 
 class LoopFinder:
-    """Find closed loops in a network by a recursive backtracking algorithm.
+    """Find closed loops in an EdgeDeposit by a recursive backtracking algorithm.
 
     (internal class)
     """
 
-    def __init__(
-        self, network: Network, discard_reverse=True, gap_tol=GAP_TOL, timeout=TIMEOUT
-    ) -> None:
-        if len(network) < 2:
-            raise ValueError("two or more network nodes required")
-        self._network = network
-        self._discard_reverse_solutions = discard_reverse
-        self._gap_tol = gap_tol
+    def __init__(self, deposit: EdgeDeposit, timeout=TIMEOUT) -> None:
+        if len(deposit.edges) < 2:
+            raise ValueError("two or more edges required")
+        self._deposit = deposit
         self._timeout = timeout
         self._solutions: SearchSolutions = {}
 
+    @property
+    def gap_tol(self) -> float:
+        return self._deposit.gap_tol
+
     def __iter__(self) -> Iterator[Sequence[Edge]]:
         return iter(self._solutions.values())
 
     def __len__(self) -> int:
         return len(self._solutions)
 
     def find_any_loop(self, start: Edge | None = None) -> Sequence[Edge]:
         """Returns the first loop found beginning with the given start edge or an
         arbitrary edge if `start` is None.
         """
         if start is None:
-            start = next(iter(self._network))
+            start = self._deposit.edges[0]
 
         self.search(start, stop_at_first_loop=True)
         try:
             return next(iter(self._solutions.values()))
         except StopIteration:
             return tuple()
 
     def search(self, start: Edge, stop_at_first_loop: bool = False) -> None:
         """Searches for all loops that begin at the given start edge.
 
-        These are not all possible loops in a network!
-        """
-        if start not in self._network:
-            raise ValueError("start edge not in network")
-        network = self._network
-        gap_tol = self._gap_tol
+        These are not all possible loops in the edge deposit!
+
+        Raises:
+            TimeoutError: search process has timed out, intermediate results are attached
+                TimeoutError.data
 
+        """
+        deposit = self._deposit
+        gap_tol = self.gap_tol
+        start_point = start.start
         watchdog = Watchdog(self._timeout)
         todo: list[tuple[Edge, ...]] = [(start,)]  # "unlimited" recursion stack
         while todo:
             if watchdog.has_timed_out:
-                raise TimeoutError("search process has timed out")
+                raise TimeoutError(
+                    "search process has timed out",
+                    solutions=tuple(self._solutions.values()),
+                )
             chain = todo.pop()
             last_edge = chain[-1]
             end_point = last_edge.end
-            candidates = network.edges_linked_to(last_edge)
+            candidates = deposit.edges_linked_to(end_point, radius=gap_tol)
             # edges must be unique in a loop
-            for edge in set(candidates) - set(chain):
+            survivers = set(candidates) - set(chain)
+            for edge in survivers:
                 if isclose(end_point, edge.start, gap_tol):
-                    extended_chain = chain + (edge,)
-                elif isclose(end_point, edge.end, gap_tol):
-                    extended_chain = chain + (edge.reversed(),)
+                    last_edge = edge
                 else:
-                    continue
-                if is_forward_connected(extended_chain[-1], start, gap_tol):
+                    last_edge = edge.reversed()
+                extended_chain = chain + (last_edge,)
+                if isclose(last_edge.end, start_point, gap_tol):
                     self.add_solution(extended_chain)
                     if stop_at_first_loop:
                         return
                 else:
                     todo.append(extended_chain)
 
     def add_solution(self, loop: Sequence[Edge]) -> None:
         solutions = self._solutions
         key = loop_key(loop)
-        if key in solutions:
-            return
-        if (
-            self._discard_reverse_solutions
-            and loop_key(loop, reverse=True) in solutions
-        ):
+        if key in solutions or loop_key(loop, reverse=True) in solutions:
             return
         solutions[key] = loop
 
 
 def loop_key(edges: Sequence[Edge], reverse=False) -> tuple[int, ...]:
     """Returns a normalized key.
 
@@ -659,7 +696,276 @@
         ids = tuple(edge.id for edge in reversed(edges))
     else:
         ids = tuple(edge.id for edge in edges)
     index = ids.index(min(ids))
     if index:
         ids = ids[index:] + ids[:index]
     return ids
+
+
+def find_all_chains(edges: Sequence[Edge], gap_tol=GAP_TOL) -> Sequence[Sequence[Edge]]:
+    """Returns all sequences of connected edges and doesn't include reversed solutions.
+    The chains are broken at junctions, which means that all sequences have a linear
+    progression without ambiguities.
+
+    Args:
+        edges: sequence of edges
+        gap_tol: maximum vertex distance to consider two edges as connected
+
+    Raises:
+        TypeError: invalid data in sequence `edges`
+    """
+    deposit = EdgeDeposit(edges, gap_tol=gap_tol)
+    if len(deposit.edges) < 1:
+        return tuple()
+    return find_all_chains_in_deposit(deposit)
+
+
+def find_all_chains_in_deposit(deposit: EdgeDeposit) -> Sequence[Sequence[Edge]]:
+    """Returns all sequences of connected edges in the edge `deposit` and doesn't
+    include reversed solutions.  The chains are broken at junctions, which means that
+    all sequences have a linear progression without ambiguities.
+    """
+    if len(deposit.edges) < 1:
+        return tuple()
+    solutions: list[Sequence[Edge]] = []
+    edges = set(deposit.edges)
+    while edges:
+        chain = find_chain_in_deposit(deposit, edges.pop())
+        solutions.append(chain)
+        edges -= set(chain)
+    return solutions
+
+
+def find_chain_in_deposit(deposit: EdgeDeposit, start: Edge) -> Sequence[Edge]:
+    """Returns the chain containing the `start` edge."""
+    forward_chain = _find_forward_chain(deposit, start)
+    if is_loop_fast(forward_chain, deposit.gap_tol):
+        return forward_chain
+    backwards_chain = _find_forward_chain(deposit, start.reversed())
+    if len(backwards_chain) == 1:
+        return forward_chain
+    backwards_chain.reverse()
+    backwards_chain.pop()  # reversed start
+    return [edge.reversed() for edge in backwards_chain] + forward_chain
+
+
+def _find_forward_chain(deposit: EdgeDeposit, edge: Edge) -> list[Edge]:
+    gap_tol = deposit.gap_tol
+    chain = [edge]
+    while True:
+        last = chain[-1]
+        linked = deposit.edges_linked_to(last.end, gap_tol)
+        if len(linked) != 2:  # no junctions allowed!
+            return chain
+        if linked[0] == last:
+            edge = linked[1]
+        else:
+            edge = linked[0]
+        if isclose(last.end, edge.start, gap_tol):
+            chain.append(edge)
+        else:
+            chain.append(edge.reversed())
+        if is_loop_fast(chain, gap_tol):
+            return chain
+
+
+def is_wrapped_chain(edge: Edge) -> bool:
+    """Returns ``True`` if `edge` is a wrapper for linked edges."""
+    return isinstance(edge.payload, EdgeWrapper)
+
+
+def wrap_chain(chain: Sequence[Edge], gap_tol=GAP_TOL) -> Edge:
+    """Wraps a sequence of linked edges into a single edge.
+
+    Two or more linked edges required. Closed loops cannot be wrapped into a single
+    edge.
+
+    Raises:
+        ValueError: less than two edges; not a chain; chain is a closed loop
+
+    """
+    if len(chain) < 2:
+        raise ValueError("two or more linked edges required")
+    if is_chain(chain, gap_tol):
+        if is_loop_fast(chain, gap_tol):
+            raise ValueError("closed loop cannot be wrapped into a single edge")
+        return _wrap_chain(chain)
+    raise ValueError("edges are not connected")
+
+
+def unwrap_chain(edge: Edge) -> Sequence[Edge]:
+    """Unwraps linked edges which are wrapped into a single edge."""
+    if isinstance(edge.payload, EdgeWrapper):
+        return _unwrap_chain(edge)
+    return (edge,)
+
+
+class EdgeWrapper:
+    """Internal class to wrap a sequence of linked edges."""
+
+    __slots__ = ("edges",)
+
+    def __init__(self, edges: Sequence[Edge]) -> None:
+        self.edges: Sequence[Edge] = tuple(edges)
+
+
+def _wrap_chain(edges: Sequence[Edge]) -> Edge:
+    return Edge(
+        edges[0].start, edges[-1].end, length(edges), payload=EdgeWrapper(edges)
+    )
+
+
+def _unwrap_chain(edge: Edge) -> Sequence[Edge]:
+    wrapper = edge.payload
+    assert isinstance(wrapper, EdgeWrapper)
+    if edge.reverse:
+        return tuple(e.reversed() for e in reversed(wrapper.edges))
+    else:
+        return wrapper.edges
+
+
+def _unwrap_chains(chains: Iterable[Iterable[Edge]]) -> Sequence[Sequence[Edge]]:
+    return tuple(tuple(flatten(chain)) for chain in chains)
+
+
+def flatten(edges: Edge | Iterable[Edge]) -> Iterator[Edge]:
+    """Yields all edges from any nested structure of edges as a flat stream of edges."""
+    edge: Edge
+    if not isinstance(edges, Edge):
+        for edge in edges:
+            yield from flatten(edge)
+    else:
+        edge = edges
+        if is_wrapped_chain(edge):
+            yield from flatten(_unwrap_chain(edge))
+        else:
+            yield edge
+
+
+def find_open_chains(
+    edges: Sequence[Edge], gap_tol=GAP_TOL, timeout=TIMEOUT
+) -> Sequence[Sequence[Edge]]:
+    """Returns all combinations of edges which create open chains with at least one
+    loose end.
+
+    A loose end is an edge end-point without further connections.  The result does not
+    include reversed solutions and closed loops.
+
+    .. note::
+
+        Recursive backtracking algorithm with time complexity of O(n!).
+
+    Args:
+        edges: sequence of edges
+        gap_tol: maximum vertex distance to consider two edges as connected
+        timeout: timeout in seconds
+
+    Raises:
+        TypeError: invalid data in sequence `edges`
+        TimeoutError: search process has timed out
+    """
+    return find_open_chains_in_deposit(EdgeDeposit(edges, gap_tol=gap_tol), timeout)
+
+
+def chain_key(edges: Sequence[Edge], reverse=False) -> tuple[int, ...]:
+    """Returns a normalized key."""
+    if reverse:
+        return tuple(edge.id for edge in reversed(edges))
+    else:
+        return tuple(edge.id for edge in edges)
+
+
+def find_open_chains_in_deposit(
+    deposit: EdgeDeposit, timeout=TIMEOUT
+) -> Sequence[Sequence[Edge]]:
+    """Returns all combinations of edges in deposit which create open chains with at
+    least one loose end.
+
+    A loose end is an edge end-point without further connections.  The result does not
+    include reversed solutions and closed loops
+
+    .. note::
+
+        Recursive backtracking algorithm with time complexity of O(n!).
+
+    Args:
+        edosit: EdgeDeposit
+        timeout: timeout in seconds
+
+    Raises:
+        TimeoutError: search process has timed out
+    """
+
+    finder = OpenChainFinder(deposit, timeout)
+    for edge in deposit.find_loose_ends():
+        finder.search(edge)
+    solutions = finder.solutions
+    solutions.sort(key=lambda x: len(x))
+    return solutions
+
+
+class OpenChainFinder:
+    def __init__(self, deposit: EdgeDeposit, timeout=TIMEOUT):
+        self.deposit = deposit
+        self.solution_keys: set[tuple[int, ...]] = set()
+        self.solutions: list[Sequence[Edge]] = []
+        self.watchdog = Watchdog(timeout)
+
+    def search(self, edge: Edge) -> None:
+        forward_chains = self.forward_search(edge)
+        self.reverse_search(forward_chains)
+
+    def forward_search(self, edge: Edge) -> list[tuple[Edge, ...]]:
+        deposit = self.deposit
+        gap_tol = deposit.gap_tol
+        watchdog = self.watchdog
+
+        forward_chains: list[tuple[Edge, ...]] = []
+        todo: list[tuple[Edge, ...]] = [(edge,)]
+        while todo:
+            if watchdog.has_timed_out:
+                raise TimeoutError("search has timed out")
+            chain = todo.pop()
+            start_point = chain[-1].end
+            candidates = deposit.edges_linked_to(start_point)
+            backwards_edges = set(candidates) - set(chain)
+            if backwards_edges:
+                for edge in backwards_edges:
+                    if not isclose(start_point, edge.start, gap_tol):
+                        edge = edge.reversed()
+                    todo.append(chain + (edge,))
+            else:
+                forward_chains.append(chain)
+        return forward_chains
+
+    def reverse_search(self, forward_chains: list[tuple[Edge, ...]]) -> None:
+        deposit = self.deposit
+        gap_tol = deposit.gap_tol
+        watchdog = self.watchdog
+        todo = forward_chains
+        while todo:
+            if watchdog.has_timed_out:
+                raise TimeoutError("search has timed out", solutions=self.solutions)
+            chain = todo.pop()
+            start_point = chain[0].start
+            candidates = deposit.edges_linked_to(start_point)
+            backwards_edges = set(candidates) - set(chain)
+            if backwards_edges:
+                for edge in backwards_edges:
+                    if not isclose(start_point, edge.end, gap_tol):
+                        edge = edge.reversed()
+                    todo.append((edge,) + chain)
+            else:
+                self.add_solution(chain)
+
+    def add_solution(self, solution: Sequence[Edge]) -> None:
+        keys = self.solution_keys
+        key = chain_key(solution)
+        if key in keys:
+            return
+        keys.add(key)
+        key = chain_key(solution, reverse=True)
+        if key in keys:
+            return
+        keys.add(key)
+        self.solutions.append(solution)
```

## Comparing `ezdxf-1.3.1b0/src/ezdxf/edgesmith.py` & `ezdxf-1.3.1b1/src/ezdxf/lldxf/fileindex.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,150 +1,158 @@
-# Copyright (c) 2024, Manfred Moitzi
+# Copyright (c) 2020-2022, Manfred Moitzi
 # License: MIT License
-"""
-EdgeSmith
-=========
+from __future__ import annotations
+from typing import Iterable, NamedTuple, BinaryIO
 
-A module for creating entities like polylines and hatch boundary paths from linked edges.
+from .const import DXFStructureError
+from ezdxf.tools.codepage import toencoding
 
-The complementary module to ezdxf.edgeminer.
 
-.. versionadded:: 1.4
+class IndexEntry(NamedTuple):
+    code: int
+    value: str
+    location: int
+    line: int
 
-"""
-from __future__ import annotations
-from typing import Iterator, Iterable
-import math
 
-from ezdxf.edgeminer import Edge, GAP_TOL, ABS_TOL
-from ezdxf import entities as et
-from ezdxf.math import arc_angle_span_deg, ellipse_param_span, Vec2, Vec3
-
-__all__ = ["is_closed_entity", "edge_from_entity"]
-
-
-def is_closed_entity(entity: et.DXFEntity) -> bool:
-    """Returns ``True`` if the given entity represents a closed loop."""
-    if isinstance(entity, et.Arc):  # Arc inherits from Circle!
-        radius = abs(entity.dxf.radius)
-        start_angle = entity.dxf.start_angle
-        end_angle = entity.dxf.end_angle
-        angle_span = arc_angle_span_deg(start_angle, end_angle)
-        return abs(radius) > ABS_TOL and math.isclose(
-            angle_span, 360.0, abs_tol=ABS_TOL
-        )
-    if isinstance(entity, et.Circle):
-        return abs(entity.dxf.radius) > ABS_TOL
-
-    if isinstance(entity, et.Ellipse):
-        start_param = entity.dxf.start_param
-        end_param = entity.dxf.end_param
-        span = ellipse_param_span(start_param, end_param)
-        if not math.isclose(span, math.tau, abs_tol=ABS_TOL):
-            return False
-        return True
+class FileStructure:
+    """DXF file structure representation stored as file locations.
+
+    Store all DXF structure tags and some other tags as :class:`IndexEntry`
+    tuples:
+
+        - code: group code
+        - value: tag value as string
+        - location: file location as int
+        - line: line number as int
+
+    Indexed tags:
+
+        - structure tags, every tag with group code 0
+        - section names, (2, name) tag following a (0, SECTION) tag
+        - entity handle tags with group code 5, the DIMSTYLE handle group code
+          105 is also stored as group code 5
 
-    if isinstance(entity, et.Spline):
-        try:
-            bspline = entity.construction_tool()
-        except ValueError:
-            return False
-        control_points = bspline.control_points
-        if len(control_points) < 3:
-            return False
-        start = control_points[0]
-        end = control_points[-1]
-        return start.isclose(end, abs_tol=ABS_TOL)
-
-    if isinstance(entity, et.LWPolyline):
-        if len(entity) < 1:
-            return False
-        if entity.closed is True:
-            return True
-        start = Vec2(entity.lwpoints[0][:2])
-        end = Vec2(entity.lwpoints[-1][:2])
-        return start.isclose(end, abs_tol=ABS_TOL)
-
-    if isinstance(entity, et.Polyline):
-        if entity.is_2d_polyline or entity.is_3d_polyline:
-            # Note: does not check if all vertices of a 3D polyline are placed on a
-            # common plane.
-            vertices = entity.vertices
-            if len(vertices) < 2:
-                return False
-            if entity.is_closed:
-                return True
-            p0: Vec3 = vertices[0].dxf.location  # type: ignore
-            p1: Vec3 = vertices[-1].dxf.location  # type: ignore
-            if p0.isclose(p1, abs_tol=ABS_TOL):
-                return True
-        return False
-    return False
-
-
-def edge_from_entity(entity: et.DXFEntity, gap_tol=GAP_TOL) -> Edge | None:
-    """Makes an :class:`Edge` instance for the DXF entity types LINE, ARC, ELLIPSE and
-    SPLINE if the entity is an open linear curve.  Returns ``None`` if the entity
-    is a closed curve or cannot represent an edge.
     """
-    edge: Edge | None = None
 
-    if isinstance(entity, et.Line):
-        start = Vec3(entity.dxf.start)
-        end = Vec3(entity.dxf.end)
-        length = start.distance(end)
-        edge = Edge(start, end, length, entity)
-    elif isinstance(entity, et.Arc):
-        try:
-            ct0 = entity.construction_tool()
-        except ValueError:
-            return None
-        radius = abs(ct0.radius)
-        if radius < ABS_TOL:
-            return None
-        span_deg = arc_angle_span_deg(ct0.start_angle, ct0.end_angle)
-        length = radius * span_deg / 180.0 * math.pi
-        edge = Edge(ct0.start_point, ct0.end_point, length, entity)
-    elif isinstance(entity, et.Ellipse):
+    def __init__(self, filename: str):
+        # stores the file system name of the DXF document.
+        self.filename: str = filename
+        # DXF version if header variable $ACADVER is present, default is DXFR12
+        self.version: str = "AC1009"
+        # Python encoding required to read the DXF document as text file.
+        self.encoding: str = "cp1252"
+        self.index: list[IndexEntry] = []
+
+    def print(self) -> None:
+        print(f"Filename: {self.filename}")
+        print(f"DXF Version: {self.version}")
+        print(f"encoding: {self.encoding}")
+        for entry in self.index:
+            print(f"Line: {entry.line} - ({entry.code}, {entry.value})")
+
+    def get(self, code: int, value: str, start: int = 0) -> int:
+        """Returns index of first entry matching `code` and `value`."""
+        self_index = self.index
+        index: int = start
+        count: int = len(self_index)
+        while index < count:
+            entry = self_index[index]
+            if entry.code == code and entry.value == value:
+                return index
+            index += 1
+        raise ValueError(f"No entry for tag ({code}, {value}) found.")
+
+    def fetchall(
+        self, code: int, value: str, start: int = 0
+    ) -> Iterable[IndexEntry]:
+        """Iterate over all specified entities.
+
+        e.g. fetchall(0, 'LINE') returns an iterator for all LINE entities.
+
+        """
+        for entry in self.index[start:]:
+            if entry.code == code and entry.value == value:
+                yield entry
+
+
+def load(filename: str) -> FileStructure:
+    """Load DXF file structure for file `filename`, the file has to be seekable.
+
+    Args:
+        filename: file system file name
+
+    Raises:
+        DXFStructureError: Invalid or incomplete DXF file.
+
+    """
+    file_structure = FileStructure(filename)
+    file: BinaryIO = open(filename, mode="rb")
+    line: int = 1
+    eof: bool = False
+    header: bool = False
+    index: list[IndexEntry] = []
+    prev_code: int = -1
+    prev_value: bytes = b""
+    structure = None  # the current structure tag: 'SECTION', 'LINE', ...
+
+    def load_tag() -> tuple[int, bytes]:
+        nonlocal line
         try:
-            ct1 = entity.construction_tool()
+            code = int(file.readline())
         except ValueError:
-            return None
-        if ct1.major_axis.magnitude < ABS_TOL or ct1.minor_axis.magnitude < ABS_TOL:
-            return None
-        span = ellipse_param_span(ct1.start_param, ct1.end_param)
-        num = max(3, round(span / 0.1745))  #  resolution of ~1 deg
-        # length of elliptic arc is an approximation:
-        points = list(ct1.vertices(ct1.params(num)))
-        length = sum(a.distance(b) for a, b in zip(points, points[1:]))
-        edge = Edge(Vec3(points[0]), Vec3(points[-1]), length, entity)
-    elif isinstance(entity, et.Spline):
+            raise DXFStructureError(f"Invalid group code in line {line}")
+
+        if code < 0 or code > 1071:
+            raise DXFStructureError(f"Invalid group code {code} in line {line}")
+        value = file.readline().rstrip(b"\r\n")
+        line += 2
+        return code, value
+
+    def load_header_var() -> str:
+        _, value = load_tag()
+        return value.decode()
+
+    while not eof:
+        location = file.tell()
+        tag_line = line
         try:
-            ct2 = entity.construction_tool()
-        except ValueError:
-            return None
-        start = Vec3(ct2.control_points[0])
-        end = Vec3(ct2.control_points[-1])
-        points = list(ct2.control_points)
-        # length of B-spline is a very rough approximation:
-        length = sum(a.distance(b) for a, b in zip(points, points[1:]))
-        edge = Edge(start, end, length, entity)
-
-    if isinstance(edge, Edge):
-        if edge.start.distance(edge.end) < gap_tol:
-            return None
-        if edge.length < gap_tol:
-            return None
-    return edge
-
-
-def edges_from_entities(
-    entities: Iterable[et.DXFEntity], gap_tol=GAP_TOL
-) -> Iterator[Edge]:
-    """Yields all DXF entities as edges. 
-    
-    Skips all entities which can not be represented as edge.
-    """
-    for entity in entities:
-        edge = edge_from_entity(entity, gap_tol)
-        if edge is not None:
-            yield edge
+            code, value = load_tag()
+            if header and code == 9:
+                if value == b"$ACADVER":
+                    file_structure.version = load_header_var()
+                elif value == b"$DWGCODEPAGE":
+                    file_structure.encoding = toencoding(load_header_var())
+                continue
+        except IOError:
+            break
+
+        if code == 0:
+            # All structure tags have group code == 0, store file location
+            structure = value
+            index.append(IndexEntry(0, value.decode(), location, tag_line))
+            eof = value == b"EOF"
+
+        elif code == 2 and prev_code == 0 and prev_value == b"SECTION":
+            # Section name is the tag (2, name) following the (0, SECTION) tag.
+            header = value == b"HEADER"
+            index.append(IndexEntry(2, value.decode(), location, tag_line))
+
+        elif code == 5 and structure != b"DIMSTYLE":
+            # Entity handles have always group code 5.
+            index.append(IndexEntry(5, value.decode(), location, tag_line))
+
+        elif code == 105 and structure == b"DIMSTYLE":
+            # Except the DIMSTYLE table entry has group code 105.
+            index.append(IndexEntry(5, value.decode(), location, tag_line))
+
+        prev_code = code
+        prev_value = value
+
+    file.close()
+    if not eof:
+        raise DXFStructureError(f"Unexpected end of file.")
+
+    if file_structure.version >= "AC1021":  # R2007 and later
+        file_structure.encoding = "utf-8"
+    file_structure.index = index
+    return file_structure
```

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entitydb.py` & `ezdxf-1.3.1b1/src/ezdxf/entitydb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/enums.py` & `ezdxf-1.3.1b1/src/ezdxf/enums.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/explode.py` & `ezdxf-1.3.1b1/src/ezdxf/explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/eztypes.py` & `ezdxf-1.3.1b1/src/ezdxf/eztypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/filemanagement.py` & `ezdxf-1.3.1b1/src/ezdxf/filemanagement.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/gfxattribs.py` & `ezdxf-1.3.1b1/src/ezdxf/gfxattribs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/graphicsfactory.py` & `ezdxf-1.3.1b1/src/ezdxf/graphicsfactory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/groupby.py` & `ezdxf-1.3.1b1/src/ezdxf/groupby.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/messenger.py` & `ezdxf-1.3.1b1/src/ezdxf/messenger.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/npshapes.py` & `ezdxf-1.3.1b1/src/ezdxf/npshapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/protocols.py` & `ezdxf-1.3.1b1/src/ezdxf/protocols.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/proxygraphic.py` & `ezdxf-1.3.1b1/src/ezdxf/proxygraphic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/query.py` & `ezdxf-1.3.1b1/src/ezdxf/query.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/queryparser.py` & `ezdxf-1.3.1b1/src/ezdxf/queryparser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/r12strict.py` & `ezdxf-1.3.1b1/src/ezdxf/r12strict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/recover.py` & `ezdxf-1.3.1b1/src/ezdxf/recover.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/reorder.py` & `ezdxf-1.3.1b1/src/ezdxf/reorder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/revcloud.py` & `ezdxf-1.3.1b1/src/ezdxf/revcloud.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/select.py` & `ezdxf-1.3.1b1/src/ezdxf/select.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/transform.py` & `ezdxf-1.3.1b1/src/ezdxf/transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/units.py` & `ezdxf-1.3.1b1/src/ezdxf/units.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/upright.py` & `ezdxf-1.3.1b1/src/ezdxf/upright.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/urecord.py` & `ezdxf-1.3.1b1/src/ezdxf/urecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/version.py` & `ezdxf-1.3.1b1/src/ezdxf/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 # examples:
 #   major pre-release alpha 2: VERSION = "0.9.0a2"; version = (0, 9, 0, 'a2')
 #   major release candidate 0: VERSION = "0.9.0rc0"; version = (0, 9, 0, 'rc0')
 #   major release: VERSION = "0.9.0"; version = (0, 9, 0, 'release')
 #   1. bug fix release beta0: VERSION = "0.9.1b0"; version = (0, 9, 1, 'b0')
 #   2. bug fix release: VERSION = "0.9.2"; version = (0, 9, 2, 'release')
 
-version = (1, 3, 1, "b0")
-__version__ = "1.3.1b0"
+version = (1, 3, 1, "b1")
+__version__ = "1.3.1b1"
```

## Comparing `ezdxf-1.3.1b0/src/ezdxf/xclip.py` & `ezdxf-1.3.1b1/src/ezdxf/xclip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/xref.py` & `ezdxf-1.3.1b1/src/ezdxf/xref.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/zoom.py` & `ezdxf-1.3.1b1/src/ezdxf/zoom.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/_options.py` & `ezdxf-1.3.1b1/src/ezdxf/_options.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/__init__.py` & `ezdxf-1.3.1b1/src/ezdxf/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/__main__.py` & `ezdxf-1.3.1b1/src/ezdxf/__main__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/acc/bezier3p.pyx` & `ezdxf-1.3.1b1/src/ezdxf/acc/bezier3p.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/acc/bezier4p.pyx` & `ezdxf-1.3.1b1/src/ezdxf/acc/bezier4p.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/acc/bspline.pyx` & `ezdxf-1.3.1b1/src/ezdxf/acc/bspline.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/acc/construct.pyx` & `ezdxf-1.3.1b1/src/ezdxf/acc/construct.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/acc/linetypes.pyx` & `ezdxf-1.3.1b1/src/ezdxf/acc/linetypes.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/acc/mapbox_earcut.pyx` & `ezdxf-1.3.1b1/src/ezdxf/acc/mapbox_earcut.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/acc/matrix44.pyx` & `ezdxf-1.3.1b1/src/ezdxf/acc/matrix44.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/acc/np_support.pyx` & `ezdxf-1.3.1b1/src/ezdxf/acc/np_support.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/acc/vector.pxd` & `ezdxf-1.3.1b1/src/ezdxf/acc/vector.pxd`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/acc/vector.pyx` & `ezdxf-1.3.1b1/src/ezdxf/acc/vector.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/acc/__init__.py` & `ezdxf-1.3.1b1/src/ezdxf/acc/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/acis/abstract.py` & `ezdxf-1.3.1b1/src/ezdxf/acis/abstract.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/acis/api.py` & `ezdxf-1.3.1b1/src/ezdxf/acis/api.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/acis/cache.py` & `ezdxf-1.3.1b1/src/ezdxf/acis/cache.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/acis/const.py` & `ezdxf-1.3.1b1/src/ezdxf/acis/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/acis/dbg.py` & `ezdxf-1.3.1b1/src/ezdxf/acis/dbg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/acis/dxf.py` & `ezdxf-1.3.1b1/src/ezdxf/acis/dxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/acis/entities.py` & `ezdxf-1.3.1b1/src/ezdxf/acis/entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/acis/hdr.py` & `ezdxf-1.3.1b1/src/ezdxf/acis/hdr.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/acis/mesh.py` & `ezdxf-1.3.1b1/src/ezdxf/acis/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/acis/sab.py` & `ezdxf-1.3.1b1/src/ezdxf/acis/sab.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/acis/sat.py` & `ezdxf-1.3.1b1/src/ezdxf/acis/sat.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/acadctb.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/acadctb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/binpacking.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/binpacking.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/dimlines.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/dimlines.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/dxf2code.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/dxf2code.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/genetic_algorithm.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/genetic_algorithm.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/geo.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/geo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/gerber_D6673.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/gerber_D6673.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/importer.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/importer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/iterdxf.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/iterdxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/menger_sponge.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/menger_sponge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/meshex.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/meshex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/mtextsurrogate.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/mtextsurrogate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/mtxpl.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/mtxpl.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/odafc.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/odafc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/openscad.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/openscad.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/pycsg.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/pycsg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/r12export.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/r12export.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/r12writer.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/r12writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/sierpinski_pyramid.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/sierpinski_pyramid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/tablepainter.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/tablepainter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/text2path.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/text2path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/xplayer.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/xplayer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/xqt.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/xqt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/acisbrowser/browser.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/acisbrowser/browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/acisbrowser/data.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/acisbrowser/data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/browser/bookmarks.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/browser/bookmarks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/browser/browser.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/browser/browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/browser/data.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/browser/data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/browser/find_dialog.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/browser/find_dialog.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/browser/loader.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/browser/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/browser/model.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/browser/model.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/browser/reflinks.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/browser/reflinks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/browser/tags.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/browser/tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/browser/views.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/browser/views.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/backend.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/drawing/backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/config.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/drawing/config.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/debug_backend.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/drawing/debug_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/debug_utils.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/drawing/debug_utils.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/dxf.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/drawing/dxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/file_output.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/drawing/file_output.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/frontend.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/drawing/frontend.py`

 * *Files 0% similar despite different names*

```diff
@@ -847,26 +847,29 @@
                 else:  # stored as vector (0, 0, elevation)
                     elevation = Vec3(entity.dxf.elevation).z
 
             trace = TraceBuilder.from_polyline(
                 entity, segments=self.config.circle_approximation_count // 2
             )
             for polygon in trace.polygons():  # polygon is a sequence of Vec2()
+                if len(polygon) < 3:
+                    continue
                 if transform:
                     points = ocs.points_to_wcs(
                         Vec3(v.x, v.y, elevation) for v in polygon
                     )
                 else:
                     points = polygon  # type: ignore
                 # Set default SOLID filling for LWPOLYLINE
                 properties.filling = Filling()
                 self.pipeline.draw_filled_polygon(points, properties)
             return
-
-        self.pipeline.draw_path(make_path(entity), properties)
+        polyline_path = make_path(entity)
+        if len(polyline_path):
+            self.pipeline.draw_path(polyline_path, properties)
 
     def draw_composite_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         def draw_insert(insert: Insert):
             # Block reference attributes are located __outside__ the block reference!
             self.draw_entities(insert.attribs)
             clip = xclip.XClip(insert)
             is_clipping_active = clip.has_clipping_path and clip.is_clipping_enabled
```

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/gfxproxy.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/drawing/gfxproxy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/hpgl2.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/drawing/hpgl2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/json.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/drawing/json.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/layout.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/drawing/layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/matplotlib.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/drawing/matplotlib.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/mtext_complex.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/drawing/mtext_complex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/pipeline.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/drawing/pipeline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/properties.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/drawing/properties.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/pymupdf.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/drawing/pymupdf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/pyqt.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/drawing/pyqt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/qtviewer.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/drawing/qtviewer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/recorder.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/drawing/recorder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/svg.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/drawing/svg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/text.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/drawing/text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/text_renderer.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/drawing/text_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/drawing/unified_text_renderer.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/drawing/unified_text_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/dwg/classes_section.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/dwg/classes_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/dwg/const.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/dwg/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/dwg/crc.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/dwg/crc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/dwg/fileheader.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/dwg/fileheader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/dwg/header_section.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/dwg/header_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/dwg/loader.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/dwg/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/api.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/api.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/backend.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/deps.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/deps.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/interpreter.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/interpreter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/page.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/page.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/plotter.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/plotter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/polygon_buffer.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/polygon_buffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/properties.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/properties.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/tokenizer.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/tokenizer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/addons/hpgl2/viewer.py` & `ezdxf-1.3.1b1/src/ezdxf/addons/hpgl2/viewer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/acad_proxy_entity.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/acad_proxy_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/acad_table.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/acad_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/acad_xrec_roundtrip.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/acad_xrec_roundtrip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/acis.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/acis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/appdata.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/appdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/appid.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/appid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/arc.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/attrib.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/attrib.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/block.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/block.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/blockrecord.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/blockrecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/boundary_paths.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/boundary_paths.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/circle.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/copy.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/copy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/dictionary.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/dictionary.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/dimension.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/dimstyle.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/dimstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/dimstyleoverride.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/dimstyleoverride.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/dxfclass.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/dxfclass.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/dxfentity.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/dxfentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/dxfgfx.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/dxfgfx.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/dxfgroups.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/dxfgroups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/dxfns.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/dxfns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/dxfobj.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/dxfobj.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/ellipse.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/factory.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/factory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/geodata.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/geodata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/gradient.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/gradient.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/hatch.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/hatch.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/helix.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/helix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/idbuffer.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/idbuffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/image.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/image.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/insert.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/insert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/layer.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/layer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/layout.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/leader.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/light.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/light.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/line.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/ltype.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/ltype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/lwpolyline.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/lwpolyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/material.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/material.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/mesh.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/mleader.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/mleader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/mline.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/mpolygon.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/mpolygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/mtext.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/mtext.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/mtext_columns.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/mtext_columns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/objectcollection.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/objectcollection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/oleframe.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/oleframe.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/pattern.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/point.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/polygon.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/polygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/polyline.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/shape.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/solid.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/solid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/spatial_filter.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/spatial_filter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/spline.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/subentity.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/subentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/sun.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/sun.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/table.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/temporary_transform.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/temporary_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/text.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/textstyle.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/textstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/tolerance.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/tolerance.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/ucs.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/underlay.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/underlay.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/view.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/view.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/viewport.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/viewport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/visualstyle.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/visualstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/vport.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/vport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/xdata.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/xdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/xdict.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/xdict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/xline.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/xline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/entities/__init__.py` & `ezdxf-1.3.1b1/src/ezdxf/entities/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/fonts/fonts.py` & `ezdxf-1.3.1b1/src/ezdxf/fonts/fonts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/fonts/font_face.py` & `ezdxf-1.3.1b1/src/ezdxf/fonts/font_face.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/fonts/font_manager.py` & `ezdxf-1.3.1b1/src/ezdxf/fonts/font_manager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/fonts/font_measurements.py` & `ezdxf-1.3.1b1/src/ezdxf/fonts/font_measurements.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/fonts/glyphs.py` & `ezdxf-1.3.1b1/src/ezdxf/fonts/glyphs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/fonts/lff.py` & `ezdxf-1.3.1b1/src/ezdxf/fonts/lff.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/fonts/shapefile.py` & `ezdxf-1.3.1b1/src/ezdxf/fonts/shapefile.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/fonts/ttfonts.py` & `ezdxf-1.3.1b1/src/ezdxf/fonts/ttfonts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/layouts/base.py` & `ezdxf-1.3.1b1/src/ezdxf/layouts/base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/layouts/blocklayout.py` & `ezdxf-1.3.1b1/src/ezdxf/layouts/blocklayout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/layouts/layout.py` & `ezdxf-1.3.1b1/src/ezdxf/layouts/layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/layouts/layouts.py` & `ezdxf-1.3.1b1/src/ezdxf/layouts/layouts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/lldxf/attributes.py` & `ezdxf-1.3.1b1/src/ezdxf/lldxf/attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/lldxf/const.py` & `ezdxf-1.3.1b1/src/ezdxf/lldxf/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/lldxf/encoding.py` & `ezdxf-1.3.1b1/src/ezdxf/lldxf/encoding.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/lldxf/extendedtags.py` & `ezdxf-1.3.1b1/src/ezdxf/lldxf/extendedtags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/lldxf/hdrvars.py` & `ezdxf-1.3.1b1/src/ezdxf/lldxf/hdrvars.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/lldxf/loader.py` & `ezdxf-1.3.1b1/src/ezdxf/lldxf/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/lldxf/packedtags.py` & `ezdxf-1.3.1b1/src/ezdxf/lldxf/packedtags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/lldxf/repair.py` & `ezdxf-1.3.1b1/src/ezdxf/lldxf/repair.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/lldxf/tagger.py` & `ezdxf-1.3.1b1/src/ezdxf/lldxf/tagger.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/lldxf/tags.py` & `ezdxf-1.3.1b1/src/ezdxf/lldxf/tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/lldxf/tagwriter.py` & `ezdxf-1.3.1b1/src/ezdxf/lldxf/tagwriter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/lldxf/types.py` & `ezdxf-1.3.1b1/src/ezdxf/lldxf/types.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/lldxf/validator.py` & `ezdxf-1.3.1b1/src/ezdxf/lldxf/validator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/arc.py` & `ezdxf-1.3.1b1/src/ezdxf/math/arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/bbox.py` & `ezdxf-1.3.1b1/src/ezdxf/math/bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/bezier.py` & `ezdxf-1.3.1b1/src/ezdxf/math/bezier.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/bezier_interpolation.py` & `ezdxf-1.3.1b1/src/ezdxf/math/bezier_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/box.py` & `ezdxf-1.3.1b1/src/ezdxf/math/box.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/bspline.py` & `ezdxf-1.3.1b1/src/ezdxf/math/bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/bulge.py` & `ezdxf-1.3.1b1/src/ezdxf/math/bulge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/circle.py` & `ezdxf-1.3.1b1/src/ezdxf/math/circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/clipping.py` & `ezdxf-1.3.1b1/src/ezdxf/math/clipping.py`

 * *Files 1% similar despite different names*

```diff
@@ -679,38 +679,18 @@
     c = v
     while c.intersect:
         c = c.next
     return c
 
 
 def is_inside_polygon(vertex: Vec2, polygon: GHPolygon) -> bool:
-    """Returns ``True`` if  `vertex` is inside `polygon` (odd-even rule).
-
-    This function calculates the "winding" number for a point, which
-    represents the number of times a ray emitted from the point to
-    infinity intersects any edge of the polygon.
-
-    An even winding number means the point lies OUTSIDE the polygon;
-    an odd number means it lies INSIDE it.
-    """
-    winding_number: int = 0
-    infinity = Vec2(polygon.max_x * 2, vertex.y)
-    for node in polygon:
-        if not node.intersect:
-            if (
-                line_intersection(
-                    vertex,
-                    infinity,
-                    node.vtx,
-                    next_vertex_node(node.next).vtx,
-                )[0]
-                is not None
-            ):
-                winding_number += 1
-    return bool(winding_number % 2)
+    """Returns ``True`` if  `vertex` is inside `polygon`."""
+    # Possible issue: are points on the boundary inside or outside the polygon?
+    #  this version: inside
+    return is_point_in_polygon_2d(vertex, polygon.points, abs_tol=TOLERANCE) >= 0
 
 
 _ERROR = None, 0, 0
 
 
 def line_intersection(
     s1: Vec2, s2: Vec2, c1: Vec2, c2: Vec2, tol: float = TOLERANCE
@@ -721,24 +701,24 @@
     points!
 
     Algorithm based on: http://paulbourke.net/geometry/lineline2d/
     """
     den = (c2.y - c1.y) * (s2.x - s1.x) - (c2.x - c1.x) * (s2.y - s1.y)
     if abs(den) < tol:
         return _ERROR
-
     us = ((c2.x - c1.x) * (s1.y - c1.y) - (c2.y - c1.y) * (s1.x - c1.x)) / den
-    uc = ((s2.x - s1.x) * (s1.y - c1.y) - (s2.y - s1.y) * (s1.x - c1.x)) / den
-
     lwr = 0.0 + tol
     upr = 1.0 - tol
     # Line end points are excluded as intersection points:
     # us =~ 0.0; us =~ 1.0
+    if not (lwr < us < upr):
+        return _ERROR
     # uc =~ 0.0; uc =~ 1.0
-    if (lwr < us < upr) and (lwr < uc < upr):
+    uc = ((s2.x - s1.x) * (s1.y - c1.y) - (s2.y - s1.y) * (s1.x - c1.x)) / den
+    if lwr < uc < upr:
         return (
             Vec2(s1.x + us * (s2.x - s1.x), s1.y + us * (s2.y - s1.y)),
             us,
             uc,
         )
     return _ERROR
```

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/clustering.py` & `ezdxf-1.3.1b1/src/ezdxf/math/clustering.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/construct2d.py` & `ezdxf-1.3.1b1/src/ezdxf/math/construct2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/construct3d.py` & `ezdxf-1.3.1b1/src/ezdxf/math/construct3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/cspline.py` & `ezdxf-1.3.1b1/src/ezdxf/math/cspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/curvetools.py` & `ezdxf-1.3.1b1/src/ezdxf/math/curvetools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/ellipse.py` & `ezdxf-1.3.1b1/src/ezdxf/math/ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/eulerspiral.py` & `ezdxf-1.3.1b1/src/ezdxf/math/eulerspiral.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/legacy.py` & `ezdxf-1.3.1b1/src/ezdxf/math/legacy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/linalg.py` & `ezdxf-1.3.1b1/src/ezdxf/math/linalg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/line.py` & `ezdxf-1.3.1b1/src/ezdxf/math/line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/offset2d.py` & `ezdxf-1.3.1b1/src/ezdxf/math/offset2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/parametrize.py` & `ezdxf-1.3.1b1/src/ezdxf/math/parametrize.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/perlin.py` & `ezdxf-1.3.1b1/src/ezdxf/math/perlin.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/polyline.py` & `ezdxf-1.3.1b1/src/ezdxf/math/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/rtree.py` & `ezdxf-1.3.1b1/src/ezdxf/math/rtree.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/shape.py` & `ezdxf-1.3.1b1/src/ezdxf/math/shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/transformtools.py` & `ezdxf-1.3.1b1/src/ezdxf/math/transformtools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/triangulation.py` & `ezdxf-1.3.1b1/src/ezdxf/math/triangulation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/ucs.py` & `ezdxf-1.3.1b1/src/ezdxf/math/ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/_bezier3p.py` & `ezdxf-1.3.1b1/src/ezdxf/math/_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/_bezier4p.py` & `ezdxf-1.3.1b1/src/ezdxf/math/_bezier4p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/_bspline.py` & `ezdxf-1.3.1b1/src/ezdxf/math/_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/_construct.py` & `ezdxf-1.3.1b1/src/ezdxf/math/_construct.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/_ctypes.py` & `ezdxf-1.3.1b1/src/ezdxf/math/_ctypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/_mapbox_earcut.py` & `ezdxf-1.3.1b1/src/ezdxf/math/_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/_matrix44.py` & `ezdxf-1.3.1b1/src/ezdxf/math/_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/_vector.py` & `ezdxf-1.3.1b1/src/ezdxf/math/_vector.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/math/__init__.py` & `ezdxf-1.3.1b1/src/ezdxf/math/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/path/commands.py` & `ezdxf-1.3.1b1/src/ezdxf/path/commands.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/path/converter.py` & `ezdxf-1.3.1b1/src/ezdxf/path/converter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/path/nesting.py` & `ezdxf-1.3.1b1/src/ezdxf/path/nesting.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/path/path.py` & `ezdxf-1.3.1b1/src/ezdxf/path/path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/path/shapes.py` & `ezdxf-1.3.1b1/src/ezdxf/path/shapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/path/tools.py` & `ezdxf-1.3.1b1/src/ezdxf/path/tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/render/abstract_mtext_renderer.py` & `ezdxf-1.3.1b1/src/ezdxf/render/abstract_mtext_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/render/arrows.py` & `ezdxf-1.3.1b1/src/ezdxf/render/arrows.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/render/curves.py` & `ezdxf-1.3.1b1/src/ezdxf/render/curves.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/render/dimension.py` & `ezdxf-1.3.1b1/src/ezdxf/render/dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/render/dim_base.py` & `ezdxf-1.3.1b1/src/ezdxf/render/dim_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/render/dim_curved.py` & `ezdxf-1.3.1b1/src/ezdxf/render/dim_curved.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/render/dim_diameter.py` & `ezdxf-1.3.1b1/src/ezdxf/render/dim_diameter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/render/dim_linear.py` & `ezdxf-1.3.1b1/src/ezdxf/render/dim_linear.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/render/dim_ordinate.py` & `ezdxf-1.3.1b1/src/ezdxf/render/dim_ordinate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/render/dim_radius.py` & `ezdxf-1.3.1b1/src/ezdxf/render/dim_radius.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/render/forms.py` & `ezdxf-1.3.1b1/src/ezdxf/render/forms.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/render/hatching.py` & `ezdxf-1.3.1b1/src/ezdxf/render/hatching.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/render/leader.py` & `ezdxf-1.3.1b1/src/ezdxf/render/leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/render/linetypes.py` & `ezdxf-1.3.1b1/src/ezdxf/render/linetypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/render/mesh.py` & `ezdxf-1.3.1b1/src/ezdxf/render/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/render/mleader.py` & `ezdxf-1.3.1b1/src/ezdxf/render/mleader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/render/mline.py` & `ezdxf-1.3.1b1/src/ezdxf/render/mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/render/point.py` & `ezdxf-1.3.1b1/src/ezdxf/render/point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/render/polyline.py` & `ezdxf-1.3.1b1/src/ezdxf/render/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/render/r12spline.py` & `ezdxf-1.3.1b1/src/ezdxf/render/r12spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/render/trace.py` & `ezdxf-1.3.1b1/src/ezdxf/render/trace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/render/_linetypes.py` & `ezdxf-1.3.1b1/src/ezdxf/render/_linetypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/render/__init__.py` & `ezdxf-1.3.1b1/src/ezdxf/render/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/resources/16x16.png` & `ezdxf-1.3.1b1/src/ezdxf/resources/16x16.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/resources/24x24.png` & `ezdxf-1.3.1b1/src/ezdxf/resources/24x24.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/resources/256x256.png` & `ezdxf-1.3.1b1/src/ezdxf/resources/256x256.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/resources/32x32.png` & `ezdxf-1.3.1b1/src/ezdxf/resources/32x32.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/resources/48x48.png` & `ezdxf-1.3.1b1/src/ezdxf/resources/48x48.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/resources/64x64.png` & `ezdxf-1.3.1b1/src/ezdxf/resources/64x64.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/resources/icon-copy-64px.png` & `ezdxf-1.3.1b1/src/ezdxf/resources/icon-copy-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/resources/icon-find-64px.png` & `ezdxf-1.3.1b1/src/ezdxf/resources/icon-find-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/resources/icon-goto-bookmark-64px.png` & `ezdxf-1.3.1b1/src/ezdxf/resources/icon-goto-bookmark-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/resources/icon-goto-handle-64px.png` & `ezdxf-1.3.1b1/src/ezdxf/resources/icon-goto-handle-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/resources/icon-goto-line-64px.png` & `ezdxf-1.3.1b1/src/ezdxf/resources/icon-goto-line-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/resources/icon-left-arrow-64px.png` & `ezdxf-1.3.1b1/src/ezdxf/resources/icon-left-arrow-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/resources/icon-next-entity-64px.png` & `ezdxf-1.3.1b1/src/ezdxf/resources/icon-next-entity-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/resources/icon-prev-entity-64px.png` & `ezdxf-1.3.1b1/src/ezdxf/resources/icon-prev-entity-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/resources/icon-right-arrow-64px.png` & `ezdxf-1.3.1b1/src/ezdxf/resources/icon-right-arrow-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/resources/icon-show-in-tree-64px.png` & `ezdxf-1.3.1b1/src/ezdxf/resources/icon-show-in-tree-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/resources/icon-store-bookmark-64px.png` & `ezdxf-1.3.1b1/src/ezdxf/resources/icon-store-bookmark-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/sections/acdsdata.py` & `ezdxf-1.3.1b1/src/ezdxf/sections/acdsdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/sections/blocks.py` & `ezdxf-1.3.1b1/src/ezdxf/sections/blocks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/sections/classes.py` & `ezdxf-1.3.1b1/src/ezdxf/sections/classes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/sections/entities.py` & `ezdxf-1.3.1b1/src/ezdxf/sections/entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/sections/header.py` & `ezdxf-1.3.1b1/src/ezdxf/sections/header.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/sections/headervars.py` & `ezdxf-1.3.1b1/src/ezdxf/sections/headervars.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/sections/objects.py` & `ezdxf-1.3.1b1/src/ezdxf/sections/objects.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/sections/table.py` & `ezdxf-1.3.1b1/src/ezdxf/sections/table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/sections/tables.py` & `ezdxf-1.3.1b1/src/ezdxf/sections/tables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/tools/analyze.py` & `ezdxf-1.3.1b1/src/ezdxf/tools/analyze.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/tools/binarydata.py` & `ezdxf-1.3.1b1/src/ezdxf/tools/binarydata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/tools/clipping_portal.py` & `ezdxf-1.3.1b1/src/ezdxf/tools/clipping_portal.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,27 +243,31 @@
         return point
 
     def clip_line(self, start: Vec2, end: Vec2) -> Sequence[tuple[Vec2, Vec2]]:
         return self.clipper.clip_line(start, end)
 
     def clip_polyline(self, points: NumpyPoints2d) -> Sequence[NumpyPoints2d]:
         clipper = self.clipper
+        if len(points) == 0:
+            return tuple()
         polyline_bbox = BoundingBox2d(points.extents())
         if self.is_completely_outside(polyline_bbox):
             return tuple()
         if self.is_completely_inside(polyline_bbox):
             return (points,)
         return [
             NumpyPoints2d(part)
             for part in clipper.clip_polyline(points.vertices())
             if len(part) > 0
         ]
 
     def clip_polygon(self, points: NumpyPoints2d) -> Sequence[NumpyPoints2d]:
         clipper = self.clipper
+        if len(points) < 2:
+            return tuple()
         polygon_bbox = BoundingBox2d(points.extents())
         if self.is_completely_outside(polygon_bbox):
             return tuple()
         if self.is_completely_inside(polygon_bbox):
             return (points,)
         return [
             NumpyPoints2d(part)
@@ -274,14 +278,16 @@
     def clip_paths(
         self, paths: Iterable[NumpyPath2d], max_sagitta: float
     ) -> Iterator[NumpyPath2d]:
         clipper = self.clipper
         for path in paths:
             for sub_path in path.sub_paths():
                 path_bbox = BoundingBox2d(sub_path.control_vertices())
+                if not path_bbox.has_data:
+                    continue
                 if self.is_completely_inside(path_bbox):
                     yield sub_path
                     continue
                 if self.is_completely_outside(path_bbox):
                     continue
                 polyline = Vec2.list(sub_path.flattening(max_sagitta, segments=4))
                 for part in clipper.clip_polyline(polyline):
```

## Comparing `ezdxf-1.3.1b0/src/ezdxf/tools/codepage.py` & `ezdxf-1.3.1b1/src/ezdxf/tools/codepage.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/tools/complex_ltype.py` & `ezdxf-1.3.1b1/src/ezdxf/tools/complex_ltype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/tools/crypt.py` & `ezdxf-1.3.1b1/src/ezdxf/tools/crypt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/tools/debug.py` & `ezdxf-1.3.1b1/src/ezdxf/tools/debug.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/tools/difftags.py` & `ezdxf-1.3.1b1/src/ezdxf/tools/difftags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/tools/handle.py` & `ezdxf-1.3.1b1/src/ezdxf/tools/handle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/tools/indexing.py` & `ezdxf-1.3.1b1/src/ezdxf/tools/indexing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/tools/juliandate.py` & `ezdxf-1.3.1b1/src/ezdxf/tools/juliandate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/tools/pattern.py` & `ezdxf-1.3.1b1/src/ezdxf/tools/pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/tools/rawloader.py` & `ezdxf-1.3.1b1/src/ezdxf/tools/rawloader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/tools/standards.py` & `ezdxf-1.3.1b1/src/ezdxf/tools/standards.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/tools/strip.py` & `ezdxf-1.3.1b1/src/ezdxf/tools/strip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/tools/test.py` & `ezdxf-1.3.1b1/src/ezdxf/tools/test.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/tools/text.py` & `ezdxf-1.3.1b1/src/ezdxf/tools/text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/tools/text_layout.py` & `ezdxf-1.3.1b1/src/ezdxf/tools/text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/tools/text_size.py` & `ezdxf-1.3.1b1/src/ezdxf/tools/text_size.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/tools/zipmanager.py` & `ezdxf-1.3.1b1/src/ezdxf/tools/zipmanager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/tools/_iso_pattern.py` & `ezdxf-1.3.1b1/src/ezdxf/tools/_iso_pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf/tools/__init__.py` & `ezdxf-1.3.1b1/src/ezdxf/tools/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/src/ezdxf.egg-info/PKG-INFO` & `ezdxf-1.3.1b1/src/ezdxf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdxf
-Version: 1.3.1b0
+Version: 1.3.1b1
 Summary: A Python package to create/manipulate DXF drawings.
 Author-email: Manfred Moitzi <me@mozman.at>
 Project-URL: Repository, https://github.com/mozman/ezdxf
 Project-URL: Documentation, https://ezdxf.readthedocs.io
 Project-URL: Changelog, https://ezdxf.mozman.at/notes/#/page/changelog
 Project-URL: Forum, https://github.com/mozman/ezdxf/discussions
 Project-URL: Issues, https://github.com/mozman/ezdxf/issues
```

## Comparing `ezdxf-1.3.1b0/src/ezdxf.egg-info/SOURCES.txt` & `ezdxf-1.3.1b1/src/ezdxf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_010_binary_data.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_010_binary_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_012_crypt.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_012_crypt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_013_juliandate.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_013_juliandate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_016_encoding.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_016_encoding.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_018_handle.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_018_handle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_024_render_tag.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_024_render_tag.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_040_tags.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_040_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_041_group_tags.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_041_group_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_056_special_string_decoding.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_056_special_string_decoding.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_00_dxf_low_level_structs/test_058_json_tags.py` & `ezdxf-1.3.1b1/tests/test_00_dxf_low_level_structs/test_058_json_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_101_dxfnamespace.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_101_dxfnamespace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_102_appdata.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_102_appdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_103_reactors.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_103_reactors.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_104_extension_dict.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_104_extension_dict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_105_xdata.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_105_xdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_110_dxfentity.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_110_dxfentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_112a_dxfgfx.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_112a_dxfgfx.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_112b_dxfobj.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_112b_dxfobj.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_113_dxfclass.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_113_dxfclass.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_114_factory.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_114_factory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_115_new_empty_drawing.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_115_new_empty_drawing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_116_dictionary.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_116_dictionary.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_117_layer_table_entry.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_117_layer_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_119_ucs_table_entry.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_119_ucs_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_120_style_table_entry.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_120_style_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_121_ltype_table_entry.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_121_ltype_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_123_view_table_entry.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_123_view_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_125_image_def.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_125_image_def.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_126_image_def_reactor.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_126_image_def_reactor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_127_raster_variables.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_127_raster_variables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_128_pdf_definition.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_128_pdf_definition.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_129_xrecord.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_129_xrecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_130_id_buffer.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_130_id_buffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_131_field_list.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_131_field_list.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_132_layer_filter.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_132_layer_filter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_133_sun.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_133_sun.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_134_material.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_134_material.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_135_geo_data.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_135_geo_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_136_vba_project.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_136_vba_project.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_137_sortentstable.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_137_sortentstable.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_138_setup_visual_styles.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_138_setup_visual_styles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_139_user_record.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_139_user_record.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_140_block_record.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_140_block_record.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_141_layer_vp_override.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_141_layer_vp_override.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_142_copy_strategy.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_142_copy_strategy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_143_spatial_filter.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_143_spatial_filter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_01_dxf_entities/test_144_roundtrip_xrecord.py` & `ezdxf-1.3.1b1/tests/test_01_dxf_entities/test_144_roundtrip_xrecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/conftest.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_200_line.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_200_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_201_point.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_201_point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_202_circle.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_202_circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_203_arc.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_203_arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_204_shape.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_204_shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_205_solid.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_205_solid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_206_text.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_206_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_207_attdef.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_207_attdef.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_208_attrib.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_208_attrib.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_209_vertex.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_209_vertex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_1.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_210_polyline_1.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_2.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_210_polyline_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_explode.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_210_polyline_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_211_viewport.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_211_viewport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_212_insert.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_212_insert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_213_minsert.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_213_minsert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_214_block.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_214_block.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_215_dimension.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_215_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_216_dimlines_R12.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_216_dimlines_R12.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_221_ellipse.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_221_ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_222_xline.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_222_xline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_223_ray.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_223_ray.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_224_group.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_224_group.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_225_mtext.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_225_mtext.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_226_spline.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_226_spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_228_mesh.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_228_mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_229b_hatch_extended.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_229b_hatch_extended.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_231_underlay.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_231_underlay.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_231_underlay_2.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_231_underlay_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232a_add_acis.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_232a_add_acis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232b_acis_export.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_232b_acis_export.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232c_acis_surface.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_232c_acis_surface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232d_acis_copy.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_232d_acis_copy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_232e_acis_transform.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_232e_acis_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_233_helix.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_233_helix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_234_light.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_234_light.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_235_leader.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_235_leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_236_multileader.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_236_multileader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_237_mline.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_237_mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_238_tolerance.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_238_tolerance.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_239_proxy_graphic.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_239_proxy_graphic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_240_arc_dimension.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_240_arc_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_241_hyperlink.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_241_hyperlink.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_242_random_transform.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_242_random_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_243_replace_entity.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_243_replace_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_245_wipeout.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_245_wipeout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_246_spline_audit.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_246_spline_audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_248_mpolygon.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_248_mpolygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_249_boundary_paths.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_249_boundary_paths.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_251_upright.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_251_upright.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_253_ole2frame.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_253_ole2frame.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_02_dxf_graphics/test_254_get_font_name.py` & `ezdxf-1.3.1b1/tests/test_02_dxf_graphics/test_254_get_font_name.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_300_layout.py` & `ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_300_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py` & `ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_302_block_references.py` & `ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_302_block_references.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_303_auto_block_references.py` & `ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_303_auto_block_references.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_304_new_entity_space.py` & `ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_304_new_entity_space.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py` & `ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py` & `ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_307_groupby.py` & `ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_307_groupby.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_308_query.py` & `ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_308_query.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_309_query_parser.py` & `ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_309_query_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py` & `ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_312_virtual_layout.py` & `ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_312_virtual_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_03_dxf_layouts/test_313_redraw_order.py` & `ezdxf-1.3.1b1/tests/test_03_dxf_layouts/test_313_redraw_order.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_401_headersection.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_401_headersection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_402_classessection.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_402_classessection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_403_entity_database.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_403_entity_database.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_404a_tables.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_404a_tables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_405_classes.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_405_classes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_407_entity_section.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_407_entity_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_408_objects_section.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_408_objects_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_409_create_objects.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_409_create_objects.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_410_table.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_410_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_411_acds_data.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_411_acds_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_415_layout_management.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_415_layout_management.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_417_bbox.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_417_bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_424_audit.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_424_audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_427_appsettings.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_427_appsettings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_04_dxf_high_level_structs/test_429_xclip.py` & `ezdxf-1.3.1b1/tests/test_04_dxf_high_level_structs/test_429_xclip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/conftest.py` & `ezdxf-1.3.1b1/tests/test_05_tools/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_500_units.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_500_units.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_501_truecolor.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_501_truecolor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_502_raw_color.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_502_raw_color.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_503_indexing.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_503_indexing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_504_suppress_zeros.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_504_suppress_zeros.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_508_read_zip.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_508_read_zip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_509_comments.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_509_comments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_510_byte_stream.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_510_byte_stream.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_511_bit_stream.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_511_bit_stream.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_512_pattern.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_512_pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_513_reorder_entities.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_513_reorder_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_514_text.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_514_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_515a_fonts_truetype.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_515a_fonts_truetype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_515b_fonts_shapefiles.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_515b_fonts_shapefiles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_515c_fonts_lff.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_515c_fonts_lff.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_516_zoom.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_516_zoom.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_517_text_layout.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_517_text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_519_mtext_editor.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_519_mtext_editor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_520_mtext_context.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_520_mtext_context.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_521_mtext_parser.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_521_mtext_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_522_text_scanner.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_522_text_scanner.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_523_text_size.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_523_text_size.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_524_block_reference_manager.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_524_block_reference_manager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_525_transparency.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_525_transparency.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_526_explode.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_526_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_527_gfxattribs.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_527_gfxattribs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_528_difftags.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_528_difftags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_529_acis_sat.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_529_acis_sat.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_530_acis_sab.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_530_acis_sab.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_531_acis_entities.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_531_acis_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_532_acis_mesh.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_532_acis_mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_533_shapefiles.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_533_shapefiles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_534_dwg_info.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_534_dwg_info.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_535_xref_basic.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_535_xref_basic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_536_xref_conflict.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_536_xref_conflict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_537_transform.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_537_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_538_scale_mtext_inline_commands.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_538_scale_mtext_inline_commands.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_539_npshapes.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_539_npshapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_540_lff_parser.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_540_lff_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_541_clipping_portal.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_541_clipping_portal.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_542_itertools.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_542_itertools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_543_select.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_543_select.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_544_revcloud.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_544_revcloud.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_545_acis_cache.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_545_acis_cache.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_05_tools/test_547_edgesmith.py` & `ezdxf-1.3.1b1/tests/test_05_tools/test_547_edgesmith.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/conftest.py` & `ezdxf-1.3.1b1/tests/test_06_math/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_600_base.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_600_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_601_bulge.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_601_bulge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_602_vec3.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_602_vec3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_603_vec2.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_603_vec2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_604_banded_matrix.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_604_banded_matrix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_604_linalg.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_604_linalg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_605_matrix44.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_605_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_606_convexhull.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_606_convexhull.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_607_perlin_noise.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_607_perlin_noise.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_608_intersection_line_line_2d.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_608_intersection_line_line_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_609_point_on_line.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_609_point_on_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_610_ocs.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_610_ocs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_611_ucs.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_611_ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_612_ucs_pass_trough.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_612_ucs_pass_trough.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_613_is_point_in_polygon_2d.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_613_is_point_in_polygon_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_614_construct_3d.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_614_construct_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_615_rytz_axis.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_615_rytz_axis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_616_plane.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_616_plane.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_617_clockwise_orientation.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_617_clockwise_orientation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_618_clipping.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_618_clipping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_619_greiner_hormann.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_619_greiner_hormann.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  Copyright (c) 2021, Manfred Moitzi
 #  License: MIT License
 
 import pytest
-from ezdxf.math import Vec2
+from ezdxf.math import Vec2, BoundingBox2d
 from ezdxf.math.clipping import (
     greiner_hormann_union,
     greiner_hormann_difference,
     greiner_hormann_intersection,
     line_intersection,
 )
 from ezdxf.render.forms import circle
@@ -17,14 +17,15 @@
 
     Start and end points of a line are not intersection points!
 
     Which also leads to issues for joining adjacent but not intersecting
     polygons.
 
     """
+
     def test_start_point_is_not_an_intersection_point(self):
         s1, s2 = Vec2(1, 1), Vec2(3, 1)
         c1, c2 = Vec2(2, 1), Vec2(2, 2)
         assert line_intersection(s1, s2, c1, c2)[0] is None
 
     def test_end_point_is_not_an_intersection_point(self):
         s1, s2 = Vec2(1, 1), Vec2(3, 1)
@@ -67,16 +68,16 @@
 
     def test_parallel_horizontal_lines_do_not_intersect(self):
         s1, s2 = Vec2(11, 0), Vec2(-11, 0)
         c1, c2 = Vec2(0, 0), Vec2(1, 0)
         assert line_intersection(s1, s2, c1, c2)[0] is None
 
     def test_collinear_lines_do_not_intersect(self):
-        s1, s2 = Vec2(0, 0), Vec2(4, 4)
-        c1, c2 = Vec2(2, 2), Vec2(4, 0)
+        s1, s2 = Vec2(0, 0), Vec2(2, 2)
+        c1, c2 = Vec2(3, 3), Vec2(4, 4)
         assert line_intersection(s1, s2, c1, c2)[0] is None
 
     @pytest.mark.parametrize(
         "p2", [(4, 0), (0, 4), (4, 4)], ids=["horiz", "vert", "diag"]
     )
     def test_coincident_lines_do_not_intersect(self, p2):
         s1, s2 = Vec2(0, 0), Vec2(p2)
@@ -158,16 +159,15 @@
         assert len(polygons) == 1
         result = polygons[0]
         assert len(result) == 9
         assert result[0] == result[-1], "expected closed polygon"
         assert set(UNION_OVERLAPPING) == set(result)
 
     def test_vertex_order_is_not_important(self, rect, overlapping):
-        """The vertex order (clockwise or counter clockwise) is not important.
-        """
+        """The vertex order (clockwise or counter clockwise) is not important."""
         rect.reverse()
         result = greiner_hormann_union(rect, overlapping)[0]
         assert set(UNION_OVERLAPPING) == set(result)
 
         overlapping.reverse()
         result = greiner_hormann_union(rect, overlapping)[0]
         assert set(UNION_OVERLAPPING) == set(result)
@@ -276,9 +276,101 @@
         """This polygons do not have any intersection points and therefore no
         intersection is calculated - which could interpreted as the expected
         result.
         """
         assert len(greiner_hormann_intersection(rect, outside)) == 0
 
 
+DATA_1094 = [
+    Vec2.list(
+        [
+            [-18.900001889999952, 1450.7000002308125],
+            [-18.900001889999952, 1470.7351470734998],
+            [1278.90012789, 1470.7351470734998],
+            [1278.90012789, 1450.70001562087],
+            [1503.6001841952093, 1450.7000156208703],
+            [1503.6001841952093, 1388.3850000081884],
+            [1503.6001841952093, 1388.3850000081884],
+            [1647.3246376764234, 1388.3850000081884],
+            [1647.3246376764234, 1548.1475422037274],
+            [1831.0471719722357, 1548.1475422037274],
+            [1831.0471719722357, 1388.3850000081884],
+            [1831.0471719722357, 1388.3850000081884],
+            [1980.6216566984945, 1388.3850000081884],
+            [1980.6216566984945, 1224.6149999918116],
+            [1831.0471719722357, 1224.6149999918116],
+            [1831.0471719722357, 1160.3525263520064],
+            [1647.3246376764234, 1160.3525263520064],
+            [1647.3246376764234, 1160.3525263520064],
+            [1647.3246376764234, 1224.6149999918116],
+            [1647.3246376764234, 1224.6149999918116],
+            [1503.6001841952093, 1224.6149999918116],
+            [1503.6001841952093, 1162.2999997691875],
+            [1278.90012789, 1162.2999997691877],
+            [1278.90012789, 1162.2999997691877],
+            [1278.90012789, 286.7000156208702],
+            [1503.6001841952093, 286.70001562087026],
+            [1503.6001841952093, 224.3850000081885],
+            [1503.6001841952093, 224.3850000081885],
+            [1647.3246376764234, 224.3850000081885],
+            [1647.3246376764234, 384.1475422037275],
+            [1831.0471719722357, 384.1475422037275],
+            [1831.0471719722357, 224.3850000081885],
+            [1831.0471719722357, 224.3850000081885],
+            [1980.6216566984945, 224.3850000081885],
+            [1980.6216566984945, 60.61499999181149],
+            [1831.0471719722357, 60.614999991811544],
+            [1831.0471719722357, -3.6474736479937064],
+            [1647.3246376764234, -3.6474736479937064],
+            [1647.3246376764234, -3.6474736479937064],
+            [1647.3246376764234, 60.61499999181149],
+            [1647.3246376764234, 60.61499999181149],
+            [1503.6001841952093, 60.61499999181149],
+            [1503.6001841952093, -1.7000002308124635],
+            [1278.90012789, -1.7000002308124635],
+            [1278.90012789, -1.7000002308124635],
+            [1278.90012789, -21.735002173499993],
+            [-18.900001890000045, -21.735002173499993],
+            [-18.900001890000045, -21.735002173499993],
+            [-18.900001890000045, -1.7000156208705448],
+            [-243.6001841952094, -1.7000156208702606],
+            [-243.6001841952094, -1.7000156208702606],
+            [-243.6001841952094, 60.61499999181149],
+            [-243.6001841952094, 60.61499999181149],
+            [-237.7502641782885, 60.61499999181149],
+            [-237.7502641782885, 224.3850000081885],
+            [-243.6001841952094, 224.3850000081885],
+            [-243.6001841952094, 286.70000023081246],
+            [-18.900001890000027, 286.7000002308125],
+            [-18.900001890000027, 286.7000002308125],
+            [-18.90000188999997, 1162.2999843791297],
+            [-243.6001841952094, 1162.2999843791297],
+            [-243.6001841952094, 1162.2999843791297],
+            [-243.6001841952094, 1450.7000002308125],
+            [-18.900001889999952, 1450.7000002308125],
+        ]
+    ),
+    Vec2.list(
+        [
+            [-392.2502641782885, 1224.6149999918116],
+            [-237.7502641782885, 1224.6149999918116],
+            [-237.7502641782885, 1388.3850000081884],
+            [-392.2502641782885, 1388.3850000081884],
+            [-392.2502641782885, 1224.6149999918116],
+        ]
+    ),
+]
+
+
+def test_issue_1094_is_inside_polygon_function_was_incorrect():
+    data = DATA_1094
+    box_expected = BoundingBox2d(data[0] + data[1])
+    result = greiner_hormann_union(data[0], data[1])
+
+    assert len(result) == 1
+    box_result = BoundingBox2d(result[0])
+    assert box_result.extmin.isclose(box_expected.extmin)
+    assert box_result.extmax.isclose(box_expected.extmax)
+
+
 if __name__ == "__main__":
     pytest.main([__file__])
```

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_620_knot.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_620_knot.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_621_bspline.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_621_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_622_bsplineu.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_622_bsplineu.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_623_rbspline.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_623_rbspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_624_global_bspline_interpolation.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_624_global_bspline_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_626_local_bspline_interpolation.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_626_local_bspline_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_627_bspline_basis.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_627_bspline_basis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_629_bezier.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_629_bezier.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_630a_bezier4p_base.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_630a_bezier4p_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_630b_bezier4p_functions.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_630b_bezier4p_functions.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_631_euler_spiral.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_631_euler_spiral.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_632_bezier3p.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_632_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_640_bbox.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_640_bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_641_construction_ray.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_641_construction_ray.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_642_construction_line.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_642_construction_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_643_construction_box.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_643_construction_box.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_644_construction_circle.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_644_construction_circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_645_construction_arc.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_645_construction_arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_646_offset_vertices_2d.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_646_offset_vertices_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_647_transform_tools.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_647_transform_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_648_construction_ellipse.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_648_construction_ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_650_elliptic_arc_span.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_650_elliptic_arc_span.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_651_construction_polyline.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_651_construction_polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_652_approx_param_t.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_652_approx_param_t.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_653_polyline_intersection.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_653_polyline_intersection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_654_rtree.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_654_rtree.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_655_dbscan.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_655_dbscan.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_656_k_means.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_656_k_means.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_657_mapbox_earcut.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_657_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_658_bevel_tools.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_658_bevel_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_659_intersection_line_polygon_3d.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_659_intersection_line_polygon_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_660_intersection_ray_polygon_3d.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_660_intersection_ray_polygon_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_662_is_convex_polygon_2d.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_662_is_convex_polygon_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_663_is_axes_aligned_rectange.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_663_is_axes_aligned_rectange.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_664_concave_clipping_polygon.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_664_concave_clipping_polygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_665_inverted_clipping_polygon.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_665_inverted_clipping_polygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_06_math/test_666_wgs84_transform.py` & `ezdxf-1.3.1b1/tests/test_06_math/test_666_wgs84_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_07_render/test_701_arrows.py` & `ezdxf-1.3.1b1/tests/test_07_render/test_701_arrows.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_07_render/test_702_render_forms.py` & `ezdxf-1.3.1b1/tests/test_07_render/test_702_render_forms.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_07_render/test_703_mesh_builder.py` & `ezdxf-1.3.1b1/tests/test_07_render/test_703_mesh_builder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_07_render/test_704_render_linear_dimension.py` & `ezdxf-1.3.1b1/tests/test_07_render/test_704_render_linear_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_07_render/test_705_shape.py` & `ezdxf-1.3.1b1/tests/test_07_render/test_705_shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_07_render/test_707_trace.py` & `ezdxf-1.3.1b1/tests/test_07_render/test_707_trace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_07_render/test_708a_path.py` & `ezdxf-1.3.1b1/tests/test_07_render/test_708a_path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_07_render/test_708b_path_tools.py` & `ezdxf-1.3.1b1/tests/test_07_render/test_708b_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_07_render/test_708c_matplotlib_path_tools.py` & `ezdxf-1.3.1b1/tests/test_07_render/test_708c_matplotlib_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_07_render/test_708d_qpainter_path_tools.py` & `ezdxf-1.3.1b1/tests/test_07_render/test_708d_qpainter_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_07_render/test_708e_path_shapes.py` & `ezdxf-1.3.1b1/tests/test_07_render/test_708e_path_shapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_07_render/test_708f_path_nesting.py` & `ezdxf-1.3.1b1/tests/test_07_render/test_708f_path_nesting.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_07_render/test_709_linetype_renderer.py` & `ezdxf-1.3.1b1/tests/test_07_render/test_709_linetype_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_07_render/test_711_points.py` & `ezdxf-1.3.1b1/tests/test_07_render/test_711_points.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_07_render/test_712_render_curved_dimension.py` & `ezdxf-1.3.1b1/tests/test_07_render/test_712_render_curved_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_07_render/test_713_mleader_builder.py` & `ezdxf-1.3.1b1/tests/test_07_render/test_713_mleader_builder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_07_render/test_714_mleader_render_engine.py` & `ezdxf-1.3.1b1/tests/test_07_render/test_714_mleader_render_engine.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_07_render/test_715_hatching.py` & `ezdxf-1.3.1b1/tests/test_07_render/test_715_hatching.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_07_render/test_715_issue_747_explode_3d_dim.py` & `ezdxf-1.3.1b1/tests/test_07_render/test_715_issue_747_explode_3d_dim.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_800_mtext_surrogate.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_800_mtext_surrogate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_801_r12spline.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_801_r12spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_802_table_painter.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_802_table_painter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_803_entities_to_code.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_803_entities_to_code.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_804_importer.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_804_importer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_805_pycsg.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_805_pycsg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_806_acadctb.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_806_acadctb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_807_dwg_loader_basics.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_807_dwg_loader_basics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_810_drawing_properties.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_810_drawing_properties.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_811a_drawing_frontend.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_811a_drawing_frontend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_811b_drawing_recorder.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_811b_drawing_recorder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_811c_viewport_processing.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_811c_viewport_processing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_812_drawing_graphic_proxy.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_812_drawing_graphic_proxy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_813_geo_interface.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_813_geo_interface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_814_text2path.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_814_text2path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_815_dxf_browser.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_815_dxf_browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_816_bin_packing.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_816_bin_packing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_817_genetic_algorithm.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_817_genetic_algorithm.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_818_meshex.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_818_meshex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_819_menger_sponge.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_819_menger_sponge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_820_openscad.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_820_openscad.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_821_hpgl2.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_821_hpgl2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_823_drawing_layout.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_823_drawing_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_824_svg_drawing_backend.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_824_svg_drawing_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_825_hpgl2_drawing_backend.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_825_hpgl2_drawing_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_826_custom_json_backend.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_826_custom_json_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_08_addons/test_827_geojson_backend.py` & `ezdxf-1.3.1b1/tests/test_08_addons/test_827_geojson_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_901_acc_vec2.py` & `ezdxf-1.3.1b1/tests/test_09_cython_acceleration/test_901_acc_vec2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_902_acc_vec3.py` & `ezdxf-1.3.1b1/tests/test_09_cython_acceleration/test_902_acc_vec3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_903_acc_matrix44.py` & `ezdxf-1.3.1b1/tests/test_09_cython_acceleration/test_903_acc_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py` & `ezdxf-1.3.1b1/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py` & `ezdxf-1.3.1b1/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_09_cython_acceleration/test_906_acc_bspline.py` & `ezdxf-1.3.1b1/tests/test_09_cython_acceleration/test_906_acc_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_10_issues/test_issue_1078_bbox_calculation.py` & `ezdxf-1.3.1b1/tests/test_10_issues/test_issue_1078_bbox_calculation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_10_issues/test_issue_414_bbox_calculation.py` & `ezdxf-1.3.1b1/tests/test_10_issues/test_issue_414_bbox_calculation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py` & `ezdxf-1.3.1b1/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_10_issues/test_issue_574_flattening_error.py` & `ezdxf-1.3.1b1/tests/test_10_issues/test_issue_574_flattening_error.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py` & `ezdxf-1.3.1b1/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_10_issues/test_issue_749_text_layout.py` & `ezdxf-1.3.1b1/tests/test_10_issues/test_issue_749_text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.1b0/tests/test_10_issues/test_issue_873_circle_inverted_normal.py` & `ezdxf-1.3.1b1/tests/test_10_issues/test_issue_873_circle_inverted_normal.py`

 * *Files identical despite different names*

