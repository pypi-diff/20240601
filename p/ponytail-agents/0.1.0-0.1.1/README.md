# Comparing `tmp/ponytail-agents-0.1.0.tar.gz` & `tmp/ponytail-agents-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ponytail-agents-0.1.0.tar", last modified: Sat Jun  1 13:13:35 2024, max compression
+gzip compressed data, was "ponytail-agents-0.1.1.tar", last modified: Sat Jun  1 13:23:29 2024, max compression
```

## Comparing `ponytail-agents-0.1.0.tar` & `ponytail-agents-0.1.1.tar`

### file list

```diff
@@ -1,119 +1,120 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 13:13:35.714762 ponytail-agents-0.1.0/
--rw-rw-rw-   0        0        0     3774 2024-05-28 10:54:43.000000 ponytail-agents-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3421 2024-06-01 13:13:35.714762 ponytail-agents-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2973 2024-05-31 14:08:52.000000 ponytail-agents-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 13:13:35.165233 ponytail-agents-0.1.0/ponytAIl/
--rw-rw-rw-   0        0        0        0 2024-05-30 10:37:23.000000 ponytail-agents-0.1.0/ponytAIl/__init__.py
--rw-rw-rw-   0        0        0     9836 2024-06-01 12:48:33.000000 ponytail-agents-0.1.0/ponytAIl/main.py
-drwxrwxrwx   0        0        0        0 2024-06-01 13:13:35.172201 ponytail-agents-0.1.0/ponytAIl/nodes_sample/
--rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample/concluder.md
--rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample/medium_sample.md
--rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample/node_creator.md
--rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample/starter.md
-drwxrwxrwx   0        0        0        0 2024-06-01 13:13:35.211956 ponytail-agents-0.1.0/ponytAIl/nodes_sample_definition_of_one/
--rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_definition_of_one/concluder.md
--rw-rw-rw-   0        0        0     2995 2024-05-30 17:13:59.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_definition_of_one/example_generator.md
--rw-rw-rw-   0        0        0     2243 2024-05-30 17:13:48.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_definition_of_one/math_concept_definition.md
--rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_definition_of_one/medium_sample.md
--rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_definition_of_one/node_creator.md
--rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_definition_of_one/starter.md
-drwxrwxrwx   0        0        0        0 2024-06-01 13:13:35.240942 ponytail-agents-0.1.0/ponytAIl/nodes_sample_ponytail/
--rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_ponytail/concluder.md
--rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_ponytail/medium_sample.md
--rw-rw-rw-   0        0        0     2647 2024-05-30 17:22:26.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_ponytail/name_combiner.md
--rw-rw-rw-   0        0        0     2907 2024-05-30 17:22:19.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_ponytail/name_generator.md
--rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_ponytail/node_creator.md
--rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_ponytail/starter.md
-drwxrwxrwx   0        0        0        0 2024-06-01 13:13:35.367241 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/
--rw-rw-rw-   0        0        0     2794 2024-05-30 18:17:11.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/anita_kumar.md
--rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/concluder.md
--rw-rw-rw-   0        0        0     2783 2024-05-30 18:18:55.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/david_brown.md
--rw-rw-rw-   0        0        0     8490 2024-05-30 18:18:14.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/gloria_martinez.md
--rw-rw-rw-   0        0        0     2932 2024-05-30 18:16:25.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/john_smith.md
--rw-rw-rw-   0        0        0     3130 2024-05-30 18:17:04.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/kevin_white.md
--rw-rw-rw-   0        0        0     3438 2024-05-30 18:17:19.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/li_wang.md
--rw-rw-rw-   0        0        0     4292 2024-05-30 18:16:57.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/maria_garcia.md
--rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/medium_sample.md
--rw-rw-rw-   0        0        0     4035 2024-05-30 18:18:35.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/michael_clark.md
--rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/node_creator.md
--rw-rw-rw-   0        0        0     3697 2024-05-30 18:16:49.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/sarah_johnson.md
--rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/starter.md
--rw-rw-rw-   0        0        0     5167 2024-05-30 18:18:44.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/yuki_tanaka.md
-drwxrwxrwx   0        0        0        0 2024-06-01 13:13:35.564793 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/
--rw-rw-rw-   0        0        0     2853 2024-05-30 18:28:28.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Ahmed_El-Sayed.md
--rw-rw-rw-   0        0        0     4853 2024-05-30 18:27:50.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Aisha_Khan.md
--rw-rw-rw-   0        0        0     2215 2024-05-30 18:33:14.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Carlos_Mendez.md
--rw-rw-rw-   0        0        0     4732 2024-05-30 18:29:06.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Elena_Petrov.md
--rw-rw-rw-   0        0        0     4884 2024-05-30 18:28:20.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Emily_Johnson.md
--rw-rw-rw-   0        0        0     5106 2024-05-30 18:33:41.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Emma_Jones.md
--rw-rw-rw-   0        0        0     6670 2024-05-30 18:33:04.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Fatou_Sangare.md
--rw-rw-rw-   0        0        0     2418 2024-05-30 18:27:58.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Haruto_Yamamoto.md
--rw-rw-rw-   0        0        0     4207 2024-05-30 18:27:31.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/John_Smith.md
--rw-rw-rw-   0        0        0     3226 2024-05-30 18:33:22.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Keisha_Anderson.md
--rw-rw-rw-   0        0        0     3599 2024-05-30 18:27:38.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Maria_Gonzalez.md
--rw-rw-rw-   0        0        0     3967 2024-05-30 18:33:31.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Mohammed_Al-Farsi.md
--rw-rw-rw-   0        0        0     2620 2024-05-30 18:28:57.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Olusegun_Adeyemi.md
--rw-rw-rw-   0        0        0     3278 2024-05-30 18:28:36.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Sofia_Rossi.md
--rw-rw-rw-   0        0        0     4576 2024-05-30 18:28:45.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Wei_Liu.md
--rw-rw-rw-   0        0        0     2359 2024-05-30 18:32:53.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Zhang_Wei.md
--rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/concluder.md
--rw-rw-rw-   0        0        0     2232 2024-05-30 18:43:18.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/math_assessment.md
--rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/medium_sample.md
--rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/node_creator.md
--rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/starter.md
-drwxrwxrwx   0        0        0        0 2024-06-01 13:13:35.595828 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/
--rw-rw-rw-   0        0        0     2059 2024-05-31 12:23:33.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/blacksmith_emily.md
--rw-rw-rw-   0        0        0     2831 2024-05-31 12:28:39.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/blacksmith_tomas.md
--rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/concluder.md
--rw-rw-rw-   0        0        0     4337 2024-05-31 12:28:20.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/farmer_jane.md
--rw-rw-rw-   0        0        0     2998 2024-05-31 12:22:54.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/farmer_john.md
--rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/medium_sample.md
--rw-rw-rw-   0        0        0     5227 2024-05-31 12:29:41.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/merchant_sophia.md
--rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/node_creator.md
--rw-rw-rw-   0        0        0     4254 2024-05-31 12:28:46.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/seamstress_maria.md
--rw-rw-rw-   0        0        0     4589 2024-05-31 12:23:14.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/seamstress_sarah.md
--rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/starter.md
--rw-rw-rw-   0        0        0     3858 2024-05-31 12:29:47.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/teacher_daniel.md
--rw-rw-rw-   0        0        0     5001 2024-05-31 12:29:22.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/woodcarver_lucas.md
--rw-rw-rw-   0        0        0     2776 2024-05-31 12:23:24.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/woodcarver_max.md
-drwxrwxrwx   0        0        0        0 2024-06-01 13:13:35.665156 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/
--rw-rw-rw-   0        0        0     3293 2024-06-01 12:55:43.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/aaron_davis.md
--rw-rw-rw-   0        0        0     4559 2024-06-01 12:50:08.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/abdul_rahman.md
--rw-rw-rw-   0        0        0     3884 2024-06-01 12:49:39.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/alice_smith.md
--rw-rw-rw-   0        0        0     2533 2024-06-01 12:50:42.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/anika_singh.md
--rw-rw-rw-   0        0        0     4072 2024-06-01 12:49:45.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/carlos_garcia.md
--rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/concluder.md
--rw-rw-rw-   0        0        0     2381 2024-06-01 12:54:42.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/david_hernandez.md
--rw-rw-rw-   0        0        0     3282 2024-06-01 12:49:51.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/emily_johnson.md
--rw-rw-rw-   0        0        0    15863 2024-06-01 12:55:37.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/fatima_zaidi.md
--rw-rw-rw-   0        0        0     4484 2024-06-01 13:03:19.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/grace_anderson.md
--rw-rw-rw-   0        0        0     3837 2024-06-01 13:02:55.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/isabella_rodriguez.md
--rw-rw-rw-   0        0        0     3449 2024-06-01 12:54:38.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/jacqueline_miller.md
--rw-rw-rw-   0        0        0     3856 2024-06-01 13:02:49.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/james_mitchell.md
--rw-rw-rw-   0        0        0     2977 2024-06-01 13:03:47.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/jason_turner.md
--rw-rw-rw-   0        0        0     3016 2024-06-01 12:49:29.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/john_doe.md
--rw-rw-rw-   0        0        0     7485 2024-06-01 12:55:05.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/li_yan.md
--rw-rw-rw-   0        0        0     2670 2024-06-01 13:03:39.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/linda_thompson.md
--rw-rw-rw-   0        0        0     2802 2024-06-01 12:50:35.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/lucas_kim.md
--rw-rw-rw-   0        0        0     3348 2024-06-01 12:50:28.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/marie_dubois.md
--rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/medium_sample.md
--rw-rw-rw-   0        0        0     3900 2024-06-01 12:54:32.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/michael_lee.md
--rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/node_creator.md
--rw-rw-rw-   0        0        0     4064 2024-06-01 12:50:22.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/oliver_taylor.md
--rw-rw-rw-   0        0        0     5337 2024-06-01 13:02:42.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/olivia_jones.md
--rw-rw-rw-   0        0        0     4453 2024-06-01 12:54:50.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/rachel_green.md
--rw-rw-rw-   0        0        0     3405 2024-06-01 13:03:01.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/ryan_clark.md
--rw-rw-rw-   0        0        0     4935 2024-06-01 13:03:33.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/samuel_brown.md
--rw-rw-rw-   0        0        0     3749 2024-06-01 12:55:51.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/sandra_brown.md
--rw-rw-rw-   0        0        0     1894 2024-06-01 12:54:21.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/sophia_khan.md
--rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/starter.md
--rw-rw-rw-   0        0        0     5606 2024-06-01 12:56:09.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/thomas_evans.md
--rw-rw-rw-   0        0        0     5299 2024-06-01 12:50:15.000000 ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/ying_chen.md
-drwxrwxrwx   0        0        0        0 2024-06-01 13:13:35.712036 ponytail-agents-0.1.0/ponytail_agents.egg-info/
--rw-rw-rw-   0        0        0     3421 2024-06-01 13:13:34.000000 ponytail-agents-0.1.0/ponytail_agents.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5049 2024-06-01 13:13:35.000000 ponytail-agents-0.1.0/ponytail_agents.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 13:13:34.000000 ponytail-agents-0.1.0/ponytail_agents.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-06-01 13:13:34.000000 ponytail-agents-0.1.0/ponytail_agents.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-01 13:13:34.000000 ponytail-agents-0.1.0/ponytail_agents.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 13:13:35.715958 ponytail-agents-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      909 2024-06-01 13:07:34.000000 ponytail-agents-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 13:23:29.698354 ponytail-agents-0.1.1/
+-rw-rw-rw-   0        0        0     3774 2024-05-28 10:54:43.000000 ponytail-agents-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3428 2024-06-01 13:23:29.698354 ponytail-agents-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2980 2024-06-01 13:22:32.000000 ponytail-agents-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 13:23:29.498819 ponytail-agents-0.1.1/ponytAIl/
+-rw-rw-rw-   0        0        0        0 2024-05-30 10:37:23.000000 ponytail-agents-0.1.1/ponytAIl/__init__.py
+-rw-rw-rw-   0        0        0     9836 2024-06-01 12:48:33.000000 ponytail-agents-0.1.1/ponytAIl/main.py
+drwxrwxrwx   0        0        0        0 2024-06-01 13:23:29.503958 ponytail-agents-0.1.1/ponytAIl/nodes_sample/
+-rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample/concluder.md
+-rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample/medium_sample.md
+-rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample/node_creator.md
+-rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample/starter.md
+drwxrwxrwx   0        0        0        0 2024-06-01 13:23:29.509868 ponytail-agents-0.1.1/ponytAIl/nodes_sample_definition_of_one/
+-rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_definition_of_one/concluder.md
+-rw-rw-rw-   0        0        0     2995 2024-05-30 17:13:59.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_definition_of_one/example_generator.md
+-rw-rw-rw-   0        0        0     2243 2024-05-30 17:13:48.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_definition_of_one/math_concept_definition.md
+-rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_definition_of_one/medium_sample.md
+-rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_definition_of_one/node_creator.md
+-rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_definition_of_one/starter.md
+drwxrwxrwx   0        0        0        0 2024-06-01 13:23:29.520673 ponytail-agents-0.1.1/ponytAIl/nodes_sample_ponytail/
+-rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_ponytail/concluder.md
+-rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_ponytail/medium_sample.md
+-rw-rw-rw-   0        0        0     2647 2024-05-30 17:22:26.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_ponytail/name_combiner.md
+-rw-rw-rw-   0        0        0     2907 2024-05-30 17:22:19.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_ponytail/name_generator.md
+-rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_ponytail/node_creator.md
+-rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_ponytail/starter.md
+drwxrwxrwx   0        0        0        0 2024-06-01 13:23:29.544905 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/
+-rw-rw-rw-   0        0        0     2794 2024-05-30 18:17:11.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/anita_kumar.md
+-rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/concluder.md
+-rw-rw-rw-   0        0        0     2783 2024-05-30 18:18:55.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/david_brown.md
+-rw-rw-rw-   0        0        0     8490 2024-05-30 18:18:14.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/gloria_martinez.md
+-rw-rw-rw-   0        0        0     2932 2024-05-30 18:16:25.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/john_smith.md
+-rw-rw-rw-   0        0        0     3130 2024-05-30 18:17:04.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/kevin_white.md
+-rw-rw-rw-   0        0        0     3438 2024-05-30 18:17:19.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/li_wang.md
+-rw-rw-rw-   0        0        0     4292 2024-05-30 18:16:57.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/maria_garcia.md
+-rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/medium_sample.md
+-rw-rw-rw-   0        0        0     4035 2024-05-30 18:18:35.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/michael_clark.md
+-rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/node_creator.md
+-rw-rw-rw-   0        0        0     3697 2024-05-30 18:16:49.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/sarah_johnson.md
+-rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/starter.md
+-rw-rw-rw-   0        0        0     5167 2024-05-30 18:18:44.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/yuki_tanaka.md
+drwxrwxrwx   0        0        0        0 2024-06-01 13:23:29.572769 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/
+-rw-rw-rw-   0        0        0     2853 2024-05-30 18:28:28.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Ahmed_El-Sayed.md
+-rw-rw-rw-   0        0        0     4853 2024-05-30 18:27:50.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Aisha_Khan.md
+-rw-rw-rw-   0        0        0     2215 2024-05-30 18:33:14.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Carlos_Mendez.md
+-rw-rw-rw-   0        0        0     4732 2024-05-30 18:29:06.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Elena_Petrov.md
+-rw-rw-rw-   0        0        0     4884 2024-05-30 18:28:20.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Emily_Johnson.md
+-rw-rw-rw-   0        0        0     5106 2024-05-30 18:33:41.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Emma_Jones.md
+-rw-rw-rw-   0        0        0     6670 2024-05-30 18:33:04.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Fatou_Sangare.md
+-rw-rw-rw-   0        0        0     2418 2024-05-30 18:27:58.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Haruto_Yamamoto.md
+-rw-rw-rw-   0        0        0     4207 2024-05-30 18:27:31.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/John_Smith.md
+-rw-rw-rw-   0        0        0     3226 2024-05-30 18:33:22.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Keisha_Anderson.md
+-rw-rw-rw-   0        0        0     3599 2024-05-30 18:27:38.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Maria_Gonzalez.md
+-rw-rw-rw-   0        0        0     3967 2024-05-30 18:33:31.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Mohammed_Al-Farsi.md
+-rw-rw-rw-   0        0        0     2620 2024-05-30 18:28:57.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Olusegun_Adeyemi.md
+-rw-rw-rw-   0        0        0     3278 2024-05-30 18:28:36.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Sofia_Rossi.md
+-rw-rw-rw-   0        0        0     4576 2024-05-30 18:28:45.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Wei_Liu.md
+-rw-rw-rw-   0        0        0     2359 2024-05-30 18:32:53.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Zhang_Wei.md
+-rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/concluder.md
+-rw-rw-rw-   0        0        0     2232 2024-05-30 18:43:18.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/math_assessment.md
+-rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/medium_sample.md
+-rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/node_creator.md
+-rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/starter.md
+drwxrwxrwx   0        0        0        0 2024-06-01 13:23:29.588392 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/
+-rw-rw-rw-   0        0        0     2059 2024-05-31 12:23:33.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/blacksmith_emily.md
+-rw-rw-rw-   0        0        0     2831 2024-05-31 12:28:39.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/blacksmith_tomas.md
+-rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/concluder.md
+-rw-rw-rw-   0        0        0     4337 2024-05-31 12:28:20.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/farmer_jane.md
+-rw-rw-rw-   0        0        0     2998 2024-05-31 12:22:54.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/farmer_john.md
+-rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/medium_sample.md
+-rw-rw-rw-   0        0        0     5227 2024-05-31 12:29:41.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/merchant_sophia.md
+-rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/node_creator.md
+-rw-rw-rw-   0        0        0     4254 2024-05-31 12:28:46.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/seamstress_maria.md
+-rw-rw-rw-   0        0        0     4589 2024-05-31 12:23:14.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/seamstress_sarah.md
+-rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/starter.md
+-rw-rw-rw-   0        0        0     3858 2024-05-31 12:29:47.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/teacher_daniel.md
+-rw-rw-rw-   0        0        0     5001 2024-05-31 12:29:22.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/woodcarver_lucas.md
+-rw-rw-rw-   0        0        0     2776 2024-05-31 12:23:24.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/woodcarver_max.md
+drwxrwxrwx   0        0        0        0 2024-06-01 13:23:29.651010 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/
+-rw-rw-rw-   0        0        0     3293 2024-06-01 12:55:43.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/aaron_davis.md
+-rw-rw-rw-   0        0        0     4559 2024-06-01 12:50:08.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/abdul_rahman.md
+-rw-rw-rw-   0        0        0     3884 2024-06-01 12:49:39.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/alice_smith.md
+-rw-rw-rw-   0        0        0     2533 2024-06-01 12:50:42.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/anika_singh.md
+-rw-rw-rw-   0        0        0     4072 2024-06-01 12:49:45.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/carlos_garcia.md
+-rw-rw-rw-   0        0        0      792 2024-05-22 06:08:35.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/concluder.md
+-rw-rw-rw-   0        0        0     2381 2024-06-01 12:54:42.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/david_hernandez.md
+-rw-rw-rw-   0        0        0     3282 2024-06-01 12:49:51.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/emily_johnson.md
+-rw-rw-rw-   0        0        0    15863 2024-06-01 12:55:37.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/fatima_zaidi.md
+-rw-rw-rw-   0        0        0     4484 2024-06-01 13:03:19.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/grace_anderson.md
+-rw-rw-rw-   0        0        0     3837 2024-06-01 13:02:55.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/isabella_rodriguez.md
+-rw-rw-rw-   0        0        0     3449 2024-06-01 12:54:38.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/jacqueline_miller.md
+-rw-rw-rw-   0        0        0     3856 2024-06-01 13:02:49.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/james_mitchell.md
+-rw-rw-rw-   0        0        0     2977 2024-06-01 13:03:47.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/jason_turner.md
+-rw-rw-rw-   0        0        0     3016 2024-06-01 12:49:29.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/john_doe.md
+-rw-rw-rw-   0        0        0     7485 2024-06-01 12:55:05.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/li_yan.md
+-rw-rw-rw-   0        0        0     2670 2024-06-01 13:03:39.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/linda_thompson.md
+-rw-rw-rw-   0        0        0     2802 2024-06-01 12:50:35.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/lucas_kim.md
+-rw-rw-rw-   0        0        0     3348 2024-06-01 12:50:28.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/marie_dubois.md
+-rw-rw-rw-   0        0        0     2084 2024-05-31 12:27:26.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/medium_sample.md
+-rw-rw-rw-   0        0        0     3900 2024-06-01 12:54:32.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/michael_lee.md
+-rw-rw-rw-   0        0        0     2863 2024-05-31 12:25:31.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/node_creator.md
+-rw-rw-rw-   0        0        0     4064 2024-06-01 12:50:22.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/oliver_taylor.md
+-rw-rw-rw-   0        0        0     5337 2024-06-01 13:02:42.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/olivia_jones.md
+-rw-rw-rw-   0        0        0     4453 2024-06-01 12:54:50.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/rachel_green.md
+-rw-rw-rw-   0        0        0     3405 2024-06-01 13:03:01.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/ryan_clark.md
+-rw-rw-rw-   0        0        0     4935 2024-06-01 13:03:33.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/samuel_brown.md
+-rw-rw-rw-   0        0        0     3749 2024-06-01 12:55:51.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/sandra_brown.md
+-rw-rw-rw-   0        0        0     1894 2024-06-01 12:54:21.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/sophia_khan.md
+-rw-rw-rw-   0        0        0     1524 2024-05-31 12:27:26.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/starter.md
+-rw-rw-rw-   0        0        0     5606 2024-06-01 12:56:09.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/thomas_evans.md
+-rw-rw-rw-   0        0        0     5299 2024-06-01 12:50:15.000000 ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/ying_chen.md
+drwxrwxrwx   0        0        0        0 2024-06-01 13:23:29.698354 ponytail-agents-0.1.1/ponytail_agents.egg-info/
+-rw-rw-rw-   0        0        0     3428 2024-06-01 13:23:29.000000 ponytail-agents-0.1.1/ponytail_agents.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5091 2024-06-01 13:23:29.000000 ponytail-agents-0.1.1/ponytail_agents.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 13:23:29.000000 ponytail-agents-0.1.1/ponytail_agents.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-06-01 13:23:29.000000 ponytail-agents-0.1.1/ponytail_agents.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       68 2024-06-01 13:23:29.000000 ponytail-agents-0.1.1/ponytail_agents.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-01 13:23:29.000000 ponytail-agents-0.1.1/ponytail_agents.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 13:23:29.698354 ponytail-agents-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2024-06-01 13:23:04.000000 ponytail-agents-0.1.1/setup.py
```

### Comparing `ponytail-agents-0.1.0/LICENSE` & `ponytail-agents-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/PKG-INFO` & `ponytail-agents-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ponytail-agents
-Version: 0.1.0
+Version: 0.1.1
 Summary: ponytAIl: Polymorphic Orchestration of Networked Youthful, Adaptable Intelligence with Language.
 Home-page: https://github.com/thepioneerjp/ponytAIl
 Author: The Pioneer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ponytAIl
-ponytAIl: Polymorphic Orchestration of Networked Youthful, Adaptable Intelligence with Language is an node based multi-agent system targeting both LLM and BCI (in the future)
+ponytAIl: Polymorphic Orchestration of Networked Youthful, Adaptable Intelligence with Language. It is an node based multi-agent system targeting both LLM and BCI (in the future)
 
 ## Installation
 
 Install ponytAIl using pip:
 
 ```
 pip install ponytail-agents
@@ -29,19 +29,21 @@
 - `-g`, `--goal` (Required): Goal or objective of the task.
 - `-m`, `--model` (Optional, default: "random-fast"): Name of the model to use. For available models, refer to the [FLUTE repository](https://github.com/ThePioneerJP/FLUTE).
 - `-r`, `--result` (Optional): Additional result or output.
 
 ### Example Commands
 
 ```bash
-ponytail-agents -f "YOUR_DIRECTORY\starter.md" -g "Define the number 1 using the mathematical collection"
-
-ponytail-agents -f "YOUR_DIRECTORY\starter.md" -g "Generate 5 candidate names for the self-reproducive LLM based multi-agent system. Note that the name must be abbreviated to 'PONYTAIL.'"
-
-ponytail-agents -f "YOUR_DIRECTORY\starter.md" -g "You are a villager. Send CREATE_NODES request by outlining other villagers, until you are satisfied with the diversity of the community. Use their names as the file names. Setup their profiles (ex. jobs, families, age, gender, etc) in a realistic and detailed manner. After, and ONLY after you are satisfied with the listed villagers, SEND_TO concluder.md to end the process."
+ponytail -f "YOUR_DIRECTORY\starter.md" -g "Define the number 1 using the mathematical collection"
+```
+```bash
+ponytail -f "YOUR_DIRECTORY\starter.md" -g "Generate 5 candidate names for the self-reproducive LLM based multi-agent system. Note that the name must be abbreviated to 'PONYTAIL.'"
+```
+```bash
+ponytail -f "YOUR_DIRECTORY\starter.md" -g "You are a villager. Send CREATE_NODES request by outlining other villagers, until you are satisfied with the diversity of the community. Use their names as the file names. Setup their profiles (ex. jobs, families, age, gender, etc) in a realistic and detailed manner. After, and ONLY after you are satisfied with the listed villagers, SEND_TO concluder.md to end the process."
 ```
 
 ### Prerequisites
 
 To run ponytAIl, prepare a folder containing all the files from `nodes_sample`: `concluder.md`, `starter.md`, and `node_creator.md`.
 
 If you want to include additional nodes from the beginning, create them following the format of `medium_sample.md`.
```

### Comparing `ponytail-agents-0.1.0/README.md` & `ponytail-agents-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ponytAIl
-ponytAIl: Polymorphic Orchestration of Networked Youthful, Adaptable Intelligence with Language is an node based multi-agent system targeting both LLM and BCI (in the future)
+ponytAIl: Polymorphic Orchestration of Networked Youthful, Adaptable Intelligence with Language. It is an node based multi-agent system targeting both LLM and BCI (in the future)
 
 ## Installation
 
 Install ponytAIl using pip:
 
 ```
 pip install ponytail-agents
@@ -17,19 +17,21 @@
 - `-g`, `--goal` (Required): Goal or objective of the task.
 - `-m`, `--model` (Optional, default: "random-fast"): Name of the model to use. For available models, refer to the [FLUTE repository](https://github.com/ThePioneerJP/FLUTE).
 - `-r`, `--result` (Optional): Additional result or output.
 
 ### Example Commands
 
 ```bash
-ponytail-agents -f "YOUR_DIRECTORY\starter.md" -g "Define the number 1 using the mathematical collection"
-
-ponytail-agents -f "YOUR_DIRECTORY\starter.md" -g "Generate 5 candidate names for the self-reproducive LLM based multi-agent system. Note that the name must be abbreviated to 'PONYTAIL.'"
-
-ponytail-agents -f "YOUR_DIRECTORY\starter.md" -g "You are a villager. Send CREATE_NODES request by outlining other villagers, until you are satisfied with the diversity of the community. Use their names as the file names. Setup their profiles (ex. jobs, families, age, gender, etc) in a realistic and detailed manner. After, and ONLY after you are satisfied with the listed villagers, SEND_TO concluder.md to end the process."
+ponytail -f "YOUR_DIRECTORY\starter.md" -g "Define the number 1 using the mathematical collection"
+```
+```bash
+ponytail -f "YOUR_DIRECTORY\starter.md" -g "Generate 5 candidate names for the self-reproducive LLM based multi-agent system. Note that the name must be abbreviated to 'PONYTAIL.'"
+```
+```bash
+ponytail -f "YOUR_DIRECTORY\starter.md" -g "You are a villager. Send CREATE_NODES request by outlining other villagers, until you are satisfied with the diversity of the community. Use their names as the file names. Setup their profiles (ex. jobs, families, age, gender, etc) in a realistic and detailed manner. After, and ONLY after you are satisfied with the listed villagers, SEND_TO concluder.md to end the process."
 ```
 
 ### Prerequisites
 
 To run ponytAIl, prepare a folder containing all the files from `nodes_sample`: `concluder.md`, `starter.md`, and `node_creator.md`.
 
 If you want to include additional nodes from the beginning, create them following the format of `medium_sample.md`.
```

### Comparing `ponytail-agents-0.1.0/ponytAIl/main.py` & `ponytail-agents-0.1.1/ponytAIl/main.py`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample/concluder.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample/concluder.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample/medium_sample.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample/medium_sample.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample/node_creator.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample/node_creator.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample/starter.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample/starter.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_definition_of_one/concluder.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_definition_of_one/concluder.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_definition_of_one/example_generator.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_definition_of_one/example_generator.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_definition_of_one/math_concept_definition.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_definition_of_one/math_concept_definition.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_definition_of_one/medium_sample.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_definition_of_one/medium_sample.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_definition_of_one/node_creator.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_definition_of_one/node_creator.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_definition_of_one/starter.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_definition_of_one/starter.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_ponytail/concluder.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_ponytail/concluder.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_ponytail/medium_sample.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_ponytail/medium_sample.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_ponytail/name_combiner.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_ponytail/name_combiner.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_ponytail/name_generator.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_ponytail/name_generator.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_ponytail/node_creator.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_ponytail/node_creator.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_ponytail/starter.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_ponytail/starter.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/anita_kumar.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/anita_kumar.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/concluder.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/concluder.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/david_brown.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/david_brown.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/gloria_martinez.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/gloria_martinez.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/john_smith.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/john_smith.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/kevin_white.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/kevin_white.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/li_wang.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/li_wang.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/maria_garcia.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/maria_garcia.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/medium_sample.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/medium_sample.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/michael_clark.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/michael_clark.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/node_creator.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/node_creator.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/sarah_johnson.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/sarah_johnson.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/starter.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/starter.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers/yuki_tanaka.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers/yuki_tanaka.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Ahmed_El-Sayed.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Ahmed_El-Sayed.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Aisha_Khan.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Aisha_Khan.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Carlos_Mendez.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Carlos_Mendez.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Elena_Petrov.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Elena_Petrov.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Emily_Johnson.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Emily_Johnson.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Emma_Jones.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Emma_Jones.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Fatou_Sangare.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Fatou_Sangare.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Haruto_Yamamoto.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Haruto_Yamamoto.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/John_Smith.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/John_Smith.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Keisha_Anderson.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Keisha_Anderson.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Maria_Gonzalez.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Maria_Gonzalez.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Mohammed_Al-Farsi.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Mohammed_Al-Farsi.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Olusegun_Adeyemi.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Olusegun_Adeyemi.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Sofia_Rossi.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Sofia_Rossi.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Wei_Liu.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Wei_Liu.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/Zhang_Wei.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/Zhang_Wei.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/concluder.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/concluder.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/math_assessment.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/math_assessment.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/medium_sample.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/medium_sample.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/node_creator.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/node_creator.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_2/starter.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_2/starter.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/blacksmith_emily.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/blacksmith_emily.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/blacksmith_tomas.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/blacksmith_tomas.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/concluder.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/concluder.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/farmer_jane.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/farmer_jane.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/farmer_john.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/farmer_john.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/medium_sample.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/medium_sample.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/merchant_sophia.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/merchant_sophia.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/node_creator.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/node_creator.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/seamstress_maria.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/seamstress_maria.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/seamstress_sarah.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/seamstress_sarah.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/starter.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/starter.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/teacher_daniel.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/teacher_daniel.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/woodcarver_lucas.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/woodcarver_lucas.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_3/woodcarver_max.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_3/woodcarver_max.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/aaron_davis.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/aaron_davis.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/abdul_rahman.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/abdul_rahman.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/alice_smith.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/alice_smith.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/anika_singh.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/anika_singh.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/carlos_garcia.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/carlos_garcia.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/concluder.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/concluder.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/david_hernandez.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/david_hernandez.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/emily_johnson.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/emily_johnson.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/fatima_zaidi.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/fatima_zaidi.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/grace_anderson.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/grace_anderson.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/isabella_rodriguez.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/isabella_rodriguez.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/jacqueline_miller.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/jacqueline_miller.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/james_mitchell.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/james_mitchell.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/jason_turner.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/jason_turner.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/john_doe.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/john_doe.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/li_yan.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/li_yan.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/linda_thompson.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/linda_thompson.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/lucas_kim.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/lucas_kim.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/marie_dubois.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/marie_dubois.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/medium_sample.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/medium_sample.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/michael_lee.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/michael_lee.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/node_creator.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/node_creator.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/oliver_taylor.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/oliver_taylor.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/olivia_jones.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/olivia_jones.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/rachel_green.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/rachel_green.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/ryan_clark.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/ryan_clark.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/samuel_brown.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/samuel_brown.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/sandra_brown.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/sandra_brown.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/sophia_khan.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/sophia_khan.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/starter.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/starter.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/thomas_evans.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/thomas_evans.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytAIl/nodes_sample_villagers_4/ying_chen.md` & `ponytail-agents-0.1.1/ponytAIl/nodes_sample_villagers_4/ying_chen.md`

 * *Files identical despite different names*

### Comparing `ponytail-agents-0.1.0/ponytail_agents.egg-info/PKG-INFO` & `ponytail-agents-0.1.1/ponytail_agents.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ponytail-agents
-Version: 0.1.0
+Version: 0.1.1
 Summary: ponytAIl: Polymorphic Orchestration of Networked Youthful, Adaptable Intelligence with Language.
 Home-page: https://github.com/thepioneerjp/ponytAIl
 Author: The Pioneer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ponytAIl
-ponytAIl: Polymorphic Orchestration of Networked Youthful, Adaptable Intelligence with Language is an node based multi-agent system targeting both LLM and BCI (in the future)
+ponytAIl: Polymorphic Orchestration of Networked Youthful, Adaptable Intelligence with Language. It is an node based multi-agent system targeting both LLM and BCI (in the future)
 
 ## Installation
 
 Install ponytAIl using pip:
 
 ```
 pip install ponytail-agents
@@ -29,19 +29,21 @@
 - `-g`, `--goal` (Required): Goal or objective of the task.
 - `-m`, `--model` (Optional, default: "random-fast"): Name of the model to use. For available models, refer to the [FLUTE repository](https://github.com/ThePioneerJP/FLUTE).
 - `-r`, `--result` (Optional): Additional result or output.
 
 ### Example Commands
 
 ```bash
-ponytail-agents -f "YOUR_DIRECTORY\starter.md" -g "Define the number 1 using the mathematical collection"
-
-ponytail-agents -f "YOUR_DIRECTORY\starter.md" -g "Generate 5 candidate names for the self-reproducive LLM based multi-agent system. Note that the name must be abbreviated to 'PONYTAIL.'"
-
-ponytail-agents -f "YOUR_DIRECTORY\starter.md" -g "You are a villager. Send CREATE_NODES request by outlining other villagers, until you are satisfied with the diversity of the community. Use their names as the file names. Setup their profiles (ex. jobs, families, age, gender, etc) in a realistic and detailed manner. After, and ONLY after you are satisfied with the listed villagers, SEND_TO concluder.md to end the process."
+ponytail -f "YOUR_DIRECTORY\starter.md" -g "Define the number 1 using the mathematical collection"
+```
+```bash
+ponytail -f "YOUR_DIRECTORY\starter.md" -g "Generate 5 candidate names for the self-reproducive LLM based multi-agent system. Note that the name must be abbreviated to 'PONYTAIL.'"
+```
+```bash
+ponytail -f "YOUR_DIRECTORY\starter.md" -g "You are a villager. Send CREATE_NODES request by outlining other villagers, until you are satisfied with the diversity of the community. Use their names as the file names. Setup their profiles (ex. jobs, families, age, gender, etc) in a realistic and detailed manner. After, and ONLY after you are satisfied with the listed villagers, SEND_TO concluder.md to end the process."
 ```
 
 ### Prerequisites
 
 To run ponytAIl, prepare a folder containing all the files from `nodes_sample`: `concluder.md`, `starter.md`, and `node_creator.md`.
 
 If you want to include additional nodes from the beginning, create them following the format of `medium_sample.md`.
```

### Comparing `ponytail-agents-0.1.0/ponytail_agents.egg-info/SOURCES.txt` & `ponytail-agents-0.1.1/ponytail_agents.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -99,9 +99,10 @@
 ponytAIl/nodes_sample_villagers_4/sophia_khan.md
 ponytAIl/nodes_sample_villagers_4/starter.md
 ponytAIl/nodes_sample_villagers_4/thomas_evans.md
 ponytAIl/nodes_sample_villagers_4/ying_chen.md
 ponytail_agents.egg-info/PKG-INFO
 ponytail_agents.egg-info/SOURCES.txt
 ponytail_agents.egg-info/dependency_links.txt
+ponytail_agents.egg-info/entry_points.txt
 ponytail_agents.egg-info/requires.txt
 ponytail_agents.egg-info/top_level.txt
```

### Comparing `ponytail-agents-0.1.0/setup.py` & `ponytail-agents-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ponytail-agents',
-    version='0.1.0',
+    version='0.1.1',
     description='ponytAIl: Polymorphic Orchestration of Networked Youthful, Adaptable Intelligence with Language.',
     author='The Pioneer',
     url='https://github.com/thepioneerjp/ponytAIl',
     packages=find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
@@ -22,8 +22,13 @@
         'ponytAIl': ['**/*'],
     },
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
     ],
+    entry_points={
+        "console_scripts": [
+            "ponytail=ponytail.main:main",
+        ],
+    },
 )
```

