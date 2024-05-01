# Comparing `tmp/minecraft-resource-pack-1.4.1.tar.gz` & `tmp/minecraft_resource_pack-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minecraft-resource-pack-1.4.1.tar", last modified: Fri Dec  8 14:55:23 2023, max compression
+gzip compressed data, was "minecraft_resource_pack-1.4.2.tar", last modified: Wed May  1 11:21:50 2024, max compression
```

## Comparing `minecraft-resource-pack-1.4.1.tar` & `minecraft_resource_pack-1.4.2.tar`

### file list

```diff
@@ -1,507 +1,507 @@
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.409711 minecraft-resource-pack-1.4.1/
--rw-rw-rw-   0        0        0     6954 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/LICENSE
--rw-rw-rw-   0        0        0      206 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0      876 2023-12-08 14:55:23.409711 minecraft-resource-pack-1.4.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.409711 minecraft-resource-pack-1.4.1/minecraft_model_reader/
--rw-rw-rw-   0        0        0      910 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.159659 minecraft-resource-pack-1.4.1/minecraft_model_reader/__pyinstaller/
--rw-rw-rw-   0        0        0       43 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/__pyinstaller/__init__.py
--rw-rw-rw-   0        0        0      194 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/__pyinstaller/hook-minecraft_model_reader.py
--rw-rw-rw-   0        0        0      518 2023-12-08 14:55:23.409711 minecraft-resource-pack-1.4.1/minecraft_model_reader/_version.py
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.159659 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/
--rw-rw-rw-   0        0        0      186 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.159659 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/amulet/
--rw-rw-rw-   0        0        0        0 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/amulet/__init__.py
--rw-rw-rw-   0        0        0    18894 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/amulet/block.py
--rw-rw-rw-   0        0        0     6410 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/comment_json.py
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.159659 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/image/
--rw-rw-rw-   0        0        0      189 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/image/__init__.py
--rw-rw-rw-   0        0        0      176 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/image/missing_no.png
--rw-rw-rw-   0        0        0    11085 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/image/missing_pack_java.png
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.159659 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/mesh/
--rw-rw-rw-   0        0        0        0 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/mesh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.175288 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/mesh/block/
--rw-rw-rw-   0        0        0       35 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/mesh/block/__init__.py
--rw-rw-rw-   0        0        0    13838 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/mesh/block/block_mesh.py
--rw-rw-rw-   0        0        0     4764 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/mesh/block/cube.py
--rw-rw-rw-   0        0        0      545 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/mesh/block/missing_block.py
--rw-rw-rw-   0        0        0      507 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/mesh/util.py
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.175288 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/
--rw-rw-rw-   0        0        0     1908 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.175288 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/base/
--rw-rw-rw-   0        0        0      105 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/base/__init__.py
--rw-rw-rw-   0        0        0     1128 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/base/resource_pack.py
--rw-rw-rw-   0        0        0     2908 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/base/resource_pack_manager.py
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.175288 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/
--rw-rw-rw-   0        0        0      111 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.175288 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/
--rw-rw-rw-   0        0        0      967 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/blocks.json
--rw-rw-rw-   0        0        0      555 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/manifest.json
--rw-rw-rw-   0        0        0    32642 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/pack_icon.png
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.175288 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.175288 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/
--rw-rw-rw-   0        0        0      580 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/grass_carried.png
--rw-rw-rw-   0        0        0      408 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/grass_side_carried.png
--rw-rw-rw-   0        0        0      927 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/water.png
--rw-rw-rw-   0        0        0      428 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/terrain_texture.json
--rw-rw-rw-   0        0        0  2864161 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/block_palette.json
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.206538 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/
--rw-rw-rw-   0        0        0     1065 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/__init__.py
--rw-rw-rw-   0        0        0     1027 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/air.py
--rw-rw-rw-   0        0        0      905 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/base_blockshape.py
--rw-rw-rw-   0        0        0      736 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/bubble_column.py
--rw-rw-rw-   0        0        0     1099 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cake.py
--rw-rw-rw-   0        0        0     1443 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/chest.py
--rw-rw-rw-   0        0        0     1439 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/comparator.py
--rw-rw-rw-   0        0        0     5340 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture.py
--rw-rw-rw-   0        0        0      449 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture0.py
--rw-rw-rw-   0        0        0      373 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture_green.py
--rw-rw-rw-   0        0        0      781 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cube.py
--rw-rw-rw-   0        0        0      688 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/default.py
--rw-rw-rw-   0        0        0     1179 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door.py
--rw-rw-rw-   0        0        0      340 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door1.py
--rw-rw-rw-   0        0        0      340 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door2.py
--rw-rw-rw-   0        0        0      340 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door3.py
--rw-rw-rw-   0        0        0      340 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door4.py
--rw-rw-rw-   0        0        0      340 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door5.py
--rw-rw-rw-   0        0        0      340 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door6.py
--rw-rw-rw-   0        0        0     1225 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/double_plant.py
--rw-rw-rw-   0        0        0      666 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/enchanting_table.py
--rw-rw-rw-   0        0        0      644 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/farmland.py
--rw-rw-rw-   0        0        0      654 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/fence.py
--rw-rw-rw-   0        0        0     1616 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat.py
--rw-rw-rw-   0        0        0     1620 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat_wall.py
--rw-rw-rw-   0        0        0     1264 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/furnace.py
--rw-rw-rw-   0        0        0      364 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/furnace_lit.py
--rw-rw-rw-   0        0        0      822 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/green_cube.py
--rw-rw-rw-   0        0        0      912 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/ladder.py
--rw-rw-rw-   0        0        0      333 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/lilypad.py
--rw-rw-rw-   0        0        0     1976 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/partial_block.py
--rw-rw-rw-   0        0        0     1318 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston.py
--rw-rw-rw-   0        0        0     2160 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston_arm.py
--rw-rw-rw-   0        0        0      654 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/portal_frame.py
--rw-rw-rw-   0        0        0      984 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pressure_plate.py
--rw-rw-rw-   0        0        0     1008 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin.py
--rw-rw-rw-   0        0        0      374 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin_carved.py
--rw-rw-rw-   0        0        0      365 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin_lit.py
--rw-rw-rw-   0        0        0      334 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/red_dust.py
--rw-rw-rw-   0        0        0     1506 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/repeater.py
--rw-rw-rw-   0        0        0     1079 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/slab.py
--rw-rw-rw-   0        0        0      444 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/slab_double.py
--rw-rw-rw-   0        0        0     1209 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/tree.py
--rw-rw-rw-   0        0        0      448 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/turtle_egg.py
--rw-rw-rw-   0        0        0     1477 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/vine.py
--rw-rw-rw-   0        0        0      645 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/wall.py
--rw-rw-rw-   0        0        0      876 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/water.py
--rw-rw-rw-   0        0        0    23188 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes.json
--rw-rw-rw-   0        0        0     5220 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/download_resources.py
--rw-rw-rw-   0        0        0     1441 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/resource_pack.py
--rw-rw-rw-   0        0        0    13738 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/resource_pack_manager.py
--rw-rw-rw-   0        0        0      446 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/sort_blockshapes.py
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.206538 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/
--rw-rw-rw-   0        0        0      105 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/__init__.py
--rw-rw-rw-   0        0        0     6399 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/download_resources.py
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.206538 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.159659 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.159659 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.253410 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/
--rw-rw-rw-   0        0        0     1153 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/acacia_sign.json
--rw-rw-rw-   0        0        0      322 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/acacia_wall_sign.json
--rw-rw-rw-   0        0        0     1137 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/birch_sign.json
--rw-rw-rw-   0        0        0      318 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/birch_wall_sign.json
--rw-rw-rw-   0        0        0     1169 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_banner.json
--rw-rw-rw-   0        0        0      685 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_bed.json
--rw-rw-rw-   0        0        0      326 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_wall_banner.json
--rw-rw-rw-   0        0        0     1153 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_banner.json
--rw-rw-rw-   0        0        0      677 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_bed.json
--rw-rw-rw-   0        0        0      322 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_wall_banner.json
--rw-rw-rw-   0        0        0     1169 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_banner.json
--rw-rw-rw-   0        0        0      685 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_bed.json
--rw-rw-rw-   0        0        0      326 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_wall_banner.json
--rw-rw-rw-   0        0        0      888 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/chest.json
--rw-rw-rw-   0        0        0     1265 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/creeper_head.json
--rw-rw-rw-   0        0        0      326 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/creeper_wall_head.json
--rw-rw-rw-   0        0        0     1169 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/crimson_sign.json
--rw-rw-rw-   0        0        0      326 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/crimson_wall_sign.json
--rw-rw-rw-   0        0        0     1153 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_banner.json
--rw-rw-rw-   0        0        0      677 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_bed.json
--rw-rw-rw-   0        0        0      322 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_wall_banner.json
--rw-rw-rw-   0        0        0     1185 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dark_oak_sign.json
--rw-rw-rw-   0        0        0      330 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dark_oak_wall_sign.json
--rw-rw-rw-   0        0        0     1249 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dragon_head.json
--rw-rw-rw-   0        0        0      322 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dragon_wall_head.json
--rw-rw-rw-   0        0        0      282 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/ender_chest.json
--rw-rw-rw-   0        0        0       84 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/grass.json
--rw-rw-rw-   0        0        0     1153 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_banner.json
--rw-rw-rw-   0        0        0      677 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_bed.json
--rw-rw-rw-   0        0        0      322 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_wall_banner.json
--rw-rw-rw-   0        0        0     1169 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_banner.json
--rw-rw-rw-   0        0        0      685 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_bed.json
--rw-rw-rw-   0        0        0      326 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_wall_banner.json
--rw-rw-rw-   0        0        0     1153 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/jungle_sign.json
--rw-rw-rw-   0        0        0      322 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/jungle_wall_sign.json
--rw-rw-rw-   0        0        0      947 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light.json
--rw-rw-rw-   0        0        0     1249 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_banner.json
--rw-rw-rw-   0        0        0      725 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_bed.json
--rw-rw-rw-   0        0        0      346 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_wall_banner.json
--rw-rw-rw-   0        0        0     1249 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_banner.json
--rw-rw-rw-   0        0        0      725 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_bed.json
--rw-rw-rw-   0        0        0      346 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_wall_banner.json
--rw-rw-rw-   0        0        0     1153 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_banner.json
--rw-rw-rw-   0        0        0      677 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_bed.json
--rw-rw-rw-   0        0        0      322 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_wall_banner.json
--rw-rw-rw-   0        0        0     1201 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_banner.json
--rw-rw-rw-   0        0        0      701 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_bed.json
--rw-rw-rw-   0        0        0      334 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_wall_banner.json
--rw-rw-rw-   0        0        0     1185 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/mangrove_sign.json
--rw-rw-rw-   0        0        0      330 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/mangrove_wall_sign.json
--rw-rw-rw-   0        0        0     1105 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/oak_sign.json
--rw-rw-rw-   0        0        0      310 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/oak_wall_sign.json
--rw-rw-rw-   0        0        0     1185 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_banner.json
--rw-rw-rw-   0        0        0      693 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_bed.json
--rw-rw-rw-   0        0        0      330 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_wall_banner.json
--rw-rw-rw-   0        0        0     1153 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_banner.json
--rw-rw-rw-   0        0        0      677 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_bed.json
--rw-rw-rw-   0        0        0      322 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_wall_banner.json
--rw-rw-rw-   0        0        0     1249 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/player_head.json
--rw-rw-rw-   0        0        0      322 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/player_wall_head.json
--rw-rw-rw-   0        0        0     1185 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_banner.json
--rw-rw-rw-   0        0        0      693 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_bed.json
--rw-rw-rw-   0        0        0      330 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_wall_banner.json
--rw-rw-rw-   0        0        0     1137 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_banner.json
--rw-rw-rw-   0        0        0      669 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_bed.json
--rw-rw-rw-   0        0        0      318 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_wall_banner.json
--rw-rw-rw-   0        0        0     1281 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/skeleton_skull.json
--rw-rw-rw-   0        0        0      330 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/skeleton_wall_skull.json
--rw-rw-rw-   0        0        0     1153 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/spruce_sign.json
--rw-rw-rw-   0        0        0      322 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/spruce_wall_sign.json
--rw-rw-rw-   0        0        0       84 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/structure_void.json
--rw-rw-rw-   0        0        0      984 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/trapped_chest.json
--rw-rw-rw-   0        0        0     1153 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/warped_sign.json
--rw-rw-rw-   0        0        0      322 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/warped_wall_sign.json
--rw-rw-rw-   0        0        0     1169 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_banner.json
--rw-rw-rw-   0        0        0      685 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_bed.json
--rw-rw-rw-   0        0        0      326 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_wall_banner.json
--rw-rw-rw-   0        0        0     1393 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/wither_skeleton_skull.json
--rw-rw-rw-   0        0        0      358 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/wither_skeleton_wall_skull.json
--rw-rw-rw-   0        0        0     1185 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_banner.json
--rw-rw-rw-   0        0        0      693 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_bed.json
--rw-rw-rw-   0        0        0      330 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_wall_banner.json
--rw-rw-rw-   0        0        0     1249 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/zombie_head.json
--rw-rw-rw-   0        0        0      322 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/zombie_wall_head.json
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.159659 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.269664 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.300335 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/
--rw-rw-rw-   0        0        0     1862 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_0.json
--rw-rw-rw-   0        0        0     1874 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_1.json
--rw-rw-rw-   0        0        0     1865 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_2.json
--rw-rw-rw-   0        0        0     1871 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_3.json
--rw-rw-rw-   0        0        0      102 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_0.json
--rw-rw-rw-   0        0        0      102 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_1.json
--rw-rw-rw-   0        0        0      102 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_2.json
--rw-rw-rw-   0        0        0      102 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_3.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_0.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_1.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_2.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_3.json
--rw-rw-rw-   0        0        0      102 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_0.json
--rw-rw-rw-   0        0        0      102 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_1.json
--rw-rw-rw-   0        0        0      102 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_2.json
--rw-rw-rw-   0        0        0      102 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_3.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_0.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_1.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_2.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_3.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_0.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_1.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_2.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_3.json
--rw-rw-rw-   0        0        0      102 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_0.json
--rw-rw-rw-   0        0        0      102 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_1.json
--rw-rw-rw-   0        0        0      102 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_2.json
--rw-rw-rw-   0        0        0      102 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_3.json
--rw-rw-rw-   0        0        0      107 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_0.json
--rw-rw-rw-   0        0        0      107 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_1.json
--rw-rw-rw-   0        0        0      107 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_2.json
--rw-rw-rw-   0        0        0      107 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_3.json
--rw-rw-rw-   0        0        0      107 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_0.json
--rw-rw-rw-   0        0        0      107 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_1.json
--rw-rw-rw-   0        0        0      107 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_2.json
--rw-rw-rw-   0        0        0      107 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_3.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_0.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_1.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_2.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_3.json
--rw-rw-rw-   0        0        0      104 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_0.json
--rw-rw-rw-   0        0        0      104 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_1.json
--rw-rw-rw-   0        0        0      104 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_2.json
--rw-rw-rw-   0        0        0      104 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_3.json
--rw-rw-rw-   0        0        0      103 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_0.json
--rw-rw-rw-   0        0        0      103 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_1.json
--rw-rw-rw-   0        0        0      103 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_2.json
--rw-rw-rw-   0        0        0      103 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_3.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_0.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_1.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_2.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_3.json
--rw-rw-rw-   0        0        0      103 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_0.json
--rw-rw-rw-   0        0        0      103 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_1.json
--rw-rw-rw-   0        0        0      103 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_2.json
--rw-rw-rw-   0        0        0      103 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_3.json
--rw-rw-rw-   0        0        0      100 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_0.json
--rw-rw-rw-   0        0        0      100 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_1.json
--rw-rw-rw-   0        0        0      100 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_2.json
--rw-rw-rw-   0        0        0      100 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_3.json
--rw-rw-rw-   0        0        0      102 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_0.json
--rw-rw-rw-   0        0        0      102 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_1.json
--rw-rw-rw-   0        0        0      102 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_2.json
--rw-rw-rw-   0        0        0      102 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_3.json
--rw-rw-rw-   0        0        0      103 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_0.json
--rw-rw-rw-   0        0        0      103 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_1.json
--rw-rw-rw-   0        0        0      103 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_2.json
--rw-rw-rw-   0        0        0      103 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_3.json
--rw-rw-rw-   0        0        0      133 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/barrier.json
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.315963 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/
--rw-rw-rw-   0        0        0       83 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/black_foot.json
--rw-rw-rw-   0        0        0       83 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/black_head.json
--rw-rw-rw-   0        0        0       82 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/blue_foot.json
--rw-rw-rw-   0        0        0       82 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/blue_head.json
--rw-rw-rw-   0        0        0       83 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/brown_foot.json
--rw-rw-rw-   0        0        0       83 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/brown_head.json
--rw-rw-rw-   0        0        0       82 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/cyan_foot.json
--rw-rw-rw-   0        0        0       82 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/cyan_head.json
--rw-rw-rw-   0        0        0       82 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/gray_foot.json
--rw-rw-rw-   0        0        0       82 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/gray_head.json
--rw-rw-rw-   0        0        0       83 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/green_foot.json
--rw-rw-rw-   0        0        0       83 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/green_head.json
--rw-rw-rw-   0        0        0       88 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_blue_foot.json
--rw-rw-rw-   0        0        0       88 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_blue_head.json
--rw-rw-rw-   0        0        0       88 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_gray_foot.json
--rw-rw-rw-   0        0        0       88 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_gray_head.json
--rw-rw-rw-   0        0        0       82 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/lime_foot.json
--rw-rw-rw-   0        0        0       82 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/lime_head.json
--rw-rw-rw-   0        0        0       85 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/magenta_foot.json
--rw-rw-rw-   0        0        0       85 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/magenta_head.json
--rw-rw-rw-   0        0        0       84 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/orange_foot.json
--rw-rw-rw-   0        0        0       84 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/orange_head.json
--rw-rw-rw-   0        0        0       82 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/pink_foot.json
--rw-rw-rw-   0        0        0       82 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/pink_head.json
--rw-rw-rw-   0        0        0       84 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/purple_foot.json
--rw-rw-rw-   0        0        0       84 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/purple_head.json
--rw-rw-rw-   0        0        0       81 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/red_foot.json
--rw-rw-rw-   0        0        0       81 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/red_head.json
--rw-rw-rw-   0        0        0       83 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/white_foot.json
--rw-rw-rw-   0        0        0       83 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/white_head.json
--rw-rw-rw-   0        0        0       84 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/yellow_foot.json
--rw-rw-rw-   0        0        0       84 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/yellow_head.json
--rw-rw-rw-   0        0        0     1525 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_foot.json
--rw-rw-rw-   0        0        0     1535 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_head.json
--rw-rw-rw-   0        0        0     1610 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_between_walls.json
--rw-rw-rw-   0        0        0     1507 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_ceiling.json
--rw-rw-rw-   0        0        0     2669 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_floor.json
--rw-rw-rw-   0        0        0     1592 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_wall.json
--rw-rw-rw-   0        0        0      153 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/black_shulker_box.json
--rw-rw-rw-   0        0        0      151 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/blue_shulker_box.json
--rw-rw-rw-   0        0        0      153 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/brown_shulker_box.json
--rw-rw-rw-   0        0        0      105 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest.json
--rw-rw-rw-   0        0        0     1855 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_base.json
--rw-rw-rw-   0        0        0      115 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_left.json
--rw-rw-rw-   0        0        0     1537 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_left_base.json
--rw-rw-rw-   0        0        0      117 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_right.json
--rw-rw-rw-   0        0        0     1527 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_right_base.json
--rw-rw-rw-   0        0        0      579 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/conduit.json
--rw-rw-rw-   0        0        0      151 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/cyan_shulker_box.json
--rw-rw-rw-   0        0        0      139 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/end_portal.json
--rw-rw-rw-   0        0        0      104 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/ender_chest.json
--rw-rw-rw-   0        0        0      109 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/grass.json
--rw-rw-rw-   0        0        0      151 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/gray_shulker_box.json
--rw-rw-rw-   0        0        0      153 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/green_shulker_box.json
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.159659 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.331586 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/
--rw-rw-rw-   0        0        0       99 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_0.json
--rw-rw-rw-   0        0        0       99 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_1.json
--rw-rw-rw-   0        0        0       99 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_2.json
--rw-rw-rw-   0        0        0       99 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_3.json
--rw-rw-rw-   0        0        0     4816 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_0.json
--rw-rw-rw-   0        0        0     4831 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_1.json
--rw-rw-rw-   0        0        0     4810 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_2.json
--rw-rw-rw-   0        0        0     4824 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_3.json
--rw-rw-rw-   0        0        0      592 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_0.json
--rw-rw-rw-   0        0        0      660 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_1.json
--rw-rw-rw-   0        0        0      657 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_2.json
--rw-rw-rw-   0        0        0      659 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_3.json
--rw-rw-rw-   0        0        0      656 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_0.json
--rw-rw-rw-   0        0        0      660 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_1.json
--rw-rw-rw-   0        0        0      657 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_2.json
--rw-rw-rw-   0        0        0      659 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_3.json
--rw-rw-rw-   0        0        0       90 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_0.json
--rw-rw-rw-   0        0        0       90 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_1.json
--rw-rw-rw-   0        0        0       90 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_2.json
--rw-rw-rw-   0        0        0       90 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_3.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_0.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_1.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_2.json
--rw-rw-rw-   0        0        0      101 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_3.json
--rw-rw-rw-   0        0        0      108 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_0.json
--rw-rw-rw-   0        0        0      108 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_1.json
--rw-rw-rw-   0        0        0      108 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_2.json
--rw-rw-rw-   0        0        0      108 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_3.json
--rw-rw-rw-   0        0        0       98 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_0.json
--rw-rw-rw-   0        0        0       98 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_1.json
--rw-rw-rw-   0        0        0       98 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_2.json
--rw-rw-rw-   0        0        0       98 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_3.json
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.347210 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/
--rw-rw-rw-   0        0        0       96 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/creeper.json
--rw-rw-rw-   0        0        0     3870 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/dragon.json
--rw-rw-rw-   0        0        0      559 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head.json
--rw-rw-rw-   0        0        0      559 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head2.json
--rw-rw-rw-   0        0        0       87 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/player.json
--rw-rw-rw-   0        0        0       98 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/skeleton.json
--rw-rw-rw-   0        0        0      105 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/wither_skeleton.json
--rw-rw-rw-   0        0        0       95 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/zombie.json
--rw-rw-rw-   0        0        0      134 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/lava.json
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.347210 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/
--rw-rw-rw-   0        0        0      133 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_0.json
--rw-rw-rw-   0        0        0      133 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_1.json
--rw-rw-rw-   0        0        0      133 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_10.json
--rw-rw-rw-   0        0        0      133 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_11.json
--rw-rw-rw-   0        0        0      133 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_12.json
--rw-rw-rw-   0        0        0      133 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_13.json
--rw-rw-rw-   0        0        0      133 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_14.json
--rw-rw-rw-   0        0        0      133 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_15.json
--rw-rw-rw-   0        0        0      133 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_2.json
--rw-rw-rw-   0        0        0      133 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_3.json
--rw-rw-rw-   0        0        0      133 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_4.json
--rw-rw-rw-   0        0        0      133 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_5.json
--rw-rw-rw-   0        0        0      133 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_6.json
--rw-rw-rw-   0        0        0      133 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_7.json
--rw-rw-rw-   0        0        0      133 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_8.json
--rw-rw-rw-   0        0        0      133 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_9.json
--rw-rw-rw-   0        0        0      163 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light_blue_shulker_box.json
--rw-rw-rw-   0        0        0      163 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light_gray_shulker_box.json
--rw-rw-rw-   0        0        0      151 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/lime_shulker_box.json
--rw-rw-rw-   0        0        0      157 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/magenta_shulker_box.json
--rw-rw-rw-   0        0        0      151 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/moving_piston.json
--rw-rw-rw-   0        0        0      155 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/orange_shulker_box.json
--rw-rw-rw-   0        0        0      151 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/pink_shulker_box.json
--rw-rw-rw-   0        0        0      155 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/purple_shulker_box.json
--rw-rw-rw-   0        0        0      149 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/red_shulker_box.json
--rw-rw-rw-   0        0        0      141 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/shulker_box.json
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.378461 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/
--rw-rw-rw-   0        0        0      127 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_0.json
--rw-rw-rw-   0        0        0      127 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_1.json
--rw-rw-rw-   0        0        0      127 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_2.json
--rw-rw-rw-   0        0        0      127 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_3.json
--rw-rw-rw-   0        0        0      125 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_0.json
--rw-rw-rw-   0        0        0      125 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_1.json
--rw-rw-rw-   0        0        0      125 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_2.json
--rw-rw-rw-   0        0        0      125 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_3.json
--rw-rw-rw-   0        0        0      129 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_0.json
--rw-rw-rw-   0        0        0      129 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_1.json
--rw-rw-rw-   0        0        0      129 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_2.json
--rw-rw-rw-   0        0        0      129 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_3.json
--rw-rw-rw-   0        0        0      131 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_0.json
--rw-rw-rw-   0        0        0      131 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_1.json
--rw-rw-rw-   0        0        0      131 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_2.json
--rw-rw-rw-   0        0        0      131 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_3.json
--rw-rw-rw-   0        0        0      127 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_0.json
--rw-rw-rw-   0        0        0      127 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_1.json
--rw-rw-rw-   0        0        0      127 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_2.json
--rw-rw-rw-   0        0        0      127 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_3.json
--rw-rw-rw-   0        0        0      131 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_0.json
--rw-rw-rw-   0        0        0      131 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_1.json
--rw-rw-rw-   0        0        0      131 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_2.json
--rw-rw-rw-   0        0        0      131 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_3.json
--rw-rw-rw-   0        0        0      121 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_0.json
--rw-rw-rw-   0        0        0      121 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_1.json
--rw-rw-rw-   0        0        0      121 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_2.json
--rw-rw-rw-   0        0        0      121 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_3.json
--rw-rw-rw-   0        0        0     1184 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_0.json
--rw-rw-rw-   0        0        0     1173 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_1.json
--rw-rw-rw-   0        0        0     1167 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_2.json
--rw-rw-rw-   0        0        0     1171 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_3.json
--rw-rw-rw-   0        0        0      127 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_0.json
--rw-rw-rw-   0        0        0      127 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_1.json
--rw-rw-rw-   0        0        0      127 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_2.json
--rw-rw-rw-   0        0        0      127 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_3.json
--rw-rw-rw-   0        0        0      127 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_0.json
--rw-rw-rw-   0        0        0      127 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_1.json
--rw-rw-rw-   0        0        0      127 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_2.json
--rw-rw-rw-   0        0        0      127 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_3.json
--rw-rw-rw-   0        0        0      147 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/structure_void.json
--rw-rw-rw-   0        0        0      106 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/trapped_chest.json
--rw-rw-rw-   0        0        0      116 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/trapped_chest_left.json
--rw-rw-rw-   0        0        0      118 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/trapped_chest_right.json
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.378461 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/
--rw-rw-rw-   0        0        0       98 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/black.json
--rw-rw-rw-   0        0        0       97 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/blue.json
--rw-rw-rw-   0        0        0       98 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/brown.json
--rw-rw-rw-   0        0        0       97 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/cyan.json
--rw-rw-rw-   0        0        0       97 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/gray.json
--rw-rw-rw-   0        0        0       98 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/green.json
--rw-rw-rw-   0        0        0      103 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/light_blue.json
--rw-rw-rw-   0        0        0      103 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/light_gray.json
--rw-rw-rw-   0        0        0       97 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/lime.json
--rw-rw-rw-   0        0        0      100 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/magenta.json
--rw-rw-rw-   0        0        0       99 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/orange.json
--rw-rw-rw-   0        0        0       97 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/pink.json
--rw-rw-rw-   0        0        0       99 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/purple.json
--rw-rw-rw-   0        0        0       96 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/red.json
--rw-rw-rw-   0        0        0       98 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/white.json
--rw-rw-rw-   0        0        0       99 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/yellow.json
--rw-rw-rw-   0        0        0     1208 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner.json
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.378461 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/
--rw-rw-rw-   0        0        0      135 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/acacia.json
--rw-rw-rw-   0        0        0      133 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/birch.json
--rw-rw-rw-   0        0        0      137 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/crimson.json
--rw-rw-rw-   0        0        0      139 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/dark_oak.json
--rw-rw-rw-   0        0        0      135 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/jungle.json
--rw-rw-rw-   0        0        0      139 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/mangrove.json
--rw-rw-rw-   0        0        0      129 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/oak.json
--rw-rw-rw-   0        0        0      135 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/spruce.json
--rw-rw-rw-   0        0        0      588 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/wall_sign.json
--rw-rw-rw-   0        0        0      135 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/warped.json
--rw-rw-rw-   0        0        0      135 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/water.json
--rw-rw-rw-   0        0        0      153 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/white_shulker_box.json
--rw-rw-rw-   0        0        0      155 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/yellow_shulker_box.json
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.159659 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.394087 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.394087 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/
--rw-rw-rw-   0        0        0     2769 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_black.png
--rw-rw-rw-   0        0        0     3786 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_blue.png
--rw-rw-rw-   0        0        0     3707 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_brown.png
--rw-rw-rw-   0        0        0     3813 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_cyan.png
--rw-rw-rw-   0        0        0     3518 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_gray.png
--rw-rw-rw-   0        0        0     3751 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_green.png
--rw-rw-rw-   0        0        0     4220 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_blue.png
--rw-rw-rw-   0        0        0     3953 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_gray.png
--rw-rw-rw-   0        0        0     4151 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_lime.png
--rw-rw-rw-   0        0        0     4178 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_magenta.png
--rw-rw-rw-   0        0        0     4298 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_orange.png
--rw-rw-rw-   0        0        0     4205 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_pink.png
--rw-rw-rw-   0        0        0     4056 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_purple.png
--rw-rw-rw-   0        0        0     3790 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_red.png
--rw-rw-rw-   0        0        0     3985 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_white.png
--rw-rw-rw-   0        0        0     4457 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_yellow.png
--rw-rw-rw-   0        0        0      651 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/barrier.png
--rw-rw-rw-   0        0        0     1265 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/end_portal.png
--rw-rw-rw-   0        0        0      213 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/grass.png
--rw-rw-rw-   0        0        0     1286 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/lava.png
--rw-rw-rw-   0        0        0     1405 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/structure_void.png
--rw-rw-rw-   0        0        0      927 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/water.png
--rw-rw-rw-   0        0        0      117 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/pack.mcmeta
--rw-rw-rw-   0        0        0    22749 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/pack.png
--rw-rw-rw-   0        0        0     1687 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/resource_pack.py
--rw-rw-rw-   0        0        0    22308 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/resource_pack_manager.py
--rw-rw-rw-   0        0        0      299 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/unknown_resource_pack.py
-drwxrwxrwx   0        0        0        0 2023-12-08 14:55:23.394087 minecraft-resource-pack-1.4.1/minecraft_resource_pack.egg-info/
--rw-rw-rw-   0        0        0      876 2023-12-08 14:55:22.000000 minecraft-resource-pack-1.4.1/minecraft_resource_pack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    48477 2023-12-08 14:55:23.000000 minecraft-resource-pack-1.4.1/minecraft_resource_pack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-08 14:55:22.000000 minecraft-resource-pack-1.4.1/minecraft_resource_pack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-12-08 14:55:22.000000 minecraft-resource-pack-1.4.1/minecraft_resource_pack.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-12-08 14:55:22.000000 minecraft-resource-pack-1.4.1/minecraft_resource_pack.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      177 2023-12-08 14:55:22.000000 minecraft-resource-pack-1.4.1/minecraft_resource_pack.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-12-08 14:55:22.000000 minecraft-resource-pack-1.4.1/minecraft_resource_pack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      135 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/pyproject.toml
--rw-rw-rw-   0        0        0     1190 2023-12-08 14:55:23.409711 minecraft-resource-pack-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0      142 2023-12-08 14:54:37.000000 minecraft-resource-pack-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.377310 minecraft_resource_pack-1.4.2/
+-rw-rw-rw-   0        0        0     6954 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/LICENSE
+-rw-rw-rw-   0        0        0      206 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      876 2024-05-01 11:21:50.377310 minecraft_resource_pack-1.4.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.111689 minecraft_resource_pack-1.4.2/minecraft_model_reader/
+-rw-rw-rw-   0        0        0      910 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.111689 minecraft_resource_pack-1.4.2/minecraft_model_reader/__pyinstaller/
+-rw-rw-rw-   0        0        0       43 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/__pyinstaller/__init__.py
+-rw-rw-rw-   0        0        0      194 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/__pyinstaller/hook-minecraft_model_reader.py
+-rw-rw-rw-   0        0        0      518 2024-05-01 11:21:50.377310 minecraft_resource_pack-1.4.2/minecraft_model_reader/_version.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.111689 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/
+-rw-rw-rw-   0        0        0      186 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.111689 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/amulet/
+-rw-rw-rw-   0        0        0        0 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/amulet/__init__.py
+-rw-rw-rw-   0        0        0    18894 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/amulet/block.py
+-rw-rw-rw-   0        0        0     6410 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/comment_json.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.127312 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/image/
+-rw-rw-rw-   0        0        0      189 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/image/__init__.py
+-rw-rw-rw-   0        0        0      176 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/image/missing_no.png
+-rw-rw-rw-   0        0        0    11085 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/image/missing_pack_java.png
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.127312 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/mesh/
+-rw-rw-rw-   0        0        0        0 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/mesh/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.127312 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/mesh/block/
+-rw-rw-rw-   0        0        0       35 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/mesh/block/__init__.py
+-rw-rw-rw-   0        0        0    13839 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/mesh/block/block_mesh.py
+-rw-rw-rw-   0        0        0     4764 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/mesh/block/cube.py
+-rw-rw-rw-   0        0        0      545 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/mesh/block/missing_block.py
+-rw-rw-rw-   0        0        0      507 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/mesh/util.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.127312 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/
+-rw-rw-rw-   0        0        0     1908 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.127312 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/base/
+-rw-rw-rw-   0        0        0      105 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/base/__init__.py
+-rw-rw-rw-   0        0        0     1128 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/base/resource_pack.py
+-rw-rw-rw-   0        0        0     2908 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/base/resource_pack_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.127312 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/
+-rw-rw-rw-   0        0        0      111 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.127312 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/
+-rw-rw-rw-   0        0        0      967 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/blocks.json
+-rw-rw-rw-   0        0        0      555 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/manifest.json
+-rw-rw-rw-   0        0        0    32642 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/pack_icon.png
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.127312 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.142941 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/
+-rw-rw-rw-   0        0        0      580 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/grass_carried.png
+-rw-rw-rw-   0        0        0      408 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/grass_side_carried.png
+-rw-rw-rw-   0        0        0      927 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/water.png
+-rw-rw-rw-   0        0        0      428 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/terrain_texture.json
+-rw-rw-rw-   0        0        0  2864161 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/block_palette.json
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.158566 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/
+-rw-rw-rw-   0        0        0     1065 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/__init__.py
+-rw-rw-rw-   0        0        0     1027 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/air.py
+-rw-rw-rw-   0        0        0      905 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/base_blockshape.py
+-rw-rw-rw-   0        0        0      736 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/bubble_column.py
+-rw-rw-rw-   0        0        0     1099 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cake.py
+-rw-rw-rw-   0        0        0     1443 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/chest.py
+-rw-rw-rw-   0        0        0     1439 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/comparator.py
+-rw-rw-rw-   0        0        0     5340 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture.py
+-rw-rw-rw-   0        0        0      449 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture0.py
+-rw-rw-rw-   0        0        0      373 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture_green.py
+-rw-rw-rw-   0        0        0      781 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cube.py
+-rw-rw-rw-   0        0        0      688 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/default.py
+-rw-rw-rw-   0        0        0     1179 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door.py
+-rw-rw-rw-   0        0        0      340 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door1.py
+-rw-rw-rw-   0        0        0      340 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door2.py
+-rw-rw-rw-   0        0        0      340 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door3.py
+-rw-rw-rw-   0        0        0      340 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door4.py
+-rw-rw-rw-   0        0        0      340 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door5.py
+-rw-rw-rw-   0        0        0      340 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door6.py
+-rw-rw-rw-   0        0        0     1225 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/double_plant.py
+-rw-rw-rw-   0        0        0      666 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/enchanting_table.py
+-rw-rw-rw-   0        0        0      644 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/farmland.py
+-rw-rw-rw-   0        0        0      654 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/fence.py
+-rw-rw-rw-   0        0        0     1616 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat.py
+-rw-rw-rw-   0        0        0     1620 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat_wall.py
+-rw-rw-rw-   0        0        0     1264 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/furnace.py
+-rw-rw-rw-   0        0        0      364 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/furnace_lit.py
+-rw-rw-rw-   0        0        0      822 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/green_cube.py
+-rw-rw-rw-   0        0        0      912 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/ladder.py
+-rw-rw-rw-   0        0        0      333 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/lilypad.py
+-rw-rw-rw-   0        0        0     1976 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/partial_block.py
+-rw-rw-rw-   0        0        0     1318 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston.py
+-rw-rw-rw-   0        0        0     2160 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston_arm.py
+-rw-rw-rw-   0        0        0      654 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/portal_frame.py
+-rw-rw-rw-   0        0        0      984 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pressure_plate.py
+-rw-rw-rw-   0        0        0     1008 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin.py
+-rw-rw-rw-   0        0        0      374 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin_carved.py
+-rw-rw-rw-   0        0        0      365 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin_lit.py
+-rw-rw-rw-   0        0        0      334 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/red_dust.py
+-rw-rw-rw-   0        0        0     1506 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/repeater.py
+-rw-rw-rw-   0        0        0     1079 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/slab.py
+-rw-rw-rw-   0        0        0      444 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/slab_double.py
+-rw-rw-rw-   0        0        0     1209 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/tree.py
+-rw-rw-rw-   0        0        0      448 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/turtle_egg.py
+-rw-rw-rw-   0        0        0     1477 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/vine.py
+-rw-rw-rw-   0        0        0      645 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/wall.py
+-rw-rw-rw-   0        0        0      876 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/water.py
+-rw-rw-rw-   0        0        0    23188 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes.json
+-rw-rw-rw-   0        0        0     5220 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/download_resources.py
+-rw-rw-rw-   0        0        0     1441 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/resource_pack.py
+-rw-rw-rw-   0        0        0    13724 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/resource_pack_manager.py
+-rw-rw-rw-   0        0        0      446 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/sort_blockshapes.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.158566 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/
+-rw-rw-rw-   0        0        0      105 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/__init__.py
+-rw-rw-rw-   0        0        0     7022 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/download_resources.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.158566 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.111689 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.111689 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.205439 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/
+-rw-rw-rw-   0        0        0     1153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/acacia_sign.json
+-rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/acacia_wall_sign.json
+-rw-rw-rw-   0        0        0     1137 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/birch_sign.json
+-rw-rw-rw-   0        0        0      318 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/birch_wall_sign.json
+-rw-rw-rw-   0        0        0     1169 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_banner.json
+-rw-rw-rw-   0        0        0      685 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_bed.json
+-rw-rw-rw-   0        0        0      326 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_wall_banner.json
+-rw-rw-rw-   0        0        0     1153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_banner.json
+-rw-rw-rw-   0        0        0      677 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_bed.json
+-rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_wall_banner.json
+-rw-rw-rw-   0        0        0     1169 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_banner.json
+-rw-rw-rw-   0        0        0      685 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_bed.json
+-rw-rw-rw-   0        0        0      326 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_wall_banner.json
+-rw-rw-rw-   0        0        0      888 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/chest.json
+-rw-rw-rw-   0        0        0     1265 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/creeper_head.json
+-rw-rw-rw-   0        0        0      326 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/creeper_wall_head.json
+-rw-rw-rw-   0        0        0     1169 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/crimson_sign.json
+-rw-rw-rw-   0        0        0      326 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/crimson_wall_sign.json
+-rw-rw-rw-   0        0        0     1153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_banner.json
+-rw-rw-rw-   0        0        0      677 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_bed.json
+-rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_wall_banner.json
+-rw-rw-rw-   0        0        0     1185 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dark_oak_sign.json
+-rw-rw-rw-   0        0        0      330 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dark_oak_wall_sign.json
+-rw-rw-rw-   0        0        0     1249 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dragon_head.json
+-rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dragon_wall_head.json
+-rw-rw-rw-   0        0        0      282 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/ender_chest.json
+-rw-rw-rw-   0        0        0       84 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/grass.json
+-rw-rw-rw-   0        0        0     1153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_banner.json
+-rw-rw-rw-   0        0        0      677 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_bed.json
+-rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_wall_banner.json
+-rw-rw-rw-   0        0        0     1169 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_banner.json
+-rw-rw-rw-   0        0        0      685 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_bed.json
+-rw-rw-rw-   0        0        0      326 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_wall_banner.json
+-rw-rw-rw-   0        0        0     1153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/jungle_sign.json
+-rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/jungle_wall_sign.json
+-rw-rw-rw-   0        0        0      947 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light.json
+-rw-rw-rw-   0        0        0     1249 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_banner.json
+-rw-rw-rw-   0        0        0      725 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_bed.json
+-rw-rw-rw-   0        0        0      346 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_wall_banner.json
+-rw-rw-rw-   0        0        0     1249 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_banner.json
+-rw-rw-rw-   0        0        0      725 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_bed.json
+-rw-rw-rw-   0        0        0      346 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_wall_banner.json
+-rw-rw-rw-   0        0        0     1153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_banner.json
+-rw-rw-rw-   0        0        0      677 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_bed.json
+-rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_wall_banner.json
+-rw-rw-rw-   0        0        0     1201 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_banner.json
+-rw-rw-rw-   0        0        0      701 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_bed.json
+-rw-rw-rw-   0        0        0      334 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_wall_banner.json
+-rw-rw-rw-   0        0        0     1185 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/mangrove_sign.json
+-rw-rw-rw-   0        0        0      330 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/mangrove_wall_sign.json
+-rw-rw-rw-   0        0        0     1105 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/oak_sign.json
+-rw-rw-rw-   0        0        0      310 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/oak_wall_sign.json
+-rw-rw-rw-   0        0        0     1185 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_banner.json
+-rw-rw-rw-   0        0        0      693 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_bed.json
+-rw-rw-rw-   0        0        0      330 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_wall_banner.json
+-rw-rw-rw-   0        0        0     1153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_banner.json
+-rw-rw-rw-   0        0        0      677 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_bed.json
+-rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_wall_banner.json
+-rw-rw-rw-   0        0        0     1249 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/player_head.json
+-rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/player_wall_head.json
+-rw-rw-rw-   0        0        0     1185 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_banner.json
+-rw-rw-rw-   0        0        0      693 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_bed.json
+-rw-rw-rw-   0        0        0      330 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_wall_banner.json
+-rw-rw-rw-   0        0        0     1137 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_banner.json
+-rw-rw-rw-   0        0        0      669 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_bed.json
+-rw-rw-rw-   0        0        0      318 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_wall_banner.json
+-rw-rw-rw-   0        0        0     1281 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/skeleton_skull.json
+-rw-rw-rw-   0        0        0      330 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/skeleton_wall_skull.json
+-rw-rw-rw-   0        0        0     1153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/spruce_sign.json
+-rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/spruce_wall_sign.json
+-rw-rw-rw-   0        0        0       84 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/structure_void.json
+-rw-rw-rw-   0        0        0      984 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/trapped_chest.json
+-rw-rw-rw-   0        0        0     1153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/warped_sign.json
+-rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/warped_wall_sign.json
+-rw-rw-rw-   0        0        0     1169 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_banner.json
+-rw-rw-rw-   0        0        0      685 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_bed.json
+-rw-rw-rw-   0        0        0      326 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_wall_banner.json
+-rw-rw-rw-   0        0        0     1393 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/wither_skeleton_skull.json
+-rw-rw-rw-   0        0        0      358 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/wither_skeleton_wall_skull.json
+-rw-rw-rw-   0        0        0     1185 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_banner.json
+-rw-rw-rw-   0        0        0      693 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_bed.json
+-rw-rw-rw-   0        0        0      330 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_wall_banner.json
+-rw-rw-rw-   0        0        0     1249 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/zombie_head.json
+-rw-rw-rw-   0        0        0      322 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/zombie_wall_head.json
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.111689 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.236684 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.267935 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/
+-rw-rw-rw-   0        0        0     1862 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_0.json
+-rw-rw-rw-   0        0        0     1874 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_1.json
+-rw-rw-rw-   0        0        0     1865 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_2.json
+-rw-rw-rw-   0        0        0     1871 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_3.json
+-rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_0.json
+-rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_1.json
+-rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_2.json
+-rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_3.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_0.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_1.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_2.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_3.json
+-rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_0.json
+-rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_1.json
+-rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_2.json
+-rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_3.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_0.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_1.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_2.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_3.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_0.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_1.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_2.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_3.json
+-rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_0.json
+-rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_1.json
+-rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_2.json
+-rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_3.json
+-rw-rw-rw-   0        0        0      107 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_0.json
+-rw-rw-rw-   0        0        0      107 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_1.json
+-rw-rw-rw-   0        0        0      107 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_2.json
+-rw-rw-rw-   0        0        0      107 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_3.json
+-rw-rw-rw-   0        0        0      107 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_0.json
+-rw-rw-rw-   0        0        0      107 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_1.json
+-rw-rw-rw-   0        0        0      107 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_2.json
+-rw-rw-rw-   0        0        0      107 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_3.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_0.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_1.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_2.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_3.json
+-rw-rw-rw-   0        0        0      104 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_0.json
+-rw-rw-rw-   0        0        0      104 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_1.json
+-rw-rw-rw-   0        0        0      104 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_2.json
+-rw-rw-rw-   0        0        0      104 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_3.json
+-rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_0.json
+-rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_1.json
+-rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_2.json
+-rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_3.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_0.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_1.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_2.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_3.json
+-rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_0.json
+-rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_1.json
+-rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_2.json
+-rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_3.json
+-rw-rw-rw-   0        0        0      100 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_0.json
+-rw-rw-rw-   0        0        0      100 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_1.json
+-rw-rw-rw-   0        0        0      100 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_2.json
+-rw-rw-rw-   0        0        0      100 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_3.json
+-rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_0.json
+-rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_1.json
+-rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_2.json
+-rw-rw-rw-   0        0        0      102 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_3.json
+-rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_0.json
+-rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_1.json
+-rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_2.json
+-rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_3.json
+-rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/barrier.json
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.283563 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/
+-rw-rw-rw-   0        0        0       83 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/black_foot.json
+-rw-rw-rw-   0        0        0       83 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/black_head.json
+-rw-rw-rw-   0        0        0       82 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/blue_foot.json
+-rw-rw-rw-   0        0        0       82 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/blue_head.json
+-rw-rw-rw-   0        0        0       83 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/brown_foot.json
+-rw-rw-rw-   0        0        0       83 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/brown_head.json
+-rw-rw-rw-   0        0        0       82 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/cyan_foot.json
+-rw-rw-rw-   0        0        0       82 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/cyan_head.json
+-rw-rw-rw-   0        0        0       82 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/gray_foot.json
+-rw-rw-rw-   0        0        0       82 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/gray_head.json
+-rw-rw-rw-   0        0        0       83 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/green_foot.json
+-rw-rw-rw-   0        0        0       83 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/green_head.json
+-rw-rw-rw-   0        0        0       88 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_blue_foot.json
+-rw-rw-rw-   0        0        0       88 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_blue_head.json
+-rw-rw-rw-   0        0        0       88 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_gray_foot.json
+-rw-rw-rw-   0        0        0       88 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_gray_head.json
+-rw-rw-rw-   0        0        0       82 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/lime_foot.json
+-rw-rw-rw-   0        0        0       82 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/lime_head.json
+-rw-rw-rw-   0        0        0       85 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/magenta_foot.json
+-rw-rw-rw-   0        0        0       85 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/magenta_head.json
+-rw-rw-rw-   0        0        0       84 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/orange_foot.json
+-rw-rw-rw-   0        0        0       84 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/orange_head.json
+-rw-rw-rw-   0        0        0       82 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/pink_foot.json
+-rw-rw-rw-   0        0        0       82 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/pink_head.json
+-rw-rw-rw-   0        0        0       84 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/purple_foot.json
+-rw-rw-rw-   0        0        0       84 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/purple_head.json
+-rw-rw-rw-   0        0        0       81 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/red_foot.json
+-rw-rw-rw-   0        0        0       81 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/red_head.json
+-rw-rw-rw-   0        0        0       83 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/white_foot.json
+-rw-rw-rw-   0        0        0       83 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/white_head.json
+-rw-rw-rw-   0        0        0       84 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/yellow_foot.json
+-rw-rw-rw-   0        0        0       84 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/yellow_head.json
+-rw-rw-rw-   0        0        0     1525 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_foot.json
+-rw-rw-rw-   0        0        0     1535 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_head.json
+-rw-rw-rw-   0        0        0     1610 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_between_walls.json
+-rw-rw-rw-   0        0        0     1507 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_ceiling.json
+-rw-rw-rw-   0        0        0     2669 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_floor.json
+-rw-rw-rw-   0        0        0     1592 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_wall.json
+-rw-rw-rw-   0        0        0      153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/black_shulker_box.json
+-rw-rw-rw-   0        0        0      151 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/blue_shulker_box.json
+-rw-rw-rw-   0        0        0      153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/brown_shulker_box.json
+-rw-rw-rw-   0        0        0      105 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest.json
+-rw-rw-rw-   0        0        0     1855 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_base.json
+-rw-rw-rw-   0        0        0      115 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_left.json
+-rw-rw-rw-   0        0        0     1537 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_left_base.json
+-rw-rw-rw-   0        0        0      117 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_right.json
+-rw-rw-rw-   0        0        0     1527 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_right_base.json
+-rw-rw-rw-   0        0        0      579 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/conduit.json
+-rw-rw-rw-   0        0        0      151 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/cyan_shulker_box.json
+-rw-rw-rw-   0        0        0      139 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/end_portal.json
+-rw-rw-rw-   0        0        0      104 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/ender_chest.json
+-rw-rw-rw-   0        0        0      109 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/grass.json
+-rw-rw-rw-   0        0        0      151 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/gray_shulker_box.json
+-rw-rw-rw-   0        0        0      153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/green_shulker_box.json
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.111689 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.299188 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/
+-rw-rw-rw-   0        0        0       99 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_0.json
+-rw-rw-rw-   0        0        0       99 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_1.json
+-rw-rw-rw-   0        0        0       99 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_2.json
+-rw-rw-rw-   0        0        0       99 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_3.json
+-rw-rw-rw-   0        0        0     4816 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_0.json
+-rw-rw-rw-   0        0        0     4831 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_1.json
+-rw-rw-rw-   0        0        0     4810 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_2.json
+-rw-rw-rw-   0        0        0     4824 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_3.json
+-rw-rw-rw-   0        0        0      592 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_0.json
+-rw-rw-rw-   0        0        0      660 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_1.json
+-rw-rw-rw-   0        0        0      657 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_2.json
+-rw-rw-rw-   0        0        0      659 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_3.json
+-rw-rw-rw-   0        0        0      656 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_0.json
+-rw-rw-rw-   0        0        0      660 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_1.json
+-rw-rw-rw-   0        0        0      657 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_2.json
+-rw-rw-rw-   0        0        0      659 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_3.json
+-rw-rw-rw-   0        0        0       90 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_0.json
+-rw-rw-rw-   0        0        0       90 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_1.json
+-rw-rw-rw-   0        0        0       90 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_2.json
+-rw-rw-rw-   0        0        0       90 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_3.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_0.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_1.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_2.json
+-rw-rw-rw-   0        0        0      101 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_3.json
+-rw-rw-rw-   0        0        0      108 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_0.json
+-rw-rw-rw-   0        0        0      108 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_1.json
+-rw-rw-rw-   0        0        0      108 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_2.json
+-rw-rw-rw-   0        0        0      108 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_3.json
+-rw-rw-rw-   0        0        0       98 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_0.json
+-rw-rw-rw-   0        0        0       98 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_1.json
+-rw-rw-rw-   0        0        0       98 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_2.json
+-rw-rw-rw-   0        0        0       98 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_3.json
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.314816 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/
+-rw-rw-rw-   0        0        0       96 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/creeper.json
+-rw-rw-rw-   0        0        0     3870 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/dragon.json
+-rw-rw-rw-   0        0        0      559 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head.json
+-rw-rw-rw-   0        0        0      559 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head2.json
+-rw-rw-rw-   0        0        0       87 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/player.json
+-rw-rw-rw-   0        0        0       98 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/skeleton.json
+-rw-rw-rw-   0        0        0      105 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/wither_skeleton.json
+-rw-rw-rw-   0        0        0       95 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/zombie.json
+-rw-rw-rw-   0        0        0      134 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/lava.json
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.314816 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/
+-rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_0.json
+-rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_1.json
+-rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_10.json
+-rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_11.json
+-rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_12.json
+-rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_13.json
+-rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_14.json
+-rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_15.json
+-rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_2.json
+-rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_3.json
+-rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_4.json
+-rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_5.json
+-rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_6.json
+-rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_7.json
+-rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_8.json
+-rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_9.json
+-rw-rw-rw-   0        0        0      163 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light_blue_shulker_box.json
+-rw-rw-rw-   0        0        0      163 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light_gray_shulker_box.json
+-rw-rw-rw-   0        0        0      151 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/lime_shulker_box.json
+-rw-rw-rw-   0        0        0      157 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/magenta_shulker_box.json
+-rw-rw-rw-   0        0        0      151 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/moving_piston.json
+-rw-rw-rw-   0        0        0      155 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/orange_shulker_box.json
+-rw-rw-rw-   0        0        0      151 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/pink_shulker_box.json
+-rw-rw-rw-   0        0        0      155 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/purple_shulker_box.json
+-rw-rw-rw-   0        0        0      149 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/red_shulker_box.json
+-rw-rw-rw-   0        0        0      141 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/shulker_box.json
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.346064 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/
+-rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_0.json
+-rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_1.json
+-rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_2.json
+-rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_3.json
+-rw-rw-rw-   0        0        0      125 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_0.json
+-rw-rw-rw-   0        0        0      125 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_1.json
+-rw-rw-rw-   0        0        0      125 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_2.json
+-rw-rw-rw-   0        0        0      125 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_3.json
+-rw-rw-rw-   0        0        0      129 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_0.json
+-rw-rw-rw-   0        0        0      129 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_1.json
+-rw-rw-rw-   0        0        0      129 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_2.json
+-rw-rw-rw-   0        0        0      129 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_3.json
+-rw-rw-rw-   0        0        0      131 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_0.json
+-rw-rw-rw-   0        0        0      131 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_1.json
+-rw-rw-rw-   0        0        0      131 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_2.json
+-rw-rw-rw-   0        0        0      131 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_3.json
+-rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_0.json
+-rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_1.json
+-rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_2.json
+-rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_3.json
+-rw-rw-rw-   0        0        0      131 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_0.json
+-rw-rw-rw-   0        0        0      131 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_1.json
+-rw-rw-rw-   0        0        0      131 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_2.json
+-rw-rw-rw-   0        0        0      131 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_3.json
+-rw-rw-rw-   0        0        0      121 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_0.json
+-rw-rw-rw-   0        0        0      121 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_1.json
+-rw-rw-rw-   0        0        0      121 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_2.json
+-rw-rw-rw-   0        0        0      121 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_3.json
+-rw-rw-rw-   0        0        0     1184 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_0.json
+-rw-rw-rw-   0        0        0     1173 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_1.json
+-rw-rw-rw-   0        0        0     1167 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_2.json
+-rw-rw-rw-   0        0        0     1171 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_3.json
+-rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_0.json
+-rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_1.json
+-rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_2.json
+-rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_3.json
+-rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_0.json
+-rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_1.json
+-rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_2.json
+-rw-rw-rw-   0        0        0      127 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_3.json
+-rw-rw-rw-   0        0        0      147 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/structure_void.json
+-rw-rw-rw-   0        0        0      106 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/trapped_chest.json
+-rw-rw-rw-   0        0        0      116 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/trapped_chest_left.json
+-rw-rw-rw-   0        0        0      118 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/trapped_chest_right.json
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.346064 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/
+-rw-rw-rw-   0        0        0       98 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/black.json
+-rw-rw-rw-   0        0        0       97 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/blue.json
+-rw-rw-rw-   0        0        0       98 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/brown.json
+-rw-rw-rw-   0        0        0       97 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/cyan.json
+-rw-rw-rw-   0        0        0       97 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/gray.json
+-rw-rw-rw-   0        0        0       98 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/green.json
+-rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/light_blue.json
+-rw-rw-rw-   0        0        0      103 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/light_gray.json
+-rw-rw-rw-   0        0        0       97 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/lime.json
+-rw-rw-rw-   0        0        0      100 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/magenta.json
+-rw-rw-rw-   0        0        0       99 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/orange.json
+-rw-rw-rw-   0        0        0       97 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/pink.json
+-rw-rw-rw-   0        0        0       99 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/purple.json
+-rw-rw-rw-   0        0        0       96 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/red.json
+-rw-rw-rw-   0        0        0       98 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/white.json
+-rw-rw-rw-   0        0        0       99 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/yellow.json
+-rw-rw-rw-   0        0        0     1208 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner.json
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.346064 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/
+-rw-rw-rw-   0        0        0      135 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/acacia.json
+-rw-rw-rw-   0        0        0      133 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/birch.json
+-rw-rw-rw-   0        0        0      137 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/crimson.json
+-rw-rw-rw-   0        0        0      139 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/dark_oak.json
+-rw-rw-rw-   0        0        0      135 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/jungle.json
+-rw-rw-rw-   0        0        0      139 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/mangrove.json
+-rw-rw-rw-   0        0        0      129 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/oak.json
+-rw-rw-rw-   0        0        0      135 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/spruce.json
+-rw-rw-rw-   0        0        0      588 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/wall_sign.json
+-rw-rw-rw-   0        0        0      135 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/warped.json
+-rw-rw-rw-   0        0        0      135 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/water.json
+-rw-rw-rw-   0        0        0      153 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/white_shulker_box.json
+-rw-rw-rw-   0        0        0      155 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/yellow_shulker_box.json
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.111689 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.361687 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.361687 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/
+-rw-rw-rw-   0        0        0     2769 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_black.png
+-rw-rw-rw-   0        0        0     3786 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_blue.png
+-rw-rw-rw-   0        0        0     3707 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_brown.png
+-rw-rw-rw-   0        0        0     3813 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_cyan.png
+-rw-rw-rw-   0        0        0     3518 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_gray.png
+-rw-rw-rw-   0        0        0     3751 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_green.png
+-rw-rw-rw-   0        0        0     4220 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_blue.png
+-rw-rw-rw-   0        0        0     3953 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_gray.png
+-rw-rw-rw-   0        0        0     4151 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_lime.png
+-rw-rw-rw-   0        0        0     4178 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_magenta.png
+-rw-rw-rw-   0        0        0     4298 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_orange.png
+-rw-rw-rw-   0        0        0     4205 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_pink.png
+-rw-rw-rw-   0        0        0     4056 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_purple.png
+-rw-rw-rw-   0        0        0     3790 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_red.png
+-rw-rw-rw-   0        0        0     3985 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_white.png
+-rw-rw-rw-   0        0        0     4457 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_yellow.png
+-rw-rw-rw-   0        0        0      651 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/barrier.png
+-rw-rw-rw-   0        0        0     1265 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/end_portal.png
+-rw-rw-rw-   0        0        0      213 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/grass.png
+-rw-rw-rw-   0        0        0     1286 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/lava.png
+-rw-rw-rw-   0        0        0     1405 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/structure_void.png
+-rw-rw-rw-   0        0        0      927 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/water.png
+-rw-rw-rw-   0        0        0      117 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/pack.mcmeta
+-rw-rw-rw-   0        0        0    22749 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/pack.png
+-rw-rw-rw-   0        0        0     1687 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/resource_pack.py
+-rw-rw-rw-   0        0        0    22312 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/resource_pack_manager.py
+-rw-rw-rw-   0        0        0      299 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/unknown_resource_pack.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:21:50.377310 minecraft_resource_pack-1.4.2/minecraft_resource_pack.egg-info/
+-rw-rw-rw-   0        0        0      876 2024-05-01 11:21:49.000000 minecraft_resource_pack-1.4.2/minecraft_resource_pack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    48947 2024-05-01 11:21:50.000000 minecraft_resource_pack-1.4.2/minecraft_resource_pack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 11:21:49.000000 minecraft_resource_pack-1.4.2/minecraft_resource_pack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-05-01 11:21:49.000000 minecraft_resource_pack-1.4.2/minecraft_resource_pack.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-01 11:21:49.000000 minecraft_resource_pack-1.4.2/minecraft_resource_pack.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      177 2024-05-01 11:21:49.000000 minecraft_resource_pack-1.4.2/minecraft_resource_pack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-01 11:21:49.000000 minecraft_resource_pack-1.4.2/minecraft_resource_pack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      131 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1190 2024-05-01 11:21:50.377310 minecraft_resource_pack-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      142 2024-05-01 11:21:19.000000 minecraft_resource_pack-1.4.2/setup.py
```

### Comparing `minecraft-resource-pack-1.4.1/LICENSE` & `minecraft_resource_pack-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/PKG-INFO` & `minecraft_resource_pack-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft-resource-pack
-Version: 1.4.1
+Version: 1.4.2
 Summary: A Python library reading Minecraft's various resource pack formats.
 Home-page: https://www.amuletmc.com
 Author: James Clare
 Author-email: amuleteditor@gmail.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/__init__.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/amulet/block.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/amulet/block.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/comment_json.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/comment_json.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/image/missing_pack_java.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/image/missing_pack_java.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/mesh/block/block_mesh.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/mesh/block/block_mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
     def vert_tables(self) -> Dict[str, numpy.ndarray]:
         """A dictionary of cull dir -> the flat vert table containing vertices, texture coords and (in the future) normals"""
         if self._vert_tables is None:
             self._vert_tables = {
                 key: numpy.hstack(
                     (
                         self._verts[key].reshape(-1, self._face_mode),
-                        self._texture_coords[key].reshape(-1, 2)
+                        self._texture_coords[key].reshape(-1, 2),
                         # TODO: add in face normals
                     )
                 ).ravel()
                 for key in self._verts.keys()
             }
             [a.setflags(write=False) for a in self._vert_tables.values()]
         return self._vert_tables
```

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/mesh/block/cube.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/mesh/block/cube.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/mesh/block/missing_block.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/mesh/block/missing_block.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/__init__.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/__init__.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/base/resource_pack.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/base/resource_pack.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/base/resource_pack_manager.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/base/resource_pack_manager.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/blocks.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/blocks.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/manifest.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/manifest.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/pack_icon.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/pack_icon.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/grass_carried.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/grass_carried.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/water.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/water.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/block_palette.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/block_palette.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/__init__.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/__init__.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/air.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/air.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/base_blockshape.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/base_blockshape.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/bubble_column.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/bubble_column.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cake.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cake.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/chest.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/chest.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/comparator.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/comparator.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cube.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cube.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/default.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/default.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/double_plant.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/double_plant.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/enchanting_table.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/enchanting_table.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/farmland.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/farmland.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/fence.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/fence.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat_wall.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat_wall.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/furnace.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/furnace.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/green_cube.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/green_cube.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/ladder.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/ladder.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/partial_block.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/partial_block.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston_arm.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston_arm.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/portal_frame.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/portal_frame.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pressure_plate.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pressure_plate.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/repeater.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/repeater.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/slab.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/slab.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/tree.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/tree.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/vine.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/vine.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/wall.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/wall.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/water.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes/water.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/blockshapes.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/blockshapes.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/download_resources.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/download_resources.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/resource_pack.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/resource_pack.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/bedrock/resource_pack_manager.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/bedrock/resource_pack_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,21 @@
 from minecraft_model_reader.api import Block, comment_json
 from minecraft_model_reader.api.resource_pack import BaseResourcePackManager
 from minecraft_model_reader.api.resource_pack.bedrock import BedrockResourcePack
 from minecraft_model_reader.api.mesh.block.block_mesh import BlockMesh
 from .blockshapes import BlockShapeClasses
 
 
-def _load_data() -> (
-    Tuple[
-        Dict[str, str],
-        Dict[
-            str,
-            Tuple[Tuple[Tuple[str, str], ...], Dict[Tuple[Union[str, int], ...], int]],
-        ],
-    ]
-):
+def _load_data() -> Tuple[
+    Dict[str, str],
+    Dict[
+        str,
+        Tuple[Tuple[Tuple[str, str], ...], Dict[Tuple[Union[str, int], ...], int]],
+    ],
+]:
     with open(os.path.join(os.path.dirname(__file__), "blockshapes.json")) as f:
         _block_shapes = comment_json.load(f)
 
     _aux_values = {}
     with open(os.path.join(os.path.dirname(__file__), "block_palette.json")) as f:
         _block_palette = comment_json.load(f)
     for block in _block_palette["blocks"]:
@@ -44,17 +42,19 @@
 
 def get_aux_value(block: Block) -> int:
     name = block.namespaced_name
     if name in AuxValues:
         property_names, aux_map = AuxValues[name]
         properties = block.properties
         key = tuple(
-            properties[property_name].py_data
-            if property_name in properties
-            else default
+            (
+                properties[property_name].py_data
+                if property_name in properties
+                else default
+            )
             for property_name, default in property_names
         )
         return aux_map.get(key, 0)
     else:
         return 0
 
 
@@ -65,20 +65,18 @@
     def __init__(
         self,
         resource_packs: Union[BedrockResourcePack, Iterable[BedrockResourcePack]],
         load=True,
     ):
         super().__init__()
         self._block_shapes: Dict[str, str] = {}  # block string to block shape
-        self._blocks: Dict[
-            str, Union[Dict[str, str], str, None]
-        ] = {}  # block string to short texture ids
-        self._terrain_texture: Dict[
-            str, Tuple[str, ...]
-        ] = (
+        self._blocks: Dict[str, Union[Dict[str, str], str, None]] = (
+            {}
+        )  # block string to short texture ids
+        self._terrain_texture: Dict[str, Tuple[str, ...]] = (
             {}
         )  # texture ids to list of relative paths. Each relates to a different data value.
         self._textures: Dict[str, str] = {}  # relative path to texture path
         self._all_textures = None
 
         self._texture_is_transparent: Dict[str, Tuple[int, bool]] = {}
```

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/download_resources.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/download_resources.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import shutil
 import zipfile
 import json
-from urllib.request import urlopen
+from urllib.request import urlopen, Request
 import io
 from typing import Generator, List
 import logging
 
 from minecraft_model_reader.api.resource_pack import JavaResourcePack
 
 log = logging.getLogger(__name__)
@@ -110,26 +110,46 @@
     temp_path = os.path.join(os.path.dirname(path), "_temp_")
     # clear the temporary location
     if os.path.isfile(temp_path):
         os.remove(temp_path)
     elif os.path.isdir(temp_path):
         shutil.rmtree(temp_path, ignore_errors=True)
 
-    try:
-        yield from download_resources_iter(temp_path, version)
-    except:
-        pass
+    yield from download_resources_iter(temp_path, version)
+    if os.path.isdir(path):
+        shutil.rmtree(path, ignore_errors=True)
+
+    shutil.move(temp_path, path)
+
+    with open(os.path.join(path, "version"), "w") as f:
+        f.write(version)
+
+
+def download_with_retry(
+    url: str, chunk_size: int = 4096, attempts: int = 5
+) -> Generator[float, None, bytes]:
+    content_length_found = 0
+    content = []
+
+    for _ in range(attempts):
+        request = Request(url, headers={"Range": f"bytes={content_length_found}-"})
+        with urlopen(request, timeout=20) as response:
+            content_length = int(response.headers["content-length"].strip())
+            while content_length_found < content_length:
+                chunk = response.read(chunk_size)
+                if not chunk:
+                    break
+                content.append(chunk)
+                content_length_found += len(chunk)
+                yield min(1.0, content_length_found / content_length)
+        if content_length == content_length_found:
+            break
     else:
-        if os.path.isdir(path):
-            shutil.rmtree(path, ignore_errors=True)
-
-        shutil.move(temp_path, path)
-
-        with open(os.path.join(path, "version"), "w") as f:
-            f.write(version)
+        raise RuntimeError(f"Failed to download")
+    return b"".join(content)
 
 
 def download_resources(path, version):
     generator_unpacker(download_resources_iter(path, version))
 
 
 def download_resources_iter(
@@ -144,26 +164,22 @@
         raise Exception(f"Could not find Java resource pack for version {version}.")
 
     try:
         with urlopen(version_url, timeout=20) as vm:
             version_manifest = json.load(vm)
         version_client_url = version_manifest["downloads"]["client"]["url"]
 
-        with urlopen(version_client_url, timeout=20) as response:
-            data = []
-            data_size = int(response.headers["content-length"].strip())
-            index = 0
-            chunk = b"hello"
-            while chunk:
-                chunk = response.read(chunk_size)
-                data.append(chunk)
-                index += 1
-                yield min(1.0, (index * chunk_size) / (data_size * 2))
+        downloader = download_with_retry(version_client_url)
+        try:
+            while True:
+                yield next(downloader) / 2
+        except StopIteration as e:
+            data = e.value
 
-        client = zipfile.ZipFile(io.BytesIO(b"".join(data)))
+        client = zipfile.ZipFile(io.BytesIO(data))
         paths: List[str] = [
             fpath for fpath in client.namelist() if fpath.startswith("assets/")
         ]
         path_count = len(paths)
         for path_index, fpath in enumerate(paths):
             if not path_index % 30:
                 yield path_index / (path_count * 2) + 0.5
```

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/acacia_sign.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/acacia_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/birch_sign.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/birch_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_banner.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_bed.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_banner.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_bed.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_banner.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_bed.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/chest.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/chest.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/creeper_head.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/creeper_head.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/crimson_sign.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/crimson_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_banner.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_bed.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dark_oak_sign.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dark_oak_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dragon_head.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dragon_head.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_banner.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_bed.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_banner.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_bed.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/jungle_sign.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/jungle_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_banner.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_bed.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_banner.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_bed.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_banner.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_bed.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_banner.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_bed.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/mangrove_sign.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/mangrove_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/oak_sign.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/oak_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_banner.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_bed.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_banner.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_bed.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/player_head.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/player_head.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_banner.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_bed.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_banner.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_bed.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/skeleton_skull.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/skeleton_skull.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/spruce_sign.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/spruce_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/trapped_chest.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/trapped_chest.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/warped_sign.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/warped_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_banner.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_bed.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/wither_skeleton_skull.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/wither_skeleton_skull.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_banner.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_bed.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_bed.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/zombie_head.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/zombie_head.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_0.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_0.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_1.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_1.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_2.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_2.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_3.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_3.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_foot.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_foot.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_head.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_head.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_between_walls.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_between_walls.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_ceiling.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_ceiling.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_floor.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_floor.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_wall.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_wall.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_base.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_base.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_left_base.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_left_base.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_right_base.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_right_base.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/conduit.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/conduit.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_0.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_0.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_1.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_1.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_2.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_2.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_3.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_3.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_0.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_0.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_1.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_1.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_2.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_2.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_3.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_3.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_0.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_0.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_1.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_1.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_2.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_2.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_3.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_3.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/dragon.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/dragon.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head2.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head2.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_0.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_0.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_1.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_1.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_2.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_2.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_3.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_3.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/wall_sign.json` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/wall_sign.json`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_black.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_black.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_blue.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_blue.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_brown.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_brown.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_cyan.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_cyan.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_gray.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_gray.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_green.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_green.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_blue.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_blue.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_gray.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_gray.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_lime.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_lime.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_magenta.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_magenta.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_orange.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_orange.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_pink.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_pink.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_purple.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_purple.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_red.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_red.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_white.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_white.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_yellow.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_yellow.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/barrier.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/barrier.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/end_portal.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/end_portal.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/lava.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/lava.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/structure_void.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/structure_void.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/water.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/water.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/pack.png` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/pack.png`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/resource_pack.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/resource_pack.py`

 * *Files identical despite different names*

### Comparing `minecraft-resource-pack-1.4.1/minecraft_model_reader/api/resource_pack/java/resource_pack_manager.py` & `minecraft_resource_pack-1.4.2/minecraft_model_reader/api/resource_pack/java/resource_pack_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,17 +141,17 @@
                 )
                 blockstate_count = len(blockstate_paths)
                 sub_progress = pack_progress + 1 / (pack_count * 3)
                 for blockstate_index, blockstate_path in enumerate(blockstate_paths):
                     _, namespace, _, blockstate_file = os.path.normpath(
                         os.path.relpath(blockstate_path, pack.root_dir)
                     ).split(os.sep)
-                    blockstate_file_paths[
-                        (namespace, blockstate_file[:-5])
-                    ] = blockstate_path
+                    blockstate_file_paths[(namespace, blockstate_file[:-5])] = (
+                        blockstate_path
+                    )
                     yield sub_progress + (blockstate_index) / (
                         blockstate_count * pack_count * 3
                     )
 
                 model_paths = glob.glob(
                     os.path.join(
                         glob.escape(pack.root_dir),
@@ -166,17 +166,17 @@
                 model_count = len(model_paths)
                 sub_progress = pack_progress + 2 / (pack_count * 3)
                 for model_index, model_path in enumerate(model_paths):
                     _, namespace, _, *rel_path_list = os.path.normpath(
                         os.path.relpath(model_path, pack.root_dir)
                     ).split(os.sep)
                     rel_path = "/".join(rel_path_list)[:-5]
-                    model_file_paths[
-                        (namespace, rel_path.replace(os.sep, "/"))
-                    ] = model_path
+                    model_file_paths[(namespace, rel_path.replace(os.sep, "/"))] = (
+                        model_path
+                    )
                     yield sub_progress + (model_index) / (model_count * pack_count * 3)
 
         os.makedirs(os.path.dirname(transparency_cache_path), exist_ok=True)
         with open(transparency_cache_path, "w") as f:
             json.dump(self._texture_is_transparent, f)
 
         for key, path in blockstate_file_paths.items():
```

### Comparing `minecraft-resource-pack-1.4.1/minecraft_resource_pack.egg-info/PKG-INFO` & `minecraft_resource_pack-1.4.2/minecraft_resource_pack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft-resource-pack
-Version: 1.4.1
+Version: 1.4.2
 Summary: A Python library reading Minecraft's various resource pack formats.
 Home-page: https://www.amuletmc.com
 Author: James Clare
 Author-email: amuleteditor@gmail.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `minecraft-resource-pack-1.4.1/minecraft_resource_pack.egg-info/SOURCES.txt` & `minecraft_resource_pack-1.4.2/minecraft_resource_pack.egg-info/SOURCES.txt`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,471 +1,471 @@
-LICENSE
-MANIFEST.in
-pyproject.toml
-setup.cfg
-setup.py
-minecraft_model_reader/__init__.py
-minecraft_model_reader/_version.py
-minecraft_model_reader/__pyinstaller/__init__.py
-minecraft_model_reader/__pyinstaller/hook-minecraft_model_reader.py
-minecraft_model_reader/api/__init__.py
-minecraft_model_reader/api/comment_json.py
-minecraft_model_reader/api/amulet/__init__.py
-minecraft_model_reader/api/amulet/block.py
-minecraft_model_reader/api/image/__init__.py
-minecraft_model_reader/api/image/missing_no.png
-minecraft_model_reader/api/image/missing_pack_java.png
-minecraft_model_reader/api/mesh/__init__.py
-minecraft_model_reader/api/mesh/util.py
-minecraft_model_reader/api/mesh/block/__init__.py
-minecraft_model_reader/api/mesh/block/block_mesh.py
-minecraft_model_reader/api/mesh/block/cube.py
-minecraft_model_reader/api/mesh/block/missing_block.py
-minecraft_model_reader/api/resource_pack/__init__.py
-minecraft_model_reader/api/resource_pack/unknown_resource_pack.py
-minecraft_model_reader/api/resource_pack/base/__init__.py
-minecraft_model_reader/api/resource_pack/base/resource_pack.py
-minecraft_model_reader/api/resource_pack/base/resource_pack_manager.py
-minecraft_model_reader/api/resource_pack/bedrock/__init__.py
-minecraft_model_reader/api/resource_pack/bedrock/block_palette.json
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes.json
-minecraft_model_reader/api/resource_pack/bedrock/download_resources.py
-minecraft_model_reader/api/resource_pack/bedrock/resource_pack.py
-minecraft_model_reader/api/resource_pack/bedrock/resource_pack_manager.py
-minecraft_model_reader/api/resource_pack/bedrock/sort_blockshapes.py
-minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/blocks.json
-minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/manifest.json
-minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/pack_icon.png
-minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/terrain_texture.json
-minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/grass_carried.png
-minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/grass_side_carried.png
-minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/water.png
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/__init__.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/air.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/base_blockshape.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/bubble_column.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cake.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/chest.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/comparator.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture0.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture_green.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cube.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/default.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door1.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door2.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door3.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door4.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door5.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door6.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/double_plant.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/enchanting_table.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/farmland.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/fence.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat_wall.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/furnace.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/furnace_lit.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/green_cube.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/ladder.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/lilypad.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/partial_block.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston_arm.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/portal_frame.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pressure_plate.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin_carved.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin_lit.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/red_dust.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/repeater.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/slab.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/slab_double.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/tree.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/turtle_egg.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/vine.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/wall.py
-minecraft_model_reader/api/resource_pack/bedrock/blockshapes/water.py
-minecraft_model_reader/api/resource_pack/java/__init__.py
-minecraft_model_reader/api/resource_pack/java/download_resources.py
-minecraft_model_reader/api/resource_pack/java/resource_pack.py
-minecraft_model_reader/api/resource_pack/java/resource_pack_manager.py
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/pack.mcmeta
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/pack.png
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/acacia_sign.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/acacia_wall_sign.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/birch_sign.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/birch_wall_sign.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_bed.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_wall_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_bed.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_wall_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_bed.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_wall_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/chest.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/creeper_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/creeper_wall_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/crimson_sign.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/crimson_wall_sign.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_bed.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_wall_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dark_oak_sign.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dark_oak_wall_sign.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dragon_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dragon_wall_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/ender_chest.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/grass.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_bed.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_wall_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_bed.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_wall_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/jungle_sign.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/jungle_wall_sign.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_bed.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_wall_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_bed.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_wall_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_bed.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_wall_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_bed.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_wall_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/mangrove_sign.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/mangrove_wall_sign.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/oak_sign.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/oak_wall_sign.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_bed.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_wall_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_bed.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_wall_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/player_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/player_wall_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_bed.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_wall_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_bed.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_wall_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/skeleton_skull.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/skeleton_wall_skull.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/spruce_sign.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/spruce_wall_sign.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/structure_void.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/trapped_chest.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/warped_sign.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/warped_wall_sign.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_bed.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_wall_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/wither_skeleton_skull.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/wither_skeleton_wall_skull.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_bed.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_wall_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/zombie_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/zombie_wall_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/barrier.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_foot.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_between_walls.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_ceiling.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_floor.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_wall.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/black_shulker_box.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/blue_shulker_box.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/brown_shulker_box.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_base.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_left.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_left_base.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_right.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_right_base.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/conduit.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/cyan_shulker_box.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/end_portal.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/ender_chest.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/grass.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/gray_shulker_box.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/green_shulker_box.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/lava.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light_blue_shulker_box.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light_gray_shulker_box.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/lime_shulker_box.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/magenta_shulker_box.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/moving_piston.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/orange_shulker_box.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/pink_shulker_box.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/purple_shulker_box.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/red_shulker_box.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/shulker_box.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/structure_void.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/trapped_chest.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/trapped_chest_left.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/trapped_chest_right.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/water.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/white_shulker_box.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/yellow_shulker_box.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/black_foot.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/black_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/blue_foot.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/blue_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/brown_foot.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/brown_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/cyan_foot.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/cyan_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/gray_foot.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/gray_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/green_foot.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/green_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_blue_foot.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_blue_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_gray_foot.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_gray_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/lime_foot.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/lime_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/magenta_foot.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/magenta_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/orange_foot.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/orange_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/pink_foot.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/pink_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/purple_foot.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/purple_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/red_foot.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/red_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/white_foot.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/white_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/yellow_foot.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/yellow_head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/creeper.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/dragon.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/player.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/skeleton.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/wither_skeleton.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/zombie.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_10.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_11.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_12.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_13.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_14.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_15.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_4.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_5.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_6.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_7.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_8.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_9.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_0.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_1.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_2.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_3.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/black.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/blue.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/brown.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/cyan.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/gray.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/green.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/light_blue.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/light_gray.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/lime.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/magenta.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/orange.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/pink.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/purple.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/red.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/white.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/yellow.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/acacia.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/birch.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/crimson.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/dark_oak.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/jungle.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/mangrove.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/oak.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/spruce.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/wall_sign.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/warped.json
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/barrier.png
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/end_portal.png
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/grass.png
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/lava.png
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/structure_void.png
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/water.png
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_black.png
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_blue.png
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_brown.png
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_cyan.png
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_gray.png
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_green.png
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_blue.png
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_gray.png
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_lime.png
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_magenta.png
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_orange.png
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_pink.png
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_purple.png
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_red.png
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_white.png
-minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_yellow.png
-minecraft_resource_pack.egg-info/PKG-INFO
-minecraft_resource_pack.egg-info/SOURCES.txt
-minecraft_resource_pack.egg-info/dependency_links.txt
-minecraft_resource_pack.egg-info/entry_points.txt
-minecraft_resource_pack.egg-info/not-zip-safe
-minecraft_resource_pack.egg-info/requires.txt
+LICENSE
+MANIFEST.in
+pyproject.toml
+setup.cfg
+setup.py
+minecraft_model_reader/__init__.py
+minecraft_model_reader/_version.py
+minecraft_model_reader/__pyinstaller/__init__.py
+minecraft_model_reader/__pyinstaller/hook-minecraft_model_reader.py
+minecraft_model_reader/api/__init__.py
+minecraft_model_reader/api/comment_json.py
+minecraft_model_reader/api/amulet/__init__.py
+minecraft_model_reader/api/amulet/block.py
+minecraft_model_reader/api/image/__init__.py
+minecraft_model_reader/api/image/missing_no.png
+minecraft_model_reader/api/image/missing_pack_java.png
+minecraft_model_reader/api/mesh/__init__.py
+minecraft_model_reader/api/mesh/util.py
+minecraft_model_reader/api/mesh/block/__init__.py
+minecraft_model_reader/api/mesh/block/block_mesh.py
+minecraft_model_reader/api/mesh/block/cube.py
+minecraft_model_reader/api/mesh/block/missing_block.py
+minecraft_model_reader/api/resource_pack/__init__.py
+minecraft_model_reader/api/resource_pack/unknown_resource_pack.py
+minecraft_model_reader/api/resource_pack/base/__init__.py
+minecraft_model_reader/api/resource_pack/base/resource_pack.py
+minecraft_model_reader/api/resource_pack/base/resource_pack_manager.py
+minecraft_model_reader/api/resource_pack/bedrock/__init__.py
+minecraft_model_reader/api/resource_pack/bedrock/block_palette.json
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes.json
+minecraft_model_reader/api/resource_pack/bedrock/download_resources.py
+minecraft_model_reader/api/resource_pack/bedrock/resource_pack.py
+minecraft_model_reader/api/resource_pack/bedrock/resource_pack_manager.py
+minecraft_model_reader/api/resource_pack/bedrock/sort_blockshapes.py
+minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/blocks.json
+minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/manifest.json
+minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/pack_icon.png
+minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/terrain_texture.json
+minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/grass_carried.png
+minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/grass_side_carried.png
+minecraft_model_reader/api/resource_pack/bedrock/bedrock_vanilla_fix/textures/blocks/water.png
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/__init__.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/air.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/base_blockshape.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/bubble_column.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cake.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/chest.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/comparator.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture0.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cross_texture_green.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/cube.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/default.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door1.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door2.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door3.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door4.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door5.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/door6.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/double_plant.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/enchanting_table.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/farmland.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/fence.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/flat_wall.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/furnace.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/furnace_lit.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/green_cube.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/ladder.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/lilypad.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/partial_block.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/piston_arm.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/portal_frame.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pressure_plate.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin_carved.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/pumpkin_lit.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/red_dust.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/repeater.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/slab.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/slab_double.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/tree.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/turtle_egg.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/vine.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/wall.py
+minecraft_model_reader/api/resource_pack/bedrock/blockshapes/water.py
+minecraft_model_reader/api/resource_pack/java/__init__.py
+minecraft_model_reader/api/resource_pack/java/download_resources.py
+minecraft_model_reader/api/resource_pack/java/resource_pack.py
+minecraft_model_reader/api/resource_pack/java/resource_pack_manager.py
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/pack.mcmeta
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/pack.png
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/acacia_sign.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/acacia_wall_sign.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/birch_sign.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/birch_wall_sign.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_bed.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/black_wall_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_bed.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/blue_wall_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_bed.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/brown_wall_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/chest.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/creeper_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/creeper_wall_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/crimson_sign.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/crimson_wall_sign.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_bed.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/cyan_wall_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dark_oak_sign.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dark_oak_wall_sign.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dragon_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/dragon_wall_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/ender_chest.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/grass.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_bed.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/gray_wall_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_bed.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/green_wall_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/jungle_sign.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/jungle_wall_sign.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_bed.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_blue_wall_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_bed.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/light_gray_wall_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_bed.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/lime_wall_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_bed.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/magenta_wall_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/mangrove_sign.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/mangrove_wall_sign.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/oak_sign.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/oak_wall_sign.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_bed.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/orange_wall_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_bed.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/pink_wall_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/player_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/player_wall_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_bed.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/purple_wall_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_bed.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/red_wall_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/skeleton_skull.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/skeleton_wall_skull.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/spruce_sign.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/spruce_wall_sign.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/structure_void.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/trapped_chest.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/warped_sign.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/warped_wall_sign.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_bed.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/white_wall_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/wither_skeleton_skull.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/wither_skeleton_wall_skull.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_bed.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/yellow_wall_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/zombie_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/blockstates/zombie_wall_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/barrier.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_foot.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_between_walls.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_ceiling.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_floor.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bell_wall.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/black_shulker_box.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/blue_shulker_box.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/brown_shulker_box.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_base.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_left.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_left_base.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_right.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/chest_right_base.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/conduit.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/cyan_shulker_box.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/end_portal.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/ender_chest.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/grass.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/gray_shulker_box.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/green_shulker_box.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/lava.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light_blue_shulker_box.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light_gray_shulker_box.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/lime_shulker_box.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/magenta_shulker_box.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/moving_piston.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/orange_shulker_box.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/pink_shulker_box.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/purple_shulker_box.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/red_shulker_box.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/shulker_box.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/structure_void.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/trapped_chest.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/trapped_chest_left.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/trapped_chest_right.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/water.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/white_shulker_box.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/yellow_shulker_box.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/banner_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/black_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/blue_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/brown_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/cyan_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/gray_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/green_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_blue_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/light_gray_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/lime_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/magenta_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/orange_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/pink_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/purple_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/red_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/white_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/banner/yellow_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/black_foot.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/black_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/blue_foot.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/blue_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/brown_foot.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/brown_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/cyan_foot.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/cyan_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/gray_foot.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/gray_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/green_foot.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/green_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_blue_foot.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_blue_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_gray_foot.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/light_gray_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/lime_foot.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/lime_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/magenta_foot.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/magenta_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/orange_foot.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/orange_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/pink_foot.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/pink_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/purple_foot.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/purple_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/red_foot.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/red_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/white_foot.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/white_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/yellow_foot.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/bed/yellow_head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/creeper_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/dragon_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head2_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/head_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/player_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/skeleton_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/wither_skeleton_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/floor/zombie_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/creeper.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/dragon.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/head2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/player.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/skeleton.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/wither_skeleton.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/head/wall/zombie.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_10.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_11.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_12.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_13.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_14.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_15.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_4.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_5.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_6.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_7.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_8.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/light/level_9.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/acacia_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/birch_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/crimson_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/dark_oak_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/jungle_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/mangrove_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/oak_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/sign_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/spruce_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_0.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_1.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_2.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/sign/warped_3.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/black.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/blue.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/brown.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/cyan.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/gray.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/green.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/light_blue.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/light_gray.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/lime.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/magenta.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/orange.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/pink.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/purple.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/red.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/white.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_banner/yellow.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/acacia.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/birch.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/crimson.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/dark_oak.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/jungle.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/mangrove.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/oak.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/spruce.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/wall_sign.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/models/block/wall_sign/warped.json
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/barrier.png
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/end_portal.png
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/grass.png
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/lava.png
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/structure_void.png
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/water.png
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_black.png
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_blue.png
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_brown.png
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_cyan.png
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_gray.png
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_green.png
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_blue.png
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_light_gray.png
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_lime.png
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_magenta.png
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_orange.png
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_pink.png
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_purple.png
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_red.png
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_white.png
+minecraft_model_reader/api/resource_pack/java/java_vanilla_fix/assets/minecraft/textures/block/banner/banner_yellow.png
+minecraft_resource_pack.egg-info/PKG-INFO
+minecraft_resource_pack.egg-info/SOURCES.txt
+minecraft_resource_pack.egg-info/dependency_links.txt
+minecraft_resource_pack.egg-info/entry_points.txt
+minecraft_resource_pack.egg-info/not-zip-safe
+minecraft_resource_pack.egg-info/requires.txt
 minecraft_resource_pack.egg-info/top_level.txt
```

### Comparing `minecraft-resource-pack-1.4.1/setup.cfg` & `minecraft_resource_pack-1.4.2/setup.cfg`

 * *Files identical despite different names*

