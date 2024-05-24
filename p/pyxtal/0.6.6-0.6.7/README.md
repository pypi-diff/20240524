# Comparing `tmp/pyxtal-0.6.6.tar.gz` & `tmp/pyxtal-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxtal-0.6.6.tar", last modified: Mon May  6 01:06:30 2024, max compression
+gzip compressed data, was "pyxtal-0.6.7.tar", last modified: Fri May 24 20:13:54 2024, max compression
```

## Comparing `pyxtal-0.6.6.tar` & `pyxtal-0.6.7.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:30.549897 pyxtal-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-06 01:06:26.000000 pyxtal-0.6.6/LICENSE.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       83 2024-05-06 01:06:26.000000 pyxtal-0.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-06 01:06:30.549897 pyxtal-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-06 01:06:26.000000 pyxtal-0.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:30.513897 pyxtal-0.6.6/pyxtal/
--rw-r--r--   0 runner    (1001) docker     (127)    31243 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/XRD.py
--rw-r--r--   0 runner    (1001) docker     (127)   126538 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/block_crystal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    15342 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/crystal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:30.533897 pyxtal-0.6.6/pyxtal/database/
--rw-r--r--   0 runner    (1001) docker     (127)    22281 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/HM_Full.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/atomic_scattering_params.json
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/bonds.json
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/bug.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:30.541897 pyxtal-0.6.6/pyxtal/database/cifs/
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/0-G62.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/1-G59.cif
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/191.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/2-G71.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/3-G139.cif
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/4-G225.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/ACBNZA01.cif
--rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/AXOSOW01.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/BTO-Amm2.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/BTO.cif
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/FAU.cif
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/Fd3.cif
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/Fd3.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/Fd3m.cif
--rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/GUMMUW.cif
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/GeF2.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/HAHCOI.cif
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/I41amd.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/I4_132.cif
--rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/JAPWIH.cif
--rw-r--r--   0 runner    (1001) docker     (127)   441469 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/LAGNAL.cif
--rw-r--r--   0 runner    (1001) docker     (127)     7132 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/LUFHAW.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/LiCs.cif
--rw-r--r--   0 runner    (1001) docker     (127)    12413 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/MERQIM.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/MPWO.cif
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/NaCl.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/NaSb3F10.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/NbO2.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/NiS-Cm.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/P3_112.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/P4_332.cif
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/P4nmm.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/P6_422.cif
--rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/PAHYON01.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/PPO.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/PVO.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/Pm3.cif
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/Pmmn.vasp
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/Pn3.vasp
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/Pn3m.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/R-3.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/R-3c.cif
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/R32.cif
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/TMPPIO03.cif
--rw-r--r--   0 runner    (1001) docker     (127)    13289 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/WEXBOS.cif
--rw-r--r--   0 runner    (1001) docker     (127)   177150 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/YICMOP.cif
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/anthracene.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/aspirin-c.cif
--rw-r--r--   0 runner    (1001) docker     (127)    12951 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/aspirin.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/benzene.cif
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/bug.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/c_bug.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/c_bug2.vasp
--rw-r--r--   0 runner    (1001) docker     (127)    17895 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/coumarin.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/dist_6_0.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/dist_6_1.cif
--rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/gdh.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/ht_KNbBO.cif
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/ht_cristobalite.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/ht_quartz.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/ice.cif
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/lt_KNbBO.cif
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/lt_cristobalite.cif
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/lt_quartz.cif
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/naphthalene.cif
--rw-r--r--   0 runner    (1001) docker     (127)   317844 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/resorcinol.cif
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/sim-0.vasp
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/sim-1.vasp
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/cifs/xxvi.cif
--rw-r--r--   0 runner    (1001) docker     (127)  1103778 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/clusters.json
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    19164 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/element.py
--rw-r--r--   0 runner    (1001) docker     (127)  9679835 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/k_subgroup.json
--rw-r--r--   0 runner    (1001) docker     (127)    20717 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/layer.csv
--rw-r--r--   0 runner    (1001) docker     (127)    25842 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/layer_generators.csv
--rw-r--r--   0 runner    (1001) docker     (127)    58872 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/layer_symmetry.csv
--rw-r--r--   0 runner    (1001) docker     (127)   294912 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/mech.db
--rw-r--r--   0 runner    (1001) docker     (127)    90734 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/molecules.json
--rw-r--r--   0 runner    (1001) docker     (127)   130892 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/point.csv
--rw-r--r--   0 runner    (1001) docker     (127)   146327 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/point_generators.csv
--rw-r--r--   0 runner    (1001) docker     (127)   301944 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/point_symmetry.csv
--rw-r--r--   0 runner    (1001) docker     (127)    18501 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/rod.csv
--rw-r--r--   0 runner    (1001) docker     (127)    21935 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/rod_generators.csv
--rw-r--r--   0 runner    (1001) docker     (127)    44320 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/rod_symmetry.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/symbols.json
--rw-r--r--   0 runner    (1001) docker     (127)  1245398 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/t_subgroup.json
--rw-r--r--   0 runner    (1001) docker     (127)   259897 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/wyckoff_generators.csv
--rw-r--r--   0 runner    (1001) docker     (127)   251719 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/wyckoff_list.csv
--rw-r--r--   0 runner    (1001) docker     (127)   117892 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/wyckoff_sets.json
--rw-r--r--   0 runner    (1001) docker     (127)   627207 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/database/wyckoff_symmetry.csv
--rw-r--r--   0 runner    (1001) docker     (127)    24634 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    18755 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)    42644 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/elasticity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:30.545897 pyxtal-0.6.6/pyxtal/interface/
--rw-r--r--   0 runner    (1001) docker     (127)    13515 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/interface/LJ.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27559 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/interface/dftb.py
--rw-r--r--   0 runner    (1001) docker     (127)    14489 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/interface/gulp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19373 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/interface/lammpslib.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/interface/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    31490 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/interface/vasprun.py
--rw-r--r--   0 runner    (1001) docker     (127)    23018 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    71828 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)    18102 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/molecular_crystal.py
--rw-r--r--   0 runner    (1001) docker     (127)    66288 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/msg.py
--rw-r--r--   0 runner    (1001) docker     (127)    36170 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:30.545897 pyxtal-0.6.6/pyxtal/optimize/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/optimize/fire.py
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/optimize/fire2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14967 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/optimize/myscipy_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     9529 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/plane.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:30.545897 pyxtal-0.6.6/pyxtal/potentials/
--rw-r--r--   0 runner    (1001) docker     (127)  1820580 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/potentials/CuAg.eam.alloy
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/potentials/LJ_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/potentials/Si.tersoff
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/potentials/SiCGe.tersoff
--rwxr-xr-x   0 runner    (1001) docker     (127)       26 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/potentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18145 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/representation.py
--rw-r--r--   0 runner    (1001) docker     (127)    46115 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/supergroup.py
--rw-r--r--   0 runner    (1001) docker     (127)   144617 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    48128 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)    11061 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/tolerance.py
--rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    13329 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/viz.py
--rw-r--r--   0 runner    (1001) docker     (127)    45527 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/wyckoff_site.py
--rw-r--r--   0 runner    (1001) docker     (127)    21753 2024-05-06 01:06:26.000000 pyxtal-0.6.6/pyxtal/wyckoff_split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:30.549897 pyxtal-0.6.6/pyxtal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-06 01:06:30.000000 pyxtal-0.6.6/pyxtal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-06 01:06:30.000000 pyxtal-0.6.6/pyxtal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 01:06:30.000000 pyxtal-0.6.6/pyxtal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-06 01:06:30.000000 pyxtal-0.6.6/pyxtal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 01:06:30.000000 pyxtal-0.6.6/pyxtal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:06:30.545897 pyxtal-0.6.6/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4251 2024-05-06 01:06:26.000000 pyxtal-0.6.6/scripts/pyxtal_main.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      960 2024-05-06 01:06:26.000000 pyxtal-0.6.6/scripts/pyxtal_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-06 01:06:30.549897 pyxtal-0.6.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1802 2024-05-06 01:06:26.000000 pyxtal-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:13:54.950050 pyxtal-0.6.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-24 20:13:50.000000 pyxtal-0.6.7/LICENSE.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       83 2024-05-24 20:13:50.000000 pyxtal-0.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-24 20:13:54.950050 pyxtal-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-24 20:13:50.000000 pyxtal-0.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:13:54.914050 pyxtal-0.6.7/pyxtal/
+-rw-r--r--   0 runner    (1001) docker     (127)    31243 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/XRD.py
+-rw-r--r--   0 runner    (1001) docker     (127)   134907 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/block_crystal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15342 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/crystal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:13:54.934050 pyxtal-0.6.7/pyxtal/database/
+-rw-r--r--   0 runner    (1001) docker     (127)    22281 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/HM_Full.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/atomic_scattering_params.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/bonds.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/bug.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:13:54.946050 pyxtal-0.6.7/pyxtal/database/cifs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/0-G62.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/1-G59.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/191.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/2-G71.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/3-G139.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/4-G225.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/ACBNZA01.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/AXOSOW01.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/BTO-Amm2.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/BTO.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/FAU.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/Fd3.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/Fd3.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/Fd3m.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/GUMMUW.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/GeF2.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/HAHCOI.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/I41amd.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/I4_132.cif
+-rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/JAPWIH.cif
+-rw-r--r--   0 runner    (1001) docker     (127)   441469 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/LAGNAL.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     7132 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/LUFHAW.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/LiCs.cif
+-rw-r--r--   0 runner    (1001) docker     (127)    12413 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/MERQIM.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/MPWO.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/NaCl.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/NaSb3F10.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/NbO2.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/NiS-Cm.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/P3_112.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/P4_332.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/P4nmm.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/P6_422.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/PAHYON01.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/PPO.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/PVO.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/Pm3.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/Pmmn.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/Pn3.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/Pn3m.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/R-3.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/R-3c.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/R32.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/TMPPIO03.cif
+-rw-r--r--   0 runner    (1001) docker     (127)    13289 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/WEXBOS.cif
+-rw-r--r--   0 runner    (1001) docker     (127)   177150 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/YICMOP.cif
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/anthracene.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/aspirin-c.cif
+-rw-r--r--   0 runner    (1001) docker     (127)    12951 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/aspirin.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/benzene.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/bug.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/c_bug.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/c_bug2.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)    17895 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/coumarin.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/dist_6_0.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/dist_6_1.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/gdh.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/ht_KNbBO.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/ht_cristobalite.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/ht_quartz.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/ice.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/lt_KNbBO.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/lt_cristobalite.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/lt_quartz.cif
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/naphthalene.cif
+-rw-r--r--   0 runner    (1001) docker     (127)   317844 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/resorcinol.cif
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/sim-0.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/sim-1.vasp
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/cifs/xxvi.cif
+-rw-r--r--   0 runner    (1001) docker     (127)  1103778 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/clusters.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19164 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)  9679835 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/k_subgroup.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20717 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/layer.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    25842 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/layer_generators.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    58872 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/layer_symmetry.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   294912 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/mech.db
+-rw-r--r--   0 runner    (1001) docker     (127)    90734 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/molecules.json
+-rw-r--r--   0 runner    (1001) docker     (127)   130892 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/point.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   146327 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/point_generators.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   301944 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/point_symmetry.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    18501 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/rod.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    21935 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/rod_generators.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    44320 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/rod_symmetry.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/symbols.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1245398 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/t_subgroup.json
+-rw-r--r--   0 runner    (1001) docker     (127)   259897 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/wyckoff_generators.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   251719 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/wyckoff_list.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   117892 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/wyckoff_sets.json
+-rw-r--r--   0 runner    (1001) docker     (127)   627207 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/database/wyckoff_symmetry.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    48416 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18755 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42644 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/elasticity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:13:54.946050 pyxtal-0.6.7/pyxtal/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)    13515 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/interface/LJ.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29392 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/interface/dftb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/interface/gulp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19373 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/interface/lammpslib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/interface/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31490 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/interface/vasprun.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23018 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71828 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18102 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/molecular_crystal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66288 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36170 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:13:54.946050 pyxtal-0.6.7/pyxtal/optimize/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/optimize/fire.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/optimize/fire2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14967 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/optimize/myscipy_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9529 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/plane.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:13:54.950050 pyxtal-0.6.7/pyxtal/potentials/
+-rw-r--r--   0 runner    (1001) docker     (127)  1820580 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/potentials/CuAg.eam.alloy
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/potentials/LJ_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/potentials/Si.tersoff
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/potentials/SiCGe.tersoff
+-rwxr-xr-x   0 runner    (1001) docker     (127)       26 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/potentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18145 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46115 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)   144617 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49017 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11061 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/tolerance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21737 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13329 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/viz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45527 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/wyckoff_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21753 2024-05-24 20:13:50.000000 pyxtal-0.6.7/pyxtal/wyckoff_split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:13:54.950050 pyxtal-0.6.7/pyxtal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-24 20:13:54.000000 pyxtal-0.6.7/pyxtal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-24 20:13:54.000000 pyxtal-0.6.7/pyxtal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 20:13:54.000000 pyxtal-0.6.7/pyxtal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-24 20:13:54.000000 pyxtal-0.6.7/pyxtal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 20:13:54.000000 pyxtal-0.6.7/pyxtal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:13:54.950050 pyxtal-0.6.7/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4251 2024-05-24 20:13:50.000000 pyxtal-0.6.7/scripts/pyxtal_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      960 2024-05-24 20:13:50.000000 pyxtal-0.6.7/scripts/pyxtal_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-24 20:13:54.950050 pyxtal-0.6.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1802 2024-05-24 20:13:50.000000 pyxtal-0.6.7/setup.py
```

### Comparing `pyxtal-0.6.6/LICENSE.txt` & `pyxtal-0.6.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/PKG-INFO` & `pyxtal-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxtal
-Version: 0.6.6
+Version: 0.6.7
 Summary: Python code for generation of crystal structures based on symmetry constraints.
 Home-page: https://github.com/qzhu2017/PyXtal
 Author: Scott Fredericks, Qiang Zhu
 Author-email: qiang.zhu@unlv.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyxtal-0.6.6/README.md` & `pyxtal-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/XRD.py` & `pyxtal-0.6.7/pyxtal/XRD.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/__init__.py` & `pyxtal-0.6.7/pyxtal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,16 +400,18 @@
             self.valid = True # Need to add a check function
             if not standard:
                 self.optimize_lattice()
         else:
             if isinstance(seed, dict):
                 self.from_dict()
             elif isinstance(seed, Atoms): #ASE atoms
-                from pymatgen.io.ase import AseAtomsAdaptor
-                pmg_struc = AseAtomsAdaptor.get_structure(seed)
+                #from pymatgen.io.ase import AseAtomsAdaptor
+                #pmg_struc = AseAtomsAdaptor.get_structure(seed)
+                from pyxtal.util import ase2pymatgen
+                pmg_struc = ase2pymatgen(seed)
                 self._from_pymatgen(pmg_struc, tol, a_tol, style=style)
             elif isinstance(seed, Structure): #Pymatgen
                 self._from_pymatgen(seed, tol, style=style)
             elif isinstance(seed, str):
                 if backend=='pymatgen':
                     pmg_struc = Structure.from_file(seed, primitive=True)
                     self._from_pymatgen(pmg_struc, tol, a_tol, style=style)
@@ -658,34 +660,41 @@
         """
 
         from pyxtal.supergroup import supergroups
 
         sup = supergroups(self, G=G, d_tol=d_tol)
         return sup.strucs
 
-
-    def subgroup(self, perms=None, H=None, eps=0.05, idx=None, group_type='t', max_cell=4, min_cell=0):
+    def subgroup(self, perms=None, H=None, eps=0.05, idx=None, group_type='t',
+                 max_cell=4, min_cell=0, N_groups=None):
         """
         Generate a structure with lower symmetry
 
         Args:
             perms: e.g., {"Si": "C"}
             H: space group number (int)
             eps: pertubation term (float)
             idx: list
             group_type (string): `t`, `k` or `t+k`
             max_cell (float): maximum cell reconstruction
             min_cell (float): maximum cell reconstruction
-
+            max_subgroups (int): maximum number of trial subgroups
         Returns:
             a list of pyxtal structures with lower symmetries
         """
 
+        idx, sites, t_types, k_types = self._get_subgroup_ids(H,
+                                                              group_type,
+                                                              idx,
+                                                              max_cell,
+                                                              min_cell)
         #randomly choose a subgroup from the available list
-        idx, sites, t_types, k_types = self._get_subgroup_ids(H, group_type, idx, max_cell, min_cell)
+        if N_groups is not None and len(idx) >= N_groups:
+            idx = sample(idx, N_groups)
+            #print('max_sub_group', len(idx), max_subgroups)
 
         valid_splitters = []
         bad_splitters = []
         for id in idx:
             gtype = (t_types + k_types)[id]
             if gtype == 'k':
                 id -= len(t_types)
@@ -979,15 +988,18 @@
             #print(np.linalg.det(lat1))
             #print(self.lattice)
             #print(self.lattice.matrix)
             #print(splitter.R[:3,:3].T)
             #print(lat1); import sys; sys.exit()
         #print(lattice); print(lattice.matrix)
         if mut_lat:
-            lattice=lattice.mutate(degree=eps, frozen=True)
+            try:
+                lattice=lattice.mutate(degree=eps, frozen=True)
+            except:
+                print('skip lattice mutation mostly for triclinic system')
 
         h = splitter.H
         split_sites = []
         if self.molecular:
             # below only works when the cell does not change
             # Fix when a, b, c swaps
             for i, site in enumerate(self.mol_sites):
@@ -1169,36 +1181,48 @@
         Get number of torsions for molecular xtal
         """
         N_torsions = 0
         for s in self.mol_sites:
             N_torsions += len(s.molecule.torsionlist)
         return N_torsions
 
-    def to_ase(self, resort=True, center_only=False):
+    def to_ase(self, resort=True, center_only=False, add_vaccum=True):
         """
         Export to ase Atoms object.
+
+        Args:
+            resort (bool): resort atoms
+            center (bool): dump only molculer center for mol. xtal
+            add_vaccum (bool): add vaccum for 0/1/2D systems
         """
         if self.valid:
             if self.dim > 0:
                 lattice = self.lattice.copy()
                 if self.molecular:
                     if center_only:
                         coords, species = [], []
                         for site in self.mol_sites:
                             _coords = site.wp.apply_ops(site.position)
                             _coords -= np.floor(_coords)
                             coords.extend(_coords.dot(self.lattice.matrix))
                             species.extend([site.type+1] * site.wp.multiplicity)
                     else:
                         coords, species = self._get_coords_and_species(True)
-                    latt, coords = lattice.add_vacuum(coords, frac=False, PBC=self.PBC)
+                    if add_vaccum:
+                        latt, coords = lattice.add_vacuum(coords, frac=False, PBC=self.PBC)
+                    else:
+                        latt = lattice.matrix
                     atoms = Atoms(species, positions=coords, cell=latt, pbc=self.PBC)
                 else:
                     coords, species = self._get_coords_and_species()
-                    latt, coords = lattice.add_vacuum(coords, PBC=self.PBC)
+                    coords -= np.floor(coords)
+                    if add_vaccum:
+                        latt, coords = lattice.add_vacuum(coords, PBC=self.PBC)
+                    else:
+                        latt = lattice.matrix
                     atoms = Atoms(species, scaled_positions=coords, cell=latt, pbc=self.PBC)
                 if resort:
                     permutation = np.argsort(atoms.numbers)
                     atoms = atoms[permutation]
                 return atoms
 
             else:
@@ -1484,37 +1508,39 @@
                     self.molecules[msite.type] = msite.molecule
             self.mol_sites = sites
         else:
             for site in dict0["sites"]:
                 sites.append(atom_site.load_dict(site))
             self.atom_sites = sites
 
-    def build(self, group, species, numIons, lattice, sites, tol=1e-2, use_hall=False):
+    def build(self, group, species, numIons, lattice, sites, tol=1e-2, dim=3, use_hall=False):
         """
         Build a atomic crystal based on the necessary input
 
         Args:
-            group: 225
-            species: ['Na', 'Cl']
-            numIons: [4, 4]
+            group (int): 225
+            species (list): ['Na', 'Cl']
+            numIons (list): [4, 4]
             lattice: lattice object
-            sites: [[{"4a": [0.0, 0.0, 0.0]}], [{"4b": [0.5, 0.5, 0.5]}]]
+            sites (list): [[{"4a": [0.0, 0.0, 0.0]}], [{"4b": [0.5, 0.5, 0.5]}]]
+            dim (int):
+            use_hll (bool):
         """
 
         from pyxtal.symmetry import choose_wyckoff
 
         if self.molecular:
             raise RuntimeError("Cannot support the molecular crystal")
 
         if type(group) == Group:
             self.group = group
         else:
-            self.group = Group(group, use_hall=use_hall)
+            self.group = Group(group, dim=dim, use_hall=use_hall)
 
-        # Lattica needs some special handling heree
+        # Lattica needs some special handling here
         if type(lattice) != Lattice:
             if type(lattice) == np.ndarray:
                 ltype = self.group.lattice_type
                 if len(lattice) == 3:
                     lattice = Lattice.from_matrix(lattice, ltype=ltype)
                 elif len(lattice) == 6: # cell para
                     [a, b, c, alpha, beta, gamma] = lattice
@@ -1527,17 +1553,17 @@
                 raise ValueError(msg, lattice)
         #else:
         #    print(lattice, type(lattice), type(lattice)==Lattice, type(lattice)!=Lattice)
         #    msg = 'The input lattice needs to be a pyxtal.lattice.Lattice class'
         #    raise ValueError(msg, lattice)
         self.lattice = lattice
 
-        self.dim = 3
+        self.dim = dim
         self.factor = 1.0
-        self.PBC = [1, 1, 1]
+        self.PBC = self.group.PBC
         self.numIons = numIons
         self.species = species
         numIons_added = np.zeros(len(numIons), dtype=int)
         _sites = []
 
         if len(sites) != len(species):
             print(len(sites), len(species))
@@ -1556,15 +1582,15 @@
                             else:
                                 pt = _wp.get_all_positions(pos)[0]
                             _sites.append(atom_site(_wp, pt, sp))
                         else:
                             raise RuntimeError("Cannot interpret site", key)
                 elif len(wp) == 4: # tuple:
                     (key, x, y, z) = wp
-                    _wp = choose_wyckoff(self.group, site=key)
+                    _wp = choose_wyckoff(self.group, site=key, dim=dim)
                     if _wp is not False:
                         if _wp.get_dof() == 0: #fixed pos
                             pt = [0.0, 0.0, 0.0]
                         else:
                             ans = _wp.get_all_positions([x, y, z])
                             if ans is not None:
                                 pt = ans[0]
@@ -1809,14 +1835,15 @@
         """
         Transform a crystal with speical sites to subgroup
         represenatation with general sites
 
         Args:
             Path: list of path to get the general sites
             iterate (bool): whether or not do it iteratively
+            species : to add
         """
         if not self.standard_setting:
             self.optimize_lattice(standard=True)
         if species is None: species = self.species
 
         # Compute the path is needed
         if path is None:
@@ -2641,14 +2668,154 @@
 
         for neigh, typ in zip(neighs, comps):
             specie0 = self.molecules[typ].mol.atomic_numbers
             molecules.append(Molecule(specie0, neigh))
 
         return display_cluster(molecules, self.lattice.matrix, engs, cmap, **kwargs)
 
+    def substitute_1_2(self, dicts, ratio=[1, 1], group_type='t+k', max_cell=4,
+                       min_cell=0, max_wp=None, N_groups=None,
+                       N_max=10, criteria=None):
+        """
+        Derive the BC compounds from A via subgroup relation
+        For example, from C to BN or from SiO2 to AlPO3.
+        The key is to split A's wyckoff site to B and C by w.r.t. composition relation.
+        If the current parent crystal doesn't allow splitting, look for the subgroup
+
+        Args:
+            dicts: e.g., {"F": "Cl"}
+            ratio: e.g., [1, 1]
+            group_type (string): `t`, `k` or `t+k`
+            max_cell (float): maximum cell reconstruction
+            min_cell (float): maximum cell reconstruction
+            max_wp (int): maximum number of wp
+            N_groups (int): maximum number of trial subgroups
+            N_max (int): maximum number of structures
+            criteria (dict): dictionary criteria
+
+        Returns:
+            A list of pyxtal structures
+        """
+        from pyxtal.util import new_struc_wo_energy
+
+        xtals = self._substitute_1_2(dicts, ratio)
+        xtals = [xtal for xtal in xtals if criteria is None or xtal.check_validity(criteria)]
+
+        if len(xtals) == 0:
+            #print("\nCannot split, look for subgroup representation")
+            subs = self.subgroup(group_type=group_type,
+                                 max_cell=max_cell,
+                                 min_cell=min_cell,
+                                 N_groups=N_groups)
+            #print("Found {:d} subgroup representatios".format(len(subs)))
+            for sub in subs:
+                #print(sub)
+                _xtals = sub._substitute_1_2(dicts, ratio)
+                for _xtal in _xtals:
+                    if max_wp is not None and len(_xtal.atom_sites) > max_wp:
+                        continue
+                    else:
+                        if new_struc_wo_energy(_xtal, xtals):
+                            add = True
+
+                            if criteria is not None and not _xtal.check_validity(criteria):
+                                add = False
+
+                            if add:
+                                xtals.append(_xtal)
+                                print('Add substitution', _xtal.get_xtal_string())
+                                if len(xtals) == N_max:
+                                    break
+                    #print('Add {:d} substitutions in subgroup {:d}'.format(len(_xtals), sub.group.number))
+        else:
+            print('Good representation ({:d})'.format(len(xtals)), self.get_xtal_string())
+        print('Found {:d} substitutions in total'.format(len(xtals)))
+        return xtals
+
+    def _substitute_1_2(self, dicts, ratio=[1, 1]): #, group_type='t', max_cell=4, min_cell=0):
+        """
+        Derive the BC compounds from A via subgroup relation
+        For example, from C to BN or from SiO2 to AlPO3.
+        The key is to split A's wyckoff site to B and C by w.r.t. composition relation.
+
+        Args:
+            dicts: e.g., {"F": "Cl"}
+            ratio: e.g., [1, 1]
+            group_type (string): `t`, `k` or `t+k`
+            max_cell (float): maximum cell reconstruction
+            min_cell (float): maximum cell reconstruction
+
+        Returns:
+            A list of pyxtal structures
+        """
+        from pyxtal.util import split_list_by_ratio
+
+        if len(dicts) > 1:
+            raise ValueError('Only one item allowed in the input dicts', dicts)
+
+        A, [B, C] = next(iter(dicts.items()))
+
+        numbers = []
+        for site in self.atom_sites:
+            if site.specie == A:
+                numbers.append(site.wp.multiplicity)
+        solutions = split_list_by_ratio(numbers, ratio)
+
+        # Output all possible substitutions
+        xtals = []
+        for (group1, group2) in solutions:
+            xtal0 = self.copy()
+            count = 0
+            for site in xtal0.atom_sites:
+                if site.specie == A:
+                    if count in group1:
+                        site.specie = B
+                    else:
+                        site.specie = C
+                    count += 1
+            xtal0.species = None
+            xtal0._get_formula() # update species
+            xtals.append(xtal0)
+        return xtals
+
+        #idx, sites, t_types, k_types = self._get_subgroup_ids(H, group_type, None, max_cell, min_cell)
+        #elements = [site.species for site in self.atom_sites]
+
+        #valid_splitters = []
+        #for id in idx:
+        #    gtype = (t_types + k_types)[id]
+        #    if gtype == 'k': id -= len(t_types)
+        #    splitter = wyckoff_split(G=self.group, wp1=sites, idx=id, gtype, elements)
+        #    # QZ: check if there is a redundancy in error and valid_split
+        #    if not splitter.error and splitter.valid_split:
+        #        for key in dicts.keys():
+        #            # check whether the splitter can make valid decomposition
+        #            # e.g., if we want to make a BN from C
+        #            # The splitter from 8 to 4+4 is valid
+        #            # The splitter from 8 to 6+2 is invalid
+        #            numbers = []
+        #            for i, wp2 in enumerate(splitter.wp2_lists):
+        #                if sp.elements[i] == key:
+        #                    for _wp2 in wp2:
+        #                        numbers.append(_wp2.multiplicity)
+        #            if not get_integer_solutions(numbers, ratio, quick=True):
+        #                bad_splitter = True
+        #                break
+        #        if bad_splitter:
+        #            continue
+        #        else:
+        #            valid_splitters.append(splitter)
+
+        #new_strucs = []
+        #for splitter in valid_splitters:
+        #    #print(splitter)
+        #    new_struc = self._apply_substitution(splitter, perms)
+        #    new_strucs.append(new_struc)
+        #return new_strucs
+
     def substitute(self, dicts):
         """
         A quick function to apply substitution
 
         Args:
             dicts: e.g., {"F": "Cl"}
         """
@@ -2777,50 +2944,56 @@
                     #print("add sites", i, m)
                     break
 
         self.molecules = molecules
         self.numMols = numMols
         self.mol_sites = sites
 
-    def set_cutoff(self, exclude_ii=False):
+    def set_cutoff(self, exclude_ii=False, value=None):
         """
         get the cutoff dictionary
+
+        Args:
+            exclude_ii (bool): whether or not exclude A-A distance
+            value (float): cutoff distance
         """
         cutoff = {}
         tm = Tol_matrix(prototype="molecular")
         for i in range(len(self.species)):
             s1 = self.species[i]
             for j in range(i, len(self.species)):
                 s2 = self.species[j]
                 select = True
                 if exclude_ii and s1 == s2:
                     select = False
                 if select:
                     tuple_elements = (s1, s2)
-                    cutoff[tuple_elements] = tm.get_tol(s1, s2)
+                    if value is None:
+                        cutoff[tuple_elements] = tm.get_tol(s1, s2)
+                    else:
+                        cutoff[tuple_elements] = value
 
         self.cutoff = cutoff
 
     def set_site_coordination(self, cutoff=None, verbose=False, exclude_ii=False):
         """
         Compute the coordination number from each atomic site
         """
         from ase.neighborlist import neighbor_list
 
-        if cutoff is None:
-            #if not hasattr(self, 'cutoff'):
-            self.set_cutoff(exclude_ii)
-            cutoff = self.cutoff
+        #if not hasattr(self, 'cutoff'):
+        self.set_cutoff(exclude_ii, cutoff)
+        my_cutoff = self.cutoff
 
         if verbose:
             print("\n The cutoff values for CN calculation are")
-            print(cutoff)
+            print(my_cutoff)
 
         atoms = self.to_ase(resort=False)
-        NL = neighbor_list('i', atoms, cutoff)
+        NL = neighbor_list('i', atoms, my_cutoff)
         coords = np.bincount(NL)
 
         count = 0
         for site in self.atom_sites:
             if count >= len(coords):
                 site.coordination = 0
             else:
@@ -3196,15 +3369,15 @@
             letter = _wp[-1]
             for wp in group:
                 if wp.letter == letter:
                     sites.append((elements[i], wp))
                     break
         self.from_1d_rep(x, sites)
 
-    def from_1d_rep(self, x, sites):
+    def from_1d_rep(self, x, sites, dim=3):
         """
         An advanced way to build pyxtal from the 1d representation
 
         Args:
             x: 1d representation
             sites: list of (element, wp)
         """
@@ -3233,15 +3406,15 @@
                 idx = species.index(specie)
                 numIons[idx] += _wp.multiplicity
                 total_sites[idx].append((label, x, y, z))
         #print(species, numIons,  total_sites)
 
         spg = sites[0][1].number
         try:
-            self.build(spg, species, numIons, lat, total_sites)
+            self.build(spg, species, numIons, lat, total_sites, dim=dim)
         except:
             print("input x", x)
             print("input build", spg, numIons, lat, total_sites)
             raise ValueError('Problem in build')
 
 
     def check_validity(self, criteria, verbose=False):
@@ -3271,27 +3444,26 @@
             den1 = self.get_density()
             den2 = criteria['MIN_Density']
             if den1 < den2:
                 if verbose:
                     msg = "===Invalid in MIN_density {:.2f}=>{:.2f}".format(den1, den2)
                     print(msg)
                 return False
-
         if 'CN' in criteria:
             if criteria['exclude_ii']:
                 options = [True, False]
             else:
                 options = [False]
 
             for option in options:
                 try:
                     self.set_site_coordination(criteria['cutoff'], exclude_ii=option)
+                    #print('exclude_ii', option, criteria['cutoff'], self)
                 except:
-                    if verbose:
-                        print("=====Invalid in CN calculation")
+                    if verbose: print("=====Invalid in CN calculation")
                     return False
                 for s in self.atom_sites:
                     ele = s.specie
                     cn1 = s.coordination
                     cn2 = criteria['CN'][ele]
                     #print(ele, cn1, option)
                     if cn1 != cn2:
@@ -3335,15 +3507,15 @@
         strs += "*{:3d} {:3d} {:4d} {:10s} {:8.2f} ".format(
                 N_atoms, dof, spg_num, spg_symbol, density)
 
         if dicts is not None:
             # Similarity, energy, status
             for key in dicts:
                 value = dicts[key]
-                if type(value) == float:
+                if type(value) in [float, np.float64]:
                     strs += " {:8.3f} ".format(value)
                 elif type(value) == str:
                     strs += " {:24s} ".format(value)
                 elif type(value) == bool:
                     strs += " {:5s} ".format(str(value))
 
         for s in self.atom_sites:
@@ -3428,8 +3600,36 @@
                     wp = group[wp_id]
                     xyz = wp.search_generator([x, y, z])#; print(wp.get_label(), xyz)
                     if xyz is not None:
                         xyz, wp, _ = wp.merge(xyz, np.eye(3), 1e-3)
                         label = wp.get_label()
                         sites.append((label, xyz[0], xyz[1], xyz[2]))#; print(x, y, z, label, xyz[0], xyz[1], xyz[2])
                         numIons += wp.multiplicity
-            self.build(group, ['C'], [numIons], lattice, [sites])
+            try:
+                self.build(group, ['C'], [numIons], lattice, [sites])
+            except:
+                print("Invalid Build", lattice, numIons, sites)
+                self.valid = False
+
+    def get_Pearson_Symbol(self):
+        """
+        Return the Pearson symbol: https://en.wikipedia.org/wiki/Pearson_symbol
+        """
+        if self.group.number <= 2:
+            l = 'a'
+        elif self.group.number <= 15:
+            l = 'm'
+        elif self.group.number <= 74:
+            l = 'o'
+        elif self.group.number <= 142:
+            l = 't'
+        elif self.group.number <= 194:
+            l = 'h'
+        else:
+            l = 'c'
+
+        if self.group.symbol[0] in ['A', 'B', 'C']:
+            b = 'S'
+        else:
+            b = self.group.symbol[0]
+
+        return l + b + str(sum(self.numIons))
```

### Comparing `pyxtal-0.6.6/pyxtal/block_crystal.py` & `pyxtal-0.6.7/pyxtal/block_crystal.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/constants.py` & `pyxtal-0.6.7/pyxtal/constants.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/crystal.py` & `pyxtal-0.6.7/pyxtal/crystal.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/HM_Full.csv` & `pyxtal-0.6.7/pyxtal/database/HM_Full.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/atomic_scattering_params.json` & `pyxtal-0.6.7/pyxtal/database/atomic_scattering_params.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/bonds.json` & `pyxtal-0.6.7/pyxtal/database/bonds.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/bug.json` & `pyxtal-0.6.7/pyxtal/database/bug.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/0-G62.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/0-G62.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/1-G59.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/1-G59.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/2-G71.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/2-G71.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/3-G139.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/3-G139.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/4-G225.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/4-G225.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/ACBNZA01.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/ACBNZA01.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/AXOSOW01.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/AXOSOW01.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/Al2SiO5_mp-4753_symmetrized.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/BTO-Amm2.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/BTO-Amm2.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/BTO.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/BTO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/FAU.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/FAU.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/Fd3.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/Fd3.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/Fd3.vasp` & `pyxtal-0.6.7/pyxtal/database/cifs/Fd3.vasp`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/Fd3m.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/Fd3m.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/GUMMUW.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/GUMMUW.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/GeF2.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/GeF2.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/HAHCOI.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/HAHCOI.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/I4_132.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/I4_132.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/JAPWIH.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/JAPWIH.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/LAGNAL.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/LAGNAL.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/LUFHAW.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/LUFHAW.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/LiCs.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/LiCs.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/MERQIM.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/MERQIM.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/MPWO.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/MPWO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/NaCl.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/NaCl.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/NaSb3F10.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/NaSb3F10.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/NbO2.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/NbO2.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/NiS-Cm.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/NiS-Cm.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/P3_112.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/P3_112.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/P4_332.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/P4_332.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/P6_422.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/P6_422.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/PAHYON01.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/PAHYON01.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/PPO.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/PPO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/PVO.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/PVO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/Pm3.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/Pm3.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/R-3.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/R-3.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/R-3c.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/R-3c.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/R32.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/R32.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/TMPPIO03.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/TMPPIO03.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/WEXBOS.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/WEXBOS.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/YICMOP.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/YICMOP.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/anthracene.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/anthracene.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/aspirin-c.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/aspirin-c.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/aspirin.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/aspirin.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/benzene.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/benzene.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/bug.vasp` & `pyxtal-0.6.7/pyxtal/database/cifs/bug.vasp`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/c_bug.vasp` & `pyxtal-0.6.7/pyxtal/database/cifs/c_bug.vasp`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/c_bug2.vasp` & `pyxtal-0.6.7/pyxtal/database/cifs/c_bug2.vasp`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/coumarin.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/coumarin.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/dist_6_0.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/dist_6_0.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/dist_6_1.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/dist_6_1.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/gdh.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/gdh.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/ht_KNbBO.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/ht_KNbBO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/ht_cristobalite.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/ht_cristobalite.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/ht_quartz.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/ht_quartz.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/ice.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/ice.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/lt_KNbBO.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/lt_KNbBO.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/lt_cristobalite.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/lt_cristobalite.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/lt_quartz.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/lt_quartz.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/naphthalene.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/naphthalene.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/resorcinol.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/resorcinol.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/cifs/xxvi.cif` & `pyxtal-0.6.7/pyxtal/database/cifs/xxvi.cif`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/clusters.json` & `pyxtal-0.6.7/pyxtal/database/clusters.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/collection.py` & `pyxtal-0.6.7/pyxtal/database/collection.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/element.py` & `pyxtal-0.6.7/pyxtal/database/element.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/k_subgroup.json` & `pyxtal-0.6.7/pyxtal/database/k_subgroup.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/layer.csv` & `pyxtal-0.6.7/pyxtal/database/layer.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/layer_generators.csv` & `pyxtal-0.6.7/pyxtal/database/layer_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/layer_symmetry.csv` & `pyxtal-0.6.7/pyxtal/database/layer_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/mech.db` & `pyxtal-0.6.7/pyxtal/database/mech.db`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/molecules.json` & `pyxtal-0.6.7/pyxtal/database/molecules.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/point.csv` & `pyxtal-0.6.7/pyxtal/database/point.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/point_generators.csv` & `pyxtal-0.6.7/pyxtal/database/point_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/point_symmetry.csv` & `pyxtal-0.6.7/pyxtal/database/point_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/rod.csv` & `pyxtal-0.6.7/pyxtal/database/rod.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/rod_generators.csv` & `pyxtal-0.6.7/pyxtal/database/rod_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/rod_symmetry.csv` & `pyxtal-0.6.7/pyxtal/database/rod_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/symbols.json` & `pyxtal-0.6.7/pyxtal/database/symbols.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/t_subgroup.json` & `pyxtal-0.6.7/pyxtal/database/t_subgroup.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/wyckoff_generators.csv` & `pyxtal-0.6.7/pyxtal/database/wyckoff_generators.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/wyckoff_list.csv` & `pyxtal-0.6.7/pyxtal/database/wyckoff_list.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/wyckoff_sets.json` & `pyxtal-0.6.7/pyxtal/database/wyckoff_sets.json`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/database/wyckoff_symmetry.csv` & `pyxtal-0.6.7/pyxtal/database/wyckoff_symmetry.csv`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/db.py` & `pyxtal-0.6.7/pyxtal/util.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,716 +1,689 @@
 """
-Database class
+some utilities
 """
-import os
+
 import numpy as np
-from ase.db import connect
-from pyxtal import pyxtal
-import pymatgen.analysis.structure_matcher as sm
-from pyxtal.util import ase2pymatgen
+from spglib import get_symmetry_dataset
+from pymatgen.symmetry.analyzer import SpacegroupAnalyzer as sga
+from pymatgen.core.structure import Structure
+from ase import Atoms
+from pyxtal.symmetry import Hall
+import re
 
-def make_entry_from_pyxtal(xtal):
+def find_dir(dirs):
+    """
+    a short function to find the correct dir from a list
     """
-    make entry from the pyxtal object, assuming that
-    the smiles/ccdc_number info is given
+    skf_dir = None
+    for d in dirs:
+        if os.path.isdir(d):
+            return d
+    raise RuntimeError("Cannot find the dirtory for dftb parameters")
 
-    Args:
-        xtal: pyxtal object
+def listToString(s):
+    # initialize an empty string
+    #str1 = " "
+    str1 = ""
+    # return string
+    return (str1.join(s))
 
-    Returns:
-        entry dictionary
+def pymatgen2ase(struc):
+    """
+    A short cut to convert between pymatgen to ase
+    """
+    atoms = Atoms(symbols = struc.atomic_numbers, cell = struc.lattice.matrix, pbc=True)
+    atoms.set_scaled_positions(struc.frac_coords)
+    return atoms
+
+def ase2pymatgen(struc):
+    """
+    A short cut to convert between pymatgen to ase
+    """
+    lattice = struc.cell
+    coordinates = struc.get_scaled_positions()
+    species = struc.get_chemical_symbols()
+    return Structure(lattice, species, coordinates)
+
+def symmetrize_cell(struc, mode='C'):
+    """
+    symmetrize structure from pymatgen, and return the struc in conventional or
+    primitive setting.
+
+    Args:
+        struc: ase type
+        mode: output conventional or primitive cell
     """
-    from rdkit.Chem.Descriptors import ExactMolWt
-    from rdkit.Chem.rdMolDescriptors import CalcMolFormula
-    from rdkit import Chem
-
-    if xtal.valid:
-        url0 = "https://www.ccdc.cam.ac.uk/structures/Search?Ccdcid="
-        m = Chem.MolFromSmiles(xtal.tag['smiles'])
-        mol_wt = ExactMolWt(m)
-        mol_formula = CalcMolFormula(m)
-        kvp = {
-                "csd_code": xtal.tag['csd_code'],
-                "mol_smi": xtal.tag['smiles'],
-                "ccdc_number": xtal.tag['ccdc_number'],
-                "space_group": xtal.group.symbol,
-                "spg_num": xtal.group.number,
-                "Z": sum(xtal.numMols),
-                "Zprime": xtal.get_zprime()[0],
-                "url": url0 + str(xtal.tag['ccdc_number']),
-                "mol_formula": mol_formula,
-                "mol_weight": mol_wt,
-                "mol_name": xtal.tag['csd_code'],
-                "l_type": xtal.lattice.ltype,
-              }
-        entry = (xtal.to_ase(), kvp, None)
-        return entry
+    P_struc = ase2pymatgen(struc)
+    finder = sga(P_struc,symprec=0.06)
+    if mode == 'C':
+        P_struc = finder.get_conventional_standard_structure()
     else:
-        return None
+        P_struc = finder.get_primitive_standard_structure()
+
+    return pymatgen2ase(P_struc)
 
-def make_entry_from_CSD_web(code, number, smiles, name=None):
+def good_lattice(struc, maxvec=25.0, minvec=1.2, maxang=150, minang=30):
     """
-    make enetry dictionary from csd web https://www.ccdc.cam.ac.uk/structures
+    check if the lattice has a good shape.
 
     Args:
-        code: CSD style letter entry
-        number: ccdc number
-        smiles: the corresponding molecular smiles
-        name: name of the compound
+        struc: pyxtal structure
     """
 
-    url0 = "https://www.ccdc.cam.ac.uk/structures/Search?Ccdcid="
-    #xtal = pyxtal(molecular=True)
-    #
-    #return make_entry_from_pyxtal(xtal)
-    raise NotImplementedError('To do in future')
+    para = struc.lattice.get_para(degree=True)
+    if (max(para[:3])<maxvec) and (min(para[:3])>minvec)\
+        and (max(para[3:])<maxang) and (min(para[3:])>minang):
+        return True
+    else:
+        return False
+
+def symmetrize(pmg, tol=1e-3, a_tol=5.0, style='pyxtal', hn=None):
+    """
+    symmetrize the structure from spglib.
 
+    Args:
+        pmg: pymatgen structure
+        tol: tolerance
+        a_tol: angle tolerance
+        style: 'pyxtal' or spglib, differing in the choice of origin
+        hn: hall_number
 
-def make_entry_from_CSD(code):
+    Returns:
+        pymatgen structure with symmetrized lattice
     """
-    make entry dictionary from CSD codes
+    numbers = [site.species.elements[0].Z for site in pmg.sites]
+    atoms = (pmg.lattice.matrix, pmg.frac_coords, numbers)
+    dataset = get_symmetry_dataset(atoms, tol, angle_tolerance=a_tol)
+    if hn is None:
+        hn = Hall(dataset['number'], style=style).hall_default
+    if hn != dataset['hall_number']:
+        dataset = get_symmetry_dataset(atoms, tol,
+                                       angle_tolerance=a_tol,
+                                       hall_number=hn)
+    cell = dataset['std_lattice']
+    pos = dataset['std_positions']
+    numbers = dataset['std_types']
+
+    return Structure(cell, numbers, pos), hn
+
+def get_symmetrized_pmg(pmg, tol=1e-3, a_tol=5.0, style='pyxtal', hn=None):
+    """
+    Get the symmetrized Pymatgen structure. A slight modification to ensure that
+    the structure adopts the standard setting according to the Interational
+    Crystallography Table.
 
     Args:
-        code: a list of CSD codes
+        pmg: input pymatgen structure
+        tol: symmetry tolerance
+        a_tol: angle tolerance
+        style: 'pyxtal' or spglib, differing in the choice of origin
+        hn: hall_number
+
+    Returns:
+        pymatgen structure with symmetrized lattice
     """
-    from pyxtal.msg import CSDError
 
-    xtal = pyxtal(molecular=True)
-    try:
-        xtal.from_CSD(code)
-        return make_entry_from_pyxtal(xtal)
+    pmg, hn = symmetrize(pmg, tol, a_tol=a_tol, style=style, hn=hn)
+    s = sga(pmg, symprec=tol, angle_tolerance=a_tol)
+    # make sure that the coordinates are in standard setting
+    #if hn is None:
+    #    hn = Hall(s._space_group_data['number'], style=style).hall_default
+    if hn != s._space_group_data["hall_number"]:
+        s._space_group_data = get_symmetry_dataset(s._cell, tol,
+                                                   angle_tolerance=a_tol,
+                                                   hall_number=hn)
+    return s.get_symmetrized_structure(), s.get_space_group_number()
+
+def extract_ase_db(db_file, id):
+    """
+    a short cut to extract the structural information
+    from the ase db file by row id
+    """
+
+    from ase.db import connect
+    from pyxtal import pyxtal
+    import os
+
+    if not os.path.exists("output"):
+        os.makedirs("output")
+    print("Dumping the structures to the folder output")
+    with connect(db_file) as db:
+        for id in ids:
+            s = db.get_atoms(id=id)
+            filename = "output/"+str(id)+".vasp"
+            s.write(filename, format='vasp', direct=True, vasp5=True)
+            my = pyxtal()
+            my.from_seed(s)
+            print(my)
 
-    except CSDError as e:
-        print("CSDError", code, e.message)
-        return None
+def parse_cif(filename, header=False, spg=False, eng=False, csd=False, sim=False):
+    """
+    read structures from a cif (our own format with #END)
+    Args:
+        filename: string
+        header: bool, whether or not return header
+        spg: bool, whether or not return the spg
+    """
+    strings = []
+    headers = []
+    spgs = []
+    engs = []
+    csds = []
+    sims = []
+    with open(filename, 'r') as f:
+        lines = f.readlines()
+        start = None
+        end = None
+        for i in range(len(lines)):
+            if lines[i].find("data_") == 0:
+                if sim:
+                    sims.append(float(lines[i].split(':')[-1]))
+                end = i
+                if start is not None:
+                    tmp = []
+                    for l in lines[start:end-1]:
+                        if len(re.findall(r"[0-9][B-C]", l))>0 or \
+                        len(re.findall(r"[A-Z][0-9]\' [0-9]", l))>0:
+                            #print(l) #; import sys; sys.exit()
+                            continue
+                        tmp.append(l)
+                    cif = listToString(tmp)
+                    strings.append(cif)
+                start = i
+                headers.append(lines[i])
+            elif lines[i].find("_symmetry_Int_Tables_number") == 0:
+                spgs.append(int(lines[i].split()[-1]))
+            elif lines[i].find("#Energy") == 0:
+                engs.append(float(lines[i].split()[1]))
+            elif lines[i].find("_database_code") == 0:
+                tmp = lines[i].split()[-1]
+                csds.append(tmp[:-1])
+
+        #Last one
+        tmp = []
+        for l in lines[start:]:
+            if len(re.findall(r"[0-9][B-D]", l))>0 or \
+            len(re.findall(r"[A-Z][0-9]\' [0-9]", l))>0:
+                #print(l);
+                continue
+            tmp.append(l)
+        cif = listToString(tmp)
+        strings.append(cif)
+
+    if header:
+        return strings, headers
+    elif spg:
+        return strings, spgs
+    elif eng:
+        return strings, engs
+    elif csd:
+        return strings, csds
+    elif sim:
+        return strings, sims
+    else:
+        return strings
 
-def make_db_from_CSD(dbname, codes):
+def process_csd_cif(cif, remove_H=False):
+    """
+    process cif from CSD, sometimes it contains multiple
+    e.g., C2
     """
-    make database from CSD codes
+    lines = cif.split('\n')
+    tmp = []
+    for l in lines:
+        if len(re.findall(r"[0-9][A-Z]", l))>0 or len(re.findall(r"[A-Z]\?", l))>0 or \
+            len(re.findall(r"[0-9]\?", l))>0 or \
+            len(re.findall(r"[A-Z][0-9]\' [0-9]", l))>0:
+            #len(re.findall(r"[0-9]_[0-9]", l))>0 or \
+            #print(l) #; import sys; sys.exit()
+            continue
+        else:
+            if remove_H and len(re.findall(r" H ", l))>0:
+                continue
+            else:
+                tmp.append(l+'\n')
+    return listToString(tmp)
 
+def get_similar_cids_from_pubchem(base, MaxRecords):
+    """
     Args:
-        dbname: db file name
-        codes: a list of CSD codes
+        base: PubChem CID of Starting chemical
+        MaxRecords: Number of Similar Compounds
+
+    Returns:
+        List of the CIDs of PubChem compounds similar to the base compound.
     """
-    # open
-    db = database(dbname)
 
-    # add structure
-    for i, code in enumerate(codes):
-        entry = make_entry_from_CSD(code)
-        if entry is not None:
-            db.add(entry)
-            print(i, code)
-    return db
+    import pubchempy as pcp
+
+    if type(base) == int: base = str(base)
+    cids = pcp.get_compounds(base,
+                             searchtype="similarity",
+                             MaxRecords=MaxRecords)
+    results = []
+    for x in cids:
+        csd_codes = search_ccdc_structures(x.cid)
+        if len(csd_codes)>0:
+            d = {"cid": x.cid,
+                 "smiles": x.canonical_smiles,
+                 "name": x.iupac_name,
+                 "csd_codes": csd_codes}
+            results.append(d)
+            print(d)
+    return results
 
-class database():
+def search_csd_code_by_pubchem(cid):
     """
-    This is a database class to process crystal data
+    Args:
+        cid: PubChem cid
 
+    Returns:
+        CIDs that have CCDC crystal structure data
+    """
+
+    import urllib
+    import json
+    from monty.json import MontyDecoder
+
+    url0 = 'https://pubchem.ncbi.nlm.nih.gov/rest/pug_view/data/compound/'
+    cid=str(cid)
+    url = url0 + cid + '/JSON'
+    csd_codes = []
+
+    try:
+        response = urllib.request.urlopen(url)
+    except urllib.error.HTTPError:
+        print("Problem in http connection", url)
+        return None
+    except urllib.error.URLError:
+        print("Problem in parsing", url)
+        return None
+
+    try:
+        contents = response.read()
+        if contents.decode().find('CCDC') > 0:
+            data = json.loads(contents, cls=MontyDecoder)
+            if 'Section' in data['Record']['Section'][0].keys():
+                if len(data['Record']['Section'][0]['Section']) == 3:
+                    infos = data['Record']['Section'][0]['Section'][2]['Section'][0]['Information']
+                    for info in infos:
+                        csd_codes.append(info['Value']['StringWithMarkup'][0]['String'])
+    except:
+        print('Failed to parse json', url, '\n')
+
+    return csd_codes
+
+def search_csd_entries_by_code(code):
+    """
     Args:
-        db_name: *.db format from ase database
+        code: CSD code, e.g., ACSALA
+
+    Returns:
+        list of csd ids
     """
 
-    def __init__(self, db_name):
-        self.db_name = db_name
-        #if not os.path.exists(db_name):
-        #    raise ValueError(db_name, 'doesnot exist')
+    from ccdc.search import TextNumericSearch
+    from ccdc.crystal import PackingSimilarity as PS
 
-        self.db = connect(db_name)
-        self.get_all_codes()
-        self.keys = ['csd_code', 'space_group', 'spg_num',
-                     'Z', 'Zprime', 'url', 'mol_name',
-                     'mol_smi', 'mol_formula', 'mol_weight',
-                     'l_type',
-                    ]
-        self.calculators = ['charmm',
-                            'gulp',
-                            'ani',
-                            'dftb_D3',
-                            'dftb_TS',
-                           ]
+    def new_cryst(cryst, crysts, n_max):
+        spg1 = cryst.spacegroup_number_and_setting[0]
+        for ref in crysts:
+            spg2 = ref.spacegroup_number_and_setting[0]
+            if spg1 == spg2:
+                h = PS().compare(cryst, ref)
+                #print(cryst.identifier, ref.identifier, h.nmatched_molecules)
+                if h is not None and h.nmatched_molecules == n_max:
+                    return False
+        return True
 
-    def vacuum(self):
-        self.db.vacuum()
+    n_max = PS().settings.packing_shell_size
+    query = TextNumericSearch()
+    query.add_identifier(code)
+    hits = query.search()
+    unique_crysts = []
+    for hit in hits:
+        if hit.entry.has_3d_structure and hit.entry.pressure is None:
+            if new_cryst(hit.crystal, unique_crysts, n_max):
+                unique_crysts.append(hit.crystal)
+                #print(hit.entry.identifier, hit.entry.deposition_date)
 
-    def get_all_codes(self):
-        codes = []
-        for row in self.db.select():
-            if row.csd_code not in codes:
-                codes.append(row.csd_code)
-            else:
-                print('find duplicate! remove', row.id, row.csd_code)
-                self.db.delete([row.id])
-        self.codes = codes
-
-    def add(self, entry):
-        (atom, kvp, data) = entry
-        if kvp['csd_code'] not in self.codes:
-            kvp0 = self.process_kvp(kvp)
-            self.db.write(atom, key_value_pairs=kvp0, data=data)
-            self.codes.append(kvp['csd_code'])
-
-    def add_from_code(self, code):
-        entry = make_entry_from_CSD(code)
-        if entry is not None:
-            self.add(entry)
-        else:
-            print("{:s} is not a valid entry".format(code))
+    return [c.identifier for c in unique_crysts]
+
+
+def get_struc_from__parser(p):
+    """
+    A utility to get the pymatgen structure from the CifParser
+    Sometimes the cif structure may have repeated atom entries
+
+    Args:
+        p: pymatgen CifParser object
+
+    Return:
+        a single pymatgen structure
+    """
+    from pymatgen.util.coord import find_in_coord_list_pbc
+    from collections import OrderedDict
+    from pymatgen.core.periodic_table import get_el_sp
+    from pymatgen.io.cif import str2float
+    import numpy as np
+
+    def get_matching_coord(coord, ops, atol=1e-4):
+        keys = list(coord_to_species.keys())
+        coords = np.array(keys)
+        for op in ops:
+            c = op.operate(coord)
+            inds = find_in_coord_list_pbc(coords, c, atol=atol)
+            if len(inds):
+                return keys[inds[0]]
+        return False
+
+
+    for i, d in enumerate(p._cif.data.values()):
+        ops = p.get_symops(d)
+        coord_to_species = OrderedDict()
+        d0 = {"_atom_site_label": [],
+              "_atom_site_fract_x": [],
+              "_atom_site_fract_y": [],
+              "_atom_site_fract_z": [],
+             }
+        for i in range(len(d["_atom_site_label"])):
+            try:
+                symbol = p._parse_symbol(d["_atom_site_type_symbol"][i])
+            except KeyError:
+                symbol = p._parse_symbol(d["_atom_site_label"][i])
+
+            el = get_el_sp(symbol)
+            x = str2float(d["_atom_site_fract_x"][i])
+            y = str2float(d["_atom_site_fract_y"][i])
+            z = str2float(d["_atom_site_fract_z"][i])
+
+            coord = (x, y, z)
+            match = get_matching_coord(coord, ops)
+            if not match:
+                d0['_atom_site_label'].append(el)
+                d0["_atom_site_fract_x"].append(str(x))
+                d0["_atom_site_fract_y"].append(str(y))
+                d0["_atom_site_fract_z"].append(str(z))
+                coord_to_species[coord] = el
+        d.data['_atom_site_label'] = d0['_atom_site_label']
+        d.data['_atom_site_fract_x'] = d0['_atom_site_fract_x']
+        d.data['_atom_site_fract_y'] = d0['_atom_site_fract_y']
+        d.data['_atom_site_fract_z'] = d0['_atom_site_fract_z']
+
+        s = p._get_structure(d, primitive=False, symmetrized=False)
+        return s
+
+def Kgrid(struc, Kresol=0.10, dimension=3):
+    """
+    Assign kpoints based on the lattice
+    """
+    #a, b, c, alpha, beta, gamma = struc.get_cell_lengths_and_angles()
+    a, b, c, alpha, beta, gamma = struc.cell.cellpar()
+    vol = struc.get_volume()
+    dist    = np.zeros(3);
+    dist[2] = np.abs(vol/(a*b*np.sin(np.radians(gamma))))
+    dist[1] = np.abs(vol/(a*c*np.sin(np.radians(beta))))
+    dist[0] = np.abs(vol/(b*c*np.sin(np.radians(alpha))))
+    Kpoints = np.ceil(1./(dist*Kresol))
+    if dimension == 2:
+        Kpoints[-1] = 1;
+    #print(a, b, c, alpha, beta, gamma)
+    #print(vol/(a*b*np.sin(gamma)), a*b, np.sin(gamma))
+    #print(vol/(a*c*np.sin(beta)), a*c, np.sin(beta))
+    #print(vol/(b*c*np.sin(alpha)), b*c, np.sin(alpha))
+    #print(Kpoints)
+    #import sys; sys.exit()
+    return Kpoints.astype(int)
 
-    def process_kvp(self, kvp):
-        kvp0 = {}
-        for key in self.keys:
-            if key in kvp:
-                kvp0[key] = kvp[key]
-            else:
-                print('Error, cannot find ', key, ' from the input')
-                return
-        return kvp0
-
-    def check_status(self, show=False):
-        """
-        Check the current status of each entry
-        """
-        ids = []
-        for row in self.db.select():
-            if len(row.data.keys())==len(self.calculators):
-                ids.append(row.id)
-                if show:
-                    row_info = self.get_row_info(id=row.id)
-                    self.view(row_info)
-            else:
-                print(row.csd_code) #, row.data['charmm_info']['prm'])
-        return ids
 
-    def copy(self, db_name, csd_codes):
-        """
-        copy the entries to another db
-
-        Args:
-            db_name: db file name
-            csd_codes: list of codes
-        """
-        if db_name == self.db_name:
-            raise RuntimeError('Cannot use the same db file for copy')
-        with connect(db_name) as db:
-            for csd_code in csd_codes:
-                row_info = self.get_row_info(code=csd_code)
-                (atom, kvp, data) = row_info
-                db.write(atom, key_value_pairs=kvp, data=data)
-
-    def view(self, row_info):
-        """
-        print the summary of benchmark results
-
-        Args:
-            row: row object
-        """
-        from pyxtal import pyxtal
-        from pyxtal.util import ase2pymatgen
-        from pyxtal.representation import representation
-        from pyxtal.msg import ReadSeedError
-
-        (atom, kvp, data) = row_info
-
-        #Reference
-        xtal = self.get_pyxtal(kvp['csd_code'])
-        rep = xtal.get_1D_representation()
-        print('\n', kvp['csd_code'], kvp['mol_smi'], xtal.lattice.volume)
-        print(rep.to_string() + ' reference')
-
-        #calcs
-        for key in data.keys():
-            calc = key[:-5]
-            time = data[key]['time']
-
-            rep = data[key]['rep']
-            if type(rep[0]) is not list: rep = [rep]
-            rep = representation(rep, kvp['mol_smi']).to_string()
-
-            (dv, msd1, msd2) = data[key]['diff']
-            strs = "{:s} {:8s} {:6.2f} {:6.3f}".format(rep, calc, time/60, dv)
-            if msd1 is not None:
-                strs += "{:6.3f}{:6.3f}".format(msd1, msd2)
-            print(strs)
-
-
-    def get_row_info(self, id=None, code=None):
-        match = False
-        if id is not None:
-            for row in self.db.select(id=id):
-                match = True
+def sort_by_dimer(atoms, N_mols, id=10, tol=4.0):
+    """
+    sort the ase atoms' xyz according to dimer
+    so far only tested on aspirin
+
+    Args:
+        atoms: atoms object from pyxtal
+        N_mols: number of molecules
+        id: the refrence atom id
+        tol: tolerence distance to check if it is a dimer
+    """
+
+    N_atoms = int(len(atoms)/N_mols)
+    pos = atoms.get_scaled_positions()
+    refs = pos[id:len(pos):N_atoms, :]
+    #print(refs)
+
+    # compuate the indices and shift
+    orders = []
+    shifts = []
+    while len(orders) < N_mols:
+        lefts = [i for i in range(N_mols) if i not in orders]
+        i = lefts[0]
+        orders.append(i)
+        shifts.append(np.zeros(3))
+        ref_i = refs[i]
+        good = False
+        for j in lefts[1:]:
+            ref_j = refs[j]
+            dist = ref_j - ref_i
+            shift = np.rint(dist)
+            dist -= shift
+            dist = np.linalg.norm(dist.dot(atoms.cell[:]))
+            if dist < tol:
+                orders.append(j)
+                shifts.append(shift)
+                good = True
                 break
-        elif code is not None:
-            for row in self.db.select(csd_code=code):
-                match = True
+        if not good:
+            raise RuntimeError('Cannot find match on molecule', i)
+        else:
+            print('get', i, j, dist, shift)
+
+    pos0 = atoms.get_positions()
+    pos1 = np.zeros([len(pos), 3])
+    for i, id in enumerate(orders):
+        s1, e1 = id*N_atoms, (id+1)*N_atoms
+        s2, e2 = i*N_atoms, (i+1)*N_atoms
+        pos1[s2:e2, :] += pos0[s1:e1, :] - shifts[i].dot(atoms.cell[:])
+
+    atoms.set_positions(pos1)
+    return atoms
+
+def generate_wp_lib(spg_list, composition,
+                    num_wp=(None, None),
+                    num_fu=(None, None),
+                    num_dof=(None, None),
+                    N_max=1000):
+    """
+    Generate wps according to the composition constraint (e.g., SiO2)
+
+    Args;
+        - spg_list: list of space group choices
+        - composition: chemical compositions [1, 2]
+        - num_wp: (min_wp, max_wp)
+        - num_fu: (min_fu, max_fu)
+        - num_dof: (min_dof, max_dof)
+
+    Returns:
+        a list of wps [spg, ([wp1, ...], ... [wp1, ...]), dof]
+    """
+
+    from pyxtal.symmetry import Group
+
+    composition = np.array(composition, dtype=int)
+    (min_wp, max_wp) = num_wp
+    (min_fu, max_fu) = num_fu
+    (min_dof, max_dof) = num_dof
+
+    if max_wp is None: max_wp = len(composition)
+    if min_wp is None: min_wp = len(composition)
+    if min_dof is None: min_dof = 1
+    if max_dof is None: max_dof = 1000
+    #print(max_wp, min_wp)
+    wps = []
+    for sg in spg_list:
+        g = Group(sg)
+        lat_dof = g.get_lattice_dof()
+        # determine the upper and lower limit
+        if min_fu is None: min_fu = max([int(len(g[-1])/min(composition)), 1])
+        if max_fu is None: max_fu = max([int(len(g[0])/max(composition)), 1])
+        count = 0
+        for i in range(max_fu, min_fu-1, -1):
+            letters, _, wp_ids = g.list_wyckoff_combinations(
+                    composition*i, numWp=(min_wp, max_wp), Nmax=100000)
+            for j, wp in enumerate(wp_ids):
+                wp_dofs = 0
+                num = 0
+                for wp0 in wp:
+                    for id in wp0:
+                        wp_dofs += g[id].get_dof()
+                        num += g[id].multiplicity
+                #print(sg, wp, letters[j])
+                num_dof = lat_dof + wp_dofs
+                if min_dof <= num_dof <= max_dof:
+                    wps.append((num, sg, wp, lat_dof + wp_dofs))
+                    count += 1
+            if count >= N_max:
                 break
-        if match:
+    return wps
 
-            kvp = {}
-            for key in self.keys:
-                kvp[key] = row.key_value_pairs[key]
-
-            data0 = {}
-            for calc in self.calculators:
-                key = calc + '_info'
-                if key in row.data.keys():
-                    data0[key] = row.data[key]
 
-            atom = self.db.get_atoms(id=row.id)
-            return (atom, kvp, data0)
-        else:
-            msg = 'cannot find the entry from ' + id + code
-            raise RuntimeError(msg)
+def reset_lammps_cell(atoms0):
+    """
+    set the cell into lammps format
+    """
+    from ase.calculators.lammpslib import convert_cell
 
-    def get_row(self, code):
-        for row in self.db.select(csd_code=code):
-            return row
-        msg = 'cannot find the entry from ' + code
-        raise RuntimeError(msg)
-
-    def get_pyxtal(self, code):
-        from pyxtal import pyxtal
-        from pyxtal.util import ase2pymatgen
-        from pyxtal.msg import ReadSeedError
-
-        row = self.get_row(code)
-        atom = self.db.get_atoms(id=row.id)
-        #Reference
-        pmg = ase2pymatgen(atom)
-        smi = row.mol_smi
-        smiles = smi.split('.')
-        molecules = [smile+'.smi' for smile in smiles]
-
-        xtal = pyxtal(molecular=True)
-        try:
-            xtal.from_seed(pmg, molecules=molecules)
-        except ReadSeedError:
-            xtal.from_seed(pmg, molecules=molecules, add_H=True)
-
-        return xtal
-
-    def compute(self, row, work_dir, skf_dir):
-        if len(row.data.keys())<len(self.calculators):
-            #not label information, run antechamber
-            atom = self.db.get_atoms(id=row.id)
-            if 'gulp_info' not in row.data.keys():
-                pmg, c_info, g_info = get_parameters(row, atom)
-                row.data = {'charmm_info': c_info,
-                            'gulp_info': g_info
-                           }
-            else:
-                pmg = ase2pymatgen(atom)
+    atoms = atoms0.copy()
+    mat, coord_transform = convert_cell(atoms0.cell)
+    if coord_transform is not None:
+        pos = np.dot(atoms0.positions, coord_transform.T)
+        atoms.set_cell(mat.T)
+        atoms.set_positions(pos)
+    return atoms
+
+def new_struc(xtal, xtals):
+    """
+    check if this is a new structure
 
-            data = compute(row, pmg, work_dir, skf_dir)
-            self.db.update(row.id, data=data)
-            print('updated the data for', row.csd_code)
-
-class database_topology():
-    """
-    This is a database class to process atomic crystal data
-
-    Args:
-        db_name: *.db format from ase database
-    """
-
-
-    def __init__(self, db_name, ltol=0.05, stol=0.05, atol=3):
-        #if not os.path.exists(db_name):
-        #    raise ValueError(db_name, 'doesnot exist')
-        self.db_name = db_name
-        self.db = connect(db_name)
-        self.keys = ['space_group_number',
-                     'similarity',
-                     'ff_energy',
-                     'density',
-                     'dof',
-                     'topology',
-                     'dimension',
-                     'similarity0',
-                     'wps'
-                    ]
-        self.matcher = sm.StructureMatcher(ltol=ltol, stol=stol, angle_tol=atol)
-
-    def vacuum(self):
-        self.db.vacuum()
-
-    def get_pyxtal(self, id):
-        from pyxtal import pyxtal
-        from pyxtal.util import ase2pymatgen
-
-        row = self.db.get(id) #; print(id, row.id)
-        atom = self.db.get_atoms(id=id)
-        pmg = ase2pymatgen(atom)
-        xtal = pyxtal()
-        try:
-            xtal.from_seed(pmg)
-            if xtal is not None and xtal.valid:
-                for key in self.keys:
-                    if hasattr(row, key):
-                        setattr(xtal, key, getattr(row, key))
-            return xtal
-        except:
-            print('Cannot load the structure')
-
-    def get_all_xtals(self):
-        """
-        Get all pyxtal instances from the current db
-        """
-        xtals = []
-        for row in self.db.select():
-            xtal = self.get_pyxtal(id=row.id)
-            if xtal is not None:
-                xtals.append(xtal)
-        return xtals
-
-    def add_xtal(self, xtal, kvp):
-        """
-        Add new xtal to the given db
-        """
-        spg_num = xtal.group.number
-        density = xtal.get_density()
-        dof = xtal.get_dof()
-        wps = [s.wp.get_label() for s in xtal.atom_sites]
-        _kvp = {"space_group_number": spg_num,
-                "wps": str(wps),
-                "density": density,
-                "dof": dof,
-               }
-        kvp.update(_kvp)
-        atoms = xtal.to_ase(resort=False)
-        self.db.write(atoms, key_value_pairs=kvp)
-
-    def check_new_structure(self, xtal, same_group=True):
-        """
-        Check if the input xtal already exists in the db
-
-        Args:
-            xtal: pyxtal object
-            same_group (bool): keep the same group or not
-        """
-
-        s_pmg = xtal.to_pymatgen()
-        for row in self.db.select():
-            ref = self.db.get_atoms(id=row.id)
-            ref_pmg = None
-            if same_group:
-                if row.space_group_number != xtal.group.number:
-                    continue
-            ref_pmg = ase2pymatgen(ref)
-            if self.matcher.fit(s_pmg, ref_pmg, symmetric=True):
-                return False
+    Args:
+        xtal: input structure
+        xtals: list of reference structures
+
+    Return:
+        `None` or the id of matched structure
+    """
+    import pymatgen.analysis.structure_matcher as sm
+
+    if xtal is None or not hasattr(xtal, 'energy'):
+        return False
+    else:
+        eng1 = xtal.energy
+        pmg_s1 = xtal.to_pymatgen()
+        pmg_s1.remove_species("H")
+        vol1 = pmg_s1.lattice.volume
+
+        for xtal2 in xtals:
+            #print(rep); print(rep2)
+            eng2 = xtal2.energy
+            if abs(eng1-eng2)<1e-2:
+                pmg_s2 = xtal2.to_pymatgen()
+                vol2 = pmg_s2.lattice.volume
+                if abs(vol1-vol2)/vol1<5e-2:
+                    pmg_s2.remove_species("H")
+                    if sm.StructureMatcher().fit(pmg_s1, pmg_s2):
+                        #print(pmg_s2); import sys; sys.exit()
+                        return False
         return True
 
-    def clean_structures(self, dtol=1e-3, etol=1e-3):
-        """
-        Clean up the db by removing the duplicate structures
-        Here we check the follow criteria
-            - same number of atoms
-            - same density
-            - same energy
-
-        Args:
-            dtol (float): tolerance of density
-            etol (float): tolerance of energy
-        """
-
-        unique_rows = []
-        to_delete = []
-
-        for row in self.db.select():
-            unique = True
-            for prop in unique_rows:
-                (natoms, den, ff_energy) = prop
-                if natoms==row.natoms and abs(den-row.density) < dtol:
-                    if hasattr(row, 'ff_energy'):
-                        if abs(row.ff_energy-ff_energy) < etol:
-                            unique = False
-                            break
-                    else:
-                        unique = False
-                        break
-            if unique:
-                if hasattr(row, 'ff_energy'):
-                    unique_rows.append((row.natoms, row.density, row.ff_energy))
-                else:
-                    unique_rows.append((row.natoms, row.density, None))
-            else:
-                to_delete.append(row.id)
-        print("The following structures were deleted", to_delete)
-        self.db.delete(to_delete)
-
-    def clean_structures_pmg(self, dtol=5e-2, criteria=None):
-        """
-        Clean up the db by removing the duplicate structures
-        Here we check the follow criteria
-            - same density
-            - pymatgen check
-
-        criteria should look like the following,
-        {'CN': {'C': 3},
-         'cutoff': 1.8,
-         'MAX_energy': -8.00,
-         #'MAX_similarity': 0.2,
-         'BAD_topology': ['hcb'],
-         'BAD_dimension': [0, 2],
-        }
-
-        Args:
-            dtol (float): tolerance of density
-            criteria (dict): including
-        """
-
-        unique_rows = []
-        to_delete = []
-
-        for row in self.db.select():
-            xtal = self.get_pyxtal(id=row.id)
-            unique = True
-
-            if criteria is not None:
-                if not xtal.check_validity(criteria, True):
-                    unique = False
-                    print('Found unsatisfied criteria', row.id, row.space_group_number, row.wps)
-
-                if unique:
-                    if 'MAX_energy' in criteria and hasattr(row, 'ff_energy') \
-                        and row.ff_energy > criteria['MAX_energy']:
-                        unique = False
-                        print('Found unsatisfied energy', row.id, row.ff_energy, row.space_group_number, row.wps)
-                if unique:
-                    if 'MAX_similarity' in criteria and hasattr(row, 'similarity') \
-                        and row.similarity > criteria['MAX_similarity']:
-                        unique = False
-                        print('Found unsatisfied similarity', row.id, row.similarity, row.space_group_number, row.wps)
-                if unique:
-                    if 'BAD_topology' in criteria and hasattr(row, 'topology') \
-                        and row.topology[:3] in criteria['BAD_topology']:
-                        unique = False
-                        print('Found unsatisfied topology', row.id, row.topology, row.space_group_number, row.wps)
-                if unique:
-                    if 'BAD_dimension' in criteria and hasattr(row, 'dimension') \
-                        and row.dimension in criteria['BAD_dimension']:
-                        unique = False
-                        print('Found unsatisfied dimension', row.id, row.topology, row.space_group_number, row.wps)
-
-
-            if unique:
-                for prop in unique_rows:
-                    (rowid, den) = prop
-                    if abs(den-row.density) < dtol:
-                        ref_pmg = xtal.to_pymatgen()
-                        s_pmg = ase2pymatgen(self.db.get_atoms(id=rowid))
-                        if self.matcher.fit(s_pmg, ref_pmg):#, symmetric=True):
-                            print('Found duplicate', row.id, row.space_group_number, row.wps)
-                            unique = False
-                            break
-            if unique:
-                unique_rows.append((row.id, row.density))
-            else:
-                to_delete.append(row.id)
-        print("The following structures were deleted", to_delete)
-        self.db.delete(to_delete)
-
-
-    def update_row_topology(self, StructureType='Auto', overwrite=True):
-        """
-        Update row topology base on the CrystalNets.jl
-        """
-        try:
-            import juliacall
-        except:
-            print("Cannot load JuliaCall, no support on topology parser")
-
-        def parse_topology(topology_info):
-            """
-            Obtain the dimensionality and topology name
-            """
-            dim = 0
-            name = ""
-            for i, x in enumerate(topology_info):
-                (d, n) = x
-                if d > dim: dim = d
-                tmp = n.split(',')[0]
-                if tmp.startswith("UNKNOWN"):
-                    tmp = 'aaa'
-                elif tmp.startswith("unstable"):
-                    tmp = 'unstable'
-                name += tmp
-                if i + 1 < len(topology_info): name += '-'
-            return dim, name
-
-        jl = juliacall.newmodule("MOF_Builder")
-        jl.seval("using CrystalNets")
-        jl.CrystalNets.toggle_warning(False) # to disable warnings
-        jl.CrystalNets.toggle_export(False) # to disable exports
-        if StructureType == 'Zeolite':
-            option = jl.CrystalNets.Options(structure=jl.StructureType.Zeolite)
-        elif StructureType == 'MOF':
-            option = jl.CrystalNets.Options(structure=jl.StructureType.MOF)
-        else:
-            option = jl.CrystalNets.Options(structure=jl.StructureType.Auto)
+def new_struc_wo_energy(xtal, xtals):
+    """
+    check if this is a new structure
 
-        for row in self.db.select():
-            if overwrite or not hasattr(row, 'topology'):
-                atoms = self.db.get_atoms(row.id)
-                atoms.write('tmp.cif', format='cif')
-
-                # Call crystalnet.jl
-                result = jl.determine_topology('tmp.cif', option)
-                #print(result)
-                if len(result) > 1:
-                    results = [x for x in result]
-                else:
-                    results = [result[0]]
-                try:
-                    topo = []
-                    for res in results:
-                        # topology for SingleNodes
-                        name = str(res[0])
-                        if res[1] > 1: name += '(' + str(res[1]) + ')'
-                        genome = res[0][jl.Clustering.Auto]
-                        dim = jl.ndims(jl.CrystalNets.PeriodicGraph(genome))
-                        topo.append((dim, name))
-
-                    # The maximum dimensionality and topology name
-                    dim, name = parse_topology(topo)
-                except:
-                    dim, name = 3, 'error'
-                print("Updating", row.space_group_number, row.wps, dim, name)
-                # Unknown will be labeled as aaa
-                self.db.update(row.id, topology=name, dimension=dim)
-            else:
-                print("Existing", row.topology)
+    Args:
+        xtal: input structure
+        xtals: list of reference structures
 
-    def update_db_description(self):
-        """
-        update db description based on robocrys
-        Call robocrys: https://github.com/hackingmaterials/robocrystallographer
-        """
-        from robocrys import StructureCondenser, StructureDescriber
-        condenser = StructureCondenser()
-        describer = StructureDescriber()
-
-        for row in self.db.select():
-            if not hasattr(row, 'description'):
-                atoms = self.db.get_atoms(row.id)
-                pmg = ase2pymatgen(atoms)
-                try:
-                    condensed_structure = condenser.condense_structure(pmg)
-                    description = describer.describe(condensed_structure)
-                except:
-                    description = 'N/A'
+    Return:
+        `None` or the id of matched structure
+    """
+    import pymatgen.analysis.structure_matcher as sm
 
-                self.db.update(row.id, description=description)
-                print("\n======Updating\n", description)
-            else:
-                print("\n======Existing\n", row.description)
+    if xtal is None:
+        return False
+    else:
+        pmg_s1 = xtal.to_pymatgen()
+        pmg_s1.remove_species("H")
+        vol1 = pmg_s1.lattice.volume
+
+        for xtal2 in xtals:
+            #print(rep); print(rep2)
+            pmg_s2 = xtal2.to_pymatgen()
+            vol2 = pmg_s2.lattice.volume
+            if abs(vol1-vol2)/vol1<5e-2:
+                pmg_s2.remove_species("H")
+                if sm.StructureMatcher().fit(pmg_s1, pmg_s2):
+                    #print(pmg_s2); import sys; sys.exit()
+                    return False
+        return True
 
-    def export_structures(self, fmt='vasp', folder='mof_out', criteria=None,
-                          sort_by='similarity'):
-        """
-        export structures from database according to the given criterion
-
-        Args:
-            fmt (str): 'vasp' or 'cif'
-            folder (str): 'path of output folders'
-            criteria (dict): check the validity with dict
-            sort_by (str): sort by which attribute
-        """
-
-        if not os.path.exists(folder): os.makedirs(folder)
-        keys = ['space_group_number',
-                'density',
-                'dof',
-                'similarity',
-                'ff_energy',
-                'topology',
-               ]
-        properties, atoms = [], []
-        for row in self.db.select():
-            spg = row.space_group_number
-            den = row.density
-            dof = row.dof
-            sim = row.similarity if hasattr(row, 'similarity') else None
-            top = row.topology if hasattr(row, 'topology') else None
-            eng = row.ff_energy if hasattr(row, 'ff_energy') else None
-            properties.append([row.id, spg, den, dof, sim, eng, top])
-            atoms.append(self.db.get_atoms(id=row.id))
+def split_list_by_ratio(nums, ratio):
+    """
+    Splits a list of integers into two groups such that the sum of each group
+    satisfies a given ratio and returns all possible ways of combinations
+    tracking the indices of the numbers.
+
+    Parameters:
+    nums (list of int): The list of integers to split.
+    ratio (tuple of int): A tuple representing the desired ratio (e.g., (1, 1) for 1:1 ratio).
 
-        if sort_by in keys:
-            col = keys.index(sort_by) + 1
-        else:
-            print("supported attributes", keys)
-            raise ValueError("Cannot sort by", sort_by)
+    Returns:
+    list of tuple: A list of tuples where each tuple contains two lists of indices.
+                   Each pair of lists represents one possible way to split the numbers
+                   to satisfy the given ratio.
+    """
+    def find_splits(i, sum1, sum2, group1, group2):
+        if i == len(nums):
+            if sum1 * ratio[1] == sum2 * ratio[0]:
+                solutions.append((group1.copy(), group2.copy()))
+            return
+
+        # Try adding the current number's index to the first group
+        group1.append(i)
+        find_splits(i + 1, sum1 + nums[i], sum2, group1, group2)
+        group1.pop()
+
+        # Try adding the current number's index to the second group
+        group2.append(i)
+        find_splits(i + 1, sum1, sum2 + nums[i], group1, group2)
+        group2.pop()
 
-        print("====Exporting {:} structures".format(len(atoms)))
-        if len(atoms)>0:
-            properties = np.array(properties)
-            mids = np.argsort(properties[:, col])
-
-            for mid in mids:
-                [id, spg, den, dof, sim, eng, top] = properties[mid]
-                id = int(id)
-                spg = int(spg)
-                sim = float(sim)
-                den = float(den)
-                dof = int(dof)
-                if eng is not None: eng = float(eng)
-                try:
-                    xtal = pyxtal()
-                    xtal.from_seed(atoms[mid])
-                    number, symbol = xtal.group.number, xtal.group.symbol.replace('/','')
-                    # convert to the desired subgroup representation if needed
-                    if number != spg:
-                        paths = xtal.group.path_to_subgroup(spg)
-                        xtal = xtal.to_subgroup(paths)
-                        number, symbol = xtal.group.number, xtal.group.symbol.replace('/','')
-
-                    label = os.path.join(folder, '{:d}-{:d}-{:s}'.format(id, number, symbol))
-
-                    if criteria is not None:
-                        status = xtal.check_validity(criteria, True)
-                    else:
-                        status = True
-                except:
-                    status = False
-
-                if status:
-                    if top is not None: print(top)
-                    try:
-                        xtal.set_site_coordination()
-                        for s in xtal.atom_sites:
-                            _l, _sp, _cn = s.wp.get_label(), s.specie, s.coordination
-                            label += '-{:s}-{:s}{:d}'.format(_l, _sp, _cn)
-                        label += '-S{:.3f}'.format(sim)
-                    except:
-                        print('Problem in setting site coordination')
-                    if len(label)>40: label = label[:40]
-
-                    if den is not None: label += '-D{:.2f}'.format(abs(den))
-                    if eng is not None: label += '-E{:.3f}'.format(abs(eng))
-                    if top is not None: label += '-T{:s}'.format(top)
-                    if sim is not None: label += '-S{:.2f}'.format(sim)
-
-                    print("====Exporting:", label)
-                    if fmt == 'vasp':
-                        atoms[mid].write(label+'.vasp', format='vasp', vasp5=True, direct=True)
-                    elif fmt == 'cif':
-                        xtal.to_file(label+'.cif')
-                else:
-                    print("====Skippng:  ", label)
+    solutions = []
+    nums = sorted(nums, reverse=True)  # Optional: Sorting can sometimes speed up the process
+
+    find_splits(0, 0, 0, [], [])
+    return solutions
 
 
 if __name__ == "__main__":
-    # open
-    if False:
-        db = database('test.db')
-        print("Total number of entries", len(db.codes))
-
-        # view structure
-        c = db.get_pyxtal('HXMTAM')
-        print(c)
-    if True:
-        db = database_topology('../MOF-Builder/reaxff.db')
-        xtal = db.get_pyxtal(1)
-        print(xtal)
-        db.add_xtal(xtal, kvp={'similarity': 0.1})
+    from argparse import ArgumentParser
+
+    parser = ArgumentParser()
+    parser.add_argument(
+        "-f",
+        dest="file",
+        help="path of database file"
+    )
+    parser.add_argument(
+        "-i",
+        dest="id",
+        help="index of the row",
+    )
+
+    options = parser.parse_args()
+    ids = options.id
+    if ids.find(",")>0:
+        ids = [int(id) for id in ids.split(",")]
+    else:
+        ids = [int(ids)]
+    extract_ase_db(options.file, ids)
```

### Comparing `pyxtal-0.6.6/pyxtal/descriptor.py` & `pyxtal-0.6.7/pyxtal/descriptor.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/elasticity.py` & `pyxtal-0.6.7/pyxtal/elasticity.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/interface/LJ.py` & `pyxtal-0.6.7/pyxtal/interface/LJ.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/interface/dftb.py` & `pyxtal-0.6.7/pyxtal/interface/dftb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import os
+import os, re
 from ase.io import read
 from ase.optimize.fire import FIRE
 from ase.constraints import ExpCellFilter
 from ase.spacegroup.symmetrize import FixSymmetry
 from pyxtal.util import Kgrid
 from ase.calculators.calculator import (FileIOCalculator, kpts2ndarray,
                                         kpts2sizeandoffsets)
 from ase.units import Hartree, Bohr
 import numpy as np
 
 
-def make_Hamiltonian(skf_dir, atom_types, disp, kpts, write_band=False, use_omp=False):
+def make_Hamiltonian(skf_dir, atom_types, disp, kpts, scc_error=1e-06,
+                     scc_iter=500, write_band=False, use_omp=False):
     """
     Generate the DFTB Hamiltonian for DFTB+
     """
     if disp == 'D3': #from dftb manual
         dispersion = '''DftD3{
                       Damping = BeckeJohnson{
                       a1 = 0.5719
@@ -59,23 +60,24 @@
     elif disp == 'LJ':
         dispersion = 'LennardJones{Parameters = UFFParameters{}}'
     else:
         dispersion = None
 
 
     kwargs = {'Hamiltonian_SCC': 'yes',
-              'Hamiltonian_SCCTolerance': 1e-06,
-              'Hamiltonian_MaxSCCIterations': 1000,
+              'Hamiltonian_SCCTolerance': scc_error, #1e-06,
+              'Hamiltonian_MaxSCCIterations': scc_iter, #1000,
               #'Hamiltonian_Mixer': 'DIIS{}', #Default is Broyden
               #'Hamiltonian_Dispersion': dispersion,
               'slako_dir': skf_dir,
               'Analysis_': '',
               'Analysis_WriteBandOut': 'No',
               'Analysis_MullikenAnalysis': 'No',
               'Analysis_CalculateForces': 'Yes',
+              'Analysis_PrintForces': 'Yes',
              }
     if write_band:
         kwargs['Analysis_WriteBandOut'] = 'Yes'
     if use_omp:
         kwargs['Parallel_'] = ''
         kwargs['Parallel_UseOmpThreads'] = 'Yes'
     if dispersion is not None:
@@ -153,15 +155,16 @@
     #pbc
     #print(calc_type, kwargs)
     return kwargs
 
 
 def DFTB_relax(struc, skf_dir, opt_cell=False, step=500, \
                fmax=0.1, kresol=0.10, folder='tmp', disp='D3', \
-               mask=None, symmetrize=True, logfile=None, use_omp=False):
+               mask=None, symmetrize=True, logfile=None, \
+               scc_error=1e-6, scc_iter=500, use_omp=False):
     """
     DFTB optimizer based on ASE
 
     Args:
         struc: ase atoms object
         mode: [`single`, `relax`, `vc_relax`] (str)
         step: optimization steps (int)
@@ -169,15 +172,17 @@
     """
     if not os.path.exists(folder):
         os.makedirs(folder)
     cwd = os.getcwd()
     os.chdir(folder)
     if type(kresol) != list: kpts = Kgrid(struc, kresol)
     atom_types = set(struc.get_chemical_symbols())
-    kwargs = make_Hamiltonian(skf_dir, atom_types, disp, kpts, use_omp=use_omp)
+    kwargs = make_Hamiltonian(skf_dir, atom_types, disp, kpts,
+                              scc_error=scc_error,
+                              use_omp=use_omp)
 
     calc = Dftb(label='test',
                 atoms=struc,
                 kpts=kpts,
                 **kwargs,
                 )
     struc.set_calculator(calc)
@@ -260,25 +265,29 @@
     def __init__(self, struc, skf_dir,
                  disp = 'D3',
                  kresol = 0.10,
                  folder = 'tmp',
                  label = 'test',
                  prefix = 'geo_final',
                  use_omp = False,
+                 scc_error = 1e-6,
+                 scc_iter = 500,
                 ):
 
         self.struc = struc
         self.skf_dir = skf_dir
         self.folder = folder
         self.kresol = kresol
         self.disp = disp
         self.label = label
         self.kpts = Kgrid(struc, kresol)
         self.prefix = prefix
         self.use_omp = use_omp
+        self.scc_error = scc_error
+        self.scc_iter = scc_iter
         if not os.path.exists(self.folder):
            os.makedirs(self.folder)
 
     def get_calculator(self, mode, step=500, ftol=1e-3, FixAngles=False, eVperA=True, md_params={}):
         """
         get the ase style calculator
 
@@ -290,15 +299,18 @@
             eVperA: unit in eV/A
 
         Returns:
             ase calculator
         """
         if eVperA: ftol *= 0.194469064593167E-01
         atom_types = set(self.struc.get_chemical_symbols())
-        kwargs = make_Hamiltonian(self.skf_dir, atom_types, self.disp, self.kpts, use_omp=self.use_omp)
+        kwargs = make_Hamiltonian(self.skf_dir, atom_types, self.disp, self.kpts,
+                                  scc_error=self.scc_error,
+                                  scc_iter=self.scc_iter,
+                                  use_omp=self.use_omp)
 
         if mode in ['relax', 'vc-relax']:
             #kwargs['Driver_'] = 'ConjugateGradient'
             kwargs['Driver_'] = 'GeometryOptimization'
             kwargs['Driver_Optimizer'] = 'FIRE {}'
             #kwargs['Driver_MaxForceComponent'] = ftol
             kwargs['Driver_MaxSteps'] = step
@@ -357,28 +369,28 @@
         execute the actual calculation
         """
         from time import time
         t0 = time()
         cwd = os.getcwd()
         os.chdir(self.folder)
 
-        calc = self.get_calculator(mode, step, ftol, FixAngles, md_params=md_params)
-        self.struc.set_calculator(calc)
+        self.calc = self.get_calculator(mode, step, ftol, FixAngles, md_params=md_params)
+        self.struc.set_calculator(self.calc)
         # self.struc.write('geo_o.gen', format='dftb')
         # execute the simulation
-        calc.calculate(self.struc)
+        self.calc.calculate(self.struc)
         if mode in ['relax', 'vc-relax']:
             final = read(self.prefix+'.gen')
         else:
             final = self.struc
 
         # get the final energy
         energy = self.struc.get_potential_energy()
 
-        with open(self.label+'.out') as f:
+        with open(self.label + '.out') as f:
             l = f.readlines()
             self.version = l[2]
         os.chdir(cwd)
         self.time = time() - t0
         return final, energy
 
 class Dftb(FileIOCalculator):
@@ -614,42 +626,71 @@
         self.atoms_input = atoms
         self.atoms = None
 
     def read_results(self):
         """ all results are read from results.tag file
             It will be destroyed after it is read to avoid
             reading it once again after some runtime error """
-
         with open(os.path.join(self.directory, 'results.tag'), 'r') as fd:
             self.lines = fd.readlines()
+        if len(self.lines) == 0:
+            #print("READ RESULTS from test.out")
+            self.results['energy'] = self.read_energy()
+            self.results['forces'] = None
+            self.results['stress'] = None
+        else:
+            self.atoms = self.atoms_input
+            self.results['energy'] = float(self.lines[1])*Hartree
+            forces = self.read_forces()
+            self.results['forces'] = forces
+
+            # stress stuff begins
+            sstring = 'stress'
+            have_stress = False
+            stress = list()
+            for iline, line in enumerate(self.lines):
+                if sstring in line:
+                    have_stress = True
+                    start = iline + 1
+                    end = start + 3
+                    for i in range(start, end):
+                        cell = [float(x) for x in self.lines[i].split()]
+                        stress.append(cell)
+            if have_stress:
+                stress = -np.array(stress) * Hartree / Bohr**3
+                self.results['stress'] = stress.flat[[0, 4, 8, 5, 2, 1]]
+            # stress stuff ends
 
-        self.atoms = self.atoms_input
-        self.results['energy'] = float(self.lines[1])*Hartree
-        forces = self.read_forces()
-        self.results['forces'] = forces
-
-        # stress stuff begins
-        sstring = 'stress'
-        have_stress = False
-        stress = list()
-        for iline, line in enumerate(self.lines):
-            if sstring in line:
-                have_stress = True
-                start = iline + 1
-                end = start + 3
-                for i in range(start, end):
-                    cell = [float(x) for x in self.lines[i].split()]
-                    stress.append(cell)
-        if have_stress:
-            stress = -np.array(stress) * Hartree / Bohr**3
-            self.results['stress'] = stress.flat[[0, 4, 8, 5, 2, 1]]
-        # stress stuff ends
+            # calculation was carried out with atoms written in write_input
+            os.remove(os.path.join(self.directory, 'results.tag'))
 
-        # calculation was carried out with atoms written in write_input
-        os.remove(os.path.join(self.directory, 'results.tag'))
+    def read_energy(self):
+        """
+        If SCC is not converged, read the last step energy from test.out
+        """
+        outfile = self.label + '.out'
+        energies = []
+        with open(os.path.join(self.directory, outfile), 'r') as fd:
+            lines = fd.readlines()
+        for line in lines:
+            m = re.match(r'Total Energy:\s+[-\d.]+ H\s+([-.\d]+) eV', line)
+            if m:
+                energies.append(float(m.group(1)))
+        if len(energies) > 0:
+            return energies[-1]
+        else:
+            try:
+                #   100   -0.38553421E+03    0.29798304E-03    0.12389437E-01
+                #ERROR!
+                #-> SCC is NOT converged, maximal SCC iterations exceeded
+                print("Cannot read energy from this file", os.getcwd())
+                eng = float(lines[-3].split()[1]) * 27.2114 # hatree to eV
+                return eng
+            except:
+                return 1.0e+5
 
     def read_forces(self):
         """Read Forces from dftb output file (results.tag)."""
 
         # Initialise the indices so their scope
         # reaches outside of the for loop
         index_force_begin = -1
```

### Comparing `pyxtal-0.6.6/pyxtal/interface/gulp.py` & `pyxtal-0.6.7/pyxtal/interface/gulp.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     ff: path of forcefield lib
     opt: `conv`, `conp`, `single`
     pstress (float): external pressure
     steps (int): relaxation steps
     symm (bool): whether or not impose the symmetry
     """
 
-    def __init__(self, struc, label="_", path='tmp', ff='reax', \
+    def __init__(self, struc, label="_", path='tmp', ff='reaxff', \
                  pstress=None, opt='conp', steps=1000, exe='gulp',\
                  input='gulp.in', output='gulp.log', dump=None,
                  symmetry=False, labels=None):
 
         if isinstance(struc, pyxtal):
             self.pyxtal = struc
             self.species = struc.species
@@ -36,25 +36,25 @@
         if isinstance(struc, Atoms):
             self.lattice = Lattice.from_matrix(struc.cell)
             self.frac_coords = struc.get_scaled_positions()
             self.sites = struc.get_chemical_symbols()
             self.species = None
         else:
             raise NotImplementedError("only support ASE atoms object")
-        
+
         self.symmetry = symmetry#; print(self.pyxtal.lattice.ltype)
         self.structure = struc
         self.pstress= pstress
         self.label = label
         self.labels = labels
         self.ff = ff
         self.opt = opt
         self.exe = exe
         self.steps = steps
-        self.folder = path  
+        self.folder = path
         if not os.path.exists(self.folder):
             os.makedirs(self.folder)
         self.input = self.folder + '/' + self.label + input
         self.output = self.folder + '/' + self.label + output
         self.dump = dump
         self.iter = 0
         self.energy = None
@@ -83,16 +83,20 @@
             self.clean()
 
     def execute(self):
         cmd = self.exe + '<' + self.input + '>' + self.output
         os.system(cmd)
 
     def clean(self):
-        os.remove(self.input)
-        os.remove(self.output)
+        if self.error:
+            os.system('mv ' + self.input + ' ' + self.input + '_error')
+            os.system('mv ' + self.output + ' ' + self.output + '_error')
+        else:
+            os.remove(self.input)
+            os.remove(self.output)
         if self.dump is not None:
             os.remove(self.dump)
 
     def to_ase(self):
         return Atoms(self.sites, scaled_positions=self.frac_coords, cell=self.lattice.matrix)
 
     def to_pymatgen(self):
@@ -110,15 +114,15 @@
                 pass
                 #print('Something is wrong', tol)
                 #struc.from_seed('bug.vasp', tol*10)
         return struc
 
     def write(self):
         a, b, c, alpha, beta, gamma = self.lattice.get_para(degree=True)
-        
+
         with open(self.input, 'w') as f:
             if self.opt == 'conv':
                 f.write('opti stress {:s} conjugate '.format(self.opt))
             elif self.opt == "single":
                 f.write('grad conp stress ')
             else:
                 f.write('opti stress {:s} conjugate '.format(self.opt))
@@ -126,15 +130,15 @@
             if not self.symmetry:
                 f.write('nosymmetry\n')
 
             f.write('\ncell\n')
             f.write('{:12.6f}{:12.6f}{:12.6f}{:12.6f}{:12.6f}{:12.6f}\n'.format(\
                     a, b, c, alpha, beta, gamma))
             f.write('\nfractional\n')
-            
+
             symbols = []
             if self.symmetry and self.pyxtal is not None:
                 # Use pyxtal here
                 for site in self.pyxtal.atom_sites:
                     symbol, coord = site.specie, site.position
                     f.write('{:4s} {:12.6f} {:12.6f} {:12.6f} core \n'.format(symbol, *coord))
                     if self.ff == 'catlow' and symbol == 'O':
@@ -188,15 +192,15 @@
         if self.pyxtal is not None:
             ltype = self.pyxtal.lattice.ltype
         else:
             ltype = 'triclinic'
 
         with open(self.output, 'r') as f:
             lines = f.readlines()
-        try: 
+        try:
             for i, line in enumerate(lines):
                 if self.symmetry and self.pyxtal.group.symbol[0] != 'P':
                     m = re.match(r'\s*Non-primitive unit cell\s*=\s*(\S+)\s*eV', line)
                 elif self.pstress is None or self.pstress == 0:
                     m = re.match(r'\s*Total lattice energy\s*=\s*(\S+)\s*eV', line)
                 else:
                     m = re.match(r'\s*Total lattice enthalpy\s*=\s*(\S+)\s*eV', line)
@@ -251,15 +255,15 @@
                         G = [-float(x) * eV / Ang for x in g]
                         forces.append(G)
                     forces = np.array(forces)
                     self.forces = forces
 
                 elif line.find(' Cycle: ') != -1:
                     self.iter = int(line.split()[1])
-    
+
                 # asymmetric unit
                 elif line.find('Final asymmetric unit coordinates') != -1:
                     s = i + 6
                     positions = []
                     for _i in range(len(self.pyxtal.atom_sites)):
                         xyz = lines[s+_i].split()[3:6]
                         XYZ = [float(x) for x in xyz]
@@ -312,53 +316,53 @@
             self.pyxtal.lattice = self.lattice
 
         if self.energy is None or np.isnan(self.energy):
             self.error = True
             self.energy = None
             print("GULP calculation is wrong, reading------")
 
-def single_optimize(struc, ff, steps=1000, pstress=None, opt="conp", 
+def single_optimize(struc, ff, steps=1000, pstress=None, opt="conp",
                     exe="gulp", path="tmp", label="_", clean=True,
                     symmetry=False, labels=None):
 
-    calc = GULP(struc, steps=steps, label=label, path=path, 
-                pstress=pstress, ff=ff, opt=opt, 
+    calc = GULP(struc, steps=steps, label=label, path=path,
+                pstress=pstress, ff=ff, opt=opt,
                 symmetry=symmetry, labels=labels)
 
     calc.run(clean=clean)
 
     if calc.error:
         print("GULP error in single optimize")
         return None, None, 0, True
     else:
         if calc.pyxtal is None:
             struc = calc.to_pyxtal()
         else:
             struc = calc.pyxtal
-        #if sum(struc.numIons) == 42: print("SSSSS"); import sys; sys.exit()   
+        #if sum(struc.numIons) == 42: print("SSSSS"); import sys; sys.exit()
         return struc, calc.energy_per_atom, calc.cputime, calc.error
 
-def optimize(struc, ff, optimizations=["conp", "conp"], exe="gulp", 
+def optimize(struc, ff, optimizations=["conp", "conp"], exe="gulp",
             pstress=None, path="tmp", label="_", clean=True, adjust=False):
     """
     Multiple calls
 
     """
     time_total = 0
     for opt in optimizations:
-        struc, energy, time, error = single_optimize(struc, ff, 
+        struc, energy, time, error = single_optimize(struc, ff,
         pstress=pstress, opt=opt, exe=exe, path=path, label=label, clean=clean)
 
         time_total += time
         if error:
             return None, None, 0, True
         elif adjust and abs(energy)<1e-8:
             matrix = struc.lattice.matrix
             struc.lattice.set_matrix(matrix*0.8)
-            
+
     return struc, energy, time_total, False
 
 
 if __name__ == "__main__":
 
     while True:
         struc = pyxtal()
```

### Comparing `pyxtal-0.6.6/pyxtal/interface/lammpslib.py` & `pyxtal-0.6.7/pyxtal/interface/lammpslib.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/interface/vasp.py` & `pyxtal-0.6.7/pyxtal/interface/vasp.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/interface/vasprun.py` & `pyxtal-0.6.7/pyxtal/interface/vasprun.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/io.py` & `pyxtal-0.6.7/pyxtal/io.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/lattice.py` & `pyxtal-0.6.7/pyxtal/lattice.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/molecular_crystal.py` & `pyxtal-0.6.7/pyxtal/molecular_crystal.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/molecule.py` & `pyxtal-0.6.7/pyxtal/molecule.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/msg.py` & `pyxtal-0.6.7/pyxtal/msg.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/operations.py` & `pyxtal-0.6.7/pyxtal/operations.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/optimize/fire.py` & `pyxtal-0.6.7/pyxtal/optimize/fire.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/optimize/fire2.py` & `pyxtal-0.6.7/pyxtal/optimize/fire2.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/optimize/myscipy_optimize.py` & `pyxtal-0.6.7/pyxtal/optimize/myscipy_optimize.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/plane.py` & `pyxtal-0.6.7/pyxtal/plane.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/potentials/CuAg.eam.alloy` & `pyxtal-0.6.7/pyxtal/potentials/CuAg.eam.alloy`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/potentials/LJ_cluster.py` & `pyxtal-0.6.7/pyxtal/potentials/LJ_cluster.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/potentials/Si.tersoff` & `pyxtal-0.6.7/pyxtal/potentials/Si.tersoff`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/potentials/SiCGe.tersoff` & `pyxtal-0.6.7/pyxtal/potentials/SiCGe.tersoff`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/representation.py` & `pyxtal-0.6.7/pyxtal/representation.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/supergroup.py` & `pyxtal-0.6.7/pyxtal/supergroup.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/symmetry.py` & `pyxtal-0.6.7/pyxtal/symmetry.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/test_all.py` & `pyxtal-0.6.7/pyxtal/test_all.py`

 * *Files 3% similar despite different names*

```diff
@@ -440,14 +440,34 @@
 
         c1 = pyxtal()
         c1.build(9, ['S'], [8], lattice=l1, sites=[sites])
         c1.optimize_lattice()
         pmg2 = c1.to_pymatgen()
         self.assertTrue(sm.StructureMatcher().fit(pmg0, pmg2))
 
+    def test_build_1D(self):
+        lat = Lattice.from_para(6.8472, 6.8472, 3.3198, 90, 90, 90, 'tetragonal')
+        c1 = pyxtal()
+        sites = [[('4g', 0.9236547993389047, 0.0, 0.5), ('4f', 0.39177300078207977, 0.0, 0.0)]]
+        c1.build(30, ['C'], [8], lat, sites=sites, dim=1)
+        self.assertTrue(c1.valid)
+
+    def test_build_2D(self):
+        lat = Lattice.from_para(6.8472, 6.8472, 3.3198, 90, 90, 90, 'tetragonal')
+        c1 = pyxtal()
+        sites = [[('4c', 0.15, 0.50, 0.28), ('4c', 0.59, 0.85, 0.87)]]
+        c1.build(30, ['C'], [8], lat, sites=sites, dim=2)
+        self.assertTrue(c1.valid)
+
+    #def test_build_0D(self):
+    #    lat = Lattice.from_para(2.85, 2.85, 2.85, 90, 90, 90, 'spherical')
+    #    c1 = pyxtal()
+    #    sites = [[('8b', 0.70, 0.70, 0.70)]]
+    #    c1.build(30, ['C'], [8], lat, sites=sites, dim=0)
+    #    self.assertTrue(c1.valid)
 
     def test_transforms(self):
         paras = [
                  (5.0317, 19.2982,  5.8004, 90.0000, 122.2672,  90.0000, 'monoclinic', 6),
                  (5.0317, 19.2982,  5.8004, 90.0000,  57.7328,  90.0000, 'monoclinic', 6),
                  (9.0640,  8.3522,  5.2856, 90.0000, 103.9699,  90.0000, 'monoclinic', 3),
                  (9.4913,  8.5844,  5.3358, 90.0000, 110.0035,  90.0000, 'monoclinic', 3),
@@ -506,15 +526,15 @@
                 (160, 2, '3m'),
                 (230, 6, '.32'),
                ]
         for d in data:
             (sg, i, symbol) = d
             wp = Group(sg)[i]
             wp.get_site_symmetry()
-            print("\n========", wp.site_symm, symbol, "==========\n")
+            #print("\n========", wp.site_symm, symbol, "==========\n")
             self.assertTrue(wp.site_symm == symbol)
 
     def test_wp_dof(self):
         for sg in range(1, 231):
             g = Group(sg)
             for wp in g:
                 axs = wp.get_frozen_axis()
```

### Comparing `pyxtal-0.6.6/pyxtal/tolerance.py` & `pyxtal-0.6.7/pyxtal/tolerance.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/viz.py` & `pyxtal-0.6.7/pyxtal/viz.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/wyckoff_site.py` & `pyxtal-0.6.7/pyxtal/wyckoff_site.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal/wyckoff_split.py` & `pyxtal-0.6.7/pyxtal/wyckoff_split.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/pyxtal.egg-info/PKG-INFO` & `pyxtal-0.6.7/pyxtal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxtal
-Version: 0.6.6
+Version: 0.6.7
 Summary: Python code for generation of crystal structures based on symmetry constraints.
 Home-page: https://github.com/qzhu2017/PyXtal
 Author: Scott Fredericks, Qiang Zhu
 Author-email: qiang.zhu@unlv.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyxtal-0.6.6/pyxtal.egg-info/SOURCES.txt` & `pyxtal-0.6.7/pyxtal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/scripts/pyxtal_main.py` & `pyxtal-0.6.7/scripts/pyxtal_main.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/scripts/pyxtal_symmetry.py` & `pyxtal-0.6.7/scripts/pyxtal_symmetry.py`

 * *Files identical despite different names*

### Comparing `pyxtal-0.6.6/setup.py` & `pyxtal-0.6.7/setup.py`

 * *Files identical despite different names*

