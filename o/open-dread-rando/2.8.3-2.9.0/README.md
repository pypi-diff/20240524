# Comparing `tmp/open-dread-rando-2.8.3.tar.gz` & `tmp/open-dread-rando-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-dread-rando-2.8.3.tar", last modified: Sat Oct 14 08:27:06 2023, max compression
+gzip compressed data, was "open-dread-rando-2.9.0.tar", last modified: Thu Feb 22 18:45:20 2024, max compression
```

## Comparing `open-dread-rando-2.8.3.tar` & `open-dread-rando-2.9.0.tar`

### file list

```diff
@@ -1,248 +1,256 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.723574 open-dread-rando-2.8.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.695574 open-dread-rando-2.8.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.695574 open-dread-rando-2.8.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      282 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.695574 open-dread-rando-2.8.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2023-10-14 08:27:06.719574 open-dread-rando-2.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.695574 open-dread-rando-2.8.3/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/icons/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/icons/noun-unplug-3033613.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-14 08:27:06.723574 open-dread-rando-2.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      606 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.687574 open-dread-rando-2.8.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.699574 open-dread-rando-2.8.3/src/open_dread_rando/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.699574 open-dread-rando-2.8.3/src/open_dread_rando/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/__pyinstaller/hook-open_dread_rando.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.699574 open-dread-rando-2.8.3/src/open_dread_rando/cosmetic_patches/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/cosmetic_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/cosmetic_patches/missile_color_patcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.699574 open-dread-rando-2.8.3/src/open_dread_rando/door_locks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/door_locks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18491 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/door_locks/custom_door_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    21290 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/door_locks/door_patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    11840 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/dread_patcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.699574 open-dread-rando-2.8.3/src/open_dread_rando/files/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18208 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/custom_scenario.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.699574 open-dread-rando-2.8.3/src/open_dread_rando/files/dread_depackager/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/dread_depackager/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/dread_depackager/main.npdm
--rw-r--r--   0 runner    (1001) docker     (127)   191054 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/dread_depackager/subsdk9
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.699574 open-dread-rando-2.8.3/src/open_dread_rando/files/exefs_patches/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/exefs_patches/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.703574 open-dread-rando-2.8.3/src/open_dread_rando/files/levels/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/levels/readme.txt
--rw-r--r--   0 runner    (1001) docker     (127)    67202 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/levels/s010_cave.lc.lua
--rw-r--r--   0 runner    (1001) docker     (127)    37804 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/levels/s020_magma.lc.lua
--rw-r--r--   0 runner    (1001) docker     (127)    23334 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/levels/s030_baselab.lc.lua
--rw-r--r--   0 runner    (1001) docker     (127)    32095 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/levels/s040_aqua.lc.lua
--rw-r--r--   0 runner    (1001) docker     (127)    25179 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/levels/s050_forest.lc.lua
--rw-r--r--   0 runner    (1001) docker     (127)    10649 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/levels/s060_quarantine.lc.lua
--rw-r--r--   0 runner    (1001) docker     (127)    30603 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/levels/s070_basesanc.lc.lua
--rw-r--r--   0 runner    (1001) docker     (127)    16611 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/levels/s080_shipyard.lc.lua
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/levels/s090_skybase.lc.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.703574 open-dread-rando-2.8.3/src/open_dread_rando/files/lua_libraries/
--rw-r--r--   0 runner    (1001) docker     (127)     8005 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/lua_libraries/bit.lua
--rw-r--r--   0 runner    (1001) docker     (127)      901 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/lua_libraries/data_structures.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/lua_libraries/death_counter.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/lua_libraries/disconnect_gui.lua
--rw-r--r--   0 runner    (1001) docker     (127)    12239 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/lua_libraries/guilib.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/lua_libraries/input_handling.lua
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/lua_libraries/room_names.lua
--rw-r--r--   0 runner    (1001) docker     (127)    26346 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/msemenu_mainmenu.lua
--rw-r--r--   0 runner    (1001) docker     (127)    20048 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/randomizer_powerup.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/item_cube/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/item_cube/model/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.707574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.707574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/
--rw-r--r--   0 runner    (1001) docker     (127)   422936 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl
--rw-r--r--   0 runner    (1001) docker     (127)   422936 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/itemsphere/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.707574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.707574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/
--rw-r--r--   0 runner    (1001) docker     (127)      938 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (127)     9508 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.707574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.707574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/
--rw-r--r--   0 runner    (1001) docker     (127)      716 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat
--rw-r--r--   0 runner    (1001) docker     (127)    19348 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.707574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.707574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat
--rw-r--r--   0 runner    (1001) docker     (127)      727 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat
--rw-r--r--   0 runner    (1001) docker     (127)    33012 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.707574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.707574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mat0001.bsmat
--rw-r--r--   0 runner    (1001) docker     (127)      742 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat
--rw-r--r--   0 runner    (1001) docker     (127)    13404 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.707574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.707574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (127)    28948 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.707574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.707574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_autoilum.bsmat
--rw-r--r--   0 runner    (1001) docker     (127)      498 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_bola.bsmat
--rw-r--r--   0 runner    (1001) docker     (127)      705 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat
--rw-r--r--   0 runner    (1001) docker     (127)    47996 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/props/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/props/doorshieldmissile/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.707574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/props/doorshieldmissile/collisions/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/props/doorshieldmissile/collisions/shield_bomb_colls.bmscd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.695574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.711574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)    28804 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex
--rw-r--r--   0 runner    (1001) docker     (127)    19894 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex
--rw-r--r--   0 runner    (1001) docker     (127)    42001 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.711574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)    14467 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex
--rw-r--r--   0 runner    (1001) docker     (127)    17196 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex
--rw-r--r--   0 runner    (1001) docker     (127)    34728 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.711574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)    75887 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.711574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)    71298 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.711574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)   155165 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.695574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.691574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.711574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)    88098 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/doorshieldbomb_alt_bc.bctex
--rw-r--r--   0 runner    (1001) docker     (127)    86766 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/doorshieldbomb_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.695574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.695574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.711574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)    97424 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/models/textures/doorshieldcrossbomb_alt_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.695574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.695574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.711574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)    97993 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/models/textures/doorshieldicemissile_alt_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.695574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.695574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.711574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)   128743 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/shield_no_attribs_at.bctex
--rw-r--r--   0 runner    (1001) docker     (127)   102269 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/shield_no_normals_nm.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.695574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.695574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.711574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)    94417 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_alt_bc.bctex
--rw-r--r--   0 runner    (1001) docker     (127)    91236 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_rdv_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.695574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.695574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.711574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)    94015 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/doorshieldstormmissile_alt_bc.bctex
--rw-r--r--   0 runner    (1001) docker     (127)    71252 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/doorshieldstormmissile_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.695574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.695574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.715574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)    85659 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/models/textures/shield_diffusion_alt_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.695574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/gui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.715574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/gui/textures/
--rw-r--r--   0 runner    (1001) docker     (127)   105443 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/gui/textures/hud_tileset.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.695574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/system/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.695574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/system/minimap/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.715574 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/system/minimap/icons/
--rw-r--r--   0 runner    (1001) docker     (127)   431407 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/system/minimap/icons/icons.bctex
--rw-r--r--   0 runner    (1001) docker     (127)    30596 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.715574 open-dread-rando-2.8.3/src/open_dread_rando/files/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/templates/boss_powerup_template.lua
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/templates/cc_to_room_name.lua
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/templates/custom_core_x.lua
--rw-r--r--   0 runner    (1001) docker     (127)      721 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/templates/custom_core_x_superquetzoa.lua
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/templates/custom_init.lua
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/templates/progressive_model_template.lua
--rw-r--r--   0 runner    (1001) docker     (127)      337 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/templates/randomizer_progressive_template.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/templates/template_doorshield_energy.bmsad
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/templates/template_doorshield_hexs.bmsad
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/templates/template_doorshield_tris.bmsad
--rw-r--r--   0 runner    (1001) docker     (127)      994 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/files/templates/template_powerup.bmsad
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.715574 open-dread-rando-2.8.3/src/open_dread_rando/misc_patches/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/misc_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/misc_patches/elevator.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/misc_patches/exefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/misc_patches/lua_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/misc_patches/material_patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/misc_patches/model_patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/misc_patches/sprite_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/misc_patches/text_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/misc_patches/tilegroup_patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/output_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/patch_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/patcher_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.719574 open-dread-rando-2.8.3/src/open_dread_rando/pickups/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/pickups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/pickups/lua_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    14358 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/pickups/map_icons.py
--rw-r--r--   0 runner    (1001) docker     (127)    27001 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/pickups/model_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    13148 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/pickups/pickup.py
--rw-r--r--   0 runner    (1001) docker     (127)    15096 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/pickups/split_pickups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.719574 open-dread-rando-2.8.3/src/open_dread_rando/specific_patches/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/specific_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/specific_patches/environmental_damage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5807 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/specific_patches/environmental_damage_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/specific_patches/game_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/specific_patches/objective.py
--rw-r--r--   0 runner    (1001) docker     (127)    13510 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/specific_patches/static_fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/src/open_dread_rando/validator_with_default.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-14 08:27:06.000000 open-dread-rando-2.8.3/src/open_dread_rando/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.699574 open-dread-rando-2.8.3/src/open_dread_rando.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2023-10-14 08:27:06.000000 open-dread-rando-2.8.3/src/open_dread_rando.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9301 2023-10-14 08:27:06.000000 open-dread-rando-2.8.3/src/open_dread_rando.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-14 08:27:06.000000 open-dread-rando-2.8.3/src/open_dread_rando.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-10-14 08:27:06.000000 open-dread-rando-2.8.3/src/open_dread_rando.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-10-14 08:27:06.000000 open-dread-rando-2.8.3/src/open_dread_rando.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-14 08:27:06.000000 open-dread-rando-2.8.3/src/open_dread_rando.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.719574 open-dread-rando-2.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/tests/test_dread_patcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.719574 open-dread-rando-2.8.3/tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (127)   248426 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/tests/test_files/april_fools_patcher.json
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/tests/test_files/randomizer_progressive_expected.lua
--rw-r--r--   0 runner    (1001) docker     (127)   139730 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/tests/test_files/starter_preset_patcher.json
--rw-r--r--   0 runner    (1001) docker     (127)      750 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/tests/test_full_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/tests/test_lua_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/tests/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.719574 open-dread-rando-2.8.3/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/tools/create_exefs_patches.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-14 08:27:06.719574 open-dread-rando-2.8.3/tools/exefs_sources/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2023-10-14 08:26:49.000000 open-dread-rando-2.8.3/tools/exefs_sources/debug_input.s
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.275800 open-dread-rando-2.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.243800 open-dread-rando-2.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.243800 open-dread-rando-2.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.243800 open-dread-rando-2.9.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-02-22 18:45:20.275800 open-dread-rando-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.247800 open-dread-rando-2.9.0/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/icons/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/icons/noun-unplug-3033613.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 18:45:20.275800 open-dread-rando-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.231800 open-dread-rando-2.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.247800 open-dread-rando-2.9.0/src/open_dread_rando/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.247800 open-dread-rando-2.9.0/src/open_dread_rando/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/__pyinstaller/hook-open_dread_rando.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.247800 open-dread-rando-2.9.0/src/open_dread_rando/cosmetic_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/cosmetic_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/cosmetic_patches/missile_color_patcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.251800 open-dread-rando-2.9.0/src/open_dread_rando/door_locks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/door_locks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20597 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/door_locks/custom_door_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21603 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/door_locks/door_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11954 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/dread_patcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.251800 open-dread-rando-2.9.0/src/open_dread_rando/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18321 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/custom_scenario.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.251800 open-dread-rando-2.9.0/src/open_dread_rando/files/dread_depackager/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/dread_depackager/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/dread_depackager/main.npdm
+-rw-r--r--   0 runner    (1001) docker     (127)   191054 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/dread_depackager/subsdk9
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.251800 open-dread-rando-2.9.0/src/open_dread_rando/files/exefs_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/exefs_patches/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.255800 open-dread-rando-2.9.0/src/open_dread_rando/files/levels/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/levels/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    67202 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/levels/s010_cave.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    37804 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/levels/s020_magma.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    23334 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/levels/s030_baselab.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    32095 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/levels/s040_aqua.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    25179 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/levels/s050_forest.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    10649 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/levels/s060_quarantine.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    30603 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/levels/s070_basesanc.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    16611 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/levels/s080_shipyard.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/levels/s090_skybase.lc.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.255800 open-dread-rando-2.9.0/src/open_dread_rando/files/lua_libraries/
+-rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/lua_libraries/bit.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/lua_libraries/data_structures.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/lua_libraries/death_counter.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/lua_libraries/disconnect_gui.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    12239 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/lua_libraries/guilib.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/lua_libraries/input_handling.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/lua_libraries/room_names.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    26346 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/msemenu_mainmenu.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    20048 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/randomizer_powerup.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.235800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.235800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.235800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.235800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/item_cube/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.235800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/item_cube/model/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.255800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.235800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.255800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/
+-rw-r--r--   0 runner    (1001) docker     (127)   422936 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl
+-rw-r--r--   0 runner    (1001) docker     (127)   422936 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.235800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/itemsphere/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.255800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.255800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.235800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.255800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.255800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat
+-rw-r--r--   0 runner    (1001) docker     (127)    19348 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.235800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.255800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.259800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (127)    33012 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.235800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.259800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.259800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mat0001.bsmat
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat
+-rw-r--r--   0 runner    (1001) docker     (127)    13404 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.235800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.259800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.259800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_icemissile_mp_opaque_01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_missile_mp_opaque_01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (127)    28948 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_icemissile.bcmdl
+-rw-r--r--   0 runner    (1001) docker     (127)    28948 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_missile.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.235800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.259800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.259800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_autoilum.bsmat
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_bola.bsmat
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat
+-rw-r--r--   0 runner    (1001) docker     (127)    47996 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.235800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/props/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.235800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/props/doorshieldmissile/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.259800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/props/doorshieldmissile/collisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/props/doorshieldmissile/collisions/shield_bomb_colls.bmscd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.243800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.259800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    28804 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)    19894 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)    42001 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.259800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    14467 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)    17196 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)    34728 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.259800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    75887 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.263800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    71298 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_icemissile_bc.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)    66662 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_missile_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.263800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)   155165 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.243800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.263800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    88098 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/doorshieldbomb_alt_bc.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)    86766 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/doorshieldbomb_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldclosed/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldclosed/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.263800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldclosed/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    69241 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldclosed/models/textures/doorshieldclosed_alt_bc.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)    73765 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldclosed/models/textures/doorshieldclosed_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.263800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    97424 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/models/textures/doorshieldcrossbomb_alt_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.263800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    97993 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/models/textures/doorshieldicemissile_alt_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.263800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)   128743 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/shield_no_attribs_at.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)   102269 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/shield_no_normals_nm.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.239800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.263800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    94417 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_alt_bc.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)    91236 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_rdv_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.243800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.243800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.267800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    94015 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/doorshieldstormmissile_alt_bc.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)    71252 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/doorshieldstormmissile_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.243800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.243800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.267800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    85659 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/models/textures/shield_diffusion_alt_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.243800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/gui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.267800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/gui/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)   105443 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/gui/textures/hud_tileset.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.243800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/system/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.243800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/system/minimap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.267800 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/system/minimap/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)   431992 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/system/minimap/icons/icons.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)    30854 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.267800 open-dread-rando-2.9.0/src/open_dread_rando/files/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/templates/boss_powerup_template.lua
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/templates/cc_to_room_name.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/templates/custom_core_x.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/templates/custom_core_x_superquetzoa.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/templates/custom_init.lua
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/templates/progressive_model_template.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/templates/randomizer_progressive_template.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/templates/template_doorshield_energy.bmsad
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/templates/template_doorshield_hexs.bmsad
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/templates/template_doorshield_tris.bmsad
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/files/templates/template_powerup.bmsad
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.271800 open-dread-rando-2.9.0/src/open_dread_rando/misc_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/misc_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/misc_patches/elevator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/misc_patches/exefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/misc_patches/lua_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/misc_patches/material_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/misc_patches/model_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/misc_patches/sprite_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/misc_patches/text_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/misc_patches/tilegroup_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/output_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/patch_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/patcher_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.271800 open-dread-rando-2.9.0/src/open_dread_rando/pickups/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/pickups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/pickups/lua_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14918 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/pickups/map_icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28059 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/pickups/model_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13148 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/pickups/pickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15400 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/pickups/split_pickups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.271800 open-dread-rando-2.9.0/src/open_dread_rando/specific_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/specific_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/specific_patches/environmental_damage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/specific_patches/environmental_damage_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/specific_patches/game_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/specific_patches/objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13510 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/specific_patches/static_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/src/open_dread_rando/validator_with_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-22 18:45:20.000000 open-dread-rando-2.9.0/src/open_dread_rando/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.275800 open-dread-rando-2.9.0/src/open_dread_rando.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-02-22 18:45:20.000000 open-dread-rando-2.9.0/src/open_dread_rando.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9855 2024-02-22 18:45:20.000000 open-dread-rando-2.9.0/src/open_dread_rando.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 18:45:20.000000 open-dread-rando-2.9.0/src/open_dread_rando.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-22 18:45:20.000000 open-dread-rando-2.9.0/src/open_dread_rando.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-22 18:45:20.000000 open-dread-rando-2.9.0/src/open_dread_rando.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-22 18:45:20.000000 open-dread-rando-2.9.0/src/open_dread_rando.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.271800 open-dread-rando-2.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/tests/test_dread_patcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.275800 open-dread-rando-2.9.0/tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (127)   248426 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/tests/test_files/april_fools_patcher.json
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/tests/test_files/randomizer_progressive_expected.lua
+-rw-r--r--   0 runner    (1001) docker     (127)   139730 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/tests/test_files/starter_preset_patcher.json
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/tests/test_full_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/tests/test_lua_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.275800 open-dread-rando-2.9.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/tools/create_exefs_patches.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:45:20.275800 open-dread-rando-2.9.0/tools/exefs_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-22 18:45:05.000000 open-dread-rando-2.9.0/tools/exefs_sources/debug_input.s
```

### Comparing `open-dread-rando-2.8.3/.github/dependabot.yml` & `open-dread-rando-2.9.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/.github/workflows/python.yml` & `open-dread-rando-2.9.0/.github/workflows/python.yml`

 * *Files 1% similar despite different names*

```diff
@@ -18,28 +18,28 @@
       - name: Checkout
         uses: actions/checkout@v4
         with:
           fetch-depth: 0
           submodules: 'recursive'
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.10"
      
       - name: Install Python packages
         run: python -m pip install --upgrade pip setuptools build
 
       - name: build
         # Not adding PYTHONWARNINGS=error as it can trigger errors in pip itself
         # See https://github.com/pypa/pip/issues/12243
         run: python -m build
       
       - name: Store the packages
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           name: python-package-distributions
           path: dist
 
   test:
     needs:
       - build
@@ -55,20 +55,20 @@
           - {version: '3.12.0-beta - 3.12.0'}
 
     steps:
       - name: Checkout
         uses: actions/checkout@v4
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python.version }}
 
       - name: Download all the dists
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: python-package-distributions
           path: dist/
 
       - name: install built wheel
         run: python -m pip install "$(ls dist/*.whl)[test]"
         shell: bash
@@ -96,15 +96,15 @@
           fetch-depth: 0
           clean: true
 
       - name: Clean source
         run: rm -rf src
 
       - name: Download all the dists
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: python-package-distributions
           path: dist/
 
       - name: Create venv
         run: python -m venv venv
 
@@ -156,28 +156,28 @@
   pypi:
     runs-on: 'ubuntu-latest'
     needs:
       - test
 
     steps:
       - name: Download all the dists
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: python-package-distributions
           path: dist/
 
       - name: Publish 📦 to TestPyPI
         if: ${{ github.ref == 'refs/heads/main' }}
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.testpypi_password }}
           repository_url: https://test.pypi.org/legacy/
 
       - name: Create GitHub release
-        uses: svenstaro/upload-release-action@2.7.0
+        uses: svenstaro/upload-release-action@2.9.0
         if: ${{ startsWith(github.ref, 'refs/tags/') }}
         with:
           repo_token: ${{ secrets.GITHUB_TOKEN }}
           file: dist/*
           file_glob: true
           tag: ${{ github.ref }}
           overwrite: true
```

### Comparing `open-dread-rando-2.8.3/.gitignore` & `open-dread-rando-2.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/LICENSE` & `open-dread-rando-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/PKG-INFO` & `open-dread-rando-2.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-dread-rando
-Version: 2.8.3
+Version: 2.9.0
 Summary: An open source randomizer patcher for Metroid Dread.
 Project-URL: Homepage, https://github.com/randovania/open-dread-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.10
@@ -15,22 +15,22 @@
 Provides-Extra: test
 Requires-Dist: lupa; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 
 # Open Dread Rando
-Open Source randomizer patcher for Metroid Dread. Intended for use in [Randovania](https://github.com/randovania).
+Open Source randomizer patcher for Metroid Dread. Intended for use in [Randovania](https://randovania.github.io/).
 Currently supports patching item pickups, starting items, and elevator/shuttle/teleportal destinations.
 
 ## Installation
 `pip install open-dread-rando`
 
 ## Usage
-You will need to provide JSON data matching the [JSON schema](https://github.com/randovania/open-dread-rando/blob/main/open_dread_rando/files/schema.json) in order to successfully patch the game. 
+You will need to provide JSON data matching the [JSON schema](https://github.com/randovania/open-dread-rando/blob/main/src/open_dread_rando/files/schema.json) in order to successfully patch the game. 
 
 The patcher expects a path to an extracted romfs directory of Metroid Dread 1.0.0 or 2.1.0 as well as the desired output directory.
 Output files are in a format compatible with either Atmosphere or Ryujinx, depending on the settings provided.
 
 With a JSON file:
 `python -m open_dread_rando --input-path path/to/dread/romfs --output-path path/to/the/output-mod --input-json path/to/patcher-config.json`
```

### Comparing `open-dread-rando-2.8.3/README.md` & `open-dread-rando-2.9.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Open Dread Rando
-Open Source randomizer patcher for Metroid Dread. Intended for use in [Randovania](https://github.com/randovania).
+Open Source randomizer patcher for Metroid Dread. Intended for use in [Randovania](https://randovania.github.io/).
 Currently supports patching item pickups, starting items, and elevator/shuttle/teleportal destinations.
 
 ## Installation
 `pip install open-dread-rando`
 
 ## Usage
-You will need to provide JSON data matching the [JSON schema](https://github.com/randovania/open-dread-rando/blob/main/open_dread_rando/files/schema.json) in order to successfully patch the game. 
+You will need to provide JSON data matching the [JSON schema](https://github.com/randovania/open-dread-rando/blob/main/src/open_dread_rando/files/schema.json) in order to successfully patch the game. 
 
 The patcher expects a path to an extracted romfs directory of Metroid Dread 1.0.0 or 2.1.0 as well as the desired output directory.
 Output files are in a format compatible with either Atmosphere or Ryujinx, depending on the settings provided.
 
 With a JSON file:
 `python -m open_dread_rando --input-path path/to/dread/romfs --output-path path/to/the/output-mod --input-json path/to/patcher-config.json`
```

### Comparing `open-dread-rando-2.8.3/icons/noun-unplug-3033613.svg` & `open-dread-rando-2.9.0/icons/noun-unplug-3033613.svg`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/pyproject.toml` & `open-dread-rando-2.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/setup.py` & `open-dread-rando-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/cli.py` & `open-dread-rando-2.9.0/src/open_dread_rando/cli.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/cosmetic_patches/__init__.py` & `open-dread-rando-2.9.0/src/open_dread_rando/cosmetic_patches/__init__.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/cosmetic_patches/missile_color_patcher.py` & `open-dread-rando-2.9.0/src/open_dread_rando/cosmetic_patches/missile_color_patcher.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,90 +1,77 @@
 import dataclasses
 
-from open_dread_rando.misc_patches.material_patcher import MaterialData, create_custom_material
-from open_dread_rando.misc_patches.model_patcher import ModelData, create_custom_model
+from open_dread_rando.misc_patches.material_patcher import MaterialData
+from open_dread_rando.misc_patches.model_patcher import StaticModelChanger
 from open_dread_rando.patcher_editor import PatcherEditor
 
 
 # model names for pride missiles
 @dataclasses.dataclass()
-class MissileVariant:
-    mat_name: str
-    model_path: str
-    shader_path: str
-    rgba: tuple[float, float, float, float]
-
+class MissileTankRecolor(StaticModelChanger):
     def __init__(self, name: str, color: tuple[float, float, float, float]):
-        self.mat_name = f"{name}_mp_fxhologram_01"
-        self.model_path = f"actors/items/item_missiletank/models/{name}.bcmdl"
-        self.shader_path = f"actors/items/item_missiletank/models/imats/{self.mat_name}.bsmat"
+        self.materials = {
+            "mp_fxhologram_01": MaterialData(
+                base_mat="actors/items/item_missiletank/models/imats/item_missiletank_mp_fxhologram_01.bsmat",
+                new_mat_name=f"{name}_mp_fxhologram_01",
+                new_path=f"actors/items/item_missiletank/models/imats/{name}_mp_fxhologram_01.bsmat",
+                uniform_params={
+                    "vTex0EmissiveColor": color
+                }
+            )
+        }
 
-        self.rgba = color
+        self.base_model_path="actors/items/item_missiletank/models/item_missiletank.bcmdl"
+        self.new_model_path=f"actors/items/item_missiletank/models/{name}.bcmdl"
 
 
-ALL_VARIANTS: dict[str, MissileVariant] = {
-    "ORANGE": MissileVariant(
+MISSILE_TANK_RECOLORS: dict[str, MissileTankRecolor] = {
+    "ORANGE": MissileTankRecolor(
         name="item_missile__OR",
         color=(75.0, 10.0, 0.0, 1.0),
     ),
-    "YELLOW": MissileVariant(
+    "YELLOW": MissileTankRecolor(
         name="item_missile__YL",
         color=(30.0, 30.0, 0.0, 1.0),
     ),
-    "GREEN": MissileVariant(
+    "GREEN": MissileTankRecolor(
         name="item_missile__GN",
         color=(0.0, 30.0, 0.0, 1.0),
     ),
-    "BLUE": MissileVariant(
+    "BLUE": MissileTankRecolor(
         name="item_missile__BL",
         color=(0.05, 0.5, 75.0, 1.0),
     ),
-    "CYAN": MissileVariant(
+    "CYAN": MissileTankRecolor(
         name="item_missile__CY",
         color=(0.05, 10.0, 10.0, 1.0),
     ),
-    "PURPLE": MissileVariant(
+    "PURPLE": MissileTankRecolor(
         name="item_missile__PR",
         color=(15.0, 0.5, 70.0, 1.0),
     ),
-    "PINK": MissileVariant(
+    "PINK": MissileTankRecolor(
         name="item_missile__PK",
         color=(70.0, 0.5, 7.0, 1.0),
     ),
-    "MAGENTA": MissileVariant(
+    "MAGENTA": MissileTankRecolor(
         name="item_missile__MG",
         color=(70.0, 0.5, 70.0, 1.0),
     ),
-    "WHITE": MissileVariant(
+    "WHITE": MissileTankRecolor(
         name="item_missile__WH",
         color=(30.0, 30.0, 30.0, 1.0),
     ),
-    "BLACK": MissileVariant(
+    "BLACK": MissileTankRecolor(
         name="item_missile__BK",
         color=(0.0, 0.0, 0.0, 1.0),
     ),
-    "GRAY": MissileVariant(
+    "GRAY": MissileTankRecolor(
         name="item_missile__GY",
         color=(0.2, 0.2, 0.2, 1.0),
     ),
 }
 
 
 def generate_missile_colors(editor: PatcherEditor):
-    for _, variant in ALL_VARIANTS.items():
-        mat_dat = MaterialData(
-            base_mat="actors/items/item_missiletank/models/imats/item_missiletank_mp_fxhologram_01.bsmat",
-            new_mat_name=variant.mat_name,
-            new_path=variant.shader_path,
-            uniform_params={
-                "vTex0EmissiveColor": variant.rgba
-            }
-        )
-
-        model_dat = ModelData(
-            base_model="actors/items/item_missiletank/models/item_missiletank.bcmdl",
-            new_path=variant.model_path,
-            materials={"mp_fxhologram_01": variant.shader_path}
-        )
-
-        create_custom_material(editor, mat_dat)
-        create_custom_model(editor, model_dat)
+    for _, recolor in MISSILE_TANK_RECOLORS.items():
+        recolor.generate(editor)
```

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/door_locks/custom_door_types.py` & `open-dread-rando-2.9.0/src/open_dread_rando/door_locks/custom_door_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -341,14 +341,61 @@
                                                   "/textures/doorshieldpowerbomb_alt_bc.bctex")},
                     "texAttributes": {"filepath": SMOOTH_NORMALS},
                     "texNormals": {"filepath": SMOOTH_NORMALS}
                 }
             )
         ],
     ),
+
+    "closed": ShieldData(
+        name="doorshieldclosed",
+        type=DoorTemplates.TRIANGLES,
+        weaknesses=[],
+        actordef="actors/props/doorshieldclosed/charclasses/doorshieldclosed.bmsad",
+        default_mdl=ModelData(
+            base_model=SUPER_MDL,
+            new_path="actors/props/doorshieldclosed/models/doorshieldclosed.bcmdl",
+            materials={
+                "mp_opaque_01": ("actors/props/doorshieldclosed/models"
+                                 "/imats/doorshieldclosed_mp_opaque_01.bsmat")
+            }
+        ),
+        default_mats=[
+            MaterialData(
+                base_mat=SUPER_MAT,
+                new_mat_name="doorshieldclosed_mp_opaque_01",
+                new_path="actors/props/doorshieldclosed/models/imats/doorshieldclosed_mp_opaque_01.bsmat",
+                uniform_params={
+                    "vAlbedoEmissiveColorMultiplier": [1.0, 0.0, 0.0, 1.0]
+                },
+                sampler_params={
+                    "texBaseColor": {"filepath": ("actors/props/doorshieldclosed/models"
+                                                  "/textures/doorshieldclosed_bc.bctex")},
+                    "texAttributes": {"filepath": SMOOTH_ATTRIBUTES},
+                    "texNormals": {"filepath": SMOOTH_NORMALS}
+                }
+            )
+        ],
+        alternate_mats=[
+            MaterialData(
+                base_mat=SUPER_MAT,
+                new_mat_name="doorshieldclosed_mp_opaque_01",
+                new_path="actors/props/doorshieldclosed/models/imats/doorshieldclosed_mp_opaque_01.bsmat",
+                uniform_params={
+                    "vAlbedoEmissiveColorMultiplier": [1.0, 0.0, 0.0, 1.0]
+                },
+                sampler_params={
+                    "texBaseColor": {"filepath": ("actors/props/doorshieldclosed/models"
+                                                  "/textures/doorshieldclosed_alt_bc.bctex")},
+                    "texAttributes": {"filepath": SMOOTH_ATTRIBUTES},
+                    "texNormals": {"filepath": SMOOTH_NORMALS}
+                }
+            )
+        ]
+    )
 }
 
 
 class BaseShield:
     def __init__(self, shield: ShieldData):
         self.data = shield
```

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/door_locks/door_patcher.py` & `open-dread-rando-2.9.0/src/open_dread_rando/door_locks/door_patcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     SHIELD_MISSILE = ("BlockageMissile", (-300, -150, 0, 300))
     SHIELD_SUPER_MISSILE = ("BlockageSuperMissile", (-300, -150, 0, 300))
     SHIELD_ICE_MISSILE = ("BlockageIce", (-300, -150, 0, 300))
     SHIELD_STORM_MISSILE = ("BlockageStorm", (-300, -150, 0, 300))
     SHIELD_BOMB = ("BlockageBomb", (-300, -150, 0, 300))
     SHIELD_CROSS_BOMB = ("BlockageCrossBomb", (-300, -150, 0, 300))
     SHIELD_POWER_BOMB = ("BlockagePowerBomb", (-300, -150, 0, 300))
+    SHIELD_CLOSED = ("BlockageClosed", (-300, -150, 0, 300))
 
     def __init__(self, icon_id: str, offsets: tuple[float, float, float, float]):
         """
         Initializes a new MinimapIconData with the given icon id and offsets for the left-facing direction
         """
         self.icon_id = icon_id
         self.oBox_min = (offsets[0], offsets[2])
@@ -105,14 +106,15 @@
     SHIELD_MISSILE = (["doorshieldmissile"], MinimapIconData.SHIELD_MISSILE)
     SHIELD_SUPER_MISSILE = (["doorshieldsupermissile"], MinimapIconData.SHIELD_SUPER_MISSILE)
     SHIELD_ICE_MISSILE = (["doorshieldicemissile"], MinimapIconData.SHIELD_ICE_MISSILE)
     SHIELD_STORM_MISSILE = (["doorshieldstormmissile"], MinimapIconData.SHIELD_STORM_MISSILE)
     SHIELD_BOMB = (["doorshieldbomb"], MinimapIconData.SHIELD_BOMB)
     SHIELD_CROSS_BOMB = (["doorshieldcrossbomb"], MinimapIconData.SHIELD_CROSS_BOMB)
     SHIELD_POWER_BOMB = (["doorshieldpowerbomb"], MinimapIconData.SHIELD_POWER_BOMB)
+    SHIELD_CLOSED = (["doorshieldclosed"], MinimapIconData.SHIELD_CLOSED)
 
     def __init__(self, actordef: list[str], minimap: MinimapIconData):
         # generate actordefs
         self.actordefs = [f"actors/props/{v}/charclasses/{v}.bmsad" for v in actordef]
         self.minimapData = minimap
 
 
@@ -148,14 +150,16 @@
                   ["actors/props/doorshieldmissile", "actors/props/doorshieldsupermissile"])
     POWER_BOMB = ("power_bomb", ActorData.DOOR_POWER, True, ActorData.SHIELD_POWER_BOMB, True, True,
                   ["actors/props/doorshieldmissile", "actors/props/doorshieldsupermissile"])
     GRAPPLE = ("grapple_beam", ActorData.DOOR_GRAPPLE, False, None, True, True,
                ["actors/props/door"])
     PRESENCE = ("phantom_cloak", ActorData.DOOR_PRESENCE, False, None, True, False,
                 ["actors/props/door"])
+    CLOSED = ("closed", ActorData.DOOR_POWER, True, ActorData.SHIELD_CLOSED, True, True,
+              ["actors/props/doorshieldmissile", "actors/props/doorshieldsupermissile"])
 
     def __init__(self, rdv_door_type: str, door_data: ActorData, need_shield: bool = False,
                  shield_data: ActorData = None, can_be_removed: bool = True, can_be_added: bool = True,
                  additional_asset_folders: list[str] = None):
         self.type = rdv_door_type
         self.need_shield = need_shield
         self.door = door_data
```

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/dread_patcher.py` & `open-dread-rando-2.9.0/src/open_dread_rando/dread_patcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from open_dread_rando.cosmetic_patches.missile_color_patcher import generate_missile_colors
 from open_dread_rando.door_locks.custom_door_types import create_all_shield_assets
 from open_dread_rando.door_locks.door_patcher import DoorPatcher
 from open_dread_rando.files import files_path
 from open_dread_rando.logger import LOG
 from open_dread_rando.misc_patches import elevator, lua_util
 from open_dread_rando.misc_patches.exefs import include_depackager, patch_exefs
+from open_dread_rando.misc_patches.model_patcher import generate_custom_models
 from open_dread_rando.misc_patches.sprite_patches import patch_sprites
 from open_dread_rando.misc_patches.text_patches import apply_text_patches, patch_credits, patch_hints, patch_text
 from open_dread_rando.misc_patches.tilegroup_patcher import patch_tilegroup
 from open_dread_rando.output_config import output_format_for_category, output_paths_for_compatibility
 from open_dread_rando.patcher_editor import PatcherEditor
 from open_dread_rando.pickups.lua_editor import LuaEditor
 from open_dread_rando.pickups.pickup import pickup_object_for
@@ -199,14 +200,15 @@
 
     editor = PatcherEditor(input_path)
     lua_scripts = LuaEditor()
 
     # Copy custom files
     add_custom_files(editor)
     generate_missile_colors(editor)
+    generate_custom_models(editor)
 
     # Apply fixes
     apply_static_fixes(editor)
 
     # Update init.lc
     lua_util.create_script_copy(editor, "system/scripts/init")
     editor.replace_asset(
```

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/custom_scenario.lua` & `open-dread-rando-2.9.0/src/open_dread_rando/files/custom_scenario.lua`

 * *Files 1% similar despite different names*

```diff
@@ -248,14 +248,18 @@
 end
 
 Scenario._BlastShieldTypes = {
     doorshieldsupermissile = {
         item = "ITEM_WEAPON_SUPER_MISSILE",
         damage = {"SUPER_MISSILE", "ICE_MISSILE"},
     },
+    doorwidebeam = {
+        item = "ITEM_WEAPON_WIDE_BEAM",
+        damage = {"POWER_BEAM", "WIDE_BEAM"}
+    },
     door_shield_plasma = {
         item = "ITEM_WEAPON_PLASMA_BEAM",
         damage = {"PLASMA_BEAM"}
     },
     doorshieldbomb = {
         item = "ITEM_WEAPON_BOMB",
         damage = {"BOMB"}
```

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/dread_depackager/main.npdm` & `open-dread-rando-2.9.0/src/open_dread_rando/files/dread_depackager/main.npdm`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/dread_depackager/subsdk9` & `open-dread-rando-2.9.0/src/open_dread_rando/files/dread_depackager/subsdk9`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/levels/s010_cave.lc.lua` & `open-dread-rando-2.9.0/src/open_dread_rando/files/levels/s010_cave.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/levels/s020_magma.lc.lua` & `open-dread-rando-2.9.0/src/open_dread_rando/files/levels/s020_magma.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/levels/s030_baselab.lc.lua` & `open-dread-rando-2.9.0/src/open_dread_rando/files/levels/s030_baselab.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/levels/s040_aqua.lc.lua` & `open-dread-rando-2.9.0/src/open_dread_rando/files/levels/s040_aqua.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/levels/s050_forest.lc.lua` & `open-dread-rando-2.9.0/src/open_dread_rando/files/levels/s050_forest.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/levels/s060_quarantine.lc.lua` & `open-dread-rando-2.9.0/src/open_dread_rando/files/levels/s060_quarantine.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/levels/s070_basesanc.lc.lua` & `open-dread-rando-2.9.0/src/open_dread_rando/files/levels/s070_basesanc.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/levels/s080_shipyard.lc.lua` & `open-dread-rando-2.9.0/src/open_dread_rando/files/levels/s080_shipyard.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/levels/s090_skybase.lc.lua` & `open-dread-rando-2.9.0/src/open_dread_rando/files/levels/s090_skybase.lc.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/lua_libraries/bit.lua` & `open-dread-rando-2.9.0/src/open_dread_rando/files/lua_libraries/bit.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/lua_libraries/data_structures.lua` & `open-dread-rando-2.9.0/src/open_dread_rando/files/lua_libraries/data_structures.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/lua_libraries/death_counter.lua` & `open-dread-rando-2.9.0/src/open_dread_rando/files/lua_libraries/death_counter.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/lua_libraries/disconnect_gui.lua` & `open-dread-rando-2.9.0/src/open_dread_rando/files/lua_libraries/disconnect_gui.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/lua_libraries/guilib.lua` & `open-dread-rando-2.9.0/src/open_dread_rando/files/lua_libraries/guilib.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/lua_libraries/input_handling.lua` & `open-dread-rando-2.9.0/src/open_dread_rando/files/lua_libraries/input_handling.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/lua_libraries/room_names.lua` & `open-dread-rando-2.9.0/src/open_dread_rando/files/lua_libraries/room_names.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/msemenu_mainmenu.lua` & `open-dread-rando-2.9.0/src/open_dread_rando/files/msemenu_mainmenu.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/randomizer_powerup.lua` & `open-dread-rando-2.9.0/src/open_dread_rando/files/randomizer_powerup.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_missile_mp_opaque_01.bsmat`

 * *Files 2% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 00000000: 4d53 5552 0200 1100 706f 7765 7275 705f  MSUR....powerup_
-00000010: 7375 7065 726d 6973 7369 6c65 5f6d 705f  supermissile_mp_
-00000020: 6f70 6171 7565 5f30 3100 0100 0000 1f00  opaque_01.......
-00000030: 0000 7379 7374 656d 2f73 6864 2f6d 705f  ..system/shd/mp_
-00000040: 6f70 6171 7565 2e62 7368 6461 7400 0000  opaque.bshdat...
-00000050: 0000 0001 0000 0000 0000 0003 0000 0000  ................
-00000060: ffff ff00 ffff ffff 0100 0000 0100 0000  ................
-00000070: 0100 0000 0100 0000 0000 0000 0006 0000  ................
-00000080: 0000 0000 3f00 0000 0001 0104 0000 0001  ....?...........
-00000090: 0000 0000 0200 0000 0000 0000 0000 0000  ................
-000000a0: 0000 0000 0100 0000 0b00 0000 6641 6c62  ............fAlb
-000000b0: 6564 6f45 6d69 7373 6976 6546 6163 746f  edoEmissiveFacto
-000000c0: 7200 6601 0000 0000 0000 0066 416c 6265  r.f........fAlbe
-000000d0: 646f 456d 6973 7369 7665 436f 6c6f 724d  doEmissiveColorM
-000000e0: 756c 7469 706c 6965 7200 6604 0000 0000  ultiplier.f.....
-000000f0: 0080 3f00 0080 3f00 0080 3f00 0080 3f66  ..?...?...?...?f
-00000100: 526f 7567 686e 6573 7346 6163 746f 7200  RoughnessFactor.
-00000110: 6601 0000 0000 0080 3f66 5370 6563 756c  f.......?fSpecul
-00000120: 6172 506f 7765 7200 6601 0000 0000 0080  arPower.f.......
-00000130: 3f66 4d65 7461 6c00 6601 0000 006f 1203  ?fMetal.f....o..
-00000140: 3b76 436f 6e73 7461 6e74 3000 6604 0000  ;vConstant0.f...
-00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000160: 0076 436f 6e73 7461 6e74 3100 6604 0000  .vConstant1.f...
-00000170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000180: 0076 436f 6e73 7461 6e74 3200 6604 0000  .vConstant2.f...
-00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001a0: 0076 436f 6e73 7461 6e74 3300 6604 0000  .vConstant3.f...
-000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001c0: 0076 436f 6e73 7461 6e74 3400 6604 0000  .vConstant4.f...
-000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001e0: 0076 436f 6e73 7461 6e74 3500 6604 0000  .vConstant5.f...
-000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0003 0000 0074 6578 4261 7365 436f 6c6f  .....texBaseColo
-00000210: 7200 7361 6d70 6c65 7230 0074 6578 7475  r.sampler0.textu
-00000220: 7265 3244 0000 0000 0061 6374 6f72 732f  re2D.....actors/
-00000230: 6974 656d 732f 706f 7765 7275 705f 7375  items/powerup_su
-00000240: 7065 726d 6973 7369 6c65 2f6d 6f64 656c  permissile/model
-00000250: 732f 7465 7874 7572 6573 2f70 6f77 6572  s/textures/power
-00000260: 7570 5f69 6365 5f5f 6d69 7373 696c 655f  up_ice__missile_
-00000270: 6263 2e62 6374 6578 0003 0000 0003 0000  bc.bctex........
-00000280: 0003 0000 0001 0000 0002 0000 0002 0000  ................
-00000290: 00ff ffff 0f00 0000 0000 0000 0000 0000  ................
-000002a0: 4100 0080 4100 0000 0074 6578 4174 7472  A...A....texAttr
-000002b0: 6962 7574 6573 0073 616d 706c 6572 3100  ibutes.sampler1.
-000002c0: 7465 7874 7572 6532 4400 0100 0000 6163  texture2D.....ac
-000002d0: 746f 7273 2f69 7465 6d73 2f70 6f77 6572  tors/items/power
-000002e0: 7570 5f73 7570 6572 6d69 7373 696c 652f  up_supermissile/
-000002f0: 6d6f 6465 6c73 2f74 6578 7475 7265 732f  models/textures/
-00000300: 706f 7765 7275 705f 7375 7065 726d 6973  powerup_supermis
-00000310: 7369 6c65 5f61 742e 6263 7465 7800 0300  sile_at.bctex...
-00000320: 0000 0300 0000 0300 0000 0100 0000 0200  ................
-00000330: 0000 0200 0000 ffff ff0f 0000 0000 0000  ................
-00000340: 0000 0000 0041 0000 8041 0000 0000 7465  .....A...A....te
-00000350: 784e 6f72 6d61 6c73 0073 616d 706c 6572  xNormals.sampler
-00000360: 3200 7465 7874 7572 6532 4400 0200 0000  2.texture2D.....
-00000370: 6163 746f 7273 2f69 7465 6d73 2f70 6f77  actors/items/pow
-00000380: 6572 7570 5f73 7570 6572 6d69 7373 696c  erup_supermissil
-00000390: 652f 6d6f 6465 6c73 2f74 6578 7475 7265  e/models/texture
-000003a0: 732f 706f 7765 7275 705f 7375 7065 726d  s/powerup_superm
-000003b0: 6973 7369 6c65 5f6e 6d2e 6263 7465 7800  issile_nm.bctex.
-000003c0: 0300 0000 0300 0000 0300 0000 0100 0000  ................
-000003d0: 0200 0000 0200 0000 ffff ff0f 0000 0000  ................
-000003e0: 0000 0000 0000 0041 0000 8041 0000 0000  .......A...A....
+00000010: 6d69 7373 696c 655f 6d70 5f6f 7061 7175  missile_mp_opaqu
+00000020: 655f 3031 0001 0000 001f 0000 0073 7973  e_01.........sys
+00000030: 7465 6d2f 7368 642f 6d70 5f6f 7061 7175  tem/shd/mp_opaqu
+00000040: 652e 6273 6864 6174 0000 0000 0000 0100  e.bshdat........
+00000050: 0000 0000 0000 0300 0000 00ff ffff 00ff  ................
+00000060: ffff ff01 0000 0001 0000 0001 0000 0001  ................
+00000070: 0000 0000 0000 0000 0600 0000 0000 003f  ...............?
+00000080: 0000 0000 0101 0400 0000 0100 0000 0002  ................
+00000090: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+000000a0: 0000 000b 0000 0066 416c 6265 646f 456d  .......fAlbedoEm
+000000b0: 6973 7369 7665 4661 6374 6f72 0066 0100  issiveFactor.f..
+000000c0: 0000 0000 0000 6641 6c62 6564 6f45 6d69  ......fAlbedoEmi
+000000d0: 7373 6976 6543 6f6c 6f72 4d75 6c74 6970  ssiveColorMultip
+000000e0: 6c69 6572 0066 0400 0000 0000 803f 0000  lier.f.......?..
+000000f0: 803f 0000 803f 0000 803f 6652 6f75 6768  .?...?...?fRough
+00000100: 6e65 7373 4661 6374 6f72 0066 0100 0000  nessFactor.f....
+00000110: 0000 803f 6653 7065 6375 6c61 7250 6f77  ...?fSpecularPow
+00000120: 6572 0066 0100 0000 0000 803f 664d 6574  er.f.......?fMet
+00000130: 616c 0066 0100 0000 6f12 033b 7643 6f6e  al.f....o..;vCon
+00000140: 7374 616e 7430 0066 0400 0000 0000 0000  stant0.f........
+00000150: 0000 0000 0000 0000 0000 0000 7643 6f6e  ............vCon
+00000160: 7374 616e 7431 0066 0400 0000 0000 0000  stant1.f........
+00000170: 0000 0000 0000 0000 0000 0000 7643 6f6e  ............vCon
+00000180: 7374 616e 7432 0066 0400 0000 0000 0000  stant2.f........
+00000190: 0000 0000 0000 0000 0000 0000 7643 6f6e  ............vCon
+000001a0: 7374 616e 7433 0066 0400 0000 0000 0000  stant3.f........
+000001b0: 0000 0000 0000 0000 0000 0000 7643 6f6e  ............vCon
+000001c0: 7374 616e 7434 0066 0400 0000 0000 0000  stant4.f........
+000001d0: 0000 0000 0000 0000 0000 0000 7643 6f6e  ............vCon
+000001e0: 7374 616e 7435 0066 0400 0000 0000 0000  stant5.f........
+000001f0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00000200: 7465 7842 6173 6543 6f6c 6f72 0073 616d  texBaseColor.sam
+00000210: 706c 6572 3000 7465 7874 7572 6532 4400  pler0.texture2D.
+00000220: 0000 0000 6163 746f 7273 2f69 7465 6d73  ....actors/items
+00000230: 2f70 6f77 6572 7570 5f73 7570 6572 6d69  /powerup_supermi
+00000240: 7373 696c 652f 6d6f 6465 6c73 2f74 6578  ssile/models/tex
+00000250: 7475 7265 732f 706f 7765 7275 705f 6d69  tures/powerup_mi
+00000260: 7373 696c 655f 6263 2e62 6374 6578 0003  ssile_bc.bctex..
+00000270: 0000 0003 0000 0003 0000 0001 0000 0002  ................
+00000280: 0000 0002 0000 00ff ffff 0f00 0000 0000  ................
+00000290: 0000 0000 0000 4100 0080 4100 0000 0074  ......A...A....t
+000002a0: 6578 4174 7472 6962 7574 6573 0073 616d  exAttributes.sam
+000002b0: 706c 6572 3100 7465 7874 7572 6532 4400  pler1.texture2D.
+000002c0: 0100 0000 6163 746f 7273 2f69 7465 6d73  ....actors/items
+000002d0: 2f70 6f77 6572 7570 5f73 7570 6572 6d69  /powerup_supermi
+000002e0: 7373 696c 652f 6d6f 6465 6c73 2f74 6578  ssile/models/tex
+000002f0: 7475 7265 732f 706f 7765 7275 705f 7375  tures/powerup_su
+00000300: 7065 726d 6973 7369 6c65 5f61 742e 6263  permissile_at.bc
+00000310: 7465 7800 0300 0000 0300 0000 0300 0000  tex.............
+00000320: 0100 0000 0200 0000 0200 0000 ffff ff0f  ................
+00000330: 0000 0000 0000 0000 0000 0041 0000 8041  ...........A...A
+00000340: 0000 0000 7465 784e 6f72 6d61 6c73 0073  ....texNormals.s
+00000350: 616d 706c 6572 3200 7465 7874 7572 6532  ampler2.texture2
+00000360: 4400 0200 0000 6163 746f 7273 2f69 7465  D.....actors/ite
+00000370: 6d73 2f70 6f77 6572 7570 5f73 7570 6572  ms/powerup_super
+00000380: 6d69 7373 696c 652f 6d6f 6465 6c73 2f74  missile/models/t
+00000390: 6578 7475 7265 732f 706f 7765 7275 705f  extures/powerup_
+000003a0: 7375 7065 726d 6973 7369 6c65 5f6e 6d2e  supermissile_nm.
+000003b0: 6263 7465 7800 0300 0000 0300 0000 0300  bctex...........
+000003c0: 0000 0100 0000 0200 0000 0200 0000 ffff  ................
+000003d0: ff0f 0000 0000 0000 0000 0000 0041 0000  .............A..
+000003e0: 8041 0000 0000                           .A....
```

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_icemissile.bcmdl`

 * *Files 1% similar despite different names*

```diff
@@ -1729,17 +1729,17 @@
 00006c00: 0394 cfbe 5238 0400 00ff ffff ffff ffff  ....R8..........
 00006c10: 1070 0000 0000 0000 0000 0000 0000 0000  .p..............
 00006c20: 2870 0000 0000 0000 0000 0000 0000 0000  (p..............
 00006c30: 6d70 5f6f 7061 7175 655f 3031 0061 6374  mp_opaque_01.act
 00006c40: 6f72 732f 6974 656d 732f 706f 7765 7275  ors/items/poweru
 00006c50: 705f 7375 7065 726d 6973 7369 6c65 2f6d  p_supermissile/m
 00006c60: 6f64 656c 732f 696d 6174 732f 706f 7765  odels/imats/powe
-00006c70: 7275 705f 6963 655f 5f6d 6973 7369 6c65  rup_ice__missile
-00006c80: 5f6d 705f 6f70 6171 7565 5f30 312e 6273  _mp_opaque_01.bs
-00006c90: 6d61 7400 0070 6f77 6572 7570 5f73 7570  mat..powerup_sup
+00006c70: 7275 705f 6963 656d 6973 7369 6c65 5f6d  rup_icemissile_m
+00006c80: 705f 6f70 6171 7565 5f30 312e 6273 6d61  p_opaque_01.bsma
+00006c90: 7400 0000 0070 6f77 6572 7570 5f73 7570  t....powerup_sup
 00006ca0: 6572 6d69 7373 696c 655f 6263 00ff ffff  ermissile_bc....
 00006cb0: 0000 0000 0000 0000 0000 0000 0000 803f  ...............?
 00006cc0: 0000 803f 0000 0000 0000 0000 0000 0000  ...?............
 00006cd0: 0200 0000 0200 0000 0000 0000 0000 0000  ................
 00006ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006cf0: 706f 7765 7275 705f 7375 7065 726d 6973  powerup_supermis
 00006d00: 7369 6c65 5f6e 6d00 0000 0000 0000 0000  sile_nm.........
```

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_icemissile_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/doorshieldbomb_alt_bc.bctex` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/doorshieldbomb_alt_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/doorshieldbomb_bc.bctex` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/doorshieldbomb_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/models/textures/doorshieldcrossbomb_alt_bc.bctex` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/models/textures/doorshieldcrossbomb_alt_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/models/textures/doorshieldicemissile_alt_bc.bctex` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/models/textures/doorshieldicemissile_alt_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/shield_no_attribs_at.bctex` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/shield_no_attribs_at.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/shield_no_normals_nm.bctex` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/shield_no_normals_nm.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_alt_bc.bctex` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_alt_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_rdv_bc.bctex` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_rdv_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/doorshieldstormmissile_alt_bc.bctex` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/doorshieldstormmissile_alt_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/doorshieldstormmissile_bc.bctex` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/doorshieldstormmissile_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/models/textures/shield_diffusion_alt_bc.bctex` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/actors/props/shield_diffusion/models/textures/shield_diffusion_alt_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/romfs/textures/gui/textures/hud_tileset.bctex` & `open-dread-rando-2.9.0/src/open_dread_rando/files/romfs/textures/gui/textures/hud_tileset.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/schema.json` & `open-dread-rando-2.9.0/src/open_dread_rando/files/schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999998973113551%*

 * *Differences: {"'properties'": "{'cosmetic_patches': {'properties': {'shield_versions': {'properties': "*

 * *                 "{'closed': OrderedDict([('type', 'string'), ('enum', ['DEFAULT', 'ALTERNATE']), "*

 * *                 "('default', 'DEFAULT')])}}}}, 'door_patches': {'items': {'properties': "*

 * *                 "{'door_type': {'enum': {insert: [(16, 'closed')]}}}}}}"}*

```diff
@@ -272,14 +272,22 @@
                             "default": "DEFAULT",
                             "enum": [
                                 "DEFAULT",
                                 "ALTERNATE"
                             ],
                             "type": "string"
                         },
+                        "closed": {
+                            "default": "DEFAULT",
+                            "enum": [
+                                "DEFAULT",
+                                "ALTERNATE"
+                            ],
+                            "type": "string"
+                        },
                         "cross_bomb": {
                             "default": "DEFAULT",
                             "enum": [
                                 "DEFAULT",
                                 "ALTERNATE"
                             ],
                             "type": "string"
@@ -354,15 +362,16 @@
                             "super_missile",
                             "storm_missile",
                             "ice_missile",
                             "grapple_beam",
                             "sensor_door",
                             "bomb",
                             "cross_bomb",
-                            "power_bomb"
+                            "power_bomb",
+                            "closed"
                         ],
                         "type": "string"
                     }
                 },
                 "required": [
                     "actor",
                     "door_type"
```

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/templates/custom_core_x.lua` & `open-dread-rando-2.9.0/src/open_dread_rando/files/templates/custom_core_x.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/templates/custom_core_x_superquetzoa.lua` & `open-dread-rando-2.9.0/src/open_dread_rando/files/templates/custom_core_x_superquetzoa.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/templates/custom_init.lua` & `open-dread-rando-2.9.0/src/open_dread_rando/files/templates/custom_init.lua`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     Game.LoadScenario("c10_samus", Init.sStartingScenario, Init.sStartingActor, "", 1)
 end
 
 function Init.SaveGameAtStartingLocation()
     Game.SaveGame("savedata", "IntroEnd", Init.sStartingActor, true)
 end
 
-Init.sThisRandoIdentifier = TEMPLATE("configuration_identifier")
+Init.sThisRandoIdentifier = TEMPLATE("configuration_identifier") .. Init.sLayoutUUID
 
 local original_Init_CreateNewGameData = Init.CreateNewGameData
 function Init.CreateNewGameData(difficulty)
     original_Init_CreateNewGameData(difficulty)
 
     local playerSection =  Game.GetPlayerBlackboardSectionName()
```

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/templates/template_doorshield_energy.bmsad` & `open-dread-rando-2.9.0/src/open_dread_rando/files/templates/template_doorshield_energy.bmsad`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/templates/template_doorshield_hexs.bmsad` & `open-dread-rando-2.9.0/src/open_dread_rando/files/templates/template_doorshield_hexs.bmsad`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/templates/template_doorshield_tris.bmsad` & `open-dread-rando-2.9.0/src/open_dread_rando/files/templates/template_doorshield_tris.bmsad`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/files/templates/template_powerup.bmsad` & `open-dread-rando-2.9.0/src/open_dread_rando/files/templates/template_powerup.bmsad`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/misc_patches/elevator.py` & `open-dread-rando-2.9.0/src/open_dread_rando/misc_patches/elevator.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/misc_patches/exefs.py` & `open-dread-rando-2.9.0/src/open_dread_rando/misc_patches/exefs.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/misc_patches/lua_util.py` & `open-dread-rando-2.9.0/src/open_dread_rando/misc_patches/lua_util.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/misc_patches/material_patcher.py` & `open-dread-rando-2.9.0/src/open_dread_rando/misc_patches/material_patcher.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/misc_patches/sprite_patches.py` & `open-dread-rando-2.9.0/src/open_dread_rando/misc_patches/sprite_patches.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/misc_patches/text_patches.py` & `open-dread-rando-2.9.0/src/open_dread_rando/misc_patches/text_patches.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import typing
 
 from mercury_engine_data_structures.formats import Txt
 
 if typing.TYPE_CHECKING:
     from open_dread_rando.patcher_editor import PatcherEditor
 
-# may want to edit all the localization files?
+# We want to edit all the localization files, not just english
 ALL_TEXT_FILES = {
-    # "eu_dutch.txt",
-    # "eu_french.txt",
-    # "eu_german.txt",
-    # "eu_italian.txt",
-    # "eu_spanish.txt",
-    # "japanese.txt",
-    # "korean.txt",
-    # "russian.txt",
-    # "simplified_chinese.txt",
-    # "traditional_chinese.txt",
+    "eu_dutch.txt",
+    "eu_french.txt",
+    "eu_german.txt",
+    "eu_italian.txt",
+    "eu_spanish.txt",
+    "japanese.txt",
+    "korean.txt",
+    "russian.txt",
+    "simplified_chinese.txt",
+    "traditional_chinese.txt",
     "us_english.txt",
-    # "us_french.txt",
-    # "us_spanish.txt"
+    "us_french.txt",
+    "us_spanish.txt"
 }
 
 
 def patch_text(editor: PatcherEditor, key: str, value: str):
     for text_file in ALL_TEXT_FILES:
         text = editor.get_file(f"system/localization/{text_file}", Txt)
         text.strings[key] = value
```

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/misc_patches/tilegroup_patcher.py` & `open-dread-rando-2.9.0/src/open_dread_rando/misc_patches/tilegroup_patcher.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/output_config.py` & `open-dread-rando-2.9.0/src/open_dread_rando/output_config.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/patch_util.py` & `open-dread-rando-2.9.0/src/open_dread_rando/patch_util.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/patcher_editor.py` & `open-dread-rando-2.9.0/src/open_dread_rando/patcher_editor.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/pickups/lua_editor.py` & `open-dread-rando-2.9.0/src/open_dread_rando/pickups/lua_editor.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/pickups/map_icons.py` & `open-dread-rando-2.9.0/src/open_dread_rando/pickups/map_icons.py`

 * *Files 2% similar despite different names*

```diff
@@ -357,14 +357,30 @@
         icon_id="BlockagePowerBombR",
         coords=(11,3),
         disabled_id="BlockageDisabledR",
         label="POWER BOMB COVER",
         offset=(0.800000011920929, -0.4000000059604645),
         auto_scale=False
     ),
+    "BlockageClosedL": MapIcon(
+        icon_id="BlockageClosedL",
+        coords=(5,1),
+        disabled_id="BlockageDisabledL",
+        label="ACCESS CLOSED",
+        offset=(-0.800000011920929, -0.4000000059604645),
+        auto_scale=False
+    ),
+    "BlockageClosedR": MapIcon(
+        icon_id="BlockageClosedR",
+        coords=(5,1),
+        disabled_id="BlockageDisabledR",
+        label="ACCESS CLOSED",
+        offset=(0.800000011920929, -0.4000000059604645),
+        auto_scale=False
+    ),
 }
 ALL_ICONS.update({f"DNA_{i + 1}": MapIcon(
     icon_id=f"ItemDNA{i + 1}",
     coords=(13, 7),
     label=f"METROID DNA {i + 1}"
 ) for i in range(12)})
 
@@ -456,9 +472,10 @@
                 actor = blockages[sName]
                 if actor["sIconId"] in blockages_to_fix:
                     actor["bFlipX"] = True
 
     def add_all_new_door_icons(self):
         for icon in ["BlockageIceL", "BlockageIceR", "BlockageDiffusionL", "BlockageDiffusionR",
                      "BlockageStormL", "BlockageStormR", "BlockageBombL", "BlockageBombR",
-                     "BlockageCrossBombL", "BlockageCrossBombR", "BlockagePowerBombL", "BlockagePowerBombR"]:
+                     "BlockageCrossBombL", "BlockageCrossBombR", "BlockagePowerBombL", "BlockagePowerBombR",
+                     "BlockageClosedL", "BlockageClosedR"]:
             self.add_icon(ALL_ICONS[icon])
```

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/pickups/model_data.py` & `open-dread-rando-2.9.0/src/open_dread_rando/pickups/model_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,31 +111,41 @@
             "actors/items/powerup_grapplebeam/fx/auraitemparticle.bcptl",
             "actors/items/powerup_grapplebeam/models/powerup_grapplebeam.bcmdl",
             "actors/items/powerup_grapplebeam/models/imats/powerup_grapplebeam_grapplebeam.bsmat",
         ),
         grapple_fx=True,
     ),
 
+    "powerup_missile": ModelData(
+        bcmdl_path="actors/items/powerup_supermissile/models/powerup_missile.bcmdl",
+        bmsas="actors/items/powerup_supermissile/charclasses/powerup_supermissile.bmsas",
+        dependencies=(
+            "actors/items/powerup_supermissile/models/powerup_missile.bcmdl",
+            "actors/items/powerup_supermissile/models/imats/powerup_supermissile_hologram.bsmat",
+            "actors/items/powerup_supermissile/models/imats/powerup_missile_mp_opaque_01.bsmat",
+        ),
+    ),
+
     "powerup_supermissile": ModelData(
         bcmdl_path="actors/items/powerup_supermissile/models/powerup_supermissile.bcmdl",
         bmsas="actors/items/powerup_supermissile/charclasses/powerup_supermissile.bmsas",
         dependencies=(
             "actors/items/powerup_supermissile/models/powerup_supermissile.bcmdl",
             "actors/items/powerup_supermissile/models/imats/powerup_supermissile_hologram.bsmat",
             "actors/items/powerup_supermissile/models/imats/powerup_supermissile_mp_opaque_01.bsmat",
         ),
     ),
 
     "powerup_icemissile": ModelData(
-        bcmdl_path="actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl",
+        bcmdl_path="actors/items/powerup_supermissile/models/powerup_icemissile.bcmdl",
         bmsas="actors/items/powerup_supermissile/charclasses/powerup_supermissile.bmsas",
         dependencies=(
-            "actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl",
+            "actors/items/powerup_supermissile/models/powerup_icemissile.bcmdl",
             "actors/items/powerup_supermissile/models/imats/powerup_supermissile_hologram.bsmat",
-            "actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat",
+            "actors/items/powerup_supermissile/models/imats/powerup_icemissile_mp_opaque_01.bsmat",
         ),
     ),
 
     "powerup_stormmissile": ModelData(
         bcmdl_path="actors/items/powerup_supermissile/models/powerup_supermissile.bcmdl",
         bmsas="actors/items/powerup_supermissile/charclasses/powerup_supermissile.bmsas",
         dependencies=(
@@ -430,14 +440,24 @@
         dependencies=(
             "actors/items/item_missiletankplus/models/item_missiletankplus.bcmdl",
             "actors/items/item_missiletankplus/models/imats/item_missiletankplus_mat01.bsmat",
             "actors/items/item_missiletankplus/models/imats/item_missiletankplus_mp_fxhologram_01.bsmat",
         ),
     ),
 
+    "super_missile_expansion": ModelData(
+        bcmdl_path="actors/items/item_missiletankplus/models/super_missile_tank.bcmdl",
+        bmsas="actors/items/item_missiletankplus/charclasses/item_missiletankplus.bmsas",
+        dependencies=(
+            "actors/items/item_missiletankplus/models/super_missile_tank.bcmdl",
+            "actors/items/item_missiletankplus/models/imats/super_missile_tank_mat01.bsmat",
+            "actors/items/item_missiletankplus/models/imats/super_missile_tank_mp_fxhologram_01.bsmat",
+        ),
+    ),
+
     "item_powerbombtank": ModelData(
         bcmdl_path="actors/items/item_powerbombtank/models/item_powerbombtank.bcmdl",
         bmsas="actors/items/item_powerbombtank/charclasses/item_powerbombtank.bmsas",
         dependencies=(
             "actors/items/item_powerbombtank/models/item_powerbombtank.bcmdl",
             "actors/items/item_powerbombtank/models/imats/item_powerbombtank_mat01.bsmat",
             "actors/items/item_powerbombtank/models/imats/item_powerbombtank_mp_fxhologram_01.bsmat",
```

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/pickups/pickup.py` & `open-dread-rando-2.9.0/src/open_dread_rando/pickups/pickup.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/pickups/split_pickups.py` & `open-dread-rando-2.9.0/src/open_dread_rando/pickups/split_pickups.py`

 * *Files 5% similar despite different names*

```diff
@@ -474,12 +474,19 @@
     supers = editor.get_file("actors/props/doorshieldsupermissile/charclasses/doorshieldsupermissile.bmsad", Bmsad)
     super_life = supers.components["LIFE"]
     funcs = list(super_life.functions)
     funcs.pop(1)  # AddDamageSource("SUPER_MISSILE")
     funcs.pop(1)  # AddDamageSource("ICE_MISSILE")
     super_life.functions = funcs
 
+    wide = editor.get_file("actors/props/doorwidebeam/charclasses/doorwidebeam.bmsad", Bmsad)
+    wide_life = wide.components["LIFE"]
+    funcs = list(wide_life.functions)
+    funcs.pop(0)  # AddDamageSource("POWER_BEAM")
+    funcs.pop(0)  # AddDamageSource("WIDE_BEAM")
+    wide_life.functions = funcs
+
     plasma = editor.get_file("actors/props/door_shield_plasma/charclasses/door_shield_plasma.bmsad", Bmsad)
     plasma_life = plasma.components["LIFE"]
     funcs = list(plasma_life.functions)
     funcs.pop(1)  # AddDamageSource("PLASMA_BEAM")
     plasma_life.functions = funcs
```

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/specific_patches/environmental_damage.py` & `open-dread-rando-2.9.0/src/open_dread_rando/specific_patches/environmental_damage.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/specific_patches/environmental_damage_sources.py` & `open-dread-rando-2.9.0/src/open_dread_rando/specific_patches/environmental_damage_sources.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/specific_patches/game_patches.py` & `open-dread-rando-2.9.0/src/open_dread_rando/specific_patches/game_patches.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/specific_patches/objective.py` & `open-dread-rando-2.9.0/src/open_dread_rando/specific_patches/objective.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/specific_patches/static_fixes.py` & `open-dread-rando-2.9.0/src/open_dread_rando/specific_patches/static_fixes.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando/validator_with_default.py` & `open-dread-rando-2.9.0/src/open_dread_rando/validator_with_default.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando.egg-info/PKG-INFO` & `open-dread-rando-2.9.0/src/open_dread_rando.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-dread-rando
-Version: 2.8.3
+Version: 2.9.0
 Summary: An open source randomizer patcher for Metroid Dread.
 Project-URL: Homepage, https://github.com/randovania/open-dread-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.10
@@ -15,22 +15,22 @@
 Provides-Extra: test
 Requires-Dist: lupa; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 
 # Open Dread Rando
-Open Source randomizer patcher for Metroid Dread. Intended for use in [Randovania](https://github.com/randovania).
+Open Source randomizer patcher for Metroid Dread. Intended for use in [Randovania](https://randovania.github.io/).
 Currently supports patching item pickups, starting items, and elevator/shuttle/teleportal destinations.
 
 ## Installation
 `pip install open-dread-rando`
 
 ## Usage
-You will need to provide JSON data matching the [JSON schema](https://github.com/randovania/open-dread-rando/blob/main/open_dread_rando/files/schema.json) in order to successfully patch the game. 
+You will need to provide JSON data matching the [JSON schema](https://github.com/randovania/open-dread-rando/blob/main/src/open_dread_rando/files/schema.json) in order to successfully patch the game. 
 
 The patcher expects a path to an extracted romfs directory of Metroid Dread 1.0.0 or 2.1.0 as well as the desired output directory.
 Output files are in a format compatible with either Atmosphere or Ryujinx, depending on the settings provided.
 
 With a JSON file:
 `python -m open_dread_rando --input-path path/to/dread/romfs --output-path path/to/the/output-mod --input-json path/to/patcher-config.json`
```

### Comparing `open-dread-rando-2.8.3/src/open_dread_rando.egg-info/SOURCES.txt` & `open-dread-rando-2.9.0/src/open_dread_rando.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -71,32 +71,37 @@
 src/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat
 src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl
 src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat
 src/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat
 src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl
 src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mat0001.bsmat
 src/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat
-src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl
-src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat
+src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_icemissile.bcmdl
+src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_missile.bcmdl
+src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_icemissile_mp_opaque_01.bsmat
+src/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_missile_mp_opaque_01.bsmat
 src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl
 src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_autoilum.bsmat
 src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_bola.bsmat
 src/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat
 src/open_dread_rando/files/romfs/actors/props/doorshieldmissile/collisions/shield_bomb_colls.bmscd
 src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex
 src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex
 src/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex
 src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex
 src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex
 src/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex
 src/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex
-src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex
+src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_icemissile_bc.bctex
+src/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_missile_bc.bctex
 src/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex
 src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/doorshieldbomb_alt_bc.bctex
 src/open_dread_rando/files/romfs/textures/actors/props/doorshieldbomb/models/textures/doorshieldbomb_bc.bctex
+src/open_dread_rando/files/romfs/textures/actors/props/doorshieldclosed/models/textures/doorshieldclosed_alt_bc.bctex
+src/open_dread_rando/files/romfs/textures/actors/props/doorshieldclosed/models/textures/doorshieldclosed_bc.bctex
 src/open_dread_rando/files/romfs/textures/actors/props/doorshieldcrossbomb/models/textures/doorshieldcrossbomb_alt_bc.bctex
 src/open_dread_rando/files/romfs/textures/actors/props/doorshieldicemissile/models/textures/doorshieldicemissile_alt_bc.bctex
 src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/shield_no_attribs_at.bctex
 src/open_dread_rando/files/romfs/textures/actors/props/doorshieldmissile/models/textures/shield_no_normals_nm.bctex
 src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_alt_bc.bctex
 src/open_dread_rando/files/romfs/textures/actors/props/doorshieldpowerbomb/models/textures/doorshieldpowerbomb_rdv_bc.bctex
 src/open_dread_rando/files/romfs/textures/actors/props/doorshieldstormmissile/models/textures/doorshieldstormmissile_alt_bc.bctex
```

### Comparing `open-dread-rando-2.8.3/tests/conftest.py` & `open-dread-rando-2.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/tests/test_dread_patcher.py` & `open-dread-rando-2.9.0/tests/test_dread_patcher.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/tests/test_files/april_fools_patcher.json` & `open-dread-rando-2.9.0/tests/test_files/april_fools_patcher.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/tests/test_files/starter_preset_patcher.json` & `open-dread-rando-2.9.0/tests/test_files/starter_preset_patcher.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/tests/test_full_patch.py` & `open-dread-rando-2.9.0/tests/test_full_patch.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/tests/test_lua_util.py` & `open-dread-rando-2.9.0/tests/test_lua_util.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/tools/create_exefs_patches.py` & `open-dread-rando-2.9.0/tools/create_exefs_patches.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-2.8.3/tools/exefs_sources/debug_input.s` & `open-dread-rando-2.9.0/tools/exefs_sources/debug_input.s`

 * *Files identical despite different names*

