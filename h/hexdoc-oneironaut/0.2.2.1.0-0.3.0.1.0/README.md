# Comparing `tmp/hexdoc_oneironaut-0.2.2.1.0.tar.gz` & `tmp/hexdoc_oneironaut-0.3.0.1.0.tar.gz`

## Comparing `hexdoc_oneironaut-0.2.2.1.0.tar` & `hexdoc_oneironaut-0.3.0.1.0.tar`

### file list

```diff
@@ -1,121 +1,136 @@
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/gradle.properties
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/__gradle_version__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/__version__.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_hooks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/py.typed
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/__init__.py
--rw-r--r--   0        0        0    12412 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/oneironaut.hexdoc.json
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/oneironaut.patterns.hexdoc.json
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/hexcasting/lang/en_us.flatten.json5
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/blockstates/circle.json
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/blockstates/noosphere_basalt.json
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/blockstates/noosphere_gate.json
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/blockstates/pseudoamethyst_block.json
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/blockstates/raycast_blocker.json
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/blockstates/raycast_blocker_glass.json
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/blockstates/sentinel_sensor.json
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/blockstates/sentinel_trap.json
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/blockstates/super_budding.json
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/blockstates/thought_slurry.json
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/blockstates/wisp_lantern.json
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/blockstates/wisp_lantern_tinted.json
--rw-r--r--   0        0        0    25554 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/lang/en_us.json
--rw-r--r--   0        0        0    38165 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/lang/zh_cn.json
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/circle.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/noosphere_basalt.json
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/pseudoamethyst_block.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/raycast_blocker.json
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/raycast_blocker_glass.json
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/sentinel_sensor.json
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/sentinel_trap_unpowered.json
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/super_budding.json
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/circle.json
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/echo_staff.json
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/endless_phial.json
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/noosphere_basalt.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/pigment_echo.json
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/pigment_flame.json
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/pigment_noosphere.json
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/pseudoamethyst_block.json
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/pseudoamethyst_shard.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/raycast_blocker.json
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/raycast_blocker_glass.json
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/reverberation_rod.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/reverberation_rod_casting.json
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/reverberation_rod_filled.json
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/sentinel_sensor.json
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/sentinel_trap.json
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/spoon_staff.json
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/super_budding.json
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/thought_slurry_bucket.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/wisp_lantern.json
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/wisp_lantern_tinted.json
--rw-r--r--   0        0        0     9564 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/black_circle.png
--rw-r--r--   0        0        0     5761 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/noosphere_basalt.png
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/noosphere_gate.png
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/pseudoamethyst_block.png
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/raycast_blocker.png
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/raycast_blocker_glass.png
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_sensor.png
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_trap_powered.png
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_trap_unpowered.png
--rw-r--r--   0        0        0     6355 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/super_budding.png
--rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/thought_slurry.png
--rw-r--r--   0        0        0    10490 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/thought_slurry_flowing.png
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/wisp_lantern.png
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/wisp_lantern_tinted.png
--rw-r--r--   0        0        0   117562 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/book/slipway_hint_image.png
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/echo_staff.png
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/endless_phial.png
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_echo.png
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_flame.png
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_noosphere.png
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pseudoamethyst_shard.png
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod.png
--rw-r--r--   0        0        0     7011 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod_castloop.png
--rw-r--r--   0        0        0     5376 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod_filled.png
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/sentinel_trap_item.png
--rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/spoon_staff.png
--rw-r--r--   0        0        0     5436 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/thought_slurry_bucket.png
--rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/wisp_lantern.png
--rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/wisp_lantern_tinted.png
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/mob_effect/detection_resistance.png
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/book.json
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/basics/slipway_hint.json
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/noosphere_main.json
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/noosphere_materials.json
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/sentinel_detection.json
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/super_budding.json
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/items/mindrender.json
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/items/raycast_assailant.json
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/items/reverberation_rod.json
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/items/wisp_lantern.json
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/dim_iotas.json
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/frame_patterns.json
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/idea_inscription.json
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/status_iotas.json
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/paint_conjured.json
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/particle_burst.json
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/detection_shielding.json
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/dim_teleport.json
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/infuse_media.json
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/swap_space.json
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/echo_staff.json
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/endless_phial.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/raycast_blocker.json
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/raycast_blocker_glass.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/reverberation_rod.json
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/sentinel_sensor.json
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/sentinel_trap.json
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/super_budding.json
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/wisp_lantern.json
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/wisp_lantern_tinted.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_templates/__init__.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/LICENSE
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/pyproject.toml
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/doc/README.md
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.2.2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/gradle.properties
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/__gradle_version__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/__version__.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_hooks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/py.typed
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/__init__.py
+-rw-r--r--   0        0        0    15700 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/oneironaut.hexdoc.json
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/oneironaut.patterns.hexdoc.json
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/hexcasting/lang/en_us.flatten.json5
+-rw-r--r--   0        0        0    43280 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/lang/en_us.json
+-rw-r--r--   0        0        0    64897 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/lang/zh_cn.json
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/cell.json
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/circle.json
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/hex_resistant_block.json
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/media_gel.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/media_ice.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/noosphere_basalt.json
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/pseudoamethyst_block.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/raycast_blocker.json
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/raycast_blocker_glass.json
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/sentinel_sensor.json
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/sentinel_trap_powered.json
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/super_budding.json
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/beacon_staff.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/cell.json
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/circle.json
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/echo_staff.json
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/endless_phial.json
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/hex_resistant_block.json
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/media_gel.json
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/media_ice.json
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/memory_fragment.json
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/noosphere_basalt.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/pigment_echo.json
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/pigment_flame.json
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/pigment_noosphere.json
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/pseudoamethyst_block.json
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/pseudoamethyst_shard.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/raycast_blocker.json
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/raycast_blocker_glass.json
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/reverberation_rod.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/reverberation_rod_casting.json
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/reverberation_rod_filled.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/sentinel_sensor.json
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/sentinel_trap.json
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/spoon_staff.json
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/super_budding.json
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/thought_slurry_bucket.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/wisp_lantern.json
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/wisp_lantern_tinted.json
+-rw-r--r--   0        0        0     9564 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/black_circle.png
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/hex_resistant_block.png
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/media_gel.png
+-rw-r--r--   0        0        0     5798 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/media_gel_energized.png
+-rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/media_ice.png
+-rw-r--r--   0        0        0     5761 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/noosphere_basalt.png
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/noosphere_gate.png
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/pseudoamethyst_block.png
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/raycast_blocker.png
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/raycast_blocker_glass.png
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_sensor.png
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_trap_powered.png
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_trap_unpowered.png
+-rw-r--r--   0        0        0     6355 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/super_budding.png
+-rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/thought_slurry.png
+-rw-r--r--   0        0        0    10490 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/thought_slurry_flowing.png
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/wisp_lantern.png
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/wisp_lantern_tinted.png
+-rw-r--r--   0        0        0   117562 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/book/slipway_hint_image.png
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/beacon_staff.png
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/echo_staff.png
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/endless_phial.png
+-rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/memory_fragment.png
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_echo.png
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_flame.png
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_noosphere.png
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pseudoamethyst_shard.png
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod.png
+-rw-r--r--   0        0        0     7011 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod_castloop.png
+-rw-r--r--   0        0        0     5376 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod_filled.png
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/sentinel_trap_item.png
+-rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/spoon_staff.png
+-rw-r--r--   0        0        0     5436 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/thought_slurry_bucket.png
+-rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/wisp_lantern.png
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/wisp_lantern_tinted.png
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/mob_effect/detection_resistance.png
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/mob_effect/not_missing.png
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/book.json
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/basics/slipway_hint.json
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/noosphere_main.json
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/noosphere_materials.json
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/sentinel_detection.json
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/super_budding.json
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/items/mindrender.json
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/items/raycast_assailant.json
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/items/reverberation_rod.json
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/items/wisp_lantern.json
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/science1.json
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/science2.json
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/science3.json
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/treatise1.json
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/treatise2.json
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/treatise3.json
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/lore/treatise4.json
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/dim_iotas.json
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/idea_inscription.json
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/misc_patterns.json
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/soulprints.json
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/status_iotas.json
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/paint_conjured.json
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/particle_burst.json
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/detection_shielding.json
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/dim_teleport.json
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/glow_ambit.json
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/infusemedia.json
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/swap_space.json
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/echo_staff.json
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/endless_phial.json
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/hex_resistant_block.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/raycast_blocker.json
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/raycast_blocker_glass.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/reverberation_rod.json
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/sentinel_sensor.json
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/sentinel_trap.json
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/super_budding.json
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/wisp_lantern.json
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/recipes/wisp_lantern_tinted.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_templates/__init__.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/LICENSE
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/doc/README.md
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 hexdoc_oneironaut-0.3.0.1.0/PKG-INFO
```

### Comparing `hexdoc_oneironaut-0.2.2.1.0/gradle.properties` & `hexdoc_oneironaut-0.3.0.1.0/gradle.properties`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 kotlin.stdlib.default.dependency=false
 
 # needed for mixins to work for forge
 asmVersion=9.4
 
 # mod info
 modID=oneironaut
-modVersion=0.2.2
+modVersion=0.3.0
 mavenGroup=net.oneironaut
 
 # publishing
 curseforgeId=
 modrinthId=
 
 # core
@@ -37,8 +37,9 @@
 serializationHooksVersion=0.3.24
 entityReachVersion=2.3.0
 trinketsVersion=3.4.1
 hexalVersion=0.2.18
 gloopVersion=0.2.0
 
 wnboiVersion=0.0.4
-geckolibVersion=3.1.40
+geckolibVersion=3.1.40
+cca_version = 5.0.2
```

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/__gradle_version__.py` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/__gradle_version__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # This file is auto-generated by hatch-gradle-version. Do not edit.
 
-GRADLE_VERSION = "0.2.2"
-FULL_VERSION = "0.2.2.1.0"
+GRADLE_VERSION = "0.3.0"
+FULL_VERSION = "0.3.0.1.0"
 
 ARCHITECTURY_VERSION = "6.5.85"
 ASM_VERSION = "9.4"
 CARDINAL_COMPONENTS_VERSION = "5.0.2"
+CCA_VERSION = "5.0.2"
 CURSEFORGE_ID = ""
 ENABLED_PLATFORMS = "fabric,forge"
 ENTITY_REACH_VERSION = "2.3.0"
 FABRIC_API_VERSION = "0.77.0+1.19.2"
 FABRIC_KOTLIN_VERSION = "1.9.0+kotlin.1.8.0"
 FABRIC_LOADER_VERSION = "0.15.0"
 FORGE_KOTLIN_VERSION = "3.12.0"
@@ -20,15 +21,15 @@
 HEXCASTING_VERSION = "0.10.3"
 JETBRAINS_ANNOTATIONS_VERSION = "23.0.0"
 KOTLIN_STDLIB_DEFAULT_DEPENDENCY = "false"
 MAVEN_GROUP = "net.oneironaut"
 MINECRAFT_VERSION = "1.19.2"
 MIXIN_EXTRAS_VERSION = "0.2.0-beta.9"
 MOD_I_D = "oneironaut"
-MOD_VERSION = "0.2.2"
+MOD_VERSION = "0.3.0"
 MODRINTH_ID = ""
 ORG_GRADLE_JVMARGS = "-Xmx2048M"
 PATCHOULI_VERSION = "77"
 PAUCAL_VERSION = "0.5.0"
 SERIALIZATION_HOOKS_VERSION = "0.3.24"
 TRINKETS_VERSION = "3.4.1"
 WNBOI_VERSION = "0.0.4"
```

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_hooks.py` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_hooks.py`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/oneironaut.hexdoc.json` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/oneironaut.hexdoc.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5947145061728395%*

 * *Differences: {"'asset_url'": "'https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a'",*

 * * "'book_url'": "'https://oneironaut.hexxy.media/v/0.3.0/1.0/en_us'",*

 * * "'textures'": "{'PNGTexture': {'oneironaut:textures/book/slipway_hint_image.png': {'url': "*

 * *               "'https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/book/slipway_hint_image.png'}, "*

 * *               "'oneironaut: […]*

```diff
@@ -1,256 +1,344 @@
 {
-    "asset_url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858",
-    "book_url": "https://oneironaut.hexxy.media/v/0.2.2/1.0/en_us",
+    "asset_url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a",
+    "book_url": "https://oneironaut.hexxy.media/v/0.3.0/1.0/en_us",
     "textures": {
+        "AnimatedTexture": {
+            "oneironaut:textures/block/thought_slurry.png": {
+                "css_class": "texture-oneironaut-textures-block-thought_slurry-png",
+                "meta": {
+                    "animation": {
+                        "frametime": 2
+                    }
+                },
+                "pixelated": true,
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/block/thought_slurry.png"
+            },
+            "oneironaut:textures/block/thought_slurry_flowing.png": {
+                "css_class": "texture-oneironaut-textures-block-thought_slurry_flowing-png",
+                "meta": {
+                    "animation": {}
+                },
+                "pixelated": true,
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/block/thought_slurry_flowing.png"
+            },
+            "oneironaut:textures/item/memory_fragment.png": {
+                "css_class": "texture-oneironaut-textures-item-memory_fragment-png",
+                "meta": {
+                    "animation": {
+                        "frametime": 2
+                    }
+                },
+                "pixelated": true,
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/memory_fragment.png"
+            }
+        },
         "PNGTexture": {
             "oneironaut:textures/block/black_circle.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/block/black_circle.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/block/black_circle.png"
+            },
+            "oneironaut:textures/block/hex_resistant_block.png": {
+                "pixelated": true,
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/block/hex_resistant_block.png"
+            },
+            "oneironaut:textures/block/media_gel.png": {
+                "pixelated": true,
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/block/media_gel.png"
+            },
+            "oneironaut:textures/block/media_gel_energized.png": {
+                "pixelated": true,
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/block/media_gel_energized.png"
+            },
+            "oneironaut:textures/block/media_ice.png": {
+                "pixelated": true,
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/block/media_ice.png"
             },
             "oneironaut:textures/block/noosphere_basalt.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/block/noosphere_basalt.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/block/noosphere_basalt.png"
             },
             "oneironaut:textures/block/noosphere_gate.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/block/noosphere_gate.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/block/noosphere_gate.png"
             },
             "oneironaut:textures/block/pseudoamethyst_block.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/block/pseudoamethyst_block.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/block/pseudoamethyst_block.png"
             },
             "oneironaut:textures/block/raycast_blocker.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/block/raycast_blocker.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/block/raycast_blocker.png"
             },
             "oneironaut:textures/block/raycast_blocker_glass.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/block/raycast_blocker_glass.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/block/raycast_blocker_glass.png"
             },
             "oneironaut:textures/block/sentinel_sensor.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/block/sentinel_sensor.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/block/sentinel_sensor.png"
             },
             "oneironaut:textures/block/sentinel_trap_powered.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/block/sentinel_trap_powered.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/block/sentinel_trap_powered.png"
             },
             "oneironaut:textures/block/sentinel_trap_unpowered.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/block/sentinel_trap_unpowered.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/block/sentinel_trap_unpowered.png"
             },
             "oneironaut:textures/block/super_budding.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/block/super_budding.png"
-            },
-            "oneironaut:textures/block/thought_slurry.png": {
-                "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/block/thought_slurry.png"
-            },
-            "oneironaut:textures/block/thought_slurry_flowing.png": {
-                "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/block/thought_slurry_flowing.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/block/super_budding.png"
             },
             "oneironaut:textures/block/wisp_lantern.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/block/wisp_lantern.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/block/wisp_lantern.png"
             },
             "oneironaut:textures/block/wisp_lantern_tinted.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/block/wisp_lantern_tinted.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/block/wisp_lantern_tinted.png"
             },
             "oneironaut:textures/book/slipway_hint_image.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/book/slipway_hint_image.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/book/slipway_hint_image.png"
+            },
+            "oneironaut:textures/item/beacon_staff.png": {
+                "pixelated": true,
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/beacon_staff.png"
             },
             "oneironaut:textures/item/echo_staff.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/echo_staff.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/echo_staff.png"
             },
             "oneironaut:textures/item/endless_phial.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/endless_phial.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/endless_phial.png"
             },
             "oneironaut:textures/item/pigment_echo.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/pigment_echo.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/pigment_echo.png"
             },
             "oneironaut:textures/item/pigment_flame.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/pigment_flame.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/pigment_flame.png"
             },
             "oneironaut:textures/item/pigment_noosphere.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/pigment_noosphere.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/pigment_noosphere.png"
             },
             "oneironaut:textures/item/pseudoamethyst_shard.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/pseudoamethyst_shard.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/pseudoamethyst_shard.png"
             },
             "oneironaut:textures/item/reverberation_rod.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/reverberation_rod.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/reverberation_rod.png"
             },
             "oneironaut:textures/item/reverberation_rod_castloop.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/reverberation_rod_castloop.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/reverberation_rod_castloop.png"
             },
             "oneironaut:textures/item/reverberation_rod_filled.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/reverberation_rod_filled.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/reverberation_rod_filled.png"
             },
             "oneironaut:textures/item/sentinel_trap_item.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/sentinel_trap_item.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/sentinel_trap_item.png"
             },
             "oneironaut:textures/item/spoon_staff.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/spoon_staff.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/spoon_staff.png"
             },
             "oneironaut:textures/item/thought_slurry_bucket.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/thought_slurry_bucket.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/thought_slurry_bucket.png"
             },
             "oneironaut:textures/item/wisp_lantern.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/wisp_lantern.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/wisp_lantern.png"
             },
             "oneironaut:textures/item/wisp_lantern_tinted.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/wisp_lantern_tinted.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/wisp_lantern_tinted.png"
             },
             "oneironaut:textures/mob_effect/detection_resistance.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/mob_effect/detection_resistance.png"
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/mob_effect/detection_resistance.png"
+            },
+            "oneironaut:textures/mob_effect/not_missing.png": {
+                "pixelated": true,
+                "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/mob_effect/not_missing.png"
             }
         },
         "SingleItemTexture": {
+            "oneironaut:beacon_staff": {
+                "inner": {
+                    "pixelated": true,
+                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/beacon_staff.png"
+                }
+            },
+            "oneironaut:cell": {
+                "inner": {
+                    "pixelated": false,
+                    "url": "https://oneironaut.hexxy.media/v/0.3.0/1.0/assets/oneironaut/textures/block/cell.png"
+                }
+            },
             "oneironaut:circle": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://oneironaut.hexxy.media/v/0.2.2/1.0/assets/oneironaut/textures/block/circle.png"
+                    "url": "https://oneironaut.hexxy.media/v/0.3.0/1.0/assets/oneironaut/textures/block/circle.png"
                 }
             },
             "oneironaut:echo_staff": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/echo_staff.png"
+                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/echo_staff.png"
                 }
             },
             "oneironaut:endless_phial": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/endless_phial.png"
+                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/endless_phial.png"
+                }
+            },
+            "oneironaut:hex_resistant_block": {
+                "inner": {
+                    "pixelated": false,
+                    "url": "https://oneironaut.hexxy.media/v/0.3.0/1.0/assets/oneironaut/textures/block/hex_resistant_block.png"
+                }
+            },
+            "oneironaut:media_gel": {
+                "inner": {
+                    "pixelated": false,
+                    "url": "https://oneironaut.hexxy.media/v/0.3.0/1.0/assets/oneironaut/textures/block/media_gel.png"
+                }
+            },
+            "oneironaut:media_ice": {
+                "inner": {
+                    "pixelated": false,
+                    "url": "https://oneironaut.hexxy.media/v/0.3.0/1.0/assets/oneironaut/textures/block/media_ice.png"
+                }
+            },
+            "oneironaut:memory_fragment": {
+                "inner": {
+                    "css_class": "texture-oneironaut-textures-item-memory_fragment-png",
+                    "meta": {
+                        "animation": {
+                            "frametime": 2
+                        }
+                    },
+                    "pixelated": true,
+                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/memory_fragment.png"
                 }
             },
             "oneironaut:noosphere_basalt": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://oneironaut.hexxy.media/v/0.2.2/1.0/assets/oneironaut/textures/block/noosphere_basalt.png"
+                    "url": "https://oneironaut.hexxy.media/v/0.3.0/1.0/assets/oneironaut/textures/block/noosphere_basalt.png"
                 }
             },
             "oneironaut:pigment_echo": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/pigment_echo.png"
+                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/pigment_echo.png"
                 }
             },
             "oneironaut:pigment_flame": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/pigment_flame.png"
+                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/pigment_flame.png"
                 }
             },
             "oneironaut:pigment_noosphere": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/pigment_noosphere.png"
+                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/pigment_noosphere.png"
                 }
             },
             "oneironaut:pseudoamethyst_block": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://oneironaut.hexxy.media/v/0.2.2/1.0/assets/oneironaut/textures/block/pseudoamethyst_block.png"
+                    "url": "https://oneironaut.hexxy.media/v/0.3.0/1.0/assets/oneironaut/textures/block/pseudoamethyst_block.png"
                 }
             },
             "oneironaut:pseudoamethyst_shard": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/pseudoamethyst_shard.png"
+                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/pseudoamethyst_shard.png"
                 }
             },
             "oneironaut:raycast_blocker": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://oneironaut.hexxy.media/v/0.2.2/1.0/assets/oneironaut/textures/block/raycast_blocker.png"
+                    "url": "https://oneironaut.hexxy.media/v/0.3.0/1.0/assets/oneironaut/textures/block/raycast_blocker.png"
                 }
             },
             "oneironaut:raycast_blocker_glass": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://oneironaut.hexxy.media/v/0.2.2/1.0/assets/oneironaut/textures/block/raycast_blocker_glass.png"
+                    "url": "https://oneironaut.hexxy.media/v/0.3.0/1.0/assets/oneironaut/textures/block/raycast_blocker_glass.png"
                 }
             },
             "oneironaut:reverberation_rod": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/reverberation_rod.png"
+                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/reverberation_rod.png"
                 }
             },
             "oneironaut:reverberation_rod_casting": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/reverberation_rod_castloop.png"
+                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/reverberation_rod_castloop.png"
                 }
             },
             "oneironaut:reverberation_rod_filled": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/reverberation_rod_filled.png"
+                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/reverberation_rod_filled.png"
                 }
             },
             "oneironaut:sentinel_sensor": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://oneironaut.hexxy.media/v/0.2.2/1.0/assets/oneironaut/textures/block/sentinel_sensor.png"
+                    "url": "https://oneironaut.hexxy.media/v/0.3.0/1.0/assets/oneironaut/textures/block/sentinel_sensor.png"
                 }
             },
             "oneironaut:sentinel_trap": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://oneironaut.hexxy.media/v/0.2.2/1.0/assets/oneironaut/textures/block/sentinel_trap.png"
+                    "url": "https://oneironaut.hexxy.media/v/0.3.0/1.0/assets/oneironaut/textures/block/sentinel_trap_powered.png"
                 }
             },
             "oneironaut:spoon_staff": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/spoon_staff.png"
+                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/spoon_staff.png"
                 }
             },
             "oneironaut:super_budding": {
                 "inner": {
                     "pixelated": false,
-                    "url": "https://oneironaut.hexxy.media/v/0.2.2/1.0/assets/oneironaut/textures/block/super_budding.png"
+                    "url": "https://oneironaut.hexxy.media/v/0.3.0/1.0/assets/oneironaut/textures/block/super_budding.png"
                 }
             },
             "oneironaut:thought_slurry_bucket": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/thought_slurry_bucket.png"
+                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/thought_slurry_bucket.png"
                 }
             },
             "oneironaut:wisp_lantern": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/wisp_lantern.png"
+                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/wisp_lantern.png"
                 }
             },
             "oneironaut:wisp_lantern_tinted": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/eae2e84812db7d4698c1dc14d7206d539f643858/common/src/main/resources/assets/oneironaut/textures/item/wisp_lantern_tinted.png"
+                    "url": "https://raw.githubusercontent.com/beholderface/oneironaut/e572d229a3fa4737552640a9a8f4c66d8302267a/common/src/main/resources/assets/oneironaut/textures/item/wisp_lantern_tinted.png"
                 }
             }
         }
     }
 }
```

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/oneironaut.patterns.hexdoc.json` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/oneironaut.patterns.hexdoc.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8953488372093024%*

 * *Differences: {"'patterns'": "{insert: [(5, OrderedDict([('startdir', 'NORTH_EAST'), ('signature', "*

 * *               "'qeeweeewddw'), ('id', 'oneironaut:readrodram')])), (6, OrderedDict([('startdir', "*

 * *               "'NORTH_WEST'), ('signature', 'eqqwqqqwaaw'), ('id', 'oneironaut:writerodram')])), "*

 * *               "(20, OrderedDict([('startdir', 'EAST'), ('signature', 'wqded'), ('id', "*

 * *               "'oneironaut:filteredentityraycast')])), (21, OrderedDict([('startdir', "*

 * *               "'NORTH_EAST'), ('signature', 'e […]*

```diff
@@ -22,14 +22,24 @@
         },
         {
             "id": "oneironaut:getrodstamp",
             "signature": "qwqqqwqawaaw",
             "startdir": "SOUTH_EAST"
         },
         {
+            "id": "oneironaut:readrodram",
+            "signature": "qeeweeewddw",
+            "startdir": "NORTH_EAST"
+        },
+        {
+            "id": "oneironaut:writerodram",
+            "signature": "eqqwqqqwaaw",
+            "startdir": "NORTH_WEST"
+        },
+        {
             "id": "oneironaut:readframerotation",
             "signature": "wwawwqwwawwaeae",
             "startdir": "SOUTH_WEST"
         },
         {
             "id": "oneironaut:readidea",
             "signature": "qwqwqwqwqwqqqwedewq",
@@ -87,14 +97,24 @@
         },
         {
             "id": "oneironaut:getbystatussingle",
             "signature": "eaeeeeeae",
             "startdir": "EAST"
         },
         {
+            "id": "oneironaut:filteredentityraycast",
+            "signature": "wqded",
+            "startdir": "EAST"
+        },
+        {
+            "id": "oneironaut:gaussianrand",
+            "signature": "eeeeq",
+            "startdir": "NORTH_EAST"
+        },
+        {
             "id": "oneironaut:paintconjured",
             "signature": "eqdweeqdwweeqddqdwwwdeww",
             "startdir": "WEST"
         },
         {
             "id": "oneironaut:particleburst",
             "signature": "deeeewaaddwqqqqa",
@@ -122,24 +142,44 @@
         },
         {
             "id": "oneironaut:writeidea",
             "signature": "eweweweweweeewqaqwe",
             "startdir": "EAST"
         },
         {
+            "id": "oneironaut:getsoulprint",
+            "signature": "qqaqwedee",
+            "startdir": "EAST"
+        },
+        {
+            "id": "oneironaut:signitem",
+            "signature": "qqaqwedeea",
+            "startdir": "EAST"
+        },
+        {
+            "id": "oneironaut:checksignature",
+            "signature": "qqaqwedeed",
+            "startdir": "EAST"
+        },
+        {
             "id": "oneironaut:circle",
             "signature": "wwwwwwqwwwwwwqwwwwwwqwwwwwwqwwwwwwqwwwwww",
             "startdir": "SOUTH_EAST"
         },
         {
             "id": "oneironaut:removestatus",
             "signature": "eeeeedaqdewed",
             "startdir": "SOUTH_WEST"
         },
         {
+            "id": "oneironaut:advanceautomaton",
+            "signature": "qqwqwqwaqeee",
+            "startdir": "SOUTH_WEST"
+        },
+        {
             "id": "oneironaut:craftrod",
             "signature": "eqqqqqawweqqqqqawweqqqqqawwdeqewwwwweqeeeqewwwwweqe",
             "startdir": "EAST"
         },
         {
             "id": "oneironaut:dimteleport",
             "is_per_world": true,
@@ -167,14 +207,20 @@
         {
             "id": "oneironaut:invisibility",
             "is_per_world": true,
             "signature": "qqqqqaewawaweqa",
             "startdir": "SOUTH_WEST"
         },
         {
+            "id": "oneironaut:applynotmissing",
+            "is_per_world": true,
+            "signature": "qdaeqeawaeqeadqqdeed",
+            "startdir": "SOUTH_WEST"
+        },
+        {
             "id": "oneironaut:applymindrender",
             "is_per_world": true,
             "signature": "qweqadeqadeqadqqqwdaqedaqedaqeqaqdwawdwawdwaqawdwawdwawddwwwwwqdeddw",
             "startdir": "EAST"
         }
     ]
 }
```

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/lang/en_us.json` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/lang/en_us.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.60431654676259%*

 * *Differences: {"'block.oneironaut.cell'": "'Dissonant Psyche'",*

 * * "'block.oneironaut.circle'": "'§0§oCircle'",*

 * * "'block.oneironaut.hex_resistant_block'": "'Hex-Warded Obsidian'",*

 * * "'block.oneironaut.media_gel'": "'Plasmodial Psyche'",*

 * * "'block.oneironaut.media_ice'": "'Sagely Ice'",*

 * * "'effect.oneironaut.not_missing'": "'Uplifting Resonance'",*

 * * "'hexcasting.iota.oneironaut:uuid'": "'Soulprint'",*

 * * "'hexcasting.iota.oneironaut:uuid.label'": "'Soulprint of %s'",*

 * * "'hexcasting.mishap.invalid_value.class.oneironaut:imprint'": " […]*

```diff
@@ -1,142 +1,227 @@
 {
     "biome.oneironaut.noosphere_sea": "Noosphere Sea",
-    "block.oneironaut.circle": "Circle",
+    "block.oneironaut.cell": "Dissonant Psyche",
+    "block.oneironaut.circle": "\u00a70\u00a7oCircle",
+    "block.oneironaut.hex_resistant_block": "Hex-Warded Obsidian",
+    "block.oneironaut.media_gel": "Plasmodial Psyche",
+    "block.oneironaut.media_ice": "Sagely Ice",
     "block.oneironaut.noosphere_basalt": "Noosphere Basalt",
     "block.oneironaut.pseudoamethyst_block": "Pseudoamethyst Block",
     "block.oneironaut.raycast_blocker": "Anti-Raycast Slate",
     "block.oneironaut.raycast_blocker_glass": "Anti-Raycast Glass",
     "block.oneironaut.sentinel_sensor": "Sentinel Sensor",
     "block.oneironaut.sentinel_trap": "Seer Impetus",
     "block.oneironaut.super_budding": "Budding Pseudoamethyst",
     "block.oneironaut.thought_slurry": "Thought Slurry",
     "block.oneironaut.thought_slurry_flowing": "Flowing Thought Slurry",
     "block.oneironaut.wisp_lantern": "Wisp Lantern",
     "block.oneironaut.wisp_lantern_tinted": "Tinted Wisp Lantern",
     "effect.oneironaut.detection_resistance": "Media Shroud",
     "effect.oneironaut.missing": "Broken Potion Iota",
+    "effect.oneironaut.not_missing": "Uplifting Resonance",
     "enchantment.oneironaut.overcast_damage": "Mind Render",
     "fluid.oneironaut.thought_slurry": "Thought Slurry",
     "hexcasting.iota.oneironaut:dim": "Dimension",
     "hexcasting.iota.oneironaut:potion": "Status Effect",
+    "hexcasting.iota.oneironaut:uuid": "Soulprint",
+    "hexcasting.iota.oneironaut:uuid.label": "Soulprint of %s",
+    "hexcasting.mishap.invalid_value.class.oneironaut:imprint": "a spatial imprint",
+    "hexcasting.mishap.invalid_value.class.oneironaut:soulprint": "a soulprint",
+    "hexcasting.mishap.invalid_value.class.oneironaut:status": "a status effect",
+    "hexcasting.mishap.invalid_value.class.oneironaut:visiblestatus": "a detectable status effect",
     "hexcasting.mishap.oneironaut:mismatchcubes": "Supplied cuboids are dissimilar.",
     "hexcasting.mishap.oneironaut:missingeffect": "Expected %s to be affected by %s, but they are not.",
     "hexcasting.mishap.oneironaut:missingenchant": "Expected %s to be enchanted with %s, but it is not.",
     "hexcasting.mishap.oneironaut:nonconjured": "Expected a conjured block at %s, but got %s.",
     "hexcasting.mishap.oneironaut:nonoosphere": "Expected one end of the transfer to be a special dimension.",
+    "hexcasting.mishap.oneironaut:norequirediota": "The slime demands %s",
     "hexcasting.mishap.oneironaut:norod": "Expected a Reverberation Rod in hand.",
+    "hexcasting.mishap.oneironaut:nostaff": "%s expected to be cast using a staff.",
+    "hexcasting.mishap.oneironaut:requiresdifferententities": "an entity different from the target",
+    "hexcasting.mishap.oneironaut:unhappyslime": "The slime says \"%s\"",
     "hexcasting.mishap.oneironaut:uninfusable": "Expected an infusable block at %s, but got %s.",
+    "hexcasting.spell.oneironaut:advanceautomaton": "Cellular Generation",
     "hexcasting.spell.oneironaut:applymindrender": "Empower Mind Render",
+    "hexcasting.spell.oneironaut:applynotmissing": "Uplifting Resonance",
+    "hexcasting.spell.oneironaut:checksignature": "Signature Purification",
     "hexcasting.spell.oneironaut:circle": "Circle",
     "hexcasting.spell.oneironaut:craftrod": "Conduct Rod",
     "hexcasting.spell.oneironaut:delayrod": "Metronome Gambit",
     "hexcasting.spell.oneironaut:detectshroud": "Discern Shroud",
     "hexcasting.spell.oneironaut:dimteleport": "Noetic Gateway",
-    "hexcasting.spell.oneironaut:dimteleport.comingsoon": "This will do something interesting eventually.",
     "hexcasting.spell.oneironaut:dimteleport.samedim": "The spell does not do anything, similar to if I told someone to go home, when they were already at home.",
+    "hexcasting.spell.oneironaut:filteredentityraycast": "Scout's Exaltation",
+    "hexcasting.spell.oneironaut:gaussianrand": "Entropy Reflection II",
     "hexcasting.spell.oneironaut:getbystatus": "Zone Exltn.: Status",
     "hexcasting.spell.oneironaut:getbystatusinverse": "Zone Exltn.: Not-Status",
     "hexcasting.spell.oneironaut:getbystatussingle": "Entity Distillation: Status",
     "hexcasting.spell.oneironaut:getdim1": "Spatial Reflection",
     "hexcasting.spell.oneironaut:getdim2": "Spatial Reflection II",
     "hexcasting.spell.oneironaut:getrodlook": "Baton Reflection",
     "hexcasting.spell.oneironaut:getrodpos": "Baton Reflection II",
     "hexcasting.spell.oneironaut:getrodstamp": "Metronome Reflection",
+    "hexcasting.spell.oneironaut:getsoulprint": "Soulprint Reflection",
     "hexcasting.spell.oneironaut:getstatus": "Apothecary's Prfn.",
     "hexcasting.spell.oneironaut:getstatuscategory": "Apothecary's Prfn. II",
     "hexcasting.spell.oneironaut:getstatusduration": "Pharmacist's Dstln.",
     "hexcasting.spell.oneironaut:getstatuslevel": "Pharmacist's Dstln. II",
     "hexcasting.spell.oneironaut:haltrod": "Finale",
     "hexcasting.spell.oneironaut:infusemedia": "Media Infusion",
     "hexcasting.spell.oneironaut:invisibility": "Hidden Sun's Zenith",
     "hexcasting.spell.oneironaut:paintconjured": "Externalize Pigment",
     "hexcasting.spell.oneironaut:particleburst": "Particle Burst",
-    "hexcasting.spell.oneironaut:readframeitem": "Deprecator's Purification lmao get it?",
     "hexcasting.spell.oneironaut:readframerotation": "Decorator's Purification",
     "hexcasting.spell.oneironaut:readidea": "Retrieve Idea",
     "hexcasting.spell.oneironaut:readideatime": "Metadata Purification",
     "hexcasting.spell.oneironaut:readideawriter": "Metadata Distillation",
+    "hexcasting.spell.oneironaut:readrodram": "Williams' Reflection",
     "hexcasting.spell.oneironaut:readsentinel": "Scrutinize Sentinel",
     "hexcasting.spell.oneironaut:removestatus": "Cleanse Status",
     "hexcasting.spell.oneironaut:resetrod": "Encore",
     "hexcasting.spell.oneironaut:resistdetection": "Stealth Shroud",
     "hexcasting.spell.oneironaut:setframerotation": "Decorator's Gambit",
+    "hexcasting.spell.oneironaut:signitem": "Sign Item",
     "hexcasting.spell.oneironaut:swapspace": "Spatial Interchange",
     "hexcasting.spell.oneironaut:writeidea": "Inscribe Idea",
+    "hexcasting.spell.oneironaut:writerodram": "Williams' Gambit",
+    "item.oneironaut.beacon_staff": "Magitech Staff",
     "item.oneironaut.echo_staff": "Echo Staff",
     "item.oneironaut.endless_phial": "Inexhaustible Phial",
+    "item.oneironaut.memory_fragment": "Memory Fragment",
+    "item.oneironaut.memory_fragment.all": "It seems I've consumed all the memories that this crystal can offer me...",
     "item.oneironaut.pigment_echo": "Echo Pigment",
     "item.oneironaut.pigment_flame": "Flame Pigment",
     "item.oneironaut.pigment_noosphere": "Noetic Pigment",
     "item.oneironaut.pseudoamethyst_shard": "Pseudoamethyst Shard",
     "item.oneironaut.reverberation_rod": "Reverberation Rod",
     "item.oneironaut.spoon_staff": "Spoon",
     "item.oneironaut.thought_slurry_bucket": "Thought Slurry Bucket",
     "itemGroup.oneironaut.oneironaut": "Oneironaut",
+    "not.real.translation.key.1": "TODO: Add a structure that is implied to be part of a laboratory that has been ripped from the overworld by an engorged gateway",
+    "oneironaut.advancements.lore.root": "Oneironaut Lore",
+    "oneironaut.advancements.lore.root.description": "Memories lost to time",
+    "oneironaut.advancements.lore.science1": "Scientist's Memory #1",
+    "oneironaut.advancements.lore.science1.description": "Research into the nature of slipways",
+    "oneironaut.advancements.lore.science2": "Scientist's Memory #2",
+    "oneironaut.advancements.lore.science2.description": "Research into the properties of the Noosphere",
+    "oneironaut.advancements.lore.science3": "Scientist's Memory #3",
+    "oneironaut.advancements.lore.science3.description": "Research into the structure of pseudoamethyst",
+    "oneironaut.advancements.lore.treatise1": "Hexcaster's Memory #1",
+    "oneironaut.advancements.lore.treatise1.description": "Reflections on iota embedding",
+    "oneironaut.advancements.lore.treatise2": "Hexcaster's Memory #2",
+    "oneironaut.advancements.lore.treatise2.description": "Reflections on efficient use of Impulse",
+    "oneironaut.advancements.lore.treatise3": "Hexcaster's Memory #3",
+    "oneironaut.advancements.lore.treatise3.description": "Reflections on repeated patterns",
+    "oneironaut.advancements.lore.treatise4": "Hexcaster's Memory #4",
+    "oneironaut.advancements.lore.treatise4.description": "Reflections on long hexes",
     "oneironaut.advancements.noosphere.enter": "A Realm of Thought and Dream",
     "oneironaut.advancements.noosphere.enter.description": "Enter the Noosphere",
+    "oneironaut.advancements.noosphere.find_media_lab": "Crystallized",
+    "oneironaut.advancements.noosphere.find_media_lab.description": "Discover a grim experiment",
+    "oneironaut.advancements.noosphere.find_tower": "A Timeless Classic",
+    "oneironaut.advancements.noosphere.find_tower.description": "Discover the tower of an unknown hexcaster",
     "oneironaut.entry.detection_shielding": "Nondetection",
     "oneironaut.entry.dim_iotas": "Dimension Iotas",
-    "oneironaut.entry.framepatterns": "Item Frame Patterns",
     "oneironaut.entry.idea_inscription": "Idea Inscription",
     "oneironaut.entry.mindrender": "Mind Render",
+    "oneironaut.entry.miscpatterns": "Misc. Oneironaut Patterns",
     "oneironaut.entry.noosphere_main": "A Strange Realm",
     "oneironaut.entry.noosphere_materials": "Thoughtful Materials",
-    "oneironaut.entry.raycast_assailant": "Raycast Blocking",
+    "oneironaut.entry.raycast_assailant": "Anti-Hex Blocks",
     "oneironaut.entry.sentinel_detection": "Sentinel Detection",
     "oneironaut.entry.slipway_hint": "A Reflection on Slipways",
+    "oneironaut.entry.soulprints": "Soulprints",
     "oneironaut.entry.status_iotas": "Status Iotas",
     "oneironaut.entry.super_budding": "Better Media Farming",
     "oneironaut.entry.wisp_lanterns": "Wisp Lanterns",
     "oneironaut.mishap.badentitykey": "an enlightened player or a flayed villager",
+    "oneironaut.mishap.entitytypelistplease": "a list of entity types",
+    "oneironaut.mishap.invalidideakey": "a vector, player, or soulprint",
     "oneironaut.mishap.noitemframe": "an item frame",
+    "oneironaut.mishap.nolistsallowed": "a non-list iota",
     "oneironaut.mishap.notbrainswept": "a flayed villager",
-    "oneironaut.mishap.novecorentity": "a vector or player",
+    "oneironaut.mishap.twovectorsplease": "List does not contain two vectors.",
     "oneironaut.mishap.unenlightenedtarget": "an enlightened player",
+    "oneironaut.mishap.wrongsizelist": "List is improperly sized.",
     "oneironaut.page.detection_shielding.1": "While conventional invisibility potions work just fine for fooling human senses, they are useless against hexes, so I've yet to find any method of making oneself completely undetectable. However, this spell I've discovered allows me to get closer to that goal, scattering media around a creature like chaff, in order to interfere with hex-based detection methods.",
     "oneironaut.page.detection_shielding.2": "Accepts a living entity and a number ($(o)n$()), and shields the entity from hex-based detection for $(o)n$() seconds. Costs two amethyst dust per second.",
     "oneironaut.page.detection_shielding.3": "Also drains media from the entity at a rate of 1/10 of a dust per second, as the shielding effect collects it to produce the chaff.$(br2)I should be careful with what I apply this to, as creatures with no loose media of their own will have their very minds fractured in order to provide this media.",
     "oneironaut.page.detection_shielding.4": "While this is very effective at blocking effects such as $(l:patterns/basics#hexcasting:raycast/entity)Scout's Distillation$(/l) and the various forms of $(l:patterns/entities#hexcasting:zone_entity/animal)Zone Distillation$(/l), it has no effect on $(l:patterns/entities#hexcasting:get_entity)Entity Distillation$(/l) variants, as those already have a fairly precise idea of where you are. What's more, the chaff itself produces an energy signautre, which, while dim, is detectable by a specialized pattern.",
     "oneironaut.page.detection_shielding.5": "Accepts a vector and a number, and returns a list of unit vectors pointing from the initial vector to shrouded entities within a radius defined by the number.",
     "oneironaut.page.detection_shielding.6": "I've also discovered a spell which applies normal Invisibility. Functions just like the normal $(l:patterns/great_spells/zeniths)Zeniths$(/l), and costs one amethyst dust per three seconds.",
     "oneironaut.page.dim_iotas.1": "I've descovered a kind of iota which seems to represent a layer of reality itself. In lieu of better understanding, I've decided to call these Spatial Imprints.",
     "oneironaut.page.dim_iotas.2": "Returns a Spatial Imprint representing the dimension I am currently in. Costs a negligible amount of media.",
     "oneironaut.page.dim_iotas.3": "Returns a Spatial Imprint representing the dimension my sentinel is currently in. Costs a slightly-less-negligible amount of media.",
     "oneironaut.page.dimteleport.1": "Accepts an entity and a Spatial Imprint and teleports the entity to its position in the corresponding dimension. Costs 20 Charged Amethyst.",
     "oneironaut.page.dimteleport.2": "Also triggers some sort of safety net once the target reaches its destination, in case it arrives somewhere inherently dangerous.$(br2)Will fail if supplied a player other than myself.$(br2)I get a strange sense of acceleration when subjected to this spell, but somehow it isn't along any axis I can comprehend.",
-    "oneironaut.page.framepatterns.1": "I've found a few patterns designed to interact with item frames. Nothing fancy, but they're nice utility for things like controlling my spell circles.$(br2)Additionally, it seems Sorter's Purification works on them just fine, so my attempts to find a dedicated frame-item pattern were pointless.",
-    "oneironaut.page.framepatterns.1.formerlink": "$(l:hexal:patterns/types#hexal:type/block_item)",
-    "oneironaut.page.framepatterns.2": "Accepted an item frame entity, and returned the type of item contained within. This pattern doesn't exist anymore because I forgot to check if normal Sorter's Purification works on item frames, and it does,",
-    "oneironaut.page.framepatterns.3": "Accepts an item frame entity, and returns its rotation, from 0 to 7.",
-    "oneironaut.page.framepatterns.4": "Accepts an item frame entity and an integer from 0 to 7, and sets its rotation to the number. Costs a negligible amount of media.",
+    "oneironaut.page.glow_ambit.1": "Despite diligent research, the source of the special properties of other hexcasters' entity references has eluded me. However, I've discovered a way to bestow one such property upon other beings, at least temporarily (and flashily).$(br)This spell allows casters to affect creatures from great distances just like the infinite-range aspect of a player reference. However, one must still be close to the target in order to perform the initial application.",
+    "oneironaut.page.glow_ambit.2": "Accepts a living entity, and allows it to be accessed from anywhere for one minute. Has a base cost of one amethyst shard, plus one additional shard per application before allowing it to expire.",
+    "oneironaut.page.glow_ambit.3": "It seems that this effect functions by causing the target to emit some sort of psionic resonance, strong enough to cause its outline to be \"visible\" through all manner of barriers (perhaps hexcasters naturally produce this same resonance, but much subtler?). However, this glow is distinct from that induced by spectral arrows and similar, so don't bet on things to detect that working for this.",
     "oneironaut.page.idea_inscription.1": "As the noosphere is a realm of thought, it stands to reason that it could be used for information storage. These patterns do just that, inscribing an iota into the noosphere and reading it back (regardless of my current dimension). They can also store iotas inside the minds of other beings, assuming their thoughts are as... $(o)unfettered$() as my own. In the notation for these patterns, \"key\" refers to any vector or compatible entity.",
     "oneironaut.page.idea_inscription.2": "While this is quite versatile, the noosphere's ambient media is constantly in motion, and as such any iota stored in it will eventually be lost, similar to if I poured hot water into the ocean. It seems to take about an hour before such information decays into unusable garbage.$(br2)It seems that $(l:greatwork/akashiclib)Akashic Libraries$(/l) work based on similar principles, where the shelves serve as insulation to prevent decay.",
     "oneironaut.page.idea_inscription.3": "Accepts a valid key and any iota, and stores it in the corresponding location. Costs about 1 amethyst dust.",
     "oneironaut.page.idea_inscription.4": "Accepts a valid key, and returns the corresponding iota. Costs about 1 amethyst dust.",
     "oneironaut.page.idea_inscription.5": "Accepts a valid key, and returns when the corresponding iota was inscribed, or NULL. Costs a negligible amount of media.",
     "oneironaut.page.idea_inscription.6": "Accepts a valid key and a player, and returns whether the corresponding iota was inscribed by that player. Costs a negligible amount of media.",
     "oneironaut.page.infusemedia.1": "Accepts a vector and infuses media into the corresponding block in order to transmute it. Cost and exact effect vary depending on target.",
     "oneironaut.page.infusemedia.2": "Conceptually, this spell is quite similar to $(l:patterns/spells/blockworks#hexcasting:edify)Edify Sapling$(/l).$(br)However, the media that the target block receives is far more finely-tuned, and can thus achieve far more interesting results.",
+    "oneironaut.page.lore.science1.1": "$(o)\"What is this and how do I get rid of it?\"$()$(br)A question asked by many people upon their first encounter with a slipway. I don't have a good answer for the second part of the question, but I believe I can provide a satisfactory response to the first.$(br)From what I can tell, a slipway is a tiny hole in space, the other side of which is the media realm known as the Noosphere.",
+    "oneironaut.page.lore.science1.2": "The wisp-like phenomena that emerge from it are formed when the vast ambient media of the Noosphere attempts to rush through the hole (much like gas leaking into a near-vacuum) and gets tangled in a manner similar to how wisp-summoning spells weave the media which they consume.",
+    "oneironaut.page.lore.science1.3": "Additionally, it seems that slipways have a sort of barrier over the entrance, preventing any matter from passing through. If this barrier could be pierced, and the hole expanded, the slipway would become capable of absorbing matter into the noosphere. It would also cease producing wisps, as the media coming through would do so far more slowly, and thus not be agitated and tangled. If one were to attempt this, they would have to be careful not to widen it too greatly, or they would risk the surrounding area being absorbed into the noosphere.",
+    "oneironaut.page.lore.science2.1": "What a strange place. The liquid that comprises the ocean here is not much denser than water, but small islands float in it despite being comprised of a rock similar in density to ordinary basalt. What's more, everything seems strangely ephemeral, like a dream. But how could this be a dream, when I am more lucid than I've ever been before?",
+    "oneironaut.page.lore.science2.2": "It seems this great lucidity is a product of the ambient media present here, lubricating my thoughts. These media levels even exceed those present at the cores of wisps, reducing their innate decay to infinitesimal levels. Interestingly, this has no effect on wisps which bear an imprint of someone else's soul, preventing me from using wisps as indefinite truename storage.$(br)This ambient media even leaks through sufficiently-large dimensional rifts, preserving wisps on the other side as long as they remain within a certain range of the rift.",
+    "oneironaut.page.lore.science3.1": "This crystal is quite fascinating. An object formed from pure media, orders of magnitude denser than conventional conjured blocks, or even the condensed media crystals that some of my colleagues at the library have been studying. It doesn't even contain the trace amounts of silicon dioxide found in amethyst of similar media density. And when I leave it unattended for a while, dust collects in fractalline patterns, as if the crystal bears a passive spell-like effect.",
+    "oneironaut.page.lore.science3.2": "Examining it more thoroughly under a microscope, it seems that these fractals extend beneath the surface of the crystal, and are constantly shifting in a consistent pattern. Could this be a time crystal?",
+    "oneironaut.page.lore.treatise1.1": "While it is possible to produce most iotas on the fly, there are cases where one finds it impractical, or simply cannot (such as very large and precise numbers, or entity references), and as such must obtain the desired iota in another way. Reading it from a Focus or a similar item works just fine, but in many cases this would require a third hand, which I do not have. Other methods of fetching iotas from external locations have their own limitations as well.",
+    "oneironaut.page.lore.treatise1.2": "In cases where no external reference method would work well, one must insert the desired iota into the hex itself. This may seem counterintuive to some, what with the conventional wisdom being that a hex is a list of patterns, but one must remember that patterns are just another type of iota, which $(l:patterns/meta#hexcasting:eval)Hermes' Gambit$(/l) (and similar patterns) works particularly well with.",
+    "oneironaut.page.lore.treatise1.3": "While you can't just shove a number into the list and expect it to be pushed to the stack as if it was a $(l:patterns/numbers)Numerical Reflection$(/l) pattern, there are ways around this.$(br2)The simplest (and least reliable) is the $(l:patterns/patterns_as_iotas#hexcasting:escape)Consideration$(/l) pattern. Similar to its use when casting freehand, anything that comes immediately after it in a list will be escaped and pushed to the stack when it might otherwise be executed, preventing mishaps due to execution of non-patterns.",
+    "oneironaut.page.lore.treatise1.4": "However, when you're more than one exeuction deep in a hex (such as with nested conditional logic, or loops), the number of Considerations required to properly escape an iota increases exponentially, making it unreliable when used in anything that could conceivably be executed by another hex.",
+    "oneironaut.page.lore.treatise1.4.link": "relevant xkcd",
+    "oneironaut.page.lore.treatise1.5": "A far more reliable method of escaping iotas is to use $(l:patterns/patterns_as_iotas#hexcasting:open_paren)Introspection$(/l) and $(l:patterns/patterns_as_iotas#hexcasting:close_paren)Retrospection$(/l). When a pattern list is being evaluated and an Introspection is encountered, everything up to (but not including) its paired Retrospection is escaped and pushed to the stack in a list, regardless of iota type. You can then work with this list as you see fit, such as using $(l:patterns/lists#hexcasting:splat)Flock's Disintegration$(/l) to push all of its contents to the stack on their own.",
+    "oneironaut.page.lore.treatise1.6": "If the contents of your list looks like this:$(br2)Introspection$(br)Any iota(s)$(br)Retrospection$(br)Flock's Disintegration$(br2)the state of the stack after all that is executed will simply be all the iotas that were contained within Introspection and Retrospection.",
+    "oneironaut.page.lore.treatise2.1": "When one wishes to impart motion upon something, the standard method is to use $(l:patterns/spells/basic#hexcasting:add_motion)Impulse$(/l). However, this can get prohibitively expensive when one wishes to make something move extremely quickly, as the cost increases exponentially with the length of the vector. This can be mitigated by simply using a magnitude-1 Impulse many times over on a single target, turning the overall cost from n^2 to 2n-1, where n is the magnitude of the vector.",
+    "oneironaut.page.lore.treatise2.2": "The easiest way to accomplish this is with $(l:patterns/meta#hexcasting:for_each)Thoth's Gambit$(/l), by giving it a list containing many instances of the same entity reference. There are other (and often better) methods, of course, but aside from simply drawing the patterns over and over, they generally fall under the broader topic of loops, which is outside the scope of this document.",
+    "oneironaut.page.lore.treatise3.1": "While $(l:patterns/meta#hexcasting:for_each)Thoth's Gambit$(/l) is perfectly-suited for casting something on many targets at once, using to it cast something on one target many times can get awkward, and short of completely halting the hex, it is not possible to add or remove targets once Thoth has begun executing.$(br)To get around these limitations, one simply needs to use a different sort of loop.",
+    "oneironaut.page.lore.treatise3.2": "A While loop is a loop that continues executing until some condition is fulfilled, such as an entity's target velocity having been reached. The most common way to accomplish this is creating a pattern list which duplicates and executes the top iota on the stack, duplicating it, then executing it. On its own this simply produces an infinite loop which does nothing but mishap.",
+    "oneironaut.page.lore.treatise3.2.header": "While Loop",
+    "oneironaut.page.lore.treatise3.3": "However, by adding actual functionality and a bit of boolean logic, you can create a proper while loop. The code for the aforementioned infinite loop is as follows:$(br)Introspection$(br)Gemini Decomposition$(br)Hermes' Gambit$(br)Retrospection$(br)Gemini Decomposition$(br)Hermes' Gambit$(br2)By adding logic that changes whether the inner Hermes' Gambit gets evaluated based on a condition, you can make it stop once that condition is fulfilled.",
+    "oneironaut.page.lore.treatise3.4": "A more complex form of loop is an unrolled loop. Like Thoth's Gambit, it's created with a fixed number of iterations which can't easily be added to, but Charon's Gambit can be used to halt it early if need be. It also has the advantage that when done competently, it only ever produces one or two levels of recursion depth (not counting anything executed in the body of the loop). Loop unrolling is accomplished by creating a pattern list you want to repeat, duplicating it many times, and then combining all those lists into one.",
+    "oneironaut.page.lore.treatise3.4.header": "Loop Unrolling",
+    "oneironaut.page.lore.treatise3.5": "The simplest way to accomplish this is to use $(l:patterns/stackmanip#hexcasting:duplicate)Gemini Decomposition$(/l) and then $(l:patterns/lists#hexcasting:concat)Combination Distillation$(/l), resulting in a doubled pattern list. This method can be repeated to achieve greater powers of 2, and only produces a single level of recursion depth, when the list is executed. A more flexible method is to use $(l:patterns/stackmanip#hexcasting:duplicate_n)Gemini Gambit$(/l) to produce $(o)n$() copies of the list, then gathering $(o)n-1$() instances of the pattern for Combination Distillation into one list and executing it, thus merging all the copies of your original list into one.",
+    "oneironaut.page.lore.treatise4.1": "Some of my, erm, \"colleagues\" have trouble transcribing long hexes.$(br)\"This is too long!\"$(br)\"The grid doesn't have enough space!\"$(br)$(bold)Skill issue$(), I say. It's not like a hex is immutable once you've drawn the last Retrospection. All you need to do is save the work-in-progress hex to a focus (though you should make sure to conserve enough grid space to actually do this).",
+    "oneironaut.page.lore.treatise4.2": "Then you just use the $(l:patterns/lists)list manipulation$(/l) patterns to combine it with the other parts once you're done.$(br2)You don't even need to use multiple foci, you can just append one part to the last one as you finish them, and then save that to one focus. The multiple-focus method makes it easier to debug your finished hex, but as far as I know that's its only benefit compared to the one-focus method.",
     "oneironaut.page.mindrender.1": "I've read legends of a particularly macabre form of weapon known as a Mind Render. This weapon, sometimes used by ancient hexcasters, is capable of severing a creature's very thoughts, dealing damage that bypasses all known forms of protection. What's more, if this damage leaves the target just on the brink of true death, it will fall into a vegetative state, never to recover. I shudder to think of what the ancients may have used this property for...",
     "oneironaut.page.mindrender.2": "Accepts an item or item frame bearing the Sharpness enchantment, and converts it into Mind Render of the same level. Cost is based on enchantment level, and increases by 50%% if the item is a book.",
+    "oneironaut.page.miscpatterns.1": "I've found a couple patterns designed to interact with item frames. Nothing fancy, but they're nice utility for things like controlling my spell circles.$(br2)Additionally, it seems Sorter's Purification works on them just fine, so my attempts to find a dedicated frame-item pattern were pointless.",
+    "oneironaut.page.miscpatterns.1.formerlink": "$(l:hexal:patterns/types#hexal:type/block_item)",
+    "oneironaut.page.miscpatterns.2": "Accepts an item frame entity, and returns its rotation, from 0 to 7.",
+    "oneironaut.page.miscpatterns.3": "Accepts an item frame entity and an integer from 0 to 7, and sets its rotation to the number. Costs a negligible amount of media.",
+    "oneironaut.page.miscpatterns.4": "As $(l:patterns/basics#hexcasting:raycast/entity)Scout's Distillation$(/l), but also accepts a list of entity type iotas. Any entity whose type is not present in the list will be ignored. Costs an amount of media slightly less negligible than that of the aforementioned pattern.",
+    "oneironaut.page.miscpatterns.5": "Returns a random number between 0 and 1, with a gaussian distribution.",
     "oneironaut.page.noosphere_main.1": "I've made it.$(br)The realm beyond the slipways. The ambient media is overwhelming. My mind is screaming at me, telling me I shouldn't be here. But I must press on. This is the next step in the journey.",
     "oneironaut.page.noosphere_main.2": "Every single thing I've examined here seems to be composed largely of media, similar to conjured matter, but orders of magnitude denser.$(br)$(o)Even the air is media. How am I breathing?$(br2)$(l)How can I even exist here?",
     "oneironaut.page.noosphere_materials.1": "A strange fluid which agitates media entering it, preventing amethyst crystal formation. Stimulates my mind in pleasing ways when I immerse myself in it.",
     "oneironaut.page.noosphere_materials.2": "A rock which is primarily composed of media, somehow. Can be used to craft spell circle blocks.",
     "oneironaut.page.noosphere_materials.3": "A large crystal of media much like amethyst, but not quite the same. Produces a buzzing sensation under my fingers when I touch it, as if its media is stimulating the nerves. Breaking it without special care causes it to shatter into 1-4 pieces.",
     "oneironaut.page.noosphere_materials.3.title": "Pseudoamethyst",
     "oneironaut.page.noosphere_materials.4": "The shards can be used to fuel spells, and yield slightly more energy than a normal amethyst shard. Can also be used to craft several interesting things.",
+    "oneironaut.page.noosphere_materials.5": "A solid form of media which is created when Thought Slurry freezes in a media-rich environment, or is caused to freeze by a hex.$(br)Its surface seems to have negative friction, causing anything sliding on it to accelerate indefinitely (albeit slowly).",
+    "oneironaut.page.noosphere_materials.6": "An extremely viscous mass of media, capable of very basic cognition, analagous to a slime mold. While it is normally quite lethargic, it uses a spell-like ability to attempt to ensnare anything that touches it.",
     "oneironaut.page.paintconjured.1": "Accepts a vector and an itemtype representing a pigment. Costs a negligible amount of media if targeting my own block, or 1 Amethyst Dust if not.",
     "oneironaut.page.paintconjured.2": "Sets the colors of the conjured block corresponding to the vector to the colorset represented by the passed pigment, or mine if passed a NULL iota.$(br2)Not guaranteed to work with unconventional forms of conjured matter. ",
     "oneironaut.page.paintconjured.3": "Feels strangely celebratory, as if something similar was once used in grand festivals where teams would splatter their colors all over their opponents' territory in a bid for ideological dominance.",
     "oneironaut.page.particleburst.1": "Accepts two vectors and two numbers, and uses them to define a burst of particles. Costs a negligible amount of media.",
     "oneironaut.page.particleburst.2": "The first vector determines the burst's origin position, and the second vector determines its direction and speed. The first number determines the scale of random numbers added to each position component, and the second does the same for the direction vector.",
     "oneironaut.page.raycast_assailant.1": "By \"threading\" pseudoamethyst through a block, I can create something which causes any raycast (including entity raycasts) that hits or passes through it to return null, as if it didn't hit anything.",
+    "oneironaut.page.raycast_assailant.3": "Strangely, combining pseudoamethyst with obsidian in the same way does not confer anti-raycast properties, instead making it nigh-indestructible to hexes. However, the resultant block loses much of its durability, being no stronger than common stone (though it retains its blast resistance).",
     "oneironaut.page.rod.1": "I've discovered that I can craft a peculiar sort of casting item, using the strange shards found in ancient cities.$(br)This item is unusual in that it casts its imbued hex twenty times per second while I concentrate on it, until it either mishaps or I cast Finale or Encore. This initiates a cooldown period, usually about one second.",
-    "oneironaut.page.rod.10": "Echo shards can also be used in the construction of a staff, though it seems the only special property of such a staff is making sculk sounds.",
+    "oneironaut.page.rod.10": "Accepts a non-list iota, and stores it inside the current cast loop. It will be lost when the cast loop ends.",
+    "oneironaut.page.rod.11": "Returns the iota stored in the current cast loop. Defaults to NULL.",
+    "oneironaut.page.rod.12": "Echo shards can also be used in the construction of a staff, though it seems the only special property of such a staff is making sculk sounds.",
     "oneironaut.page.rod.2": "The echo shards seem to bear some bizarre form of media, with a tendency to loop back on itself while retaining a bit of the previous cast.",
     "oneironaut.page.rod.3": "Acts just like $(l:patterns/spells/hexcasting)the spells used to program conventional casting items$(). Costs 10 Charged Amethyst.",
     "oneironaut.page.rod.4": "When cast with a Reverberation Rod, returns my look vector from when I started the current cast loop.",
     "oneironaut.page.rod.5": "When cast with a Reverberation Rod, returns my eye position from when I started the current cast loop.",
     "oneironaut.page.rod.6": "When cast with a Reverberation Rod, returns the timestamp from when I started the current cast loop.",
     "oneironaut.page.rod.7": "Accepts a positive integer. When cast with a Reverberation Rod, delays the current cast loop's next cast until that many twentieths of a second have passed.",
     "oneironaut.page.rod.8": "When cast with a Reverberation Rod, forcibly halts the current cast loop.",
@@ -146,36 +231,39 @@
     "oneironaut.page.sentinel_detection.3": "Additionally, this sensor can be incorporated into a Cleric Impetus, allowing it to activate when a sentinel is placed in the area (albeit with a lower range than the plain sensor). I've dubbed this contraption a Seer Impetus. Though it no longer responds to redstone, the circle's hex will start with a reference to the owner of the triggering sentinel on the stack.$(br)Due to the media interference produced by the cast, the impetus cannot detect sentinels it places itself.",
     "oneironaut.page.sentinel_detection.4": "As the sensor does not care whose sentinel it sees, I should take care to avoid allowing my trap circles to target me.",
     "oneironaut.page.sentinel_detection.5": "Accepts a vector and a player, and returns either the distance from the vector to the target player's sentinel or NULL. Costs a negligible amount of media.",
     "oneironaut.page.sentinel_detection.6": "Conjures a fleeting sensor at the target coordinates, which \"listens\" to the patterns in the ambient media to seek out the telltale signature of a sentinel.",
     "oneironaut.page.slipway_hint.1": "The slipways, they must lead $(o)somewhere$(). Wisps do not simply manifest from nothing. No matter what I try, I cannot insert so much as a finger through that chaotic rift.$(br2)I'm going about this wrong. Perhaps rather than attempting to force my way through, I should be attempting to calm the storm.",
     "oneironaut.page.slipway_hint.2": "A large amount of harmonious media may just do it...",
     "oneironaut.page.slipway_hint.2.title": "Hmm...",
+    "oneironaut.page.soulprints.1": "A soulprint is an iota similar to my player reference in that it represents me, but significantly more limited in use. It is impossible for anyone to obtain my soulprint without my involvement, though it is not subject to the same write-restrictions as ordinary player references.$(br2)Interestingly, soulprints are valid keys for $(l:patterns/idea_inscription)Idea Inscription$(/l).",
+    "oneironaut.page.soulprints.2": "Returns my soulprint, mishapping if cast using anything other than a staff. Costs a negligible amount of media.",
+    "oneironaut.page.soulprints.3": "Invisibly engraves my soulprint onto the item in my other hand, or erases it if it is already there. Costs 1 amethyst dust.$(br)I should be careful to seal any focuses or similar that I sign, as acquiring an unsealed signed focus may allow someone to impersonate me, and Erase Item gets rid of the signature.",
+    "oneironaut.page.soulprints.4": "Accepts a soulprint, and checks if the item in my other hand is engraved with it. Returns true if so, false otherwise. Costs a negligible amount of media.",
     "oneironaut.page.spaceswap.1": "Accepts two lists of two vectors, to define two cuboids, and a Spatial Imprint. These cuboids must have the exact same dimensions and rotation.",
     "oneironaut.page.spaceswap.2": "I'm not quite sure what this one is supposed to do, it's always yelling at me about special dimensions. Perhaps it needs to use this special dimension as an intermediary?",
     "oneironaut.page.spaceswap.3": "Exchanges the blocks within the first cuboid in your current dimension (which must be within ambit) for the blocks within the second cuboid in the dimension corresponding to the Spatial Imprint. Costs 5 Charged Amethyst, plus half an Amethyst dust per cubic meter in the cuboid.$(br)Will not exchange any unbreakable blocks, or blocks with significant data.$(br)One or both of the endpoint dimensions must be the noosphere.",
     "oneironaut.page.spaceswap.4": "One or both of the endpoint dimensions must be the noosphere.",
     "oneironaut.page.status_iotas.1": "These patterns work with a type of iota that represents lingering effects on a creature, which can allow me to asses the state of a creature more thoroughly than with only Nurse's Purification.$(br)While my research suggests that status iotas representing instantaneous effects are possible, they would be very difficult to obtain, and I cannot think of any use case for them at the moment.",
     "oneironaut.page.status_iotas.10": "Costs more if attempting to remove a positive effect from an entity other than myself.$(br2)All of the patterns which deal with a specific status effect on an entity have the side effect that if the entity does not currently have the specified effect, the pattern will fail and inflict nausea upon me.",
-    "oneironaut.page.status_iotas.2": "Accepts a living entity, and returns a list status iotas representing all effects on the target.",
+    "oneironaut.page.status_iotas.2": "Accepts a living entity, and returns a list of status iotas representing all effects on the target.",
     "oneironaut.page.status_iotas.3": "Accepts a status effect type, and returns a number based on whether the effect is likely to be helpful, harmful, or neutral to a creature.",
     "oneironaut.page.status_iotas.4": "Accepts an entity and a status effect type, and returns the effect on the target's duration in seconds.",
     "oneironaut.page.status_iotas.5": "Accepts an entity and a status effect type, and returns the effect on the target's potency.",
     "oneironaut.page.status_iotas.6": "Accepts a status effect type and a vector, and returns an entity at that position which has that effect.",
     "oneironaut.page.status_iotas.7": "Accepts a status effect type, a vector, and a number ($(o)n$()), and returns a list of entities within radius $(o)n$() of the vector which have that effect.",
     "oneironaut.page.status_iotas.8": "Accepts a status effect type, a vector, and a number ($(o)n$()), and returns a list of entities within radius $(o)n$() of the vector which do not have that effect.",
     "oneironaut.page.status_iotas.9": "Accepts an entity and a status effect type, and removes that status effect from the entity. Cost is based on the effect's innate harmfulness, its potency, and its remaining duration.",
     "oneironaut.page.super_budding.1": "I've found that the amethyst-like material native to the noosphere can be imbued with a villager's mind, much like normal amethyst. What's more, the block that results from this process produces significantly more media than normal Budding Amethyst, and it can be picked up and moved if one takes special care.",
     "oneironaut.page.super_budding.2": "Pseudoamethyst requires a stronger mind than normal amethyst, but the cost is well worth it.",
     "oneironaut.page.super_budding.3": "Amazingly, the media generation rate of budding pseudoamethyst is such that even when immersed in thought slurry to inhibit crystal formation, it will still yield usable amounts of media. While the overall supply is nigh-endless, the amount accessible to any given action is quite small, like an inch-deep ocean a million miles across. However, due to this minimal depth, the media will dissipate rapidly before reaching my staff when accessed from afar, such as when recharging an item.",
     "oneironaut.page.super_budding.4": "Constantly provides about a tenth of an amethyst dust worth of media. While I certainly $(o)can$() hold several of these in order to gain access to more easy media, this results in rapidly-diminishing returns.",
     "oneironaut.page.wisp_lanterns.1": "I've found that by using materials unique to the Noosphere, I can create a special jar capable of producing and containing a tiny wisp. While this wisp cannot cast anything, it emits quite a bit of light, and will mimic pigments shown to it.$(br)I can also craft a version with tinted glass, in case the wisp's light would disrupt my study's aesthetic.",
     "text.oneironaut.clearIdeasResponse": "Cleared iota storage map.",
     "text.oneironaut.lorem_ipsum": "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
-    "text.oneironaut.noforgeyet": "This has not yet been implemented on Forge. Sorry!",
     "this.is.a.comment.1": "Pattern names--------------------------------------------------------------------------------------------",
     "this.is.a.comment.2": "Block/Item names--------------------------------------------------------------------------------------------",
     "this.is.a.comment.3": "Book entry titles--------------------------------------------------------------------------------------------",
     "this.is.a.comment.4": "Book pages--------------------------------------------------------------------------------------------",
     "this.is.a.comment.5": "Advancements--------------------------------------------------------------------------------------------",
     "this.is.a.comment.6": "Mishaps--------------------------------------------------------------------------------------------",
     "this.is.a.comment.7": "Other---------------------------------------------------------------------------------------------"
```

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/lang/zh_cn.json` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/lang/zh_cn.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5719424460431655%*

 * *Differences: {"'block.oneironaut.cell'": "'不协和精神'",*

 * * "'block.oneironaut.circle'": "'§0§o圆'",*

 * * "'block.oneironaut.hex_resistant_block'": "'咒术防护黑曜石'",*

 * * "'block.oneironaut.media_gel'": "'精神原质团'",*

 * * "'block.oneironaut.media_ice'": "'贤能智冰'",*

 * * "'effect.oneironaut.not_missing'": "'扬升共振'",*

 * * "'hexcasting.iota.oneironaut:uuid'": "'灵魂印记'",*

 * * "'hexcasting.iota.oneironaut:uuid.label'": "'%s的灵魂印记'",*

 * * "'hexcasting.mishap.invalid_value.class.oneironaut:imprint'": "'一个空间印记'",*

 * * "'hexcasting.mishap.invalid_value.class.oneironaut:soulprint'" […]*

```diff
@@ -1,138 +1,227 @@
 {
     "biome.oneironaut.noosphere_sea": "\u667a\u8bc6\u4e4b\u6d77",
-    "block.oneironaut.circle": "\u5706",
+    "block.oneironaut.cell": "\u4e0d\u534f\u548c\u7cbe\u795e",
+    "block.oneironaut.circle": "\u00a70\u00a7o\u5706",
+    "block.oneironaut.hex_resistant_block": "\u5492\u672f\u9632\u62a4\u9ed1\u66dc\u77f3",
+    "block.oneironaut.media_gel": "\u7cbe\u795e\u539f\u8d28\u56e2",
+    "block.oneironaut.media_ice": "\u8d24\u80fd\u667a\u51b0",
     "block.oneironaut.noosphere_basalt": "\u667a\u8bc6\u754c\u7384\u6b66\u5ca9",
     "block.oneironaut.pseudoamethyst_block": "\u4f2a\u7d2b\u6c34\u6676\u5757",
     "block.oneironaut.raycast_blocker": "\u53cd\u5c04\u7ebf\u8ffd\u8e2a\u677f\u5ca9",
     "block.oneironaut.raycast_blocker_glass": "\u53cd\u5c04\u7ebf\u8ffd\u8e2a\u73bb\u7483",
     "block.oneironaut.sentinel_sensor": "\u54e8\u536b\u63a2\u6d4b\u5668",
     "block.oneironaut.sentinel_trap": "\u63a2\u5bdf\u4fc3\u52a8\u77f3",
     "block.oneironaut.super_budding": "\u4f2a\u7d2b\u6c34\u6676\u6bcd\u5ca9",
     "block.oneironaut.thought_slurry": "\u601d\u7ef4\u6d46\u6db2",
     "block.oneironaut.thought_slurry_flowing": "\u6d41\u52a8\u7684\u601d\u7ef4\u6d46\u6db2",
     "block.oneironaut.wisp_lantern": "\u5492\u7075\u706f\u7b3c",
     "block.oneironaut.wisp_lantern_tinted": "\u906e\u5149\u5492\u7075\u706f\u7b3c",
     "effect.oneironaut.detection_resistance": "\u5a92\u8d28\u906e\u7f69",
     "effect.oneironaut.missing": "\u635f\u574f\u7684\u72b6\u6001\u6548\u679ciota",
+    "effect.oneironaut.not_missing": "\u626c\u5347\u5171\u632f",
     "enchantment.oneironaut.overcast_damage": "\u610f\u8bc6\u6495\u88c2",
     "fluid.oneironaut.thought_slurry": "\u601d\u7ef4\u6d46\u6db2",
     "hexcasting.iota.oneironaut:dim": "\u7ef4\u5ea6",
     "hexcasting.iota.oneironaut:potion": "\u72b6\u6001\u6548\u679c",
-    "hexcasting.mishap.oneironaut:mismatchcubes": "\u63d0\u4f9b\u7684\u957f\u65b9\u4f53\u4e0d\u76f8\u540c\u3002",
+    "hexcasting.iota.oneironaut:uuid": "\u7075\u9b42\u5370\u8bb0",
+    "hexcasting.iota.oneironaut:uuid.label": "%s\u7684\u7075\u9b42\u5370\u8bb0",
+    "hexcasting.mishap.invalid_value.class.oneironaut:imprint": "\u4e00\u4e2a\u7a7a\u95f4\u5370\u8bb0",
+    "hexcasting.mishap.invalid_value.class.oneironaut:soulprint": "\u4e00\u4e2a\u7075\u9b42\u5370\u8bb0",
+    "hexcasting.mishap.invalid_value.class.oneironaut:status": "\u4e00\u4e2a\u72b6\u6001\u6548\u679c",
+    "hexcasting.mishap.invalid_value.class.oneironaut:visiblestatus": "\u4e00\u4e2a\u53ef\u68c0\u6d4b\u7684\u72b6\u6001\u6548\u679c",
+    "hexcasting.mishap.oneironaut:mismatchcubes": "\u63d0\u4f9b\u7684\u957f\u65b9\u4f53\u5c3a\u5bf8\u4e0d\u76f8\u540c\u3002",
     "hexcasting.mishap.oneironaut:missingeffect": "%s\u672c\u5e94\u62e5\u6709%s\uff0c\u800c\u5b9e\u9645\u6ca1\u6709\u3002",
     "hexcasting.mishap.oneironaut:missingenchant": "%s\u672c\u5e94\u5e26\u6709%s\u9b54\u5492\uff0c\u800c\u5b9e\u9645\u6ca1\u6709\u3002",
     "hexcasting.mishap.oneironaut:nonconjured": "\u672c\u5e94\u5728%s\u5904\u6709\u4e00\u4e2a\u6784\u7b51\u7684\u65b9\u5757\uff0c\u800c\u5b9e\u9645\u4e3a%s\u3002",
-    "hexcasting.mishap.oneironaut:nonoosphere": "\u9700\u8981\u4e92\u6362\u7684\u5176\u4e2d\u4e00\u65b9\u4e3a\u4e00\u4e2a\u7279\u6b8a\u7ef4\u5ea6\u3002",
+    "hexcasting.mishap.oneironaut:nonoosphere": "\u4e92\u6362\u7684\u5176\u4e2d\u4e00\u65b9\u9700\u4e3a\u4e00\u4e2a\u7279\u6b8a\u7ef4\u5ea6\u3002",
+    "hexcasting.mishap.oneironaut:norequirediota": "\u9ecf\u6db2\u9700\u8981%s",
     "hexcasting.mishap.oneironaut:norod": "\u9700\u8981\u624b\u6301\u56de\u54cd\u4e4b\u6756\u3002",
+    "hexcasting.mishap.oneironaut:nostaff": "%s\u672c\u5e94\u7531\u6cd5\u6756\u65bd\u653e\u3002",
+    "hexcasting.mishap.oneironaut:requiresdifferententities": "\u4e00\u4e2a\u4e0e\u76ee\u6807\u4e0d\u540c\u7684\u5b9e\u4f53",
+    "hexcasting.mishap.oneironaut:unhappyslime": "\u9ecf\u6db2\u8bf4\u9053\uff1a\u201c%s\u201d",
     "hexcasting.mishap.oneironaut:uninfusable": "\u672c\u5e94\u5728%s\u5904\u6709\u4e00\u4e2a\u53ef\u704c\u6ce8\u65b9\u5757\uff0c\u800c\u5b9e\u9645\u4e3a%s\u3002",
+    "hexcasting.spell.oneironaut:advanceautomaton": "\u8d28\u80de\u751f\u6210",
     "hexcasting.spell.oneironaut:applymindrender": "\u8d4b\u80fd\u610f\u8bc6\u6495\u88c2\u8005",
+    "hexcasting.spell.oneironaut:applynotmissing": "\u626c\u5347\u5171\u632f",
+    "hexcasting.spell.oneironaut:checksignature": "\u7b7e\u5370\u4e4b\u7eaf\u5316",
     "hexcasting.spell.oneironaut:circle": "\u5706",
     "hexcasting.spell.oneironaut:craftrod": "\u6307\u6325\u6cd5\u6756",
     "hexcasting.spell.oneironaut:delayrod": "\u8282\u62cd\u5668\u4e4b\u7b56\u7565",
     "hexcasting.spell.oneironaut:detectshroud": "\u8fa8\u5bdf\u906e\u7f69",
     "hexcasting.spell.oneironaut:dimteleport": "\u667a\u8bc6\u95e8\u5f84",
-    "hexcasting.spell.oneironaut:dimteleport.comingsoon": "\u8fd9\u4e2a\u56fe\u6848\u5c06\u6765\u5fc5\u7136\u4f1a\u6709\u4e00\u5b9a\u7528\u5904\u3002",
     "hexcasting.spell.oneironaut:dimteleport.samedim": "\u8fd9\u4e2a\u6cd5\u672f\u4ec0\u4e48\u90fd\u4e0d\u4f1a\u505a\uff0c\u5c31\u597d\u50cf\u8ba9\u5df2\u7ecf\u5728\u5bb6\u7684\u4eba\u56de\u5bb6\u4e00\u6837\u3002",
+    "hexcasting.spell.oneironaut:filteredentityraycast": "\u4fa6\u67e5\u5458\u4e4b\u63d0\u6574",
+    "hexcasting.spell.oneironaut:gaussianrand": "\u71b5\u4e4b\u7cbe\u601d\uff0c\u7b2c\u4e8c\u578b",
     "hexcasting.spell.oneironaut:getbystatus": "\u533a\u57df\u4e4b\u63d0\u6574\uff1a\u72b6\u6001",
     "hexcasting.spell.oneironaut:getbystatusinverse": "\u533a\u57df\u4e4b\u63d0\u6574\uff1a\u975e\u72b6\u6001",
     "hexcasting.spell.oneironaut:getbystatussingle": "\u5b9e\u4f53\u4e4b\u998f\u5316\uff1a\u72b6\u6001",
     "hexcasting.spell.oneironaut:getdim1": "\u7a7a\u95f4\u4e4b\u7cbe\u601d",
     "hexcasting.spell.oneironaut:getdim2": "\u7a7a\u95f4\u4e4b\u7cbe\u601d\uff0c\u7b2c\u4e8c\u578b",
     "hexcasting.spell.oneironaut:getrodlook": "\u6307\u6325\u68d2\u4e4b\u7cbe\u601d",
     "hexcasting.spell.oneironaut:getrodpos": "\u6307\u6325\u68d2\u4e4b\u7cbe\u601d\uff0c\u7b2c\u4e8c\u578b",
     "hexcasting.spell.oneironaut:getrodstamp": "\u8282\u62cd\u5668\u4e4b\u7cbe\u601d",
+    "hexcasting.spell.oneironaut:getsoulprint": "\u7075\u9b42\u5370\u8bb0\u4e4b\u7cbe\u601d",
     "hexcasting.spell.oneironaut:getstatus": "\u836f\u5e08\u4e4b\u7eaf\u5316",
     "hexcasting.spell.oneironaut:getstatuscategory": "\u836f\u5e08\u4e4b\u7eaf\u5316\uff0c\u7b2c\u4e8c\u578b",
-    "hexcasting.spell.oneironaut:getstatusduration": "\u836f\u5242\u5e08\u4e4b\u7eaf\u5316",
-    "hexcasting.spell.oneironaut:getstatuslevel": "\u836f\u5242\u5e08\u4e4b\u7eaf\u5316\uff0c\u7b2c\u4e8c\u578b",
+    "hexcasting.spell.oneironaut:getstatusduration": "\u836f\u5242\u5e08\u4e4b\u998f\u5316",
+    "hexcasting.spell.oneironaut:getstatuslevel": "\u836f\u5242\u5e08\u4e4b\u998f\u5316\uff0c\u7b2c\u4e8c\u578b",
     "hexcasting.spell.oneironaut:haltrod": "\u7ec8\u66f2",
     "hexcasting.spell.oneironaut:infusemedia": "\u5a92\u8d28\u704c\u6ce8",
     "hexcasting.spell.oneironaut:invisibility": "\u9690\u9633\u5f53\u7a7a",
     "hexcasting.spell.oneironaut:paintconjured": "\u5916\u5316\u67d3\u8272\u5242",
     "hexcasting.spell.oneironaut:particleburst": "\u7c92\u5b50\u8ff8\u53d1",
-    "hexcasting.spell.oneironaut:readframeitem": "\u88c5\u6f62\u5e08\u4e4b\u7eaf\u5316\uff08\u5f03\u7528\uff09",
     "hexcasting.spell.oneironaut:readframerotation": "\u88c5\u6f62\u5e08\u4e4b\u7eaf\u5316",
     "hexcasting.spell.oneironaut:readidea": "\u6536\u56de\u601d\u7eea",
     "hexcasting.spell.oneironaut:readideatime": "\u5143\u6570\u636e\u4e4b\u7eaf\u5316",
     "hexcasting.spell.oneironaut:readideawriter": "\u5143\u6570\u636e\u4e4b\u998f\u5316",
+    "hexcasting.spell.oneironaut:readrodram": "\u5a01\u5ec9\u59c6\u65af\u4e4b\u7cbe\u601d",
     "hexcasting.spell.oneironaut:readsentinel": "\u68c0\u89c6\u54e8\u536b",
     "hexcasting.spell.oneironaut:removestatus": "\u6e05\u9664\u72b6\u6001",
     "hexcasting.spell.oneironaut:resetrod": "\u5b89\u53ef",
     "hexcasting.spell.oneironaut:resistdetection": "\u9690\u533f\u906e\u7f69",
     "hexcasting.spell.oneironaut:setframerotation": "\u88c5\u6f62\u5e08\u4e4b\u7b56\u7565",
+    "hexcasting.spell.oneironaut:signitem": "\u7b7e\u5370\u7269\u54c1",
     "hexcasting.spell.oneironaut:swapspace": "\u7a7a\u95f4\u4e92\u6362",
     "hexcasting.spell.oneironaut:writeidea": "\u523b\u5370\u601d\u7eea",
+    "hexcasting.spell.oneironaut:writerodram": "\u5a01\u5ec9\u59c6\u65af\u4e4b\u7b56\u7565",
+    "item.oneironaut.beacon_staff": "\u79d1\u6280\u6cd5\u6756",
     "item.oneironaut.echo_staff": "\u56de\u54cd\u6cd5\u6756",
     "item.oneironaut.endless_phial": "\u65e0\u7a77\u5a92\u8d28\u4e4b\u74f6",
+    "item.oneironaut.memory_fragment": "\u8bb0\u5fc6\u788e\u7247",
+    "item.oneironaut.memory_fragment.all": "\u4f3c\u4e4e\u6211\u5df2\u7ecf\u96c6\u9f50\u4e86\u8fd9\u4e9b\u6676\u4f53\u4e2d\u6240\u6709\u6211\u80fd\u627e\u5230\u7684\u8bb0\u5fc6\u2026\u2026",
+    "item.oneironaut.pigment_echo": "\u56de\u54cd\u67d3\u8272\u5242",
+    "item.oneironaut.pigment_flame": "\u706b\u7130\u67d3\u8272\u5242",
+    "item.oneironaut.pigment_noosphere": "\u667a\u8bc6\u67d3\u8272\u5242",
     "item.oneironaut.pseudoamethyst_shard": "\u4f2a\u7d2b\u6c34\u6676\u788e\u7247",
     "item.oneironaut.reverberation_rod": "\u56de\u54cd\u4e4b\u6756",
     "item.oneironaut.spoon_staff": "\u52fa\u5b50",
     "item.oneironaut.thought_slurry_bucket": "\u601d\u7ef4\u6d46\u6db2\u6876",
+    "itemGroup.oneironaut.oneironaut": "\u822a\u68a6",
+    "not.real.translation.key.1": "TODO: Add a structure that is implied to be part of a laboratory that has been ripped from the overworld by an engorged gateway",
+    "oneironaut.advancements.lore.root": "\u822a\u68a6\u6545\u4e8b",
+    "oneironaut.advancements.lore.root.description": "\u5931\u843d\u4e8e\u65f6\u95f4\u7684\u8bb0\u5fc6",
+    "oneironaut.advancements.lore.science1": "\u79d1\u5b66\u5bb6\u7684\u8bb0\u5fc6\uff0c#1",
+    "oneironaut.advancements.lore.science1.description": "\u6709\u5173\u8d28\u9053\u672c\u8d28\u7684\u7814\u7a76",
+    "oneironaut.advancements.lore.science2": "\u79d1\u5b66\u5bb6\u7684\u8bb0\u5fc6\uff0c#2",
+    "oneironaut.advancements.lore.science2.description": "\u6709\u5173\u667a\u8bc6\u754c\u6027\u8d28\u7684\u7814\u7a76",
+    "oneironaut.advancements.lore.science3": "\u79d1\u5b66\u5bb6\u7684\u8bb0\u5fc6\uff0c#3",
+    "oneironaut.advancements.lore.science3.description": "\u6709\u5173\u4f2a\u7d2b\u6c34\u6676\u7ed3\u6784\u7684\u7814\u7a76",
+    "oneironaut.advancements.lore.treatise1": "\u5492\u672f\u5e08\u7684\u8bb0\u5fc6\uff0c#1",
+    "oneironaut.advancements.lore.treatise1.description": "\u6709\u5173iota\u5d4c\u5165\u7684\u7cbe\u601d",
+    "oneironaut.advancements.lore.treatise2": "\u5492\u672f\u5e08\u7684\u8bb0\u5fc6\uff0c#2",
+    "oneironaut.advancements.lore.treatise2.description": "\u6709\u5173\u6709\u6548\u5229\u7528\u9a71\u52a8\u7684\u7cbe\u601d",
+    "oneironaut.advancements.lore.treatise3": "\u5492\u672f\u5e08\u7684\u8bb0\u5fc6\uff0c#3",
+    "oneironaut.advancements.lore.treatise3.description": "\u6709\u5173\u91cd\u590d\u56fe\u6848\u7684\u7cbe\u601d",
+    "oneironaut.advancements.lore.treatise4": "\u5492\u672f\u5e08\u7684\u8bb0\u5fc6\uff0c#4",
+    "oneironaut.advancements.lore.treatise4.description": "\u6709\u5173\u957f\u5492\u672f\u7684\u7cbe\u601d",
     "oneironaut.advancements.noosphere.enter": "\u601d\u7ef4\u4e0e\u68a6\u7684\u9886\u57df",
     "oneironaut.advancements.noosphere.enter.description": "\u8fdb\u5165\u667a\u8bc6\u754c",
+    "oneironaut.advancements.noosphere.find_media_lab": "\u7ed3\u6676",
+    "oneironaut.advancements.noosphere.find_media_lab.description": "\u53d1\u73b0\u4e00\u6b21\u7ed3\u5c40\u60e8\u6de1\u7684\u5b9e\u9a8c",
+    "oneironaut.advancements.noosphere.find_tower": "\u6c38\u5b58\u7ecf\u5178",
+    "oneironaut.advancements.noosphere.find_tower.description": "\u53d1\u73b0\u4e00\u5ea7\u5c5e\u4e8e\u8eab\u4efd\u4e0d\u8be6\u5492\u672f\u5e08\u7684\u9ad8\u5854",
     "oneironaut.entry.detection_shielding": "\u4fa6\u6d4b\u56de\u907f",
     "oneironaut.entry.dim_iotas": "\u7ef4\u5ea6 Iota",
-    "oneironaut.entry.framepatterns": "\u7269\u54c1\u5c55\u793a\u6846\u56fe\u6848",
     "oneironaut.entry.idea_inscription": "\u601d\u7eea\u523b\u5370",
     "oneironaut.entry.mindrender": "\u610f\u8bc6\u6495\u88c2\u8005",
-    "oneironaut.entry.noosphere_main": "\u5947\u602a\u9886\u57df",
+    "oneironaut.entry.miscpatterns": "\u822a\u68a6\uff1a\u6742\u9879\u56fe\u6848",
+    "oneironaut.entry.noosphere_main": "\u5947\u602a\u7684\u9886\u57df",
     "oneironaut.entry.noosphere_materials": "\u5bcc\u601d\u7ef4\u6750\u6599",
-    "oneironaut.entry.raycast_assailant": "\u5c04\u7ebf\u8ffd\u8e2a\u963b\u585e",
+    "oneironaut.entry.raycast_assailant": "\u53cd\u5492\u672f\u65b9\u5757",
     "oneironaut.entry.sentinel_detection": "\u54e8\u536b\u4fa6\u6d4b",
     "oneironaut.entry.slipway_hint": "\u6709\u5173\u8d28\u9053\u7684\u7cbe\u601d",
+    "oneironaut.entry.soulprints": "\u7075\u9b42\u5370\u8bb0",
     "oneironaut.entry.status_iotas": "\u72b6\u6001 Iota",
-    "oneironaut.entry.super_budding": "\u66f4\u597d\u7684\u5a92\u8d28\u91cf\u4ea7",
+    "oneironaut.entry.super_budding": "\u66f4\u597d\u5730\u91cf\u4ea7\u5a92\u8d28",
     "oneironaut.entry.wisp_lanterns": "\u5492\u7075\u706f\u7b3c",
     "oneironaut.mishap.badentitykey": "\u4e00\u4e2a\u7ecf\u8fc7\u542f\u8fea\u7684\u73a9\u5bb6\u6216\u5265\u9664\u610f\u8bc6\u7684\u6751\u6c11",
+    "oneironaut.mishap.entitytypelistplease": "\u4e00\u4e2a\u5b9e\u4f53\u7c7b\u578b\u5217\u8868",
+    "oneironaut.mishap.invalidideakey": "\u4e00\u4e2a\u5411\u91cf\u3001\u73a9\u5bb6\u6216\u7075\u9b42\u5370\u8bb0",
     "oneironaut.mishap.noitemframe": "\u4e00\u4e2a\u7269\u54c1\u5c55\u793a\u6846",
+    "oneironaut.mishap.nolistsallowed": "\u4e00\u4e2a\u975e\u5217\u8868iota",
     "oneironaut.mishap.notbrainswept": "\u4e00\u4e2a\u5265\u9664\u610f\u8bc6\u7684\u6751\u6c11",
-    "oneironaut.mishap.novecorentity": "\u4e00\u4e2a\u5411\u91cf\u6216\u73a9\u5bb6",
+    "oneironaut.mishap.twovectorsplease": "\u5217\u8868\u672a\u5305\u542b\u4e24\u4e2a\u5411\u91cf\u3002",
     "oneironaut.mishap.unenlightenedtarget": "\u4e00\u4e2a\u7ecf\u8fc7\u542f\u8fea\u7684\u73a9\u5bb6",
+    "oneironaut.mishap.wrongsizelist": "\u5217\u8868\u957f\u5ea6\u4e0d\u5408\u9002\u3002",
     "oneironaut.page.detection_shielding.1": "\u4f20\u7edf\u7684\u9690\u8eab\u836f\u6c34\u8db3\u4ee5\u8ff7\u60d1\u5e38\u4eba\u7684\u611f\u5b98\uff0c\u4f46\u9762\u5bf9\u5492\u672f\u5219\u6beb\u65e0\u4f5c\u7528\uff0c\u8ba9\u4e8b\u7269\u5b8c\u5168\u65e0\u6cd5\u4fa6\u6d4b\u7684\u65b9\u6cd5\u8fd8\u6709\u5f85\u53d1\u73b0\u3002\u7136\u800c\uff0c\u6211\u627e\u5230\u7684\u8fd9\u4e2a\u6cd5\u672f\u5e94\u5f53\u662f\u5411\u4e0a\u8ff0\u76ee\u6807\u8fc8\u51fa\u7684\u7b2c\u4e00\u6b65\u3002\u5b83\u80fd\u5c06\u5a92\u8d28\u50cf\u7ce0\u76ae\u4e00\u6837\u6563\u5728\u751f\u7269\u5468\u56f4\uff0c\u4ee5\u6b64\u5e72\u6270\u5492\u672f\u7684\u4fa6\u6d4b\u624b\u6bb5\u3002",
     "oneironaut.page.detection_shielding.2": "\u63a5\u53d7\u4e00\u4e2a\u751f\u7269\u548c\u4e00\u4e2a\u6570\uff0c\u5e76\u7ed9\u4e88\u8be5\u5b9e\u4f53\u6301\u7eed\u6240\u7ed9\u6570\u79d2\u7684\u5492\u672f\u4fa6\u6d4b\u62a4\u76fe\u3002\u6bcf\u79d2\u6301\u7eed\u65f6\u95f4\u6d88\u8017 2 \u4e2a\u7d2b\u6c34\u6676\u7c89\u3002",
     "oneironaut.page.detection_shielding.3": "\u540c\u65f6\u6bcf\u79d2\u4f1a\u6d88\u8017\u6240\u5f71\u54cd\u5b9e\u4f53 1/10 \u4e2a\u7d2b\u6c34\u6676\u7c89\uff0c\u62a4\u76fe\u7684\u6784\u7b51\u9700\u8981\u8fd9\u4e9b\u5a92\u8d28\u3002$(br2)\u6211\u9700\u8981\u6ce8\u610f\u6211\u628a\u8fd9\u79cd\u6548\u679c\u7ed9\u4e88\u4e86\u4ec0\u4e48\u4e8b\u7269\uff0c\u56e0\u4e3a\u6ca1\u6709\u643a\u5e26\u5176\u4ed6\u5a92\u8d28\u6765\u6e90\u7684\u751f\u7269\u4f1a\u6d88\u8017\u81ea\u8eab\u7684\u610f\u8bc6\u6765\u4f9b\u7ed9\u62a4\u76fe\u3002",
     "oneironaut.page.detection_shielding.4": "\u8fd9\u79cd\u62a4\u76fe\u5728\u963b\u6321$(l:patterns/basics#hexcasting:raycast/entity)\u4fa6\u67e5\u5458\u4e4b\u998f\u5316$(/l)\u548c\u5404\u79cd$(l:patterns/entities#hexcasting:zone_entity/animal)\u533a\u57df\u4e4b\u998f\u5316$(/l)\u65f6\u6548\u679c\u826f\u597d\uff0c\u4f46\u5b83\u5bf9$(l:patterns/entities#hexcasting:get_entity)\u5b9e\u4f53\u4e4b\u7eaf\u5316$(/l)\u7684\u53d8\u79cd\u6ca1\u6709\u4f5c\u7528\uff0c\u90a3\u4e9b\u64cd\u4f5c\u5df2\u7ecf\u5305\u542b\u6240\u5904\u4f4d\u7f6e\u7684\u7cbe\u786e\u6982\u5ff5\u3002\u800c\u4e14\uff0c\u8fd9\u5c42\u7ce0\u76ae\u81ea\u8eab\u4e5f\u6709\u80fd\u91cf\u7279\u5f81\uff0c\u5c3d\u7ba1\u6697\u6de1\uff0c\u4f9d\u7136\u53ef\u7528\u7279\u79cd\u56fe\u6848\u4fa6\u6d4b\u3002",
     "oneironaut.page.detection_shielding.5": "\u63a5\u53d7\u4e00\u4e2a\u5411\u91cf\u548c\u4e00\u4e2a\u6570\uff0c\u5e76\u8fd4\u56de\u4ee5\u6240\u7ed9\u4f4d\u7f6e\u4e3a\u8d77\u59cb\uff0c\u6307\u5411\u8303\u56f4\u5185\u5e26\u6709\u906e\u7f69\u7684\u5b9e\u4f53\u7684\u5355\u4f4d\u5411\u91cf\u5217\u8868\uff0c\u4fa6\u6d4b\u534a\u5f84\u4e3a\u6240\u7ed9\u6570\u3002",
     "oneironaut.page.detection_shielding.6": "\u6211\u8fd8\u53d1\u73b0\u4e86\u80fd\u7ed9\u4e88\u666e\u901a\u9690\u8eab\u6548\u679c\u7684\u6cd5\u672f\u3002\u548c\u5176\u4ed6$(l:patterns/great_spells/zeniths)\u5929\u9876\u6cd5\u672f$(/l)\u529f\u80fd\u4e00\u81f4\uff0c\u6bcf 3 \u79d2\u6301\u7eed\u65f6\u95f4\u6d88\u8017 1 \u4e2a\u7d2b\u6c34\u6676\u7c89\u3002",
     "oneironaut.page.dim_iotas.1": "\u6211\u53d1\u73b0\u4e86\u4e00\u79cd\u65b0 iota\uff0c\u5b83\u4eec\u4f3c\u4e4e\u8c61\u5f81\u7740\u73b0\u5b9e\u672c\u8eab\u7684\u67d0\u4e00\u5c42\u9762\u3002\u4e3a\u65b9\u4fbf\u7406\u89e3\uff0c\u6211\u51b3\u5b9a\u79f0\u5176\u4e3a\u201c\u7a7a\u95f4\u5370\u8bb0\u201d\u3002",
     "oneironaut.page.dim_iotas.2": "\u8fd4\u56de\u8c61\u5f81\u7740\u6211\u6240\u5904\u7ef4\u5ea6\u7684\u7a7a\u95f4\u5370\u8bb0\u3002\u6d88\u8017\u6781\u5c11\u91cf\u5a92\u8d28\u3002",
     "oneironaut.page.dim_iotas.3": "\u8fd4\u56de\u8c61\u5f81\u7740\u6211\u54e8\u536b\u6240\u5904\u7ef4\u5ea6\u7684\u7a7a\u95f4\u5370\u8bb0\u3002\u6d88\u8017\u6ca1\u90a3\u4e48\u5c11\u91cf\u4f46\u8fd8\u7b97\u5c11\u91cf\u7684\u5a92\u8d28\u3002",
     "oneironaut.page.dimteleport.1": "\u63a5\u53d7\u4e00\u4e2a\u5b9e\u4f53\u548c\u4e00\u4e2a\u7a7a\u95f4\u5143\u4ef6\uff0c\u5c06\u6240\u7ed9\u5b9e\u4f53\u4f20\u9001\u5165\u5bf9\u5e94\u7ef4\u5ea6\u7684\u540c\u4e00\u4f4d\u7f6e\u3002\u6d88\u8017 20 \u4e2a\u5145\u80fd\u7d2b\u6c34\u6676\u3002",
     "oneironaut.page.dimteleport.2": "\u76ee\u6807\u62b5\u8fbe\u76ee\u7684\u5730\u65f6\u4e5f\u4f1a\u89e6\u53d1\u67d0\u79cd\u4fdd\u62a4\u63aa\u65bd\uff0c\u4ee5\u9632\u76ee\u7684\u5730\u7684\u5371\u9669\u73af\u5883\u9020\u6210\u4f24\u5bb3\u3002$(br2)\u9001\u5165\u5176\u4ed6\u73a9\u5bb6\u65f6\u4f1a\u5931\u6548\u3002$(br2)\u53d7\u6b64\u6cd5\u672f\u5f71\u54cd\u65f6\uff0c\u6211\u4f1a\u6709\u79cd\u5947\u602a\u7684\u52a0\u901f\u611f\uff0c\u4f46\u5e76\u975e\u671d\u7740\u6211\u80fd\u7406\u89e3\u7684\u4efb\u4f55\u8f74\u52a0\u901f\u3002",
-    "oneironaut.page.framepatterns.1": "\u6211\u53d1\u73b0\u4e86\u4e00\u4e9b\u4e3a\u4e0e\u7269\u54c1\u5c55\u793a\u6846\u4ea4\u4e92\u8bbe\u8ba1\u7684\u56fe\u6848\u3002\u5b83\u4eec\u4e0d\u662f\u4ec0\u4e48\u9ad8\u7aef\u6cd5\u672f\uff0c\u4f46\u786e\u5b9e\u662f\u9002\u5408\u63a7\u5236\u6cd5\u672f\u73af\u4e4b\u7c7b\u4e8b\u7269\u7684\u5b9e\u7528\u624b\u6bb5\u3002$(br2)\u6b64\u5916\uff0c\u5206\u62e3\u5458\u4e4b\u7eaf\u5316\u5bf9\u5b83\u4eec\u540c\u6837\u6709\u6548\uff0c\u56e0\u6b64\u8bd5\u56fe\u5bfb\u627e\u7269\u54c1\u5c55\u793a\u6846\u4e13\u7528\u7684\u7269\u54c1\u56fe\u6848\u6ca1\u6709\u610f\u4e49\u3002",
-    "oneironaut.page.framepatterns.1.formerlink": "$(l:hexal:patterns/types#hexal:type/block_item)",
-    "oneironaut.page.framepatterns.2": "\u63a5\u53d7\u4e00\u4e2a\u7269\u54c1\u5c55\u793a\u6846\u5b9e\u4f53\uff0c\u5e76\u8fd4\u56de\u5176\u4e2d\u7269\u54c1\u7684\u7c7b\u578b\u3002\u6b64\u56fe\u6848\u5df2\u4e0d\u518d\u5b58\u5728\uff0c\u6211\u5fd8\u8bb0\u68c0\u9a8c\u5206\u62e3\u5458\u4e4b\u7eaf\u5316\u5bf9\u7269\u54c1\u5c55\u793a\u6846\u6709\u6ca1\u6709\u4f5c\u7528\u4e86\u3002\u5b9e\u9645\u4e0a\u786e\u5b9e\u662f\u6709\u7684\u3002",
-    "oneironaut.page.framepatterns.3": "\u63a5\u53d7\u4e00\u4e2a\u7269\u54c1\u5c55\u793a\u6846\u5b9e\u4f53\uff0c\u5e76\u8fd4\u56de\u5176\u4e2d\u7269\u54c1\u7684\u671d\u5411\uff0c\u503c\u5fc5\u7136\u5728 0 \u5230 7 \u4e4b\u95f4\u3002",
-    "oneironaut.page.framepatterns.4": "\u63a5\u53d7\u4e00\u4e2a\u7269\u54c1\u5c55\u793a\u6846\u5b9e\u4f53\u4e0e\u4e00\u4e2a 0 \u5230 7 \u7684\u6574\u6570\uff0c\u5e76\u5c06\u7269\u54c1\u671d\u5411\u8bbe\u7f6e\u4e3a\u8be5\u6570\u3002\u6d88\u8017\u6781\u5c11\u91cf\u5a92\u8d28\u3002",
+    "oneironaut.page.glow_ambit.1": "\u5c3d\u7ba1\u7ecf\u8fc7\u4e86\u957f\u4e45\u7684\u7814\u7a76\uff0c\u4ee3\u8868\u5176\u4ed6\u5492\u672f\u5e08\u7684 iota \u4e2d\u4ecd\u6709\u4e9b\u7279\u6b8a\u6027\u8d28\u7684\u6765\u6e90\u672a\u80fd\u5398\u6e05\u3002\u4e0d\u8fc7\uff0c\u6211\u627e\u5230\u4e86\u4e00\u79cd\u8d4b\u4e88\u5176\u4ed6\u4e8b\u7269\u540c\u6837\u6027\u8d28\u7684\u65b9\u6cd5\uff0c\u4e0d\u6562\u8bf4\u6301\u4e45\uff0c\u4f46\u81f3\u5c11\u80fd\u6682\u65f6\u505a\u5230\u3002\uff08\u8fd8\u5f88\u6602\u8d35\u3002\uff09$(br)\u8fd9\u79cd\u6cd5\u672f\u5141\u8bb8\u65bd\u6cd5\u8005\u8de8\u8d8a\u6781\u8fdc\u7684\u8ddd\u79bb\u5f71\u54cd\u751f\u7269\uff0c\u5c31\u548c\u73a9\u5bb6 iota \u7684\u65e0\u9650\u5f71\u54cd\u8ddd\u79bb\u4e00\u6837\u3002\u4f46\u5bf9\u76ee\u6807\u65bd\u653e\u8fd9\u79cd\u6cd5\u672f\u65f6\uff0c\u4f9d\u7136\u9700\u8981\u79bb\u76ee\u6807\u8db3\u591f\u8fd1\u3002",
+    "oneironaut.page.glow_ambit.2": "\u63a5\u53d7\u4e00\u4e2a\u6d3b\u4f53\uff0c\u5728 1 \u5206\u949f\u5185\u5373\u53ef\u5728\u4e16\u754c\u5404\u5904\u8bbf\u95ee\u6240\u7ed9\u6d3b\u4f53\u3002\u57fa\u7840\u6d88\u8017 1 \u4e2a\u7d2b\u6c34\u6676\u788e\u7247\uff0c\u5728\u6548\u5e94\u6d88\u9000\u524d\u6bcf\u65bd\u653e\u4e00\u6b21\u989d\u5916\u6d88\u8017 1 \u4e2a\u7d2b\u6c34\u6676\u788e\u7247\u3002",
+    "oneironaut.page.glow_ambit.3": "\u8fd9\u79cd\u6548\u679c\u7684\u539f\u7406\u4f3c\u4e4e\u662f\u8ba9\u76ee\u6807\u6563\u53d1\u51fa\u67d0\u79cd\u8d85\u81ea\u7136\u5171\u632f\u3002\u8fd9\u79cd\u5171\u632f\u76f8\u5f53\u5f3a\u5927\uff0c\u76ee\u6807\u7684\u8f6e\u5ed3\u9694\u7740\u5404\u79cd\u5f62\u5f0f\u7684\u969c\u788d\u4f9d\u7136\u201c\u53ef\u89c1\u201d\u3002\uff08\u5492\u672f\u5e08\u4eec\u4e5f\u8bb8\u5c31\u5728\u6301\u7eed\u4ea7\u751f\u8fd9\u79cd\u5171\u632f\uff0c\u53ea\u4e0d\u8fc7\u662f\u6ca1\u6709\u5982\u6b64\u6548\u679c\u663e\u8457\uff1f\uff09\u4f46\u662f\uff0c\u8fd9\u79cd\u8f89\u5149\u4e0e\u5149\u7075\u7bad\u7b49\u9020\u6210\u7684\u8f89\u5149\u4e0d\u4e00\u6837\uff0c\u4e0d\u8981\u6307\u671b\u76d1\u6d4b\u90a3\u79cd\u8f89\u5149\u7684\u4eea\u5668\u5bf9\u8fd9\u79cd\u4e5f\u6709\u6548\u3002",
     "oneironaut.page.idea_inscription.1": "\u667a\u8bc6\u754c\u662f\u601d\u7ef4\u7684\u9886\u57df\uff0c\u5b83\u80fd\u7528\u6765\u5b58\u50a8\u4fe1\u606f\u4e5f\u5c31\u987a\u7406\u6210\u7ae0\u3002\u8fd9\u4e9b\u56fe\u6848\u5c31\u80fd\u628a iota \u523b\u5370\u5165\u667a\u8bc6\u754c\uff0c\u5e76\u80fd\u8bfb\u51fa\u5b83\u4eec\uff08\u4e0d\u8bba\u5f53\u524d\u6240\u5904\u4ec0\u4e48\u7ef4\u5ea6\uff09\u3002\u5b83\u4eec\u8fd8\u80fd\u628a iota \u5b58\u50a8\u5230\u5176\u4ed6\u751f\u7269\u7684\u610f\u8bc6\u4e2d\uff0c\u5f53\u7136\u5b83\u4eec\u7684\u610f\u8bc6\u4e5f\u9700\u548c\u6211\u4e00\u6837\u2026\u2026$(o)\u65e0\u62d8\u65e0\u675f$()\u3002\u5728\u76f8\u5173\u63cf\u8ff0\u4e2d\uff0c\u7528\u4e8e\u6307\u4ee3\u5411\u91cf\u548c\u6709\u6548\u5b9e\u4f53\u7684\u8bcd\u662f\u201c\u952e\u201d/\u201ckey\u201d\u3002",
     "oneironaut.page.idea_inscription.2": "\u8fd9\u79cd\u64cd\u4f5c\u7528\u9014\u4e0d\u5c11\uff0c\u4f46\u667a\u8bc6\u754c\u7684\u73af\u5883\u5a92\u8d28\u5904\u4e8e\u5e38\u6001\u7684\u8fd0\u52a8\u4e2d\uff0c\u4efb\u4f55\u5b58\u5165\u5176\u4e2d\u7684 iota \u7ec8\u4f1a\u6d88\u89e3\uff0c\u5c31\u597d\u50cf\u5f80\u6d77\u6d0b\u4e2d\u5012\u70ed\u6c34\u4e00\u6837\u3002\u4f3c\u4e4e\u8fd9\u79cd\u4fe1\u606f\u5728\u53d8\u4e3a\u65e0\u7528\u7684\u5783\u573e\u524d\u80fd\u5b58\u5728\u4e00\u5c0f\u65f6\u3002$(br2)$(l:greatwork/akashiclib)\u963f\u5361\u590f\u56fe\u4e66\u9986$(/l)\u7684\u539f\u7406\u8c8c\u4f3c\u4e0e\u4e4b\u7c7b\u4f3c\uff0c\u4e66\u67b6\u5219\u76f8\u5f53\u4e8e\u7528\u6765\u907f\u514d\u6d88\u89e3\u7684\u963b\u9694\u5c42\u3002",
     "oneironaut.page.idea_inscription.3": "\u63a5\u53d7\u4e00\u4e2a\u6709\u6548\u952e\u4ee5\u53ca\u4efb\u610f iota\uff0c\u5e76\u5c06\u6240\u7ed9 iota \u5b58\u5165\u76f8\u5e94\u4f4d\u7f6e\u3002\u6d88\u8017\u5927\u7ea6 1 \u4e2a\u7d2b\u6c34\u6676\u7c89\u3002",
     "oneironaut.page.idea_inscription.4": "\u63a5\u53d7\u4e00\u4e2a\u6709\u6548\u952e\uff0c\u5e76\u8fd4\u56de\u76f8\u5e94 iota\u3002\u6d88\u8017\u5927\u7ea6 1 \u4e2a\u7d2b\u6c34\u6676\u7c89\u3002",
     "oneironaut.page.idea_inscription.5": "\u63a5\u53d7\u4e00\u4e2a\u6709\u6548\u952e, \u5e76\u8fd4\u56de\u523b\u5370\u5bf9\u5e94 iota \u7684\u65f6\u95f4\uff0c\u6216\u662f\u8fd4\u56de Null\u3002\u6d88\u8017\u6781\u5c11\u91cf\u5a92\u8d28\u3002",
     "oneironaut.page.idea_inscription.6": "\u63a5\u53d7\u4e00\u4e2a\u6709\u6548\u952e\u548c\u4e00\u4e2a\u4ee3\u8868\u73a9\u5bb6\u7684 iota\uff0c\u5e76\u68c0\u9a8c\u5bf9\u5e94 iota \u662f\u5426\u7531\u6240\u7ed9\u73a9\u5bb6\u523b\u5370\u3002\u6d88\u8017\u6781\u5c11\u91cf\u5a92\u8d28\u3002",
     "oneironaut.page.infusemedia.1": "\u63a5\u53d7\u4e00\u4e2a\u5411\u91cf\uff0c\u5e76\u5411\u8be5\u4f4d\u7f6e\u65b9\u5757\u4e2d\u6ce8\u5165\u5a92\u8d28\uff0c\u4ee5\u5b17\u53d8\u8be5\u65b9\u5757\u3002\u6d88\u8017\u91cf\u4e0e\u5177\u4f53\u6548\u679c\u968f\u76ee\u6807\u53d8\u5316\u800c\u53d8\u3002",
     "oneironaut.page.infusemedia.2": "\u6982\u5ff5\u4e0a\u6765\u770b\uff0c\u6b64\u6cd5\u672f\u4e0e$(l:patterns/spells/blockworks#hexcasting:edify)\u542f\u8fea\u6811\u82d7$(/l)\u7c7b\u4f3c\u3002$(br)\u7136\u800c\uff0c\u8fd9\u79cd\u65b9\u6cd5\u704c\u6ce8\u7684\u5a92\u8d28\u76f8\u8f83\u4e4b\u4e0b\u7ecf\u8fc7\u7cbe\u7ec6\u8c03\u6821\uff0c\u56e0\u6b64\u80fd\u4ea7\u751f\u66f4\u4e3a\u6709\u610f\u601d\u7684\u6548\u679c\u3002",
-    "oneironaut.page.mindrender.1": "\u6211\u66fe\u8bfb\u5230\u8fc7\u4e00\u79cd\u6781\u5176\u53ef\u6016\u7684\u6b66\u5668\uff0c\u201c\u610f\u8bc6\u6495\u88c2\u8005\u201d\u3002\u53e4\u4ee3\u7684\u5492\u672f\u5e08\u5076\u5c14\u4f1a\u7528\u8fd9\u79cd\u6b66\u5668\uff0c\u5b83\u80fd\u5c06\u751f\u7269\u7684\u601d\u7ef4\u76f4\u63a5\u65a9\u65ad\uff0c\u9020\u6210\u65e0\u89c6\u6240\u6709\u5df2\u77e5\u4fdd\u62a4\u624b\u6bb5\u7684\u4f24\u5bb3\u3002\u800c\u4e14\uff0c\u5982\u679c\u9020\u6210\u7684\u4f24\u5bb3\u4ee4\u76ee\u6807\u79bb\u771f\u6b63\u7684\u6b7b\u4ea1\u4ec5\u4e00\u6b65\u4e4b\u9065\uff0c\u5219\u5176\u4f1a\u8fdb\u5165\u690d\u7269\u4eba\u72b6\u6001\uff0c\u6c38\u8fdc\u65e0\u6cd5\u6062\u590d\u5982\u521d\u3002\u601d\u8003\u53e4\u4ee3\u4eba\u4e3a\u4ec0\u4e48\u4f7f\u7528\u8fd9\u79cd\u7269\u4ef6\u4ee4\u6211\u4e0d\u7531\u5f97\u5bd2\u900f\u810a\u9aa8\u2026\u2026",
+    "oneironaut.page.lore.science1.1": "$(o)\u201c\u8fd9\u662f\u4ec0\u4e48\uff1f\u6211\u8be5\u600e\u4e48\u628a\u5b83\u5f04\u8d70\uff1f\u201d$()$(br)\u5927\u591a\u6570\u4eba\u5728\u7b2c\u4e00\u6b21\u9047\u89c1\u8d28\u9053\u65f6\u90fd\u4f1a\u4ea7\u751f\u8fd9\u4e9b\u7591\u95ee\u3002\u6211\u5bf9\u7b2c\u4e8c\u4e2a\u95ee\u9898\u6682\u65f6\u6ca1\u6709\u7b54\u6848\uff0c\u4f46\u56de\u7b54\u7b2c\u4e00\u4e2a\u95ee\u9898\u8fd8\u662f\u53ef\u4ee5\u7684\u3002$(br)\u5c31\u6211\u6240\u77e5\uff0c\u8d28\u9053\u662f\u7a7a\u95f4\u4e2d\u7684\u5fae\u5c0f\u5b54\u6d1e\uff0c\u5176\u53e6\u4e00\u4fa7\u662f\u79f0\u4f5c\u201c\u667a\u8bc6\u754c\u201d\u7684\u5a92\u8d28\u754c\u3002",
+    "oneironaut.page.lore.science1.2": "\u8d28\u9053\u4e2d\u9038\u6563\u7684\u7c7b\u5492\u7075\u73b0\u8c61\u662f\u667a\u8bc6\u754c\u4e2d\u5de8\u91cf\u7684\u73af\u5883\u5a92\u8d28\u8bd5\u56fe\u8fc5\u901f\u901a\u8fc7\u5b54\u6d1e\u7684\u7ed3\u679c\uff08\u5c31\u50cf\u662f\u6c14\u4f53\u6269\u6563\u5165\u63a5\u8fd1\u771f\u7a7a\u7684\u7a7a\u95f4\uff09\uff0c\u8fd9\u4e9b\u5a92\u8d28\u7684\u7ea0\u7f20\u5377\u7ed5\u65b9\u5f0f\u4e0e\u53ec\u5524\u5492\u7075\u6cd5\u672f\u4e2d\u7f16\u7ec7\u4f9b\u5492\u7075\u6d88\u8017\u7684\u5a92\u8d28\u7684\u65b9\u5f0f\u7c7b\u4f3c\u3002",
+    "oneironaut.page.lore.science1.3": "\u6b64\u5916\uff0c\u8d28\u9053\u7684\u5165\u53e3\u5904\u4f3c\u4e4e\u5b58\u5728\u67d0\u79cd\u5c4f\u969c\uff0c\u4efb\u4f55\u7269\u8d28\u90fd\u4f1a\u88ab\u963b\u6321\u4e0d\u5f97\u901a\u8fc7\u3002\u5982\u679c\u8fd9\u4e00\u5c4f\u969c\u53ef\u88ab\u7a7f\u900f\uff0c\u5b54\u6d1e\u53ef\u88ab\u6269\u5c55\uff0c\u8d28\u9053\u5c31\u53ef\u5c06\u7269\u8d28\u5438\u6536\u5165\u667a\u8bc6\u754c\u3002\u8fd9\u4e48\u505a\u540e\u8d28\u9053\u4e0d\u4f1a\u518d\u4ea7\u751f\u5492\u7075\uff0c\u662f\u5a92\u8d28\u7684\u901a\u8fc7\u901f\u5ea6\u5927\u5927\u964d\u4f4e\uff0c\u4e0d\u4f1a\u518d\u53d7\u6270\u52a8\u800c\u7f20\u7ed5\u7684\u7f18\u6545\u3002\u5982\u679c\u60f3\u8981\u5c1d\u8bd5\uff0c\u5c31\u9700\u5c0f\u5fc3\u4e0d\u8981\u8fc7\u5ea6\u6269\u5c55\uff0c\u5426\u5219\u5468\u56f4\u533a\u57df\u90fd\u6709\u88ab\u5438\u6536\u5165\u667a\u8bc6\u754c\u7684\u5371\u9669\u3002",
+    "oneironaut.page.lore.science2.1": "\u771f\u662f\u4e2a\u5947\u602a\u7684\u5730\u65b9\u3002\u7ec4\u6210\u6b64\u5904\u6d77\u6d0b\u7684\u6db2\u4f53\u4e0d\u6bd4\u6c34\u81f4\u5bc6\u591a\u5c11\uff0c\u90a3\u4e9b\u5c9b\u5c7f\u7531\u5bc6\u5ea6\u7c7b\u4f3c\u7384\u6b66\u5ca9\u7684\u5ca9\u77f3\u6784\u6210\uff0c\u5374\u80fd\u6d6e\u5728\u5176\u4e2d\u3002\u800c\u4e14\uff0c\u6b64\u5904\u7684\u6240\u6709\u4e8b\u7269\u90fd\u4f3c\u4e4e\u77ac\u606f\u4e07\u53d8\uff0c\u5982\u68a6\u4f3c\u5e7b\u3002\u4f46\u6211\u6bd4\u4ece\u524d\u4efb\u4f55\u65f6\u5019\u90fd\u8981\u6e05\u9192\uff0c\u8fd9\u53c8\u600e\u4e48\u4f1a\u662f\u68a6\u5883\uff1f",
+    "oneironaut.page.lore.science2.2": "\u8fd9\u79cd\u6e05\u9192\u611f\u5e94\u5f53\u662f\u6b64\u5904\u73af\u5883\u5a92\u8d28\u7684\u6548\u679c\uff0c\u5b83\u4f1a\u6da6\u6ed1\u6211\u7684\u601d\u7ef4\u3002\u8fd9\u91cc\u7684\u5a92\u8d28\u6d53\u5ea6\u751a\u81f3\u8d85\u8fc7\u4e86\u5492\u7075\u7684\u6838\u5fc3\uff0c\u5b83\u4eec\u7684\u5929\u7136\u6d88\u8017\u4e5f\u56e0\u6b64\u7f29\u51cf\u5230\u65e0\u7a77\u5c0f\u3002\u6709\u8da3\u7684\u662f\uff0c\u90a3\u4e9b\u5e26\u6709\u67d0\u4eba\u7075\u9b42\u5370\u8bb0\u7684\u5492\u7075\u4e0d\u4f1a\u53d7\u6b64\u6548\u5e94\u5f71\u54cd\uff0c\u56e0\u6b64\u5492\u7075\u65e0\u6cd5\u7528\u4e8e\u957f\u65f6\u5b58\u50a8\u771f\u540d\u3002$(br)\u8fd9\u4e9b\u73af\u5883\u5a92\u8d28\u751a\u81f3\u4f1a\u4ece\u8db3\u591f\u5927\u7684\u7ef4\u5ea6\u88c2\u7f1d\u4e2d\u6e17\u6f0f\u51fa\u53bb\uff0c\u6b63\u662f\u5b83\u7ef4\u6301\u4e86\u88c2\u9699\u53e6\u4e00\u4fa7\u8ddd\u79bb\u8db3\u591f\u8fd1\u7684\u5492\u7075\u7684\u5f62\u6001\u3002",
+    "oneironaut.page.lore.science3.1": "\u8fd9\u79cd\u6676\u4f53\u5f88\u662f\u6709\u8da3\u3002\u4e00\u4ef6\u4ec5\u7531\u5a92\u8d28\u6784\u6210\u7684\u7269\u4f53\uff0c\u6d53\u5ea6\u8d85\u8d8a\u4e86\u4f20\u7edf\u7684\u6784\u7b51\u65b9\u5757\uff0c\u751a\u81f3\u8d85\u8d8a\u4e86\u6211\u5728\u56fe\u4e66\u9986\u4e2d\u7684\u540c\u4e8b\u4eec\u7814\u7a76\u7684\u90a3\u4e9b\u81f4\u5bc6\u5a92\u8d28\u6676\u4f53\u3002\u8fde\u5a92\u8d28\u5bc6\u5ea6\u76f8\u8fd1\u7684\u7d2b\u6c34\u6676\u4e2d\u7684\u90fd\u6709\u75d5\u91cf\u4e8c\u6c27\u5316\u7845\uff0c\u6b64\u6676\u4f53\u4e2d\u5374\u5b8c\u5168\u4e0d\u5b58\u5728\u6742\u8d28\u3002\u800c\u4ee4\u5176\u9759\u7f6e\u4e00\u6bb5\u65f6\u95f4\u540e\uff0c\u6676\u4f53\u7c89\u672b\u4f1a\u4ee5\u5206\u5f62\u6a21\u5f0f\u7d2f\u79ef\uff0c\u5c31\u597d\u50cf\u5728\u6301\u7eed\u4e0d\u65ad\u5730\u65bd\u6cd5\u3002",
+    "oneironaut.page.lore.science3.2": "\u6211\u5728\u663e\u5fae\u955c\u4e0b\u8be6\u7ec6\u68c0\u9a8c\u4e86\u8fd9\u79cd\u6676\u4f53\uff0c\u53ef\u89c2\u5bdf\u5230\u8fd9\u4e9b\u5206\u5f62\u72b6\u7ed3\u6784\u4f1a\u5411\u6676\u4f53\u5185\u90e8\u5ef6\u4f38\uff0c\u4e14\u4f1a\u4ee5\u56fa\u5b9a\u6a21\u5f0f\u4e00\u76f4\u53d8\u5316\u3002\u8fd9\u6709\u65e0\u53ef\u80fd\u662f\u4e00\u79cd\u65f6\u95f4\u6676\u4f53\uff1f",
+    "oneironaut.page.lore.treatise1.1": "\u867d\u7136\u65bd\u653e\u5492\u672f\u65f6\u80fd\u76f4\u63a5\u4ea7\u751f\u5927\u591a\u6570 iota\uff0c\u4f46\u603b\u4f1a\u6709\u4e0d\u591f\u4fbf\u6377\u7684\u60c5\u51b5\uff0c\u751a\u81f3\u4e8e\u65e0\u6cd5\u4ea7\u751f\uff08\u4f8b\u5982\u5e9e\u5927\u800c\u7cbe\u786e\u7684\u6570\u548c\u5b9e\u4f53 iota\uff09\u800c\u4e0d\u5f97\u4e0d\u53e6\u8f9f\u8e4a\u5f84\u3002\u4ece\u6838\u5fc3\u4e4b\u7c7b\u7684\u7269\u54c1\u4e2d\u8bfb\u53d6 iota \u4e5f\u4e0d\u9519\uff0c\u4f46\u5927\u591a\u6570\u60c5\u51b5\u4e0b\u8fd9\u4e48\u505a\u9700\u8981\u7b2c\u4e09\u53ea\u624b\uff0c\u800c\u6211\u5e76\u6ca1\u6709\u3002\u4ece\u5916\u90e8\u4f4d\u7f6e\u83b7\u53d6 iota \u7684\u5176\u4ed6\u65b9\u6cd5\u4e5f\u5404\u6709\u5404\u7684\u5c40\u9650\u6027\u3002",
+    "oneironaut.page.lore.treatise1.2": "\u800c\u5728\u65e0\u5916\u90e8\u5f15\u7528\u624b\u6bb5\u53ef\u7528\u7684\u60c5\u51b5\u4e0b\uff0c\u6240\u9700\u7684 iota \u5fc5\u987b\u76f4\u63a5\u63d2\u5165\u5492\u672f\u672c\u8eab\u3002\u5bf9\u90e8\u5206\u4eba\u800c\u8a00\uff0c\u8fd9\u4e48\u505a\u4f1a\u6709\u4e9b\u4e0d\u5408\u5e38\u7406\u3002\u8fd9\u662f\u56e0\u4e3a\u4f20\u7edf\u4e0a\u800c\u8a00\uff0c\u5492\u672f\u662f\u4e00\u4e2a\u56fe\u6848\u5217\u8868\uff0c\u4f46\u4e5f\u5e94\u7262\u8bb0\u56fe\u6848\u4e5f\u662f\u4e00\u79cd iota\uff0c\u4e00\u79cd\u4e0e$(l:patterns/meta#hexcasting:eval)\u8d6b\u5c14\u58a8\u65af\u4e4b\u7b56\u7565$(/l)\uff08\u4ee5\u53ca\u540c\u7c7b\u56fe\u6848\uff09\u534f\u540c\u6548\u679c\u5f88\u597d\u7684 iota\u3002",
+    "oneironaut.page.lore.treatise1.3": "\u5c3d\u7ba1\u4f60\u6ca1\u6cd5\u76f4\u63a5\u628a\u6570\u653e\u5230\u5217\u8868\u91cc\u9762\uff0c\u7136\u540e\u8ba9\u5b83\u548c\u4f7f\u7528$(l:patterns/numbers)\u6570\u5b57\u4e4b\u7cbe\u601d$(/l)\u4e00\u6837\u538b\u5165\u6808\u9876\uff0c\u4f46\u6709\u65b9\u6cd5\u80fd\u505a\u5230\u3002$(br2)\u6700\u7b80\u5355\uff08\u4e5f\u662f\u6700\u53ef\u9760\uff09\u7684\u65b9\u6cd5\u662f$(l:patterns/patterns_as_iotas#hexcasting:escape)\u8003\u5bdf$(/l)\u3002\u548c\u624b\u52a8\u65bd\u6cd5\u65f6\u4e00\u6837\uff0c\u5217\u8868\u4e2d\u5176\u540e\u65b9\u7684\u4efb\u610f\u4e8b\u7269\u4f1a\u88ab\u8f6c\u4e49\u5e76\u76f4\u63a5\u538b\u5165\u6808\u9876\uff0c\u800c\u975e\u548c\u5e73\u65f6\u4e00\u6837\u8fd0\u884c\uff0c\u5982\u6b64\u5c31\u53ef\u907f\u514d\u8fd0\u884c\u975e\u56fe\u6848\u5bfc\u81f4\u7684\u4e8b\u6545\u3002",
+    "oneironaut.page.lore.treatise1.4": "\u7136\u800c\uff0c\u5f53\u4f60\u4f4d\u4e8e\u5492\u672f\u4e2d\u8d85\u8fc7\u4e00\u5c42\u8fd0\u884c\u6df1\u5ea6\u5904\uff08\u6bd4\u5982\u5faa\u73af\u548c\u5d4c\u5957\u7684\u6761\u4ef6\u903b\u8f91\uff09\uff0c\u8f6c\u4e49 iota \u6240\u9700\u7684\u8003\u5bdf\u6570\u91cf\u4f1a\u6781\u901f\u589e\u957f\u3002\u5728\u90a3\u4e9b\u80fd\u591f\u7531\u53e6\u4e00\u5492\u672f\u8fd0\u884c\u7684\u4e8b\u7269\u4e2d\uff0c\u8fd9\u79cd\u65b9\u6cd5\u4fbf\u4e0d\u518d\u53ef\u9760\u3002",
+    "oneironaut.page.lore.treatise1.4.link": "\u76f8\u5173\u7684 xkcd",
+    "oneironaut.page.lore.treatise1.5": "\u66f4\u4e3a\u53ef\u9760\u7684\u8f6c\u4e49 iota \u65b9\u6cd5\u662f$(l:patterns/patterns_as_iotas#hexcasting:open_paren)\u5185\u7701$(/l)\u548c$(l:patterns/patterns_as_iotas#hexcasting:close_paren)\u53cd\u601d$(/l)\u3002\u8fd0\u884c\u56fe\u6848\u5217\u8868\u65f6\uff0c\u5185\u7701\u540e\u65b9\u76f4\u5230\u76f8\u5e94\u53cd\u601d\u4e4b\u95f4\uff08\u5185\u7701\u548c\u53cd\u601d\u4e0d\u8ba1\uff09\u7684\u4e8b\u7269\u4f1a\u88ab\u8f6c\u4e49\uff0c\u5e76\u4ee5\u5217\u8868\u5f62\u5f0f\u538b\u5165\u6808\u9876\uff0c\u4e0d\u8bba iota \u7684\u7c7b\u578b\u5982\u4f55\u3002\u7136\u540e\u5c31\u53ef\u4ee5\u7528\u5408\u9002\u65b9\u5f0f\u64cd\u4f5c\u6b64\u5217\u8868\uff0c\u6bd4\u5982\u7528$(l:patterns/lists#hexcasting:splat)\u7fa4\u4f53\u4e4b\u62c6\u89e3$(/l)\u628a\u5217\u8868\u4e2d\u5404\u9879\u5206\u522b\u538b\u5165\u6808\u9876\u3002",
+    "oneironaut.page.lore.treatise1.6": "\u5982\u679c\u4f60\u7684\u5217\u8868\u7684\u7ed3\u6784\u4e0e\u6b64\u7c7b\u4f3c\uff1a$(br2)\u5185\u7701$(br)\u4efb\u610f iota(s)$(br)\u53cd\u601d$(br)\u7fa4\u4f53\u4e4b\u62c6\u89e3$(br2)\u8fd0\u884c\u8fd9\u4e9b iota \u4e4b\u540e\uff0c\u6808\u4e2d\u4f1a\u538b\u5165\u5185\u7701\u4e0e\u53cd\u601d\u4e4b\u95f4\u7684\u6240\u6709 iota\u3002",
+    "oneironaut.page.lore.treatise2.1": "\u63a8\u52a8\u4e8b\u7269\u7684\u6807\u51c6\u505a\u6cd5\u662f$(l:patterns/spells/basic#hexcasting:add_motion)\u9a71\u52a8$(/l)\u3002\u4f46\u662f\uff0c\u5982\u679c\u60f3\u8981\u4e8b\u7269\u6781\u4e3a\u8fc5\u901f\u5730\u79fb\u52a8\uff0c\u8fd9\u79cd\u65b9\u6cd5\u53ef\u80fd\u4f1a\u6602\u8d35\u5230\u65e0\u6cd5\u4f7f\u7528\u3002\u8fd9\u662f\u56e0\u4e3a\u6d88\u8017\u4f1a\u968f\u5411\u91cf\u6a21\u957f\u6781\u901f\u589e\u957f\u3002\u5bf9\u5355\u4e2a\u76ee\u6807\u4f7f\u7528\u591a\u6b21\u6a21\u957f\u4e3a 1 \u7684\u9a71\u52a8\u5c31\u80fd\u51cf\u5c11\u8fd9\u79cd\u5f71\u54cd\uff0c\u603b\u6d88\u8017\u4f1a\u4ece n^2 \u964d\u5230 2n-1\uff0c\u5176\u4e2d n \u662f\u5411\u91cf\u7684\u6a21\u957f\u3002",
+    "oneironaut.page.lore.treatise2.2": "\u8fd9\u79cd\u65b9\u6cd5\u6700\u7b80\u5355\u7684\u5b9e\u73b0\u65b9\u5f0f\u9700\u8981$(l:patterns/meta#hexcasting:for_each)\u6258\u7279\u4e4b\u7b56\u7565$(/l)\uff0c\u4f20\u5165\u591a\u4e2a\u91cd\u590d\u7684\u5b9e\u4f53 iota \u7ec4\u6210\u7684\u5217\u8868\u5373\u53ef\u3002\u5f53\u7136\u4e5f\u6709\u5176\u4ed6\uff08\u4e14\u901a\u5e38\u66f4\u597d\u7684\uff09\u65b9\u6cd5\u5b58\u5728\u3002\u4f46\u9664\u53bb\u91cd\u590d\u7ed8\u5236\u56fe\u6848\u5916\uff0c\u8fd9\u4e9b\u65b9\u6cd5\u5927\u591a\u79bb\u4e0d\u5f00\u5faa\u73af\u8fd9\u4e00\u547d\u9898\uff0c\u8fd9\u5c31\u6709\u70b9\u8d85\u51fa\u8fd9\u7bc7\u6587\u6863\u7684\u8303\u7574\u4e86\u3002",
+    "oneironaut.page.lore.treatise3.1": "\u867d\u7136$(l:patterns/meta#hexcasting:for_each)\u6258\u7279\u4e4b\u7b56\u7565$(/l)\u6781\u5176\u9002\u5408\u540c\u65f6\u5bf9\u591a\u4e2a\u76ee\u6807\u65bd\u653e\u540c\u4e00\u6cd5\u672f\uff0c\u4f46\u5bf9\u540c\u4e00\u76ee\u6807\u65bd\u653e\u591a\u6b21\u6cd5\u672f\u5c31\u6709\u70b9\u9ebb\u70e6\u4e86\u3002\u5b83\u4e0d\u4ec5\u5bb9\u6613\u5bfc\u81f4\u5492\u672f\u7684\u505c\u6b62\uff0c\u8fd0\u884c\u5f00\u59cb\u540e\u8fd8\u65e0\u6cd5\u6dfb\u52a0\u6216\u79fb\u9664\u4f5c\u7528\u76ee\u6807\u3002$(br)\u800c\u7ed5\u8fc7\u8fd9\u4e9b\u5c40\u9650\u4e5f\u5f88\u7b80\u5355\uff0c\u6362\u7528\u53e6\u4e00\u79cd\u5faa\u73af\u5373\u53ef\u3002",
+    "oneironaut.page.lore.treatise3.2": "While \u5faa\u73af\u662f\u4e00\u79cd\u5728\u65e2\u5b9a\u6761\u4ef6\u8fbe\u6210\u4e4b\u524d\u4e00\u76f4\u8fd0\u884c\u7684\u5faa\u73af\uff0c\u6bd4\u5982\u6761\u4ef6\u53ef\u4ee5\u662f\u5b9e\u4f53\u7684\u901f\u5ea6\u8fbe\u5230\u4e86\u7ed9\u5b9a\u503c\u3002\u4e00\u4e2a\u4ec5\u4f1a\u590d\u5236\u81ea\u8eab\u518d\u8fd0\u884c\u6808\u9876 iota \u7684\u56fe\u6848\u5217\u8868\u5c31\u662f\u8fd9\u79cd\u5faa\u73af\u6700\u7b80\u5355\u7684\u5b9e\u73b0\u65b9\u5f0f\u3002\u5982\u679c\u5355\u72ec\u8fd0\u884c\u5b83\uff0c\u90a3\u4e48\u5492\u672f\u4f1a\u8fdb\u5165\u65e0\u9650\u5faa\u73af\uff0c\u9664\u975e\u4ea7\u751f\u4e8b\u6545\u4e0d\u7136\u4e0d\u4f1a\u505c\u6b62\u3002",
+    "oneironaut.page.lore.treatise3.2.header": "While \u5faa\u73af",
+    "oneironaut.page.lore.treatise3.3": "\u5411\u5176\u4e2d\u52a0\u5165\u5b9e\u9645\u529f\u80fd\u548c\u4e00\u4e9b\u5e03\u5c14\u903b\u8f91\uff0c\u5c31\u80fd\u521b\u9020\u51fa\u6709\u7528\u7684 while \u5faa\u73af\u3002\u524d\u6587\u6240\u63d0\u65e0\u9650\u5faa\u73af\u7684\u4ee3\u7801\u5982\u4e0b\uff1a$(br)\u5185\u7701$(br)\u53cc\u5b50\u4e4b\u5206\u89e3$(br)\u8d6b\u5c14\u58a8\u65af\u4e4b\u7b56\u7565$(br)\u53cd\u601d$(br)\u53cc\u5b50\u4e4b\u5206\u89e3$(br)\u8d6b\u5c14\u58a8\u65af\u4e4b\u7b56\u7565$(br2)\u5411\u5176\u4e2d\u52a0\u5165\u6839\u636e\u6761\u4ef6\u662f\u5426\u8fd0\u884c\u5217\u8868\u5185\u8d6b\u5c14\u58a8\u65af\u4e4b\u7b56\u7565\u7684\u903b\u8f91\uff0c\u8fbe\u6210\u76f8\u5e94\u6761\u4ef6\u540e\u5faa\u73af\u4fbf\u4f1a\u7ec8\u6b62\u3002",
+    "oneironaut.page.lore.treatise3.4": "\u201c\u5df2\u5c55\u5f00\u5faa\u73af\u201d/\u201cUnrolled loop\u201d\u662f\u4e00\u79cd\u66f4\u4e3a\u590d\u6742\u7684\u5faa\u73af\u3002\u548c\u6258\u7279\u4e4b\u7b56\u7565\u4e00\u6837\uff0c\u6784\u5efa\u65f6\u5176\u8fed\u4ee3\u6b21\u6570\u540c\u6837\u56fa\u5b9a\uff0c\u96be\u4ee5\u589e\u52a0\u4fee\u6539\u3002\u4f46\u5982\u6709\u9700\u8981\uff0c\u5361\u620e\u4e4b\u7b56\u7565\u53ef\u4ee5\u4ee4\u5176\u63d0\u524d\u505c\u6b62\u3002\u6bd4\u8f83\u6765\u770b\uff0c\u8fd9\u79cd\u5faa\u73af\u4ec5\u4ea7\u751f\u4e00\u5230\u4e24\u5c42\u9012\u5f52\u6df1\u5ea6\uff08\u5faa\u73af\u4f53\u8fd0\u884c\u6240\u81f4\u6df1\u5ea6\u4e0d\u8ba1\uff09\uff0c\u662f\u5176\u4f18\u52bf\u6240\u5728\u3002\u5148\u5199\u5b9a\u60f3\u8981\u91cd\u590d\u7684\u56fe\u6848\u5217\u8868\uff0c\u518d\u591a\u6b21\u590d\u5236\uff0c\u6700\u540e\u628a\u6240\u6709\u5217\u8868\u5408\u6210\u4e00\u4f53\uff0c\u5c31\u5b9e\u73b0\u4e86\u5faa\u73af\u5c55\u5f00\u3002",
+    "oneironaut.page.lore.treatise3.4.header": "\u5faa\u73af\u5c55\u5f00",
+    "oneironaut.page.lore.treatise3.5": "\u8fd9\u4e00\u76ee\u6807\u6700\u7b80\u5355\u7684\u8fbe\u6210\u65b9\u5f0f\u662f$(l:patterns/stackmanip#hexcasting:duplicate)\u53cc\u5b50\u4e4b\u5206\u89e3$(/l)\u63a5$(l:patterns/lists#hexcasting:concat)\u7ec4\u5408\u4e4b\u998f\u5316$(/l)\uff0c\u8fd0\u884c\u540e\u539f\u5217\u8868\u4f1a\u91cd\u590d 2 \u6b21\u3002\u53ef\u91cd\u590d\u4f7f\u7528\u6b64\u65b9\u6cd5\u4ee5\u590d\u5236\u539f\u5217\u8868 2 \u7684\u5e42\u6b21\uff0c\u6240\u5f97\u7684\u5217\u8868\u5728\u8fd0\u884c\u65f6\u53ea\u4f1a\u4ea7\u751f\u4e00\u5c42\u9012\u5f52\u6df1\u5ea6\u3002\u66f4\u7075\u6d3b\u7684\u505a\u6cd5\u5219\u662f\u4f7f\u7528$(l:patterns/stackmanip#hexcasting:duplicate_n)\u53cc\u5b50\u4e4b\u7b56\u7565$(/l)\u4ea7\u751f $(o)n$() \u4e2a\u526f\u672c\uff0c\u518d\u5c06 $(o)n-1$() \u4e2a\u7ec4\u5408\u4e4b\u998f\u5316\u653e\u5165\u5217\u8868\u5e76\u8fd0\u884c\uff0c\u5982\u6b64\u4fbf\u80fd\u628a\u6240\u6709\u539f\u5217\u8868\u526f\u672c\u5408\u4e3a\u4e00\u4f53\u3002",
+    "oneironaut.page.lore.treatise4.1": "\u6211\u7684\u4e00\u4e9b\u5443\uff0c\u201c\u540c\u4e8b\u201d\uff0c\u5728\u6284\u5f55\u957f\u5492\u672f\u65f6\u9047\u5230\u4e86\u9ebb\u70e6\u3002$(br)\u201c\u8fd9\u4e1c\u897f\u597d\u957f\uff01\u201d$(br)\u201c\u5492\u672f\u7f51\u683c\u90fd\u4e0d\u591f\u7528\u4e86\uff01\u201d$(br)\u6211\u8ba4\u4e3a\u8fd9\u662f$(bold)\u80fd\u529b\u95ee\u9898$()\u3002\u8fd9\u53c8\u4e0d\u662f\u90a3\u4e9b\u7ed8\u5236\u5b8c\u6700\u540e\u4e00\u4e2a\u53cd\u601d\u540e\u6ca1\u6cd5\u4fee\u6539\u5492\u672f\u7684\u9ebb\u70e6\u3002\u53ea\u9700\u628a\u672a\u5b8c\u6210\u7684\u5492\u672f\u5b58\u5230\u6838\u5fc3\u4e2d\u5373\u53ef\u3002\uff08\u4e0d\u8fc7\u4f60\u5e94\u8be5\u6ce8\u610f\u4e3a\u5b58\u50a8\u64cd\u4f5c\u7559\u51fa\u7a7a\u95f4\u3002\uff09",
+    "oneironaut.page.lore.treatise4.2": "\u5b8c\u6210\u4e4b\u540e\uff0c\u518d\u7528$(l:patterns/lists)\u5217\u8868\u64cd\u4f5c$(/l)\u56fe\u6848\u628a\u5404\u90e8\u5206\u5408\u8d77\u6765\u5c31\u884c\u4e86\u3002$(br2)\u751a\u81f3\u90fd\u4e0d\u9700\u8981\u7528\u591a\u4e2a\u6838\u5fc3\uff0c\u5199\u5b8c\u4e00\u90e8\u5206\u540e\u628a\u5b83\u63a5\u5230\u6838\u5fc3\u4e2d\u5217\u8868\u7684\u540e\u65b9\uff0c\u518d\u628a\u6240\u5f97\u5217\u8868\u5b58\u5165\u6838\u5fc3\u5373\u53ef\u3002\u591a\u6838\u5fc3\u4f1a\u8ba9\u8c03\u8bd5\u5492\u672f\u66f4\u8f7b\u677e\uff0c\u4f46\u636e\u6211\u76ee\u524d\u6240\u77e5\uff0c\u8fd9\u4e5f\u662f\u591a\u6838\u5fc3\u76f8\u5bf9\u5355\u6838\u5fc3\u552f\u4e00\u7684\u4f18\u52bf\u3002",
+    "oneironaut.page.mindrender.1": "\u6211\u66fe\u8bfb\u5230\u8fc7\u4e00\u79cd\u6781\u5176\u53ef\u6016\u7684\u6b66\u5668\uff0c\u201c\u610f\u8bc6\u6495\u88c2\u8005\u201d\u3002\u53e4\u4ee3\u7684\u5492\u672f\u5e08\u5076\u5c14\u4f1a\u7528\u8fd9\u79cd\u6b66\u5668\uff0c\u5b83\u80fd\u5c06\u751f\u7269\u7684\u601d\u7ef4\u76f4\u63a5\u65a9\u65ad\uff0c\u9020\u6210\u65e0\u89c6\u6240\u6709\u5df2\u77e5\u4fdd\u62a4\u624b\u6bb5\u7684\u4f24\u5bb3\u3002\u800c\u4e14\uff0c\u5982\u679c\u9020\u6210\u7684\u4f24\u5bb3\u4ee4\u76ee\u6807\u79bb\u771f\u6b63\u7684\u6b7b\u4ea1\u4ec5\u4e00\u6b65\u4e4b\u9065\uff0c\u5219\u5176\u4f1a\u8fdb\u5165\u690d\u7269\u4eba\u72b6\u6001\uff0c\u6c38\u8fdc\u65e0\u6cd5\u6062\u590d\u5982\u521d\u3002\u60f3\u5230\u53e4\u4ee3\u4eba\u4f7f\u7528\u8fd9\u79cd\u7269\u4ef6\u7684\u539f\u56e0\uff0c\u6211\u4e0d\u7531\u5f97\u5bd2\u900f\u810a\u9aa8\u2026\u2026",
     "oneironaut.page.mindrender.2": "\u63a5\u53d7\u5e26\u6709\u950b\u5229\u9b54\u5492\u7684\u7269\u54c1\uff0c\u6216\u653e\u6709\u6b64\u7c7b\u7269\u54c1\u7684\u7269\u54c1\u5c55\u793a\u6846\uff0c\u5e76\u5c06\u950b\u5229\u8f6c\u6362\u4e3a\u540c\u7b49\u7ea7\u7684\u610f\u8bc6\u6495\u88c2\u3002\u6d88\u8017\u7531\u9b54\u5492\u7b49\u7ea7\u51b3\u5b9a\uff0c\u76ee\u6807\u4e3a\u4e66\u65f6\u989d\u5916\u6d88\u8017 50%%\u3002",
+    "oneironaut.page.miscpatterns.1": "\u6211\u53d1\u73b0\u4e86\u4e00\u4e9b\u4e13\u4e3a\u7269\u54c1\u5c55\u793a\u6846\u4ea4\u4e92\u8bbe\u8ba1\u7684\u56fe\u6848\u3002\u5b83\u4eec\u4e0d\u662f\u4ec0\u4e48\u9ad8\u7aef\u6cd5\u672f\uff0c\u4f46\u786e\u5b9e\u662f\u9002\u5408\u63a7\u5236\u6cd5\u672f\u73af\u4e4b\u7c7b\u4e8b\u7269\u7684\u5b9e\u7528\u624b\u6bb5\u3002$(br2)\u6b64\u5916\uff0c\u5206\u62e3\u5458\u4e4b\u7eaf\u5316\u5bf9\u5b83\u4eec\u540c\u6837\u6709\u6548\uff0c\u56e0\u6b64\u8bd5\u56fe\u5bfb\u627e\u7269\u54c1\u5c55\u793a\u6846\u4e13\u7528\u7684\u7269\u54c1\u56fe\u6848\u6ca1\u6709\u610f\u4e49\u3002",
+    "oneironaut.page.miscpatterns.1.formerlink": "$(l:hexal:patterns/types#hexal:type/block_item)",
+    "oneironaut.page.miscpatterns.2": "\u63a5\u53d7\u4e00\u4e2a\u7269\u54c1\u5c55\u793a\u6846\u5b9e\u4f53\uff0c\u5e76\u8fd4\u56de\u5176\u4e2d\u7269\u54c1\u7684\u671d\u5411\uff0c\u503c\u5fc5\u7136\u5728 0 \u5230 7 \u4e4b\u95f4\u3002",
+    "oneironaut.page.miscpatterns.3": "\u63a5\u53d7\u4e00\u4e2a\u7269\u54c1\u5c55\u793a\u6846\u5b9e\u4f53\u4e0e\u4e00\u4e2a 0 \u5230 7 \u7684\u6574\u6570\uff0c\u5e76\u5c06\u7269\u54c1\u671d\u5411\u8bbe\u7f6e\u4e3a\u8be5\u6570\u3002\u6d88\u8017\u6781\u5c11\u91cf\u5a92\u8d28\u3002",
+    "oneironaut.page.miscpatterns.4": "\u4e0e$(l:patterns/basics#hexcasting:raycast/entity)\u4fa6\u67e5\u5458\u4e4b\u998f\u5316$(/l)\u7c7b\u4f3c\uff0c\u4f46\u80fd\u591f\u63a5\u53d7\u4e00\u4e2a\u5b9e\u4f53\u7c7b\u578b iota \u5217\u8868\u3002\u7c7b\u578b\u4e0d\u5728\u8be5\u5217\u8868\u5185\u7684\u5b9e\u4f53\u4f1a\u88ab\u5ffd\u7565\u3002\u6d88\u8017\u7684\u5a92\u8d28\u91cf\u7565\u591a\u4e8e\u4e0a\u6587\u6240\u63d0\u56fe\u6848\u7684\u201c\u6781\u5c11\u91cf\u201d\u3002",
+    "oneironaut.page.miscpatterns.5": "\u8fd4\u56de 0 \u4e0e 1 \u4e4b\u95f4\u7684\u968f\u673a\u6570\uff0c\u670d\u4ece\u6b63\u6001\u5206\u5e03\u3002",
     "oneironaut.page.noosphere_main.1": "\u6211\u6210\u529f\u4e86\u3002$(br)\u8d28\u9053\u53e6\u4e00\u7aef\u7684\u9886\u57df\u3002\u73af\u5883\u4e2d\u7684\u5a92\u8d28\u591a\u5230\u96be\u4ee5\u60f3\u8c61\u3002\u6211\u7684\u610f\u8bc6\u6b63\u671d\u6211\u5c16\u5578\uff0c\u53eb\u558a\u7740\u6211\u4e0d\u5e94\u8be5\u5728\u8fd9\u91cc\u3002\u4f46\u6211\u5fc5\u987b\u524d\u8fdb\u3002\u8fd9\u91cc\u5c31\u662f\u65c5\u9014\u7684\u4e0b\u4e00\u7ad9\u3002",
     "oneironaut.page.noosphere_main.2": "\u6211\u5728\u6b64\u52d8\u6d4b\u7684\u6bcf\u4e00\u4ef6\u4e8b\u7269\u4f3c\u4e4e\u4e3b\u8981\u90fd\u7531\u5a92\u8d28\u6784\u6210\uff0c\u4e0e\u6784\u7b51\u7269\u8d28\u7c7b\u4f3c\uff0c\u4f46\u6d53\u5ea6\u9ad8\u51fa\u4e86\u51e0\u4e2a\u6570\u91cf\u7ea7\u3002$(br)$(o)\u5c31\u8fde\u7a7a\u6c14\u90fd\u662f\u5a92\u8d28\u3002\u6211\u662f\u600e\u4e48\u547c\u5438\u7684\uff1f$(br2)$(l)\u6211\u53c8\u662f\u600e\u4e48\u80fd\u5b58\u5728\u4e8e\u6b64\u7684\uff1f",
     "oneironaut.page.noosphere_materials.1": "\u4e00\u79cd\u5947\u602a\u7684\u6d41\u4f53\uff0c\u4f1a\u6405\u6df7\u8fdb\u5165\u5176\u4e2d\u7684\u5a92\u8d28\uff0c\u5e76\u963b\u6b62\u7d2b\u6c34\u6676\u6676\u4f53\u7684\u5f62\u6210\u3002\u6d78\u5728\u5176\u4e2d\u65f6\uff0c\u5b83\u4f1a\u4ee5\u6109\u60a6\u7684\u65b9\u5f0f\u523a\u6fc0\u6211\u7684\u610f\u8bc6\u3002",
     "oneironaut.page.noosphere_materials.2": "\u4e3b\u8981\u7531\u5a92\u8d28\u6784\u6210\u7684\u5ca9\u77f3\uff0c\u539f\u7406\u4e0d\u660e\u3002\u53ef\u5408\u6210\u6cd5\u672f\u73af\u65b9\u5757\u3002",
     "oneironaut.page.noosphere_materials.3": "\u4e00\u5927\u5757\u5a92\u8d28\u6676\u4f53\uff0c\u4e0e\u7d2b\u6c34\u6676\u7c7b\u4f3c\u4f46\u4e0d\u5b8c\u5168\u76f8\u540c\u3002\u89e6\u6478\u65f6\u4f1a\u6709\u79cd\u55e1\u9e23\u611f\uff0c\u5c31\u597d\u50cf\u5a92\u8d28\u81ea\u8eab\u5728\u523a\u6fc0\u795e\u7ecf\u4e00\u822c\u3002\u4e0d\u52a0\u4ee5\u7279\u6b8a\u63aa\u65bd\u76f4\u63a5\u7834\u574f\u4f1a\u5c06\u5176\u7834\u788e\u4e3a 1 \u5230 4 \u5757\u788e\u7247\u3002",
     "oneironaut.page.noosphere_materials.3.title": "\u4f2a\u7d2b\u6c34\u6676",
-    "oneironaut.page.noosphere_materials.4": "\u8fd9\u4e9b\u788e\u7247\u80fd\u9a71\u52a8\u6cd5\u672f\uff0c\u4e14\u6bd4\u666e\u901a\u7d2b\u6c34\u6676\u63d0\u4f9b\u7684\u80fd\u91cf\u7a0d\u591a\u4e00\u4e9b\u3002\u4f46\u662f\uff0c\u5b83\u4eec\u8c8c\u4f3c\u4f1a\u6392\u65a5\u4e00\u5207\u7269\u54c1\u7684\u5185\u90e8\u5a92\u8d28\u50a8\u5e93\u3002\u6211\u4e0d\u77e5\u9053\u4e3a\u4ec0\u4e48\u4f1a\u8fd9\u6837\uff0c\u4e0d\u8fc7\u666e\u901a\u7684\u5145\u80fd\u7d2b\u6c34\u6676\u66f4\u597d\u7528\u4e00\u4e9b\u3002",
+    "oneironaut.page.noosphere_materials.4": "\u8fd9\u4e9b\u788e\u7247\u80fd\u9a71\u52a8\u6cd5\u672f\uff0c\u4e14\u6bd4\u666e\u901a\u7d2b\u6c34\u6676\u63d0\u4f9b\u7684\u80fd\u91cf\u7a0d\u591a\u4e00\u4e9b\u3002\u4e5f\u80fd\u7528\u6765\u5236\u9020\u4e9b\u6709\u8da3\u7684\u7269\u4ef6\u3002",
+    "oneironaut.page.noosphere_materials.5": "\u4e00\u79cd\u56fa\u6001\u7684\u5a92\u8d28\uff0c\u7531\u601d\u7ef4\u6d46\u6db2\u5728\u5bcc\u5a92\u8d28\u73af\u5883\u4e2d\u51bb\u7ed3\u800c\u5f97\uff0c\u8fd9\u79cd\u51bb\u7ed3\u4e5f\u53ef\u7531\u5492\u672f\u9020\u6210\u3002$(br)\u5176\u8868\u9762\u7684\u6469\u64e6\u7cfb\u6570\u4f3c\u4e4e\u4e3a\u8d1f\uff0c\u4efb\u4f55\u5728\u5176\u4e0a\u6ed1\u52a8\u7684\u4e8b\u7269\u4f1a\u65e0\u9650\u52a0\u901f\uff08\u867d\u7136\u8f83\u6162\uff09\u3002",
+    "oneironaut.page.noosphere_materials.6": "\u4e00\u7c7b\u6781\u5176\u9ecf\u7a20\u7684\u5a92\u8d28\uff0c\u62e5\u6709\u6781\u4e3a\u57fa\u7840\u7684\u8ba4\u77e5\u80fd\u529b\uff0c\u4e0e\u9ecf\u83cc\u7c7b\u4f3c\u3002\u5b83\u901a\u5e38\u60c5\u51b5\u4e0b\u8868\u73b0\u51fa\u60f0\u6027\uff0c\u4f46\u4f1a\u4ee5\u7c7b\u4f3c\u6cd5\u672f\u7684\u80fd\u529b\u8bd5\u56fe\u56f0\u4f4f\u89e6\u78b0\u5230\u5b83\u7684\u4e8b\u7269\u3002",
     "oneironaut.page.paintconjured.1": "\u63a5\u53d7\u4e00\u4e2a\u5411\u91cf\u4e0e\u4ee3\u8868\u67d3\u8272\u5242\u7684\u7269\u54c1\u7c7b\u578b\u3002\u5982\u679c\u76ee\u6807\u4e3a\u6211\u81ea\u5df1\u7684\u65b9\u5757\uff0c\u6d88\u8017\u6781\u5c11\u91cf\u5a92\u8d28\uff1b\u5426\u5219\u6d88\u8017 1 \u4e2a\u7d2b\u6c34\u6676\u7c89\u3002",
     "oneironaut.page.paintconjured.2": "\u5c06\u6240\u7ed9\u4f4d\u7f6e\u5904\u6784\u7b51\u65b9\u5757\u7684\u989c\u8272\u8bbe\u7f6e\u4e3a\u6240\u7ed9\u67d3\u8272\u5242\u7684\u989c\u8272\uff1b\u5982\u679c\u9001\u5165\u7684\u662f Null\uff0c\u5219\u5c06\u5176\u8bbe\u7f6e\u4e3a\u6211\u610f\u8bc6\u7684\u989c\u8272\u3002$(br2)\u4e0d\u4fdd\u8bc1\u5bf9\u975e\u4f20\u7edf\u7684\u6784\u7b51\u7269\u8d28\u6709\u6548\u3002",
     "oneironaut.page.paintconjured.3": "\u8fd9\u79cd\u6548\u679c\u6709\u7740\u5947\u602a\u7684\u5e86\u5178\u611f\uff0c\u5c31\u597d\u50cf\u5b83\u66fe\u7528\u4e8e\u67d0\u4e2a\u76db\u5927\u7684\u8282\u5e86\u6d3b\u52a8\uff0c\u4e0e\u4f1a\u961f\u4f0d\u4f1a\u628a\u81ea\u5df1\u961f\u7684\u989c\u8272\u6cfc\u6d12\u5230\u5bf9\u624b\u7684\u9886\u5730\u4e0a\uff0c\u7c7b\u4f3c\u4e8e\u610f\u8bc6\u5c42\u9762\u4e0a\u7684\u5360\u9886\u3002",
     "oneironaut.page.particleburst.1": "\u63a5\u53d7\u4e24\u4e2a\u5411\u91cf\u548c\u4e24\u4e2a\u6570\uff0c\u5e76\u7531\u5176\u89e6\u53d1\u4e00\u675f\u7c92\u5b50\u3002\u6d88\u8017\u6781\u5c11\u91cf\u5a92\u8d28\u3002",
     "oneironaut.page.particleburst.2": "\u7b2c\u4e00\u4e2a\u5411\u91cf\u51b3\u5b9a\u4e86\u7c92\u5b50\u675f\u7684\u8d77\u59cb\u4f4d\u7f6e\uff0c\u7b2c\u4e8c\u4e2a\u5411\u91cf\u5219\u51b3\u5b9a\u5176\u65b9\u5411\u548c\u901f\u5ea6\u3002\u7b2c\u4e00\u4e2a\u6570\u51b3\u5b9a\u5404\u4f4d\u7f6e\u5411\u91cf\u5206\u91cf\u9644\u52a0\u591a\u5927\u7684\u968f\u673a\u6570\uff0c\u7b2c\u4e8c\u4e2a\u6570\u5219\u4ee5\u540c\u79cd\u65b9\u5f0f\u51b3\u5b9a\u65b9\u5411\u5411\u91cf\u7684\u968f\u673a\u6027\u3002",
     "oneironaut.page.raycast_assailant.1": "\u5f80\u65b9\u5757\u4e2d\u201c\u7ec7\u5165\u201d\u4f2a\u7d2b\u6c34\u6676\uff0c\u4ea7\u7269\u4fbf\u80fd\u4ee4\u62b5\u8fbe\u6216\u7a7f\u8fc7\u5176\u7684\u5c04\u7ebf\u8ffd\u8e2a\uff08\u5bf9\u5b9e\u4f53\u7684\u5c04\u7ebf\u8ffd\u8e2a\u4e5f\u6709\u6548\uff09\u8fd4\u56de Null\uff0c\u5c31\u597d\u50cf\u5c04\u7ebf\u8ffd\u8e2a\u6ca1\u6709\u68c0\u6d4b\u5230\u4efb\u4f55\u4e8b\u7269\u4e00\u6837\u3002",
+    "oneironaut.page.raycast_assailant.3": "\u5947\u602a\u7684\u662f\uff0c\u4ee5\u540c\u79cd\u65b9\u5f0f\u52a0\u5de5\u4f2a\u7d2b\u6c34\u6676\u548c\u9ed1\u66dc\u77f3\u7684\u4ea7\u7269\u4e0d\u5177\u5907\u963b\u788d\u5c04\u7ebf\u8ffd\u8e2a\u7684\u80fd\u529b\uff0c\u800c\u662f\u53d8\u5f97\u8fd1\u4e4e\u65e0\u6cd5\u88ab\u5492\u672f\u6467\u6bc1\u3002However, the resultant block loses much of its durability, being no stronger than common stone (though it retains its blast resistance).",
     "oneironaut.page.rod.1": "\u6211\u53d1\u73b0\u6211\u80fd\u7528\u8fdc\u53e4\u57ce\u5e02\u4e2d\u627e\u5230\u7684\u5947\u602a\u788e\u7247\u5408\u6210\u4e00\u79cd\u5947\u5f02\u7684\u65bd\u6cd5\u7269\u54c1\u3002$(br)\u8fd9\u4ef6\u7269\u54c1\u7684\u5947\u5f02\u4e4b\u5904\uff0c\u5c31\u5728\u4e8e\u96c6\u4e2d\u601d\u7ef4\u65f6\uff0c\u5b83\u80fd\u4ee5\u6bcf\u79d2 20 \u6b21\u7684\u9891\u7387\u65bd\u653e\u5176\u4e2d\u7684\u5492\u672f\uff0c\u76f4\u5230\u4ea7\u751f\u4e8b\u6545\u6216\u8005\u6211\u65bd\u653e\u7ec8\u66f2\u548c\u5b89\u53ef\u65f6\u624d\u505c\u6b62\u3002\u5982\u6b64\u4f1a\u89e6\u53d1\u4e00\u6bb5\u51b7\u5374\u65f6\u95f4\uff0c\u901a\u5e38\u6709\u5927\u7ea6 1 \u79d2\u3002",
-    "oneironaut.page.rod.10": "\u56de\u54cd\u788e\u7247\u4e5f\u53ef\u7528\u4e8e\u5236\u9020\u6cd5\u6756\uff0c\u4e0d\u8fc7\u8fd9\u79cd\u6cd5\u6756\u552f\u4e00\u7684\u7279\u6b8a\u6027\u8d28\u4fbf\u662f\u53d1\u51fa\u4e9b\u5e7d\u533f\u7684\u58f0\u97f3\u3002",
+    "oneironaut.page.rod.10": "\u63a5\u53d7\u4e00\u4e2a\u975e\u5217\u8868 iota\uff0c\u5e76\u5c06\u5176\u5b58\u5165\u5f53\u524d\u5faa\u73af\u3002\u8be5 iota \u4f1a\u5728\u5faa\u73af\u7ed3\u675f\u65f6\u4e22\u5931\u3002",
+    "oneironaut.page.rod.11": "\u8fd4\u56de\u5f53\u524d\u5faa\u73af\u4e2d\u5b58\u50a8\u7684 iota\u3002\u9ed8\u8ba4\u4e3a Null\u3002",
+    "oneironaut.page.rod.12": "\u56de\u54cd\u788e\u7247\u4e5f\u53ef\u7528\u4e8e\u5236\u9020\u6cd5\u6756\uff0c\u4e0d\u8fc7\u8fd9\u79cd\u6cd5\u6756\u552f\u4e00\u7684\u7279\u6b8a\u6027\u8d28\u4fbf\u662f\u53d1\u51fa\u4e9b\u5e7d\u533f\u7684\u58f0\u97f3\u3002",
     "oneironaut.page.rod.2": "\u56de\u54cd\u788e\u7247\u4f3c\u4e4e\u5305\u542b\u7740\u67d0\u79cd\u602a\u5f02\u5f62\u6001\u7684\u5a92\u8d28\u3002\u56e0\u6b64\u5b83\u5177\u6709\u5faa\u73af\u81ea\u8eab\u7684\u503e\u5411\uff0c\u540c\u65f6\u4f1a\u4fdd\u7559\u4e00\u90e8\u5206\u4e0a\u4e00\u6b21\u65bd\u6cd5\u65f6\u7684\u4fe1\u606f\u3002",
     "oneironaut.page.rod.3": "\u548c$(l:patterns/spells/hexcasting)\u7528\u4e8e\u5236\u9020\u4f20\u7edf\u65bd\u6cd5\u7269\u54c1\u7684\u6cd5\u672f$()\u7c7b\u4f3c\u3002\u6d88\u8017 10 \u4e2a\u5145\u80fd\u7d2b\u6c34\u6676\u3002",
     "oneironaut.page.rod.4": "\u4f7f\u7528\u56de\u54cd\u4e4b\u6756\u65bd\u653e\u65f6\uff0c\u8fd4\u56de\u5f53\u524d\u5faa\u73af\u5f00\u59cb\u65f6\u6211\u7684\u89c6\u7ebf\u5411\u91cf\u3002",
     "oneironaut.page.rod.5": "\u4f7f\u7528\u56de\u54cd\u4e4b\u6756\u65bd\u653e\u65f6\uff0c\u8fd4\u56de\u5f53\u524d\u5faa\u73af\u5f00\u59cb\u65f6\u6211\u7684\u773c\u90e8\u4f4d\u7f6e\u3002",
     "oneironaut.page.rod.6": "\u4f7f\u7528\u56de\u54cd\u4e4b\u6756\u65bd\u653e\u65f6\uff0c\u8fd4\u56de\u5f53\u524d\u5faa\u73af\u5f00\u59cb\u65f6\u7684\u65f6\u95f4\u6233\u3002",
     "oneironaut.page.rod.7": "\u63a5\u53d7\u4e00\u4e2a\u6b63\u6574\u6570\u3002\u4f7f\u7528\u56de\u54cd\u4e4b\u6756\u65bd\u653e\u65f6\uff0c\u5c06\u4e0b\u4e00\u6b21\u65bd\u6cd5\u5ef6\u8fdf\u6240\u7ed9\u6570\u4e2a 1/20 \u79d2\u3002",
     "oneironaut.page.rod.8": "\u4f7f\u7528\u56de\u54cd\u4e4b\u6756\u65bd\u653e\u65f6\uff0c\u5f3a\u5236\u505c\u6b62\u5f53\u524d\u5faa\u73af\u3002",
@@ -142,37 +231,40 @@
     "oneironaut.page.sentinel_detection.3": "\u9664\u6b64\u4e4b\u5916\uff0c\u8fd9\u79cd\u63a2\u6d4b\u5668\u8fd8\u53ef\u6574\u5408\u5230\u7267\u5e08\u4fc3\u52a8\u77f3\u4e2d\uff0c\u4ea7\u7269\u4f1a\u5728\u533a\u57df\u5185\u5b58\u5728\u54e8\u536b\u65f6\u542f\u52a8\uff08\u4e0d\u8fc7\u63a2\u6d4b\u534a\u5f84\u8f83\u666e\u901a\u63a2\u6d4b\u5668\u8f83\u4f4e\uff09\u3002\u6211\u53eb\u8fd9\u79cd\u88c5\u7f6e\u201c\u63a2\u5bdf\u4fc3\u52a8\u77f3\u201d\u3002\u5c3d\u7ba1\u5b83\u4e0d\u518d\u5bf9\u7ea2\u77f3\u4fe1\u53f7\u4ea7\u751f\u53cd\u5e94\uff0c\u4f46\u4f1a\u83b7\u53d6\u4ee3\u8868\u89e6\u53d1\u54e8\u536b\u7684\u6240\u6709\u8005\u7684 iota\uff0c\u5e76\u7f6e\u5165\u6cd5\u672f\u73af\u5492\u672f\u7684\u521d\u59cb\u6808\u3002$(br)\u800c\u7531\u4e8e\u65bd\u6cd5\u65f6\u4ea7\u751f\u7684\u5a92\u8d28\u5e72\u6270\uff0c\u8fd9\u79cd\u4fc3\u52a8\u77f3\u65e0\u6cd5\u4fa6\u6d4b\u5230\u81ea\u8eab\u653e\u7f6e\u7684\u54e8\u536b\u3002",
     "oneironaut.page.sentinel_detection.4": "\u8fd9\u79cd\u63a2\u6d4b\u5668\u4e0d\u8bba\u4fa6\u6d4b\u5230\u8c01\u7684\u54e8\u536b\u90fd\u4e3a\u4ea7\u751f\u53cd\u5e94\uff0c\u6211\u5e94\u5f53\u907f\u514d\u8ba9\u6211\u94fa\u8bbe\u7684\u9677\u9631\u6cd5\u672f\u73af\u7784\u51c6\u6211\u81ea\u5df1\u3002",
     "oneironaut.page.sentinel_detection.5": "\u63a5\u53d7\u4e00\u4e2a\u5411\u91cf\u548c\u4e00\u4e2a\u73a9\u5bb6\uff0c\u5e76\u8fd4\u56de\u8be5\u4f4d\u7f6e\u5230\u6240\u7ed9\u73a9\u5bb6\u54e8\u536b\u7684\u8ddd\u79bb\uff0c\u6216\u8005\u8fd4\u56de Null\u3002\u6d88\u8017\u6781\u5c11\u91cf\u5a92\u8d28\u3002",
     "oneironaut.page.sentinel_detection.6": "\u5728\u6240\u7ed9\u4f4d\u7f6e\u5750\u6807\u6784\u7b51\u4e00\u4e2a\u77ed\u65f6\u63a2\u6d4b\u5668\uff0c\u5b83\u4f1a\u201c\u76d1\u542c\u201d\u73af\u5883\u5a92\u8d28\u4e2d\u7684\u6a21\u5f0f\uff0c\u4ee5\u6b64\u5206\u8fa8\u51fa\u6700\u4e3a\u660e\u663e\u7684\u54e8\u536b\u6807\u8bb0\u3002",
     "oneironaut.page.slipway_hint.1": "\u90a3\u4e9b\u8d28\u9053\uff0c\u5b83\u4eec\u4e00\u5b9a\u80fd\u8054\u901a\u5230$(o)\u67d0\u4e9b\u5730\u65b9$()\u3002\u5492\u7075\u4e0d\u4f1a\u51ed\u7a7a\u51fa\u73b0\u3002\u4e0d\u7ba1\u6211\u600e\u4e48\u5c1d\u8bd5\uff0c\u6211\u6700\u591a\u53ea\u80fd\u8ba9\u4e00\u6839\u624b\u6307\u7a7f\u8fc7\u90a3\u9053\u6df7\u6c8c\u7684\u88c2\u53e3\u3002$(br2)\u6211\u5927\u6982\u662f\u60f3\u9519\u4e86\u3002\u4e0e\u5176\u51ed\u86ee\u529b\u7a7f\u8fc7\u88c2\u53e3\uff0c\u4e5f\u8bb8\u8fd8\u662f\u5c1d\u8bd5\u5e73\u606f\u98ce\u66b4\u66f4\u4e3a\u6709\u6548\u3002",
     "oneironaut.page.slipway_hint.2": "\u5927\u91cf\u7684\u8c03\u8c10\u5a92\u8d28\u5e94\u8be5\u5c31\u80fd\u505a\u5230\u2026\u2026",
     "oneironaut.page.slipway_hint.2.title": "\u55ef\u2026\u2026",
+    "oneironaut.page.soulprints.1": "\u7075\u9b42\u5370\u8bb0\u548c\u4ee3\u8868\u6211\u81ea\u5df1\u7684 iota \u7c7b\u4f3c\uff0c\u529f\u80fd\u4e2d\u4e5f\u6709\u201c\u4ee3\u8868\u6211\u201d\u8fd9\u4e00\u9879\uff0c\u4f46\u4f7f\u7528\u7684\u9650\u5236\u4f1a\u591a\u51fa\u8bb8\u591a\u3002\u9664\u4e86\u901a\u8fc7\u6211\u672c\u4eba\u4e4b\u5916\uff0c\u4ed6\u4eba\u6ca1\u6709\u65b9\u5f0f\u83b7\u5f97\u7075\u9b42\u5370\u8bb0\uff0c\u4e0d\u8fc7\u8fd9\u4e9b\u7075\u9b42\u5370\u8bb0\u4e0d\u53d7\u5199\u5165\u9650\u5236\uff0c\u548c\u666e\u901a\u7684\u73a9\u5bb6 iota \u4e0d\u4e00\u6837\u3002$(br2)\u6709\u610f\u601d\u7684\u662f\uff0c\u7075\u9b42\u5370\u8bb0\u4e5f\u662f$(l:patterns/idea_inscription)\u601d\u7eea\u523b\u5370$(/l)\u7684\u6709\u6548\u952e\u3002",
+    "oneironaut.page.soulprints.2": "\u8fd4\u56de\u6211\u81ea\u5df1\u7684\u7075\u9b42\u5370\u8bb0\uff0c\u4f7f\u7528\u9664\u6cd5\u6756\u4e4b\u5916\u7684\u65bd\u6cd5\u624b\u6bb5\u65f6\u4f1a\u62db\u81f4\u4e8b\u6545\u3002\u6d88\u8017\u6781\u5c11\u91cf\u5a92\u8d28\u3002",
+    "oneironaut.page.soulprints.3": "\u5c06\u6211\u7684\u7075\u9b42\u5370\u8bb0\u9690\u5199\u5230\u53e6\u4e00\u53ea\u624b\u4e2d\u7684\u7269\u54c1\u4e0a\uff0c\u82e5\u5df2\u6709\u7075\u9b42\u5370\u8bb0\u5219\u6e05\u9664\u3002\u6d88\u8017 1 \u4e2a\u7d2b\u6c34\u6676\u7c89\u3002$(br)\u7b7e\u5370\u7269\u54c1\u524d\u8981\u6ce8\u610f\u5148\u5c06\u6838\u5fc3\u4e00\u7c7b\u7684\u7269\u54c1\u5bc6\u5c01\uff0c\u7ecf\u8fc7\u7b7e\u5370\u7684\u672a\u5bc6\u5c01\u6838\u5fc3\u6709\u8eab\u4efd\u6cc4\u9732\u7684\u98ce\u9669\uff0c\u6e05\u9664\u7269\u54c1\u4f1a\u540c\u65f6\u53bb\u9664\u7b7e\u5370\u3002",
+    "oneironaut.page.soulprints.4": "\u63a5\u53d7\u4e00\u4e2a\u7075\u9b42\u5370\u8bb0\uff0c\u5e76\u68c0\u67e5\u6211\u53e6\u4e00\u53ea\u624b\u4e2d\u7269\u54c1\u4e0a\u662f\u5426\u6709\u5bf9\u5e94\u7684\u9690\u5199\u3002\u82e5\u6709\uff0c\u8fd4\u56de True\uff1b\u5426\u5219\u8fd4\u56de False\u3002\u6d88\u8017\u6781\u5c11\u91cf\u5a92\u8d28\u3002",
     "oneironaut.page.spaceswap.1": "\u63a5\u53d7\u5747\u7531\u4e24\u4e2a\u5411\u91cf\u7ec4\u6210\u7684\u4e24\u4e2a\u5217\u8868\uff0c\u7528\u4e8e\u5b9a\u4e49\u4e24\u4e2a\u957f\u65b9\u4f53\uff0c\u4ee5\u53ca\u4e00\u4e2a\u7a7a\u95f4\u5370\u8bb0\u3002\u6240\u5b9a\u4e49\u7684\u957f\u65b9\u4f53\u5fc5\u987b\u4fdd\u8bc1\u5c3a\u5bf8\u4e0e\u671d\u5411\u4e00\u81f4\u3002",
     "oneironaut.page.spaceswap.2": "\u6211\u4e0d\u592a\u6e05\u695a\u8fd9\u4e2a\u56fe\u6848\u5177\u4f53\u80fd\u505a\u4ec0\u4e48\uff0c\u5b83\u603b\u662f\u53eb\u558a\u7740\u4ec0\u4e48\u7279\u6b8a\u7ef4\u5ea6\u3002\u4e5f\u8bb8\u5b83\u9700\u8981\u8fd9\u79cd\u7279\u6b8a\u7ef4\u5ea6\u4f5c\u4e3a\u4e2d\u4ecb\uff1f",
     "oneironaut.page.spaceswap.3": "\u5c06\u6211\u6240\u5904\u7ef4\u5ea6\u4e2d\u7b2c\u4e00\u4e2a\u957f\u65b9\u4f53\u5305\u542b\u7684\u65b9\u5757\uff08\u9700\u5728\u5f71\u54cd\u8303\u56f4\u5185\uff09\u4e0e\u7a7a\u95f4\u5370\u8bb0\u5bf9\u5e94\u7ef4\u5ea6\u4e2d\u7b2c\u4e8c\u4e2a\u957f\u65b9\u4f53\u5305\u542b\u7684\u65b9\u5757\u4e92\u6362\u3002\u6d88\u8017 5 \u4e2a\u5145\u80fd\u7d2b\u6c34\u6676\uff0c\u957f\u65b9\u4f53\u4e2d\u6bcf 1 \u7acb\u65b9\u7c73\u989d\u5916\u6d88\u8017 1/2 \u4e2a\u7d2b\u6c34\u6676\u7c89\u3002$(br)\u4e0d\u4f1a\u4e92\u6362\u4e0d\u53ef\u7834\u574f\u7684\u65b9\u5757\uff0c\u5bf9\u5305\u542b\u5927\u91cf\u6570\u636e\u7684\u65b9\u5757\u4e5f\u65e0\u6548\u3002$(br)\u4e24\u7ef4\u5ea6\u4e4b\u4e00\u6216\u4e24\u8005\u5747\u9700\u4e3a\u667a\u8bc6\u754c\u3002",
     "oneironaut.page.spaceswap.4": "\u4e24\u7ef4\u5ea6\u4e4b\u4e00\u6216\u4e24\u8005\u5747\u9700\u4e3a\u667a\u8bc6\u754c\u3002",
     "oneironaut.page.status_iotas.1": "\u8fd9\u4e9b\u56fe\u6848\u4e3b\u8981\u64cd\u4f5c\u4ee3\u8868\u751f\u7269\u8eab\u4e0a\u957f\u65f6\u6548\u679c\u7684 iota\uff0c\u6211\u53ef\u4ee5\u7528\u8fd9\u4e9b\u56fe\u6848\u8bc4\u4f30\u751f\u7269\u7684\u72b6\u6001\uff0c\u6bd4\u53ea\u7528\u62a4\u58eb\u4e4b\u7eaf\u5316\u66f4\u52a0\u6df1\u5165\u5f7b\u5e95\u3002$(br)\u867d\u7136\u6211\u7684\u7814\u7a76\u8868\u660e\u4ee3\u8868\u77ac\u65f6\u6548\u679c\u7684\u72b6\u6001 iota \u4e5f\u53ef\u80fd\u5b58\u5728\uff0c\u4f46\u975e\u5e38\u96be\u4ee5\u83b7\u53d6\uff0c\u800c\u4e14\u6211\u76ee\u524d\u6ca1\u60f3\u5230\u4efb\u4f55\u6709\u5173\u7528\u9014\u3002",
     "oneironaut.page.status_iotas.10": "\u82e5\u662f\u8981\u79fb\u9664\u975e\u81ea\u8eab\u5b9e\u4f53\u8eab\u4e0a\u7684\u6b63\u9762\u6548\u679c\uff0c\u5219\u6d88\u8017\u4f1a\u589e\u52a0\u3002$(br2)\u6240\u6709\u9700\u8981\u68c0\u6d4b\u5b9e\u4f53\u8eab\u4e0a\u6709\u65e0\u6240\u7ed9\u72b6\u6001\u6548\u679c\u7684\u56fe\u6848\u90fd\u6709\u526f\u4f5c\u7528\u3002\u5982\u679c\u8be5\u5b9e\u4f53\u5f53\u524d\u6ca1\u6709\u8fd9\u79cd\u6548\u679c\uff0c\u5219\u56fe\u6848\u4f1a\u5931\u6548\uff0c\u5e76\u7ed9\u4e88\u6211\u53cd\u80c3\u3002",
-    "oneironaut.page.status_iotas.2": "\u63a5\u53d7\u4e00\u4e2a\u751f\u7269\uff0c\u5e76\u8fd4\u56de\u76ee\u6807\u5f53\u524d\u6240\u6709\u6548\u679c\u7ec4\u6210\u7684 iota\u3002",
+    "oneironaut.page.status_iotas.2": "\u63a5\u53d7\u4e00\u4e2a\u751f\u7269\uff0c\u5e76\u8fd4\u56de\u76ee\u6807\u5f53\u524d\u6240\u6709\u6548\u679c\u7ec4\u6210\u7684\u5217\u8868 iota\u3002",
     "oneironaut.page.status_iotas.3": "\u63a5\u53d7\u4e00\u4e2a\u72b6\u6001\u6548\u679c\uff0c\u5e76\u6839\u636e\u8be5\u6548\u679c\u5bf9\u751f\u7269\u4ea7\u751f\u6b63\u9762\u3001\u8d1f\u9762\uff0c\u6216\u4e2d\u6027\u5f71\u54cd\u8fd4\u56de\u4e00\u4e2a\u6570\u3002",
     "oneironaut.page.status_iotas.4": "\u63a5\u53d7\u4e00\u4e2a\u5b9e\u4f53\u548c\u4e00\u4e2a\u72b6\u6001\u6548\u679c\uff0c\u5e76\u8fd4\u56de\u76ee\u6807\u8eab\u4e0a\u6240\u7ed9\u72b6\u6001\u6548\u679c\u7684\u6301\u7eed\u65f6\u95f4\uff0c\u4ee5\u79d2\u8ba1\u3002",
     "oneironaut.page.status_iotas.5": "\u63a5\u53d7\u4e00\u4e2a\u5b9e\u4f53\u548c\u4e00\u4e2a\u72b6\u6001\u6548\u679c\uff0c\u5e76\u8fd4\u56de\u76ee\u6807\u8eab\u4e0a\u6240\u7ed9\u72b6\u6001\u6548\u679c\u7684\u5f3a\u5ea6\u3002",
     "oneironaut.page.status_iotas.6": "\u63a5\u53d7\u4e00\u4e2a\u72b6\u6001\u6548\u679c\u548c\u4e00\u4e2a\u5411\u91cf\uff0c\u5e76\u8fd4\u56de\u8be5\u5904\u5e26\u6709\u8be5\u72b6\u6001\u6548\u679c\u7684\u5b9e\u4f53\u3002",
     "oneironaut.page.status_iotas.7": "\u63a5\u53d7\u4e00\u4e2a\u72b6\u6001\u6548\u679c\uff0c\u4e00\u4e2a\u5411\u91cf\u548c\u4e00\u4e2a\u6570\uff0c\u8fd4\u56de\u8be5\u4f4d\u7f6e\u7ed9\u5b9a\u8ddd\u79bb\u8303\u56f4\u5185\u6240\u6709\u5e26\u6709\u7ed9\u5b9a\u72b6\u6001\u6548\u679c\u751f\u7269\u7684\u5217\u8868\u3002",
     "oneironaut.page.status_iotas.8": "\u63a5\u53d7\u4e00\u4e2a\u72b6\u6001\u6548\u679c\uff0c\u4e00\u4e2a\u5411\u91cf\u548c\u4e00\u4e2a\u6570\uff0c\u8fd4\u56de\u8be5\u4f4d\u7f6e\u7ed9\u5b9a\u8ddd\u79bb\u8303\u56f4\u5185\u6240\u6709\u65e0\u7ed9\u5b9a\u72b6\u6001\u6548\u679c\u751f\u7269\u7684\u5217\u8868\u3002",
     "oneironaut.page.status_iotas.9": "\u63a5\u53d7\u4e00\u4e2a\u5b9e\u4f53\u548c\u4e00\u4e2a\u72b6\u6001\u6548\u679c\uff0c\u5e76\u79fb\u9664\u8be5\u5b9e\u4f53\u8eab\u4e0a\u7684\u6240\u7ed9\u72b6\u6001\u6548\u679c\u3002\u6d88\u8017\u7531\u6548\u679c\u81ea\u8eab\u7684\u4f24\u5bb3\u6027\u3001\u5f3a\u5ea6\u3001\u5269\u4f59\u6301\u7eed\u65f6\u95f4\u51b3\u5b9a\u3002",
     "oneironaut.page.super_budding.1": "\u6211\u53d1\u73b0\u667a\u8bc6\u754c\u51fa\u4ea7\u7684\u4e00\u79cd\u7c7b\u7d2b\u6c34\u6676\u7269\u8d28\u4f1a\u63a5\u53d7\u6751\u6c11\u7684\u610f\u8bc6\uff0c\u8fd9\u70b9\u4e0a\u548c\u666e\u901a\u7684\u7d2b\u6c34\u6676\u4e00\u6837\u3002\u6b64\u5916\uff0c\u8fd9\u4e00\u8fc7\u7a0b\u5f97\u5230\u7684\u65b9\u5757\u4ea7\u51fa\u7684\u5a92\u8d28\u91cf\u6bd4\u666e\u901a\u7684\u7d2b\u6c34\u6676\u6bcd\u5ca9\u591a\u51fa\u8bb8\u591a\uff0c\u5e76\u4e14\u53ea\u8981\u8db3\u591f\u5c0f\u5fc3\u5c31\u80fd\u6361\u8d77\u642c\u8fd0\u3002",
     "oneironaut.page.super_budding.2": "\u6bd4\u8d77\u666e\u901a\u7d2b\u6c34\u6676\u6765\u8bf4\uff0c\u4f2a\u7d2b\u6c34\u6676\u9700\u8981\u66f4\u5f3a\u5927\u7684\u610f\u8bc6\uff0c\u4f46\u5f97\u5230\u7684\u56de\u62a5\u7edd\u5bf9\u503c\u5f97\u3002",
-    "oneironaut.page.super_budding.3": "\u4f2a\u7d2b\u6c34\u6676\u6bcd\u5ca9\u6709\u4e00\u5947\u7279\u4e4b\u5904\uff0c\u5c31\u7b97\u6d78\u6ca1\u5728\u601d\u7ef4\u6d46\u6db2\u4e2d\u6291\u5236\u6676\u4f53\u5f62\u6210\uff0c\u5176\u5a92\u8d28\u751f\u6210\u7387\u4f9d\u7136\u8db3\u591f\u5e73\u5e38\u4f7f\u7528\u3002\u5c3d\u7ba1\u603b\u4f9b\u7ed9\u91cf\u8fd1\u4e4e\u65e0\u7a77\uff0c\u4f46\u4efb\u4e00\u64cd\u4f5c\u80fd\u4f7f\u7528\u7684\u5a92\u8d28\u91cf\u5219\u76f8\u5f53\u5c11\uff0c\u5c31\u50cf\u4e00\u7247\u51e0\u5341\u4e07\u51e0\u767e\u4e07\u5343\u7c73\u5bbd\u4f46\u53ea\u6709\u51e0\u5398\u7c73\u6df1\u7684\u6d77\u6d0b\u3002$(br)\u6211\u5e94\u8be5\u6ce8\u610f\u5728\u7269\u54c1\u680f\u4e2d\u628a\u5b83\u653e\u5728\u5176\u4ed6\u5a92\u8d28\u4e4b\u74f6\u524d\u9762\uff0c\u4e0d\u7136\u4e0d\u4f1a\u4f18\u5148\u4f7f\u7528\u5b83\u4eec\u3002",
+    "oneironaut.page.super_budding.3": "\u4f2a\u7d2b\u6c34\u6676\u6bcd\u5ca9\u6709\u4e00\u5947\u7279\u4e4b\u5904\uff0c\u5c31\u7b97\u6d78\u6ca1\u5728\u601d\u7ef4\u6d46\u6db2\u4e2d\u6291\u5236\u6676\u4f53\u5f62\u6210\uff0c\u5176\u5a92\u8d28\u751f\u6210\u7387\u4f9d\u7136\u8db3\u591f\u5e73\u5e38\u4f7f\u7528\u3002\u5c3d\u7ba1\u603b\u4f9b\u7ed9\u91cf\u8fd1\u4e4e\u65e0\u7a77\uff0c\u4f46\u4efb\u4e00\u64cd\u4f5c\u80fd\u4f7f\u7528\u7684\u5a92\u8d28\u91cf\u76f8\u5f53\u5c11\uff0c\u5c31\u50cf\u4e00\u7247\u51e0\u5341\u4e07\u51e0\u767e\u4e07\u5343\u7c73\u5bbd\u4f46\u53ea\u6709\u51e0\u5398\u7c73\u6df1\u7684\u6d77\u6d0b\u3002\u800c\u4e14\uff0c\u7531\u4e8e\u5176\u6df1\u5ea6\u6781\u4e3a\u6709\u9650\uff0c\u82e5\u8981\u5982\u4e3a\u7269\u54c1\u5145\u80fd\u7b49\u8fdc\u8ddd\u83b7\u53d6\u4f7f\u7528\uff0c\u5176\u4e2d\u7684\u5a92\u8d28\u4f1a\u5728\u62b5\u8fbe\u6cd5\u6756\u524d\u8fc5\u901f\u6d88\u6563\u3002",
     "oneironaut.page.super_budding.4": "\u5e38\u6001\u63d0\u4f9b\u5927\u7ea6\u4e0e 1/10 \u4e2a\u7d2b\u6c34\u6676\u7c89\u76f8\u5f53\u7684\u5a92\u8d28\u3002\u867d\u7136\u6211$(o)\u53ef\u4ee5$()\u540c\u65f6\u6301\u6709\u597d\u591a\u4e2a\u4ee5\u8f7b\u677e\u83b7\u53d6\u5a92\u8d28\uff0c\u4f46\u6bcf\u4e2a\u5a92\u8d28\u74f6\u7684\u589e\u91cf\u4f1a\u5feb\u901f\u51cf\u5c11\u3002",
     "oneironaut.page.wisp_lanterns.1": "\u6211\u53d1\u73b0\uff0c\u82e5\u662f\u4f7f\u7528\u4e86\u72ec\u5c5e\u4e8e\u667a\u8bc6\u754c\u7684\u6750\u6599\uff0c\u4fbf\u80fd\u5236\u9020\u51fa\u4e00\u79cd\u7279\u6b8a\u7684\u7f50\u5b50\uff0c\u5b83\u80fd\u4ea7\u751f\u5e76\u5bb9\u7eb3\u4e00\u53ea\u5fae\u578b\u5492\u7075\u3002\u8fd9\u79cd\u5492\u7075\u5c3d\u7ba1\u65e0\u6cd5\u65bd\u6cd5\uff0c\u4f46\u80fd\u53d1\u51fa\u76f8\u5f53\u7684\u5149\uff0c\u8fd8\u4f1a\u6a21\u62df\u5b83\u770b\u89c1\u7684\u67d3\u8272\u5242\u3002$(br)\u6211\u8fd8\u80fd\u7528\u906e\u5149\u73bb\u7483\u5236\u9020\u540c\u7c7b\u7269\u54c1\uff0c\u907f\u514d\u5492\u7075\u7684\u5149\u4eae\u5f71\u54cd\u5230\u6211\u4e66\u623f\u7684\u7f8e\u5b66\u8bbe\u8ba1\u3002",
     "text.oneironaut.clearIdeasResponse": "\u5df2\u6e05\u9664iota\u5b58\u50a8\u6620\u5c04\u3002",
     "text.oneironaut.lorem_ipsum": "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
-    "text.oneironaut.noforgeyet": "\u6b64\u7279\u6027\u76ee\u524d\u6682\u672a\u5728Forge\u4e0a\u5b9e\u88c5\u3002\u975e\u5e38\u62b1\u6b49\uff01",
     "this.is.a.comment.1": "Pattern names--------------------------------------------------------------------------------------------",
     "this.is.a.comment.2": "Block/Item names--------------------------------------------------------------------------------------------",
     "this.is.a.comment.3": "Book entry titles--------------------------------------------------------------------------------------------",
     "this.is.a.comment.4": "Book pages--------------------------------------------------------------------------------------------",
     "this.is.a.comment.5": "Advancements--------------------------------------------------------------------------------------------",
     "this.is.a.comment.6": "Mishaps--------------------------------------------------------------------------------------------",
-    "this.is.a.comment.7": "Other?--------------------------------------------------------------------------------------------"
+    "this.is.a.comment.7": "Other---------------------------------------------------------------------------------------------"
 }
```

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/circle.json` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/circle.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/reverberation_rod.json` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/reverberation_rod.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/sentinel_sensor.json` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/block/sentinel_trap_powered.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8691798941798942%*

 * *Differences: {"'display'": "{'gui': {'scale': {insert: [(1, 0.625)], delete: [1]}}, 'ground': {'scale': "*

 * *              "{insert: [(1, 0.25)], delete: [1]}}, 'fixed': {'scale': {insert: [(1, 0.5)], "*

 * *              "delete: [1]}}, 'thirdperson_righthand': {'scale': {insert: [(1, 0.375)], delete: "*

 * *              "[1]}}, 'firstperson_righthand': {'scale': {insert: [(1, 0.4)], delete: [1]}}, "*

 * *              "'firstperson_lefthand': {'scale': {insert: [(1, 0.4)], delete: [1]}}}",*

 * * "'elements'": "{0: {'faces': {'north': {'uv' […]*

```diff
@@ -5,15 +5,15 @@
             "rotation": [
                 0,
                 225,
                 0
             ],
             "scale": [
                 0.4,
-                0.15,
+                0.4,
                 0.4
             ],
             "translation": [
                 0,
                 0,
                 0
             ]
@@ -22,15 +22,15 @@
             "rotation": [
                 0,
                 45,
                 0
             ],
             "scale": [
                 0.4,
-                0.15,
+                0.4,
                 0.4
             ],
             "translation": [
                 0,
                 0,
                 0
             ]
@@ -39,15 +39,15 @@
             "rotation": [
                 0,
                 0,
                 0
             ],
             "scale": [
                 0.5,
-                0.1875,
+                0.5,
                 0.5
             ],
             "translation": [
                 0,
                 0,
                 0
             ]
@@ -56,15 +56,15 @@
             "rotation": [
                 0,
                 0,
                 0
             ],
             "scale": [
                 0.25,
-                0.09375,
+                0.25,
                 0.25
             ],
             "translation": [
                 0,
                 3,
                 0
             ]
@@ -73,15 +73,15 @@
             "rotation": [
                 30,
                 225,
                 0
             ],
             "scale": [
                 0.625,
-                0.234375,
+                0.625,
                 0.625
             ],
             "translation": [
                 0,
                 0,
                 0
             ]
@@ -90,15 +90,15 @@
             "rotation": [
                 75,
                 45,
                 0
             ],
             "scale": [
                 0.375,
-                0.140625,
+                0.375,
                 0.375
             ],
             "translation": [
                 0,
                 2.5,
                 0
             ]
@@ -106,63 +106,63 @@
     },
     "elements": [
         {
             "faces": {
                 "down": {
                     "texture": "#0",
                     "uv": [
-                        0,
-                        0,
                         8,
+                        10.66667,
+                        12,
                         16
                     ]
                 },
                 "east": {
                     "texture": "#0",
                     "uv": [
-                        0,
-                        10,
+                        4,
+                        5.33333,
                         8,
-                        16
+                        10.66667
                     ]
                 },
                 "north": {
                     "texture": "#0",
                     "uv": [
-                        0,
-                        10,
                         8,
-                        16
+                        5.33333,
+                        12,
+                        10.66667
                     ]
                 },
                 "south": {
                     "texture": "#0",
                     "uv": [
                         0,
-                        10,
-                        8,
-                        16
+                        5.33333,
+                        4,
+                        10.66667
                     ]
                 },
                 "up": {
                     "texture": "#0",
                     "uv": [
                         8,
                         0,
-                        16,
-                        16
+                        12,
+                        5.33333
                     ]
                 },
                 "west": {
                     "texture": "#0",
                     "uv": [
-                        0,
-                        10,
-                        8,
-                        16
+                        12,
+                        5.33333,
+                        16,
+                        10.66667
                     ]
                 }
             },
             "from": [
                 0,
                 0,
                 0
@@ -171,15 +171,15 @@
                 16,
                 16,
                 16
             ]
         }
     ],
     "texture_size": [
-        32,
-        16
+        64,
+        48
     ],
     "textures": {
-        "0": "oneironaut:block/sentinel_sensor",
+        "0": "oneironaut:block/sentinel_trap_powered",
         "particle": "hexcasting:block/slate"
     }
 }
```

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/spoon_staff.json` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/models/item/spoon_staff.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/black_circle.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/black_circle.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/noosphere_basalt.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/noosphere_basalt.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/noosphere_gate.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/noosphere_gate.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/pseudoamethyst_block.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/pseudoamethyst_block.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/raycast_blocker.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/raycast_blocker.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/raycast_blocker_glass.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/raycast_blocker_glass.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_sensor.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_sensor.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_trap_powered.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_trap_powered.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_trap_unpowered.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/sentinel_trap_unpowered.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/super_budding.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/super_budding.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/thought_slurry.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/thought_slurry.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/thought_slurry_flowing.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/thought_slurry_flowing.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/wisp_lantern.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/wisp_lantern.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/wisp_lantern_tinted.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/block/wisp_lantern_tinted.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/book/slipway_hint_image.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/book/slipway_hint_image.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/echo_staff.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/echo_staff.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/endless_phial.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/endless_phial.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_echo.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_echo.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_flame.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_flame.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_noosphere.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pigment_noosphere.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pseudoamethyst_shard.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/pseudoamethyst_shard.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod_castloop.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod_castloop.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod_filled.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/reverberation_rod_filled.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/sentinel_trap_item.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/sentinel_trap_item.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/spoon_staff.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/spoon_staff.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/thought_slurry_bucket.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/thought_slurry_bucket.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/wisp_lantern.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/wisp_lantern.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/wisp_lantern_tinted.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/item/wisp_lantern_tinted.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/mob_effect/detection_resistance.png` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/assets/oneironaut/textures/mob_effect/detection_resistance.png`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/basics/slipway_hint.json` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/glow_ambit.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3958333333333333%*

 * *Differences: {"'advancement'": "'hexcasting:root'",*

 * * "'category'": "'hexcasting:patterns/great_spells'",*

 * * "'icon'": "'minecraft:beacon'",*

 * * "'name'": "'hexcasting.spell.oneironaut:applynotmissing'",*

 * * "'pages'": "{0: {'text': 'oneironaut.page.glow_ambit.1'}, 2: {'type': 'patchouli:text', 'text': "*

 * *            "'oneironaut.page.glow_ambit.3', delete: ['images', 'title']}, insert: [(1, "*

 * *            "OrderedDict([('type', 'hexcasting:pattern'), ('op_id', 'oneironaut:applynotmissing'), "*

 * *            "('anchor', 'oneironaut:a […]*

```diff
@@ -1,22 +1,26 @@
 {
-    "advancement": "hexcasting:enlightenment",
-    "category": "hexcasting:basics",
-    "entry_color": "54398a",
-    "icon": "minecraft:iron_door",
-    "name": "oneironaut.entry.slipway_hint",
+    "advancement": "hexcasting:root",
+    "category": "hexcasting:patterns/great_spells",
+    "icon": "minecraft:beacon",
+    "name": "hexcasting.spell.oneironaut:applynotmissing",
     "pages": [
         {
-            "text": "oneironaut.page.slipway_hint.1",
+            "text": "oneironaut.page.glow_ambit.1",
             "type": "patchouli:text"
         },
         {
-            "images": [
-                "oneironaut:textures/book/slipway_hint_image.png"
-            ],
-            "text": "oneironaut.page.slipway_hint.2",
-            "title": "oneironaut.page.slipway_hint.2.title",
-            "type": "patchouli:image"
+            "anchor": "oneironaut:applynotmissing",
+            "input": "entity",
+            "op_id": "oneironaut:applynotmissing",
+            "output": "",
+            "text": "oneironaut.page.glow_ambit.2",
+            "type": "hexcasting:pattern"
+        },
+        {
+            "text": "oneironaut.page.glow_ambit.3",
+            "type": "patchouli:text"
         }
     ],
-    "sortnum": 6
+    "read_by_default": false,
+    "sortnum": 5
 }
```

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/noosphere_materials.json` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/paint_conjured.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.38764880952380953%*

 * *Differences: {"'advancement'": "'hexcasting:root'",*

 * * "'category'": "'hexcasting:patterns/spells'",*

 * * "'icon'": "'hexcasting:uuid_colorizer'",*

 * * "'name'": "'hexcasting.spell.oneironaut:paintconjured'",*

 * * "'pages'": "{0: {'type': 'hexcasting:pattern', 'text': 'oneironaut.page.paintconjured.1', "*

 * *            "'op_id': 'oneironaut:paintconjured', 'anchor': 'oneironaut:paintconjured', 'input': "*

 * *            "'Vector, itemtype', 'output': '', delete: ['item']}, 1: {'type': 'patchouli:text', "*

 * *            "'text': 'oneironaut.pag […]*

```diff
@@ -1,31 +1,26 @@
 {
-    "advancement": "oneironaut:enter_noosphere",
-    "category": "hexcasting:greatwork",
-    "entry_color": "54398a",
-    "icon": "oneironaut:pseudoamethyst_shard",
-    "name": "oneironaut.entry.noosphere_materials",
+    "advancement": "hexcasting:root",
+    "category": "hexcasting:patterns/spells",
+    "icon": "hexcasting:uuid_colorizer",
+    "name": "hexcasting.spell.oneironaut:paintconjured",
     "pages": [
         {
-            "item": "oneironaut:thought_slurry_bucket",
-            "text": "oneironaut.page.noosphere_materials.1",
-            "title": "fluid.oneironaut.thought_slurry",
-            "type": "patchouli:spotlight"
+            "anchor": "oneironaut:paintconjured",
+            "input": "Vector, itemtype",
+            "op_id": "oneironaut:paintconjured",
+            "output": "",
+            "text": "oneironaut.page.paintconjured.1",
+            "type": "hexcasting:pattern"
         },
         {
-            "item": "oneironaut:noosphere_basalt",
-            "text": "oneironaut.page.noosphere_materials.2",
-            "type": "patchouli:spotlight"
+            "text": "oneironaut.page.paintconjured.2",
+            "type": "patchouli:text"
         },
         {
-            "item": "oneironaut:pseudoamethyst_block",
-            "text": "oneironaut.page.noosphere_materials.3",
-            "type": "patchouli:spotlight"
-        },
-        {
-            "item": "oneironaut:pseudoamethyst_shard",
-            "text": "oneironaut.page.noosphere_materials.4",
-            "type": "patchouli:spotlight"
+            "text": "oneironaut.page.paintconjured.3",
+            "type": "patchouli:text"
         }
     ],
-    "sortnum": 4
+    "read_by_default": false,
+    "sortnum": 6
 }
```

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/sentinel_detection.json` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/sentinel_detection.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/super_budding.json` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/greatwork/super_budding.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/items/reverberation_rod.json` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/status_iotas.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.45995670995670995%*

 * *Differences: {"'advancement'": "'hexcasting:root'",*

 * * "'category'": "'hexcasting:patterns'",*

 * * "'icon'": "'minecraft:potion'",*

 * * "'name'": "'oneironaut.entry.status_iotas'",*

 * * "'pages'": "{0: {'type': 'patchouli:text', 'text': 'oneironaut.page.status_iotas.1', delete: "*

 * *            "['recipe']}, 2: {'op_id': 'oneironaut:getstatuscategory', 'anchor': "*

 * *            "'oneironaut:getstatuscategory', 'input': 'status', 'output': 'num', 'text': "*

 * *            "'oneironaut.page.status_iotas.3'}, 3: {'op_id': 'oneironaut:getstatusdu […]*

```diff
@@ -1,76 +1,82 @@
 {
-    "advancement": "minecraft:adventure/avoid_vibration",
-    "category": "hexcasting:items",
-    "icon": "oneironaut:reverberation_rod",
-    "name": "item.oneironaut.reverberation_rod",
+    "advancement": "hexcasting:root",
+    "category": "hexcasting:patterns",
+    "icon": "minecraft:potion",
+    "name": "oneironaut.entry.status_iotas",
     "pages": [
-        "oneironaut.page.rod.1",
         {
-            "recipe": "oneironaut:reverberation_rod",
-            "text": "oneironaut.page.rod.2",
-            "type": "patchouli:crafting"
+            "text": "oneironaut.page.status_iotas.1",
+            "type": "patchouli:text"
         },
         {
-            "anchor": "oneironaut:craftrod",
-            "input": "entity, list of patterns",
-            "op_id": "oneironaut:craftrod",
-            "output": "",
-            "text": "oneironaut.page.rod.3",
+            "anchor": "oneironaut:getstatus",
+            "input": "entity",
+            "op_id": "oneironaut:getstatus",
+            "output": "[status]",
+            "text": "oneironaut.page.status_iotas.2",
             "type": "hexcasting:pattern"
         },
         {
-            "anchor": "oneironaut:getrodlook",
-            "input": "",
-            "op_id": "oneironaut:getrodlook",
-            "output": "vector",
-            "text": "oneironaut.page.rod.4",
+            "anchor": "oneironaut:getstatuscategory",
+            "input": "status",
+            "op_id": "oneironaut:getstatuscategory",
+            "output": "num",
+            "text": "oneironaut.page.status_iotas.3",
             "type": "hexcasting:pattern"
         },
         {
-            "anchor": "oneironaut:getrodpos",
-            "input": "",
-            "op_id": "oneironaut:getrodpos",
-            "output": "vector",
-            "text": "oneironaut.page.rod.5",
+            "anchor": "oneironaut:getstatusduration",
+            "input": "entity, status",
+            "op_id": "oneironaut:getstatusduration",
+            "output": "num",
+            "text": "oneironaut.page.status_iotas.4",
             "type": "hexcasting:pattern"
         },
         {
-            "anchor": "oneironaut:getrodstamp",
-            "input": "",
-            "op_id": "oneironaut:getrodstamp",
-            "output": "number",
-            "text": "oneironaut.page.rod.6",
+            "anchor": "oneironaut:getstatuslevel",
+            "input": "entity, status",
+            "op_id": "oneironaut:getstatuslevel",
+            "output": "num",
+            "text": "oneironaut.page.status_iotas.5",
             "type": "hexcasting:pattern"
         },
         {
-            "anchor": "oneironaut:delayrod",
-            "input": "number",
-            "op_id": "oneironaut:delayrod",
-            "output": "",
-            "text": "oneironaut.page.rod.7",
+            "anchor": "oneironaut:getbystatussingle",
+            "input": "status, vector",
+            "op_id": "oneironaut:getbystatussingle",
+            "output": "entity | NULL",
+            "text": "oneironaut.page.status_iotas.6",
             "type": "hexcasting:pattern"
         },
         {
-            "anchor": "oneironaut:haltrod",
-            "input": "",
-            "op_id": "oneironaut:haltrod",
-            "output": "",
-            "text": "oneironaut.page.rod.8",
+            "anchor": "oneironaut:getbystatus",
+            "input": "status, vec, num",
+            "op_id": "oneironaut:getbystatus",
+            "output": "[entity]",
+            "text": "oneironaut.page.status_iotas.7",
+            "type": "hexcasting:pattern"
+        },
+        {
+            "anchor": "oneironaut:getbystatusinverse",
+            "input": "status, vec, num",
+            "op_id": "oneironaut:getbystatusinverse",
+            "output": "[entity]",
+            "text": "oneironaut.page.status_iotas.8",
             "type": "hexcasting:pattern"
         },
         {
-            "anchor": "oneironaut:resetrod",
-            "input": "number",
-            "op_id": "oneironaut:resetrod",
+            "anchor": "oneironaut:removestatus",
+            "input": "entity, status",
+            "op_id": "oneironaut:removestatus",
             "output": "",
-            "text": "oneironaut.page.rod.9",
+            "text": "oneironaut.page.status_iotas.9",
             "type": "hexcasting:pattern"
         },
         {
-            "recipe": "oneironaut:echo_staff",
-            "text": "oneironaut.page.rod.10",
-            "type": "patchouli:crafting"
+            "text": "oneironaut.page.status_iotas.10",
+            "type": "patchouli:text"
         }
     ],
-    "sortnum": 6
+    "read_by_default": false,
+    "sortnum": 3
 }
```

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/dim_iotas.json` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/dim_iotas.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/frame_patterns.json` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/infusemedia.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6607142857142857%*

 * *Differences: {"'category'": "'hexcasting:patterns/great_spells'",*

 * * "'icon'": "'hexcasting:charged_amethyst'",*

 * * "'name'": "'hexcasting.spell.oneironaut:infusemedia'",*

 * * "'pages'": "{0: {'op_id': 'oneironaut:infusemedia', 'anchor': 'oneironaut:infusemedia', 'input': "*

 * *            "'Vector', 'output': '', 'text': 'oneironaut.page.infusemedia.1'}, 1: {'type': "*

 * *            "'patchouli:text', 'text': 'oneironaut.page.infusemedia.2', delete: ['op_id', "*

 * *            "'anchor', 'input', 'output']}, delete: [0]}",*

 * * "'sortnum'": ' […]*

```diff
@@ -1,30 +1,22 @@
 {
     "advancement": "hexcasting:root",
-    "category": "hexcasting:patterns",
-    "icon": "minecraft:item_frame",
-    "name": "oneironaut.entry.framepatterns",
+    "category": "hexcasting:patterns/great_spells",
+    "icon": "hexcasting:charged_amethyst",
+    "name": "hexcasting.spell.oneironaut:infusemedia",
     "pages": [
         {
-            "text": "oneironaut.page.framepatterns.1",
-            "type": "patchouli:text"
-        },
-        {
-            "anchor": "oneironaut:readframerotation",
-            "input": "item frame",
-            "op_id": "oneironaut:readframerotation",
-            "output": "number",
-            "text": "oneironaut.page.framepatterns.3",
+            "anchor": "oneironaut:infusemedia",
+            "input": "Vector",
+            "op_id": "oneironaut:infusemedia",
+            "output": "",
+            "text": "oneironaut.page.infusemedia.1",
             "type": "hexcasting:pattern"
         },
         {
-            "anchor": "oneironaut:setframerotation",
-            "input": "item frame, number",
-            "op_id": "oneironaut:setframerotation",
-            "output": "",
-            "text": "oneironaut.page.framepatterns.4",
-            "type": "hexcasting:pattern"
+            "text": "oneironaut.page.infusemedia.2",
+            "type": "patchouli:text"
         }
     ],
     "read_by_default": false,
-    "sortnum": 3
+    "sortnum": 0
 }
```

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/idea_inscription.json` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/idea_inscription.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/status_iotas.json` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/misc_patterns.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8083333333333333%*

 * *Differences: {"'icon'": "'minecraft:item_frame'",*

 * * "'name'": "'oneironaut.entry.miscpatterns'",*

 * * "'pages'": "{0: {'text': 'oneironaut.page.miscpatterns.1'}, 1: {'op_id': "*

 * *            "'oneironaut:readframerotation', 'anchor': 'oneironaut:readframerotation', 'input': "*

 * *            "'item frame', 'output': 'number', 'text': 'oneironaut.page.miscpatterns.2'}, 2: "*

 * *            "{'op_id': 'oneironaut:setframerotation', 'anchor': 'oneironaut:setframerotation', "*

 * *            "'input': 'item frame, number', 'output': '', 'text […]*

```diff
@@ -1,82 +1,46 @@
 {
     "advancement": "hexcasting:root",
     "category": "hexcasting:patterns",
-    "icon": "minecraft:potion",
-    "name": "oneironaut.entry.status_iotas",
+    "icon": "minecraft:item_frame",
+    "name": "oneironaut.entry.miscpatterns",
     "pages": [
         {
-            "text": "oneironaut.page.status_iotas.1",
+            "text": "oneironaut.page.miscpatterns.1",
             "type": "patchouli:text"
         },
         {
-            "anchor": "oneironaut:getstatus",
-            "input": "entity",
-            "op_id": "oneironaut:getstatus",
-            "output": "[status]",
-            "text": "oneironaut.page.status_iotas.2",
+            "anchor": "oneironaut:readframerotation",
+            "input": "item frame",
+            "op_id": "oneironaut:readframerotation",
+            "output": "number",
+            "text": "oneironaut.page.miscpatterns.2",
             "type": "hexcasting:pattern"
         },
         {
-            "anchor": "oneironaut:getstatuscategory",
-            "input": "status",
-            "op_id": "oneironaut:getstatuscategory",
-            "output": "num",
-            "text": "oneironaut.page.status_iotas.3",
-            "type": "hexcasting:pattern"
-        },
-        {
-            "anchor": "oneironaut:getstatusduration",
-            "input": "entity, status",
-            "op_id": "oneironaut:getstatusduration",
-            "output": "num",
-            "text": "oneironaut.page.status_iotas.4",
-            "type": "hexcasting:pattern"
-        },
-        {
-            "anchor": "oneironaut:getstatuslevel",
-            "input": "entity, status",
-            "op_id": "oneironaut:getstatuslevel",
-            "output": "num",
-            "text": "oneironaut.page.status_iotas.5",
+            "anchor": "oneironaut:setframerotation",
+            "input": "item frame, number",
+            "op_id": "oneironaut:setframerotation",
+            "output": "",
+            "text": "oneironaut.page.miscpatterns.3",
             "type": "hexcasting:pattern"
         },
         {
-            "anchor": "oneironaut:getbystatussingle",
-            "input": "status, vector",
-            "op_id": "oneironaut:getbystatussingle",
+            "anchor": "oneironaut:filteredentityraycast",
+            "input": "[type], vec, vec",
+            "op_id": "oneironaut:filteredentityraycast",
             "output": "entity | NULL",
-            "text": "oneironaut.page.status_iotas.6",
+            "text": "oneironaut.page.miscpatterns.4",
             "type": "hexcasting:pattern"
         },
         {
-            "anchor": "oneironaut:getbystatus",
-            "input": "status, vec, num",
-            "op_id": "oneironaut:getbystatus",
-            "output": "[entity]",
-            "text": "oneironaut.page.status_iotas.7",
-            "type": "hexcasting:pattern"
-        },
-        {
-            "anchor": "oneironaut:getbystatusinverse",
-            "input": "status, vec, num",
-            "op_id": "oneironaut:getbystatusinverse",
-            "output": "[entity]",
-            "text": "oneironaut.page.status_iotas.8",
-            "type": "hexcasting:pattern"
-        },
-        {
-            "anchor": "oneironaut:removestatus",
-            "input": "entity, status",
-            "op_id": "oneironaut:removestatus",
-            "output": "",
-            "text": "oneironaut.page.status_iotas.9",
+            "anchor": "oneironaut:gaussianrand",
+            "input": "",
+            "op_id": "oneironaut:gaussianrand",
+            "output": "num",
+            "text": "oneironaut.page.miscpatterns.5",
             "type": "hexcasting:pattern"
-        },
-        {
-            "text": "oneironaut.page.status_iotas.10",
-            "type": "patchouli:text"
         }
     ],
     "read_by_default": false,
     "sortnum": 3
 }
```

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/paint_conjured.json` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/swap_space.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6884920634920635%*

 * *Differences: {"'category'": "'hexcasting:patterns/great_spells'",*

 * * "'icon'": "'minecraft:ender_chest'",*

 * * "'name'": "'hexcasting.spell.oneironaut:swapspace'",*

 * * "'pages'": "{0: {'op_id': 'oneironaut:swapspace', 'anchor': 'oneironaut:swapspace', 'input': "*

 * *            "'[vec, vec], [vec, vec], Imprint', 'text': 'oneironaut.page.spaceswap.1'}, 1: "*

 * *            "{'text': 'oneironaut.page.spaceswap.2'}, 2: {'text': 'oneironaut.page.spaceswap.3', "*

 * *            "'advancement': 'oneironaut:enter_noosphere'}}",*

 * * "'sortnum'": '0'}*

```diff
@@ -1,26 +1,27 @@
 {
     "advancement": "hexcasting:root",
-    "category": "hexcasting:patterns/spells",
-    "icon": "hexcasting:uuid_colorizer",
-    "name": "hexcasting.spell.oneironaut:paintconjured",
+    "category": "hexcasting:patterns/great_spells",
+    "icon": "minecraft:ender_chest",
+    "name": "hexcasting.spell.oneironaut:swapspace",
     "pages": [
         {
-            "anchor": "oneironaut:paintconjured",
-            "input": "Vector, itemtype",
-            "op_id": "oneironaut:paintconjured",
+            "anchor": "oneironaut:swapspace",
+            "input": "[vec, vec], [vec, vec], Imprint",
+            "op_id": "oneironaut:swapspace",
             "output": "",
-            "text": "oneironaut.page.paintconjured.1",
+            "text": "oneironaut.page.spaceswap.1",
             "type": "hexcasting:pattern"
         },
         {
-            "text": "oneironaut.page.paintconjured.2",
+            "text": "oneironaut.page.spaceswap.2",
             "type": "patchouli:text"
         },
         {
-            "text": "oneironaut.page.paintconjured.3",
+            "advancement": "oneironaut:enter_noosphere",
+            "text": "oneironaut.page.spaceswap.3",
             "type": "patchouli:text"
         }
     ],
     "read_by_default": false,
-    "sortnum": 6
+    "sortnum": 0
 }
```

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/particle_burst.json` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/particle_burst.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/detection_shielding.json` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/detection_shielding.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/dim_teleport.json` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/dim_teleport.json`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/patterns/spells/great/infuse_media.json` & `hexdoc_oneironaut-0.3.0.1.0/doc/src/hexdoc_oneironaut/_export/generated/data/oneironaut/patchouli_books/oneironautbook/en_us/entries/items/raycast_assailant.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3785807291666667%*

 * *Differences: {"'advancement'": "'oneironaut:enter_noosphere'",*

 * * "'category'": "'hexcasting:items'",*

 * * "'entry_color'": "'54398a'",*

 * * "'icon'": "'oneironaut:raycast_blocker'",*

 * * "'name'": "'oneironaut.entry.raycast_assailant'",*

 * * "'pages'": "{1: {'type': 'patchouli:crafting', 'recipe': 'oneironaut:raycast_blocker', 'recipe2': "*

 * *            "'oneironaut:raycast_blocker_glass', delete: ['op_id', 'anchor', 'input', 'output', "*

 * *            "'text']}, 3: {'type': 'patchouli:crafting', 'recipe': "*

 * *            "'oneironaut:hex_resi […]*

```diff
@@ -1,22 +1,21 @@
 {
-    "advancement": "hexcasting:root",
-    "category": "hexcasting:patterns/great_spells",
-    "icon": "hexcasting:charged_amethyst",
-    "name": "hexcasting.spell.oneironaut:infusemedia",
+    "advancement": "oneironaut:enter_noosphere",
+    "category": "hexcasting:items",
+    "entry_color": "54398a",
+    "icon": "oneironaut:raycast_blocker",
+    "name": "oneironaut.entry.raycast_assailant",
     "pages": [
+        "oneironaut.page.raycast_assailant.1",
         {
-            "anchor": "oneironaut:infusemedia",
-            "input": "Vector",
-            "op_id": "oneironaut:infusemedia",
-            "output": "",
-            "text": "oneironaut.page.infusemedia.1",
-            "type": "hexcasting:pattern"
+            "recipe": "oneironaut:raycast_blocker",
+            "recipe2": "oneironaut:raycast_blocker_glass",
+            "type": "patchouli:crafting"
         },
+        "oneironaut.page.raycast_assailant.3",
         {
-            "text": "oneironaut.page.infusemedia.2",
-            "type": "patchouli:text"
+            "recipe": "oneironaut:hex_resistant_block",
+            "type": "patchouli:crafting"
         }
     ],
-    "read_by_default": false,
-    "sortnum": 0
+    "sortnum": 6
 }
```

### Comparing `hexdoc_oneironaut-0.2.2.1.0/.gitignore` & `hexdoc_oneironaut-0.3.0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/LICENSE` & `hexdoc_oneironaut-0.3.0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/pyproject.toml` & `hexdoc_oneironaut-0.3.0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/doc/README.md` & `hexdoc_oneironaut-0.3.0.1.0/doc/README.md`

 * *Files identical despite different names*

### Comparing `hexdoc_oneironaut-0.2.2.1.0/PKG-INFO` & `hexdoc_oneironaut-0.3.0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: hexdoc-oneironaut
-Version: 0.2.2.1.0
+Version: 0.3.0.1.0
 Summary: Python web book docgen and hexdoc plugin for Oneironaut.
 Project-URL: Homepage, https://beholderface.github.io/oneironaut
 Project-URL: Source, https://github.com/beholderface/oneironaut
 Author: beholderface
 License-File: LICENSE
 Keywords: hexdoc
 Requires-Python: >=3.11
```

