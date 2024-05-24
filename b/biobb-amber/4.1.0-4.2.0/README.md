# Comparing `tmp/biobb_amber-4.1.0.tar.gz` & `tmp/biobb_amber-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_amber-4.1.0.tar", last modified: Wed Sep  6 08:37:55 2023, max compression
+gzip compressed data, was "biobb_amber-4.2.0.tar", last modified: Fri May 24 07:40:14 2024, max compression
```

## Comparing `biobb_amber-4.1.0.tar` & `biobb_amber-4.2.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-09-06 08:37:55.320545 biobb_amber-4.1.0/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11357 2022-05-26 11:32:14.000000 biobb_amber-4.1.0/LICENSE
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      977 2023-09-06 08:37:55.320379 biobb_amber-4.1.0/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5315 2023-09-06 08:30:58.000000 biobb_amber-4.1.0/README.md
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-09-06 08:37:55.314620 biobb_amber-4.1.0/biobb_amber/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      155 2023-09-06 08:29:05.000000 biobb_amber-4.1.0/biobb_amber/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-09-06 08:37:55.315752 biobb_amber-4.1.0/biobb_amber/ambpdb/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       43 2022-05-26 11:32:14.000000 biobb_amber-4.1.0/biobb_amber/ambpdb/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7407 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/ambpdb/amber_to_pdb.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1898 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/ambpdb/common.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-09-06 08:37:55.316427 biobb_amber-4.1.0/biobb_amber/cphstats/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       60 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/cphstats/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    17622 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/cphstats/cestats_run.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2327 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/cphstats/common.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    17574 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/cphstats/cphstats_run.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-09-06 08:37:55.316918 biobb_amber-4.1.0/biobb_amber/cpptraj/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       54 2022-05-26 11:32:14.000000 biobb_amber-4.1.0/biobb_amber/cpptraj/__init__.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1968 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/cpptraj/common.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11027 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/cpptraj/cpptraj_randomize_ions.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-09-06 08:37:55.317747 biobb_amber-4.1.0/biobb_amber/leap/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      105 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/leap/__init__.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2144 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/leap/common.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    26378 2023-06-08 07:37:01.000000 biobb_amber-4.1.0/biobb_amber/leap/leap_add_ions.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8046 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/leap/leap_build_linear_structure.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    16671 2023-06-08 07:49:29.000000 biobb_amber-4.1.0/biobb_amber/leap/leap_gen_top.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    21736 2023-06-08 07:49:46.000000 biobb_amber-4.1.0/biobb_amber/leap/leap_solvate.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-09-06 08:37:55.318134 biobb_amber-4.1.0/biobb_amber/nab/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       51 2022-05-26 11:32:14.000000 biobb_amber-4.1.0/biobb_amber/nab/__init__.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1769 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/nab/common.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8722 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/nab/nab_build_dna_structure.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-09-06 08:37:55.318610 biobb_amber-4.1.0/biobb_amber/parmed/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       73 2022-05-26 11:32:14.000000 biobb_amber-4.1.0/biobb_amber/parmed/__init__.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1887 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/parmed/common.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9081 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/parmed/parmed_cpinutil.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7633 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/parmed/parmed_hmassrepartition.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-09-06 08:37:55.318962 biobb_amber-4.1.0/biobb_amber/pdb4amber/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       47 2022-05-26 11:32:14.000000 biobb_amber-4.1.0/biobb_amber/pdb4amber/__init__.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1810 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/pdb4amber/common.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7603 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/pdb4amber/pdb4amber_run.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-09-06 08:37:55.319317 biobb_amber-4.1.0/biobb_amber/pmemd/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       41 2022-05-26 11:32:14.000000 biobb_amber-4.1.0/biobb_amber/pmemd/__init__.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2414 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/pmemd/common.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    25615 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/pmemd/pmemd_mdrun.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-09-06 08:37:55.319813 biobb_amber-4.1.0/biobb_amber/process/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       63 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/process/__init__.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1841 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/process/common.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9046 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/process/process_mdout.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9149 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/process/process_minout.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-09-06 08:37:55.320177 biobb_amber-4.1.0/biobb_amber/sander/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       43 2022-05-26 11:32:14.000000 biobb_amber-4.1.0/biobb_amber/sander/__init__.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2472 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/sander/common.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    29424 2023-04-12 08:27:46.000000 biobb_amber-4.1.0/biobb_amber/sander/sander_mdrun.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-09-06 08:37:55.315373 biobb_amber-4.1.0/biobb_amber.egg-info/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      977 2023-09-06 08:37:55.000000 biobb_amber-4.1.0/biobb_amber.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1475 2023-09-06 08:37:55.000000 biobb_amber-4.1.0/biobb_amber.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-09-06 08:37:55.000000 biobb_amber-4.1.0/biobb_amber.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      954 2023-09-06 08:37:55.000000 biobb_amber-4.1.0/biobb_amber.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2023-09-06 08:37:55.000000 biobb_amber-4.1.0/biobb_amber.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       12 2023-09-06 08:37:55.000000 biobb_amber-4.1.0/biobb_amber.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-09-06 08:37:55.320590 biobb_amber-4.1.0/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2515 2023-09-06 08:28:38.000000 biobb_amber-4.1.0/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 07:40:14.239162 biobb_amber-4.2.0/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573    11357 2022-05-26 11:32:14.000000 biobb_amber-4.2.0/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1012 2024-05-24 07:40:14.238884 biobb_amber-4.2.0/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     5854 2024-05-24 07:39:24.000000 biobb_amber-4.2.0/README.md
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 07:40:14.232351 biobb_amber-4.2.0/biobb_amber/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      155 2024-05-24 07:39:02.000000 biobb_amber-4.2.0/biobb_amber/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 07:40:14.233816 biobb_amber-4.2.0/biobb_amber/ambpdb/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       43 2022-05-26 11:32:14.000000 biobb_amber-4.2.0/biobb_amber/ambpdb/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7407 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/ambpdb/amber_to_pdb.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1898 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/ambpdb/common.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 07:40:14.234465 biobb_amber-4.2.0/biobb_amber/cphstats/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       60 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/cphstats/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17622 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/cphstats/cestats_run.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     2327 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/cphstats/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17574 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/cphstats/cphstats_run.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 07:40:14.234917 biobb_amber-4.2.0/biobb_amber/cpptraj/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       54 2022-05-26 11:32:14.000000 biobb_amber-4.2.0/biobb_amber/cpptraj/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1968 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/cpptraj/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11027 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/cpptraj/cpptraj_randomize_ions.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 07:40:14.235780 biobb_amber-4.2.0/biobb_amber/leap/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      105 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/leap/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     2144 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/leap/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    26378 2023-06-08 07:37:01.000000 biobb_amber-4.2.0/biobb_amber/leap/leap_add_ions.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     8046 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/leap/leap_build_linear_structure.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    16671 2023-06-08 07:49:29.000000 biobb_amber-4.2.0/biobb_amber/leap/leap_gen_top.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    21736 2023-06-08 07:49:46.000000 biobb_amber-4.2.0/biobb_amber/leap/leap_solvate.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 07:40:14.236169 biobb_amber-4.2.0/biobb_amber/nab/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       51 2022-05-26 11:32:14.000000 biobb_amber-4.2.0/biobb_amber/nab/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1769 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/nab/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     8722 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/nab/nab_build_dna_structure.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 07:40:14.236704 biobb_amber-4.2.0/biobb_amber/parmed/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       73 2022-05-26 11:32:14.000000 biobb_amber-4.2.0/biobb_amber/parmed/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1887 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/parmed/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9081 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/parmed/parmed_cpinutil.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7633 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/parmed/parmed_hmassrepartition.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 07:40:14.237083 biobb_amber-4.2.0/biobb_amber/pdb4amber/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       47 2022-05-26 11:32:14.000000 biobb_amber-4.2.0/biobb_amber/pdb4amber/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1810 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/pdb4amber/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7603 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/pdb4amber/pdb4amber_run.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 07:40:14.237536 biobb_amber-4.2.0/biobb_amber/pmemd/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       41 2022-05-26 11:32:14.000000 biobb_amber-4.2.0/biobb_amber/pmemd/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     2414 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/pmemd/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    25615 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/pmemd/pmemd_mdrun.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 07:40:14.238154 biobb_amber-4.2.0/biobb_amber/process/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       63 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/process/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1841 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/process/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9046 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/process/process_mdout.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9149 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/process/process_minout.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 07:40:14.238537 biobb_amber-4.2.0/biobb_amber/sander/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       43 2022-05-26 11:32:14.000000 biobb_amber-4.2.0/biobb_amber/sander/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     2472 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/sander/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    29424 2023-04-12 08:27:46.000000 biobb_amber-4.2.0/biobb_amber/sander/sander_mdrun.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 07:40:14.233404 biobb_amber-4.2.0/biobb_amber.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1012 2024-05-24 07:40:14.000000 biobb_amber-4.2.0/biobb_amber.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1475 2024-05-24 07:40:14.000000 biobb_amber-4.2.0/biobb_amber.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2024-05-24 07:40:14.000000 biobb_amber-4.2.0/biobb_amber.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      954 2024-05-24 07:40:14.000000 biobb_amber-4.2.0/biobb_amber.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       20 2024-05-24 07:40:14.000000 biobb_amber-4.2.0/biobb_amber.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       12 2024-05-24 07:40:14.000000 biobb_amber-4.2.0/biobb_amber.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2024-05-24 07:40:14.239216 biobb_amber-4.2.0/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     2515 2024-05-24 07:38:52.000000 biobb_amber-4.2.0/setup.py
```

### Comparing `biobb_amber-4.1.0/LICENSE` & `biobb_amber-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/PKG-INFO` & `biobb_amber-4.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: biobb_amber
-Version: 4.1.0
+Version: 4.2.0
 Summary: Biobb_amber is a BioBB category for AMBER MD package.
 Home-page: https://github.com/bioexcel/biobb_amber
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
-Project-URL: Documentation, http://biobb_amber.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-amber.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility MD Amber
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: biobb_common==4.2.0
 
 Biobb_amber allows setup and simulation of atomistic MD simulations using AMBER MD package and its associated AMBER tools.
```

### Comparing `biobb_amber-4.1.0/README.md` & `biobb_amber-4.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_amber?label=Version)](https://GitHub.com/bioexcel/biobb_amber/tags/)
 [![](https://img.shields.io/pypi/v/biobb-amber.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-amber/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_amber?label=Conda)](https://anaconda.org/bioconda/biobb_amber)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_amber?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_amber)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_amber?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_amber:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_amber:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_amber)
 [![](https://img.shields.io/pypi/pyversions/biobb-amber.svg?label=Python%20Versions)](https://pypi.org/project/biobb-amber/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_amber)
 
 [![](https://readthedocs.org/projects/biobb-amber/badge/?version=latest&label=Docs)](https://biobb-amber.readthedocs.io/en/latest/?badge=latest)
@@ -18,86 +18,93 @@
 
 [![](https://docs.bioexcel.eu/biobb_amber/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_amber/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_amber/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_amber/coverage/)
 [![](https://docs.bioexcel.eu/biobb_amber/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_amber/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_amber?label=Last%20Commit)](https://github.com/bioexcel/biobb_amber/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_amber.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_amber/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_amber
 
 ### Introduction
 biobb_amber is a BioBB category for AMBER MD package.
 biobb_amber allows setup and simulation of atomistic MD simulations using AMBER MD package and its associated AMBER tools.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_amber.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-amber.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.3
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
 
-        pip install "biobb_amber>=4.1.0"
+        pip install "biobb_amber>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-amber.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_amber>=4.1.0"
+        conda install -c bioconda "biobb_amber>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-amber.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-amber.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_amber:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_amber:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_amber:4.1.0--pyhdfd78af_0
+        docker run quay.io/biocontainers/biobb_amber:4.2.0--pyhdfd78af_0
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_amber.sif https://depot.galaxyproject.org/singularity/biobb_amber:4.1.0--pyhdfd78af_0
+        singularity pull --name biobb_amber.sif https://depot.galaxyproject.org/singularity/biobb_amber:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_amber.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-amber.readthedocs.io/en/latest/command_line.html).
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_amber-4.1.0/biobb_amber/ambpdb/amber_to_pdb.py` & `biobb_amber-4.2.0/biobb_amber/ambpdb/amber_to_pdb.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/ambpdb/common.py` & `biobb_amber-4.2.0/biobb_amber/ambpdb/common.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/cphstats/cestats_run.py` & `biobb_amber-4.2.0/biobb_amber/cphstats/cestats_run.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/cphstats/common.py` & `biobb_amber-4.2.0/biobb_amber/cphstats/common.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/cphstats/cphstats_run.py` & `biobb_amber-4.2.0/biobb_amber/cphstats/cphstats_run.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/cpptraj/common.py` & `biobb_amber-4.2.0/biobb_amber/cpptraj/common.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/cpptraj/cpptraj_randomize_ions.py` & `biobb_amber-4.2.0/biobb_amber/cpptraj/cpptraj_randomize_ions.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/leap/common.py` & `biobb_amber-4.2.0/biobb_amber/leap/common.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/leap/leap_add_ions.py` & `biobb_amber-4.2.0/biobb_amber/leap/leap_add_ions.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/leap/leap_build_linear_structure.py` & `biobb_amber-4.2.0/biobb_amber/leap/leap_build_linear_structure.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/leap/leap_gen_top.py` & `biobb_amber-4.2.0/biobb_amber/leap/leap_gen_top.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/leap/leap_solvate.py` & `biobb_amber-4.2.0/biobb_amber/leap/leap_solvate.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/nab/common.py` & `biobb_amber-4.2.0/biobb_amber/nab/common.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/nab/nab_build_dna_structure.py` & `biobb_amber-4.2.0/biobb_amber/nab/nab_build_dna_structure.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/parmed/common.py` & `biobb_amber-4.2.0/biobb_amber/parmed/common.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/parmed/parmed_cpinutil.py` & `biobb_amber-4.2.0/biobb_amber/parmed/parmed_cpinutil.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/parmed/parmed_hmassrepartition.py` & `biobb_amber-4.2.0/biobb_amber/parmed/parmed_hmassrepartition.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/pdb4amber/common.py` & `biobb_amber-4.2.0/biobb_amber/pdb4amber/common.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/pdb4amber/pdb4amber_run.py` & `biobb_amber-4.2.0/biobb_amber/pdb4amber/pdb4amber_run.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/pmemd/common.py` & `biobb_amber-4.2.0/biobb_amber/pmemd/common.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/pmemd/pmemd_mdrun.py` & `biobb_amber-4.2.0/biobb_amber/pmemd/pmemd_mdrun.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/process/common.py` & `biobb_amber-4.2.0/biobb_amber/process/common.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/process/process_mdout.py` & `biobb_amber-4.2.0/biobb_amber/process/process_mdout.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/process/process_minout.py` & `biobb_amber-4.2.0/biobb_amber/process/process_minout.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/sander/common.py` & `biobb_amber-4.2.0/biobb_amber/sander/common.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber/sander/sander_mdrun.py` & `biobb_amber-4.2.0/biobb_amber/sander/sander_mdrun.py`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber.egg-info/PKG-INFO` & `biobb_amber-4.2.0/biobb_amber.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: biobb-amber
-Version: 4.1.0
+Version: 4.2.0
 Summary: Biobb_amber is a BioBB category for AMBER MD package.
 Home-page: https://github.com/bioexcel/biobb_amber
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
-Project-URL: Documentation, http://biobb_amber.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-amber.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility MD Amber
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: biobb_common==4.2.0
 
 Biobb_amber allows setup and simulation of atomistic MD simulations using AMBER MD package and its associated AMBER tools.
```

### Comparing `biobb_amber-4.1.0/biobb_amber.egg-info/SOURCES.txt` & `biobb_amber-4.2.0/biobb_amber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/biobb_amber.egg-info/entry_points.txt` & `biobb_amber-4.2.0/biobb_amber.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `biobb_amber-4.1.0/setup.py` & `biobb_amber-4.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_amber",
-    version="4.1.0",
+    version="4.2.0",
     author="Biobb developers",
     author_email="adam.hospital@irbbarcelona.org",
     description="Biobb_amber is a BioBB category for AMBER MD package.",
     long_description="Biobb_amber allows setup and simulation of atomistic MD simulations using AMBER MD package and its associated AMBER tools.",
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility MD Amber",
     url="https://github.com/bioexcel/biobb_amber",
     project_urls={
-        "Documentation": "http://biobb_amber.readthedocs.io/en/latest/",
+        "Documentation": "http://biobb-amber.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
-    install_requires=['biobb_common==4.1.0'],
+    install_requires=['biobb_common==4.2.0'],
     python_requires='>=3.8',
     entry_points={
         "console_scripts": [
             "amber_to_pdb = biobb_amber.ambpdb.amber_to_pdb:main",
             "cestats_run = biobb_amber.cphstats.cestats_run:main",
             "cphstats_run = biobb_amber.cphstats.cphstats_run:main",
             "cpptraj_randomize_ions = biobb_amber.cpptraj.cpptraj_randomize_ions:main",
```

