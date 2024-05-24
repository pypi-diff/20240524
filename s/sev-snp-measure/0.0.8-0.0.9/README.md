# Comparing `tmp/sev-snp-measure-0.0.8.tar.gz` & `tmp/sev-snp-measure-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sev-snp-measure-0.0.8.tar", last modified: Thu Feb  1 22:04:34 2024, max compression
+gzip compressed data, was "sev-snp-measure-0.0.9.tar", last modified: Fri Feb  9 15:24:42 2024, max compression
```

## Comparing `sev-snp-measure-0.0.8.tar` & `sev-snp-measure-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 dovmurik   (502) staff       (20)        0 2024-02-01 22:04:34.684548 sev-snp-measure-0.0.8/
--rw-r--r--   0 dovmurik   (502) staff       (20)    11358 2023-09-13 01:50:22.000000 sev-snp-measure-0.0.8/LICENSE
--rw-r--r--   0 dovmurik   (502) staff       (20)     7918 2024-02-01 22:04:34.684421 sev-snp-measure-0.0.8/PKG-INFO
--rw-r--r--   0 dovmurik   (502) staff       (20)     7088 2024-02-01 21:46:32.000000 sev-snp-measure-0.0.8/README.md
--rw-r--r--   0 dovmurik   (502) staff       (20)       85 2023-09-13 01:50:22.000000 sev-snp-measure-0.0.8/pyproject.toml
--rw-r--r--   0 dovmurik   (502) staff       (20)     1040 2024-02-01 22:04:34.684845 sev-snp-measure-0.0.8/setup.cfg
-drwxr-xr-x   0 dovmurik   (502) staff       (20)        0 2024-02-01 22:04:34.684066 sev-snp-measure-0.0.8/sev_snp_measure.egg-info/
--rw-r--r--   0 dovmurik   (502) staff       (20)     7918 2024-02-01 22:04:34.000000 sev-snp-measure-0.0.8/sev_snp_measure.egg-info/PKG-INFO
--rw-r--r--   0 dovmurik   (502) staff       (20)      640 2024-02-01 22:04:34.000000 sev-snp-measure-0.0.8/sev_snp_measure.egg-info/SOURCES.txt
--rw-r--r--   0 dovmurik   (502) staff       (20)        1 2024-02-01 22:04:34.000000 sev-snp-measure-0.0.8/sev_snp_measure.egg-info/dependency_links.txt
--rw-r--r--   0 dovmurik   (502) staff       (20)      109 2024-02-01 22:04:34.000000 sev-snp-measure-0.0.8/sev_snp_measure.egg-info/entry_points.txt
--rw-r--r--   0 dovmurik   (502) staff       (20)       40 2024-02-01 22:04:34.000000 sev-snp-measure-0.0.8/sev_snp_measure.egg-info/requires.txt
--rw-r--r--   0 dovmurik   (502) staff       (20)       14 2024-02-01 22:04:34.000000 sev-snp-measure-0.0.8/sev_snp_measure.egg-info/top_level.txt
-drwxr-xr-x   0 dovmurik   (502) staff       (20)        0 2024-02-01 22:04:34.681732 sev-snp-measure-0.0.8/sevsnpmeasure/
--rw-r--r--   0 dovmurik   (502) staff       (20)       89 2023-09-13 01:50:22.000000 sev-snp-measure-0.0.8/sevsnpmeasure/__init__.py
--rw-r--r--   0 dovmurik   (502) staff       (20)     5222 2024-02-01 21:47:23.000000 sev-snp-measure-0.0.8/sevsnpmeasure/cli.py
--rw-r--r--   0 dovmurik   (502) staff       (20)     2462 2023-09-13 01:50:22.000000 sev-snp-measure-0.0.8/sevsnpmeasure/gctx.py
--rw-r--r--   0 dovmurik   (502) staff       (20)     6777 2024-02-01 21:46:32.000000 sev-snp-measure-0.0.8/sevsnpmeasure/guest.py
--rw-r--r--   0 dovmurik   (502) staff       (20)     5813 2023-12-08 14:28:12.000000 sev-snp-measure-0.0.8/sevsnpmeasure/id_block.py
--rw-r--r--   0 dovmurik   (502) staff       (20)     5748 2024-01-23 18:25:34.000000 sev-snp-measure-0.0.8/sevsnpmeasure/ovmf.py
--rw-r--r--   0 dovmurik   (502) staff       (20)     3488 2023-09-13 01:50:22.000000 sev-snp-measure-0.0.8/sevsnpmeasure/sev_hashes.py
--rw-r--r--   0 dovmurik   (502) staff       (20)      727 2024-01-23 18:25:34.000000 sev-snp-measure-0.0.8/sevsnpmeasure/sev_mode.py
--rw-r--r--   0 dovmurik   (502) staff       (20)     1732 2023-09-13 01:50:22.000000 sev-snp-measure-0.0.8/sevsnpmeasure/vcpu_types.py
--rw-r--r--   0 dovmurik   (502) staff       (20)       70 2023-09-13 01:50:22.000000 sev-snp-measure-0.0.8/sevsnpmeasure/vmm_types.py
--rw-r--r--   0 dovmurik   (502) staff       (20)     7735 2024-02-01 21:46:32.000000 sev-snp-measure-0.0.8/sevsnpmeasure/vmsa.py
-drwxr-xr-x   0 dovmurik   (502) staff       (20)        0 2024-02-01 22:04:34.683570 sev-snp-measure-0.0.8/tests/
--rw-r--r--   0 dovmurik   (502) staff       (20)    12839 2024-02-01 21:46:32.000000 sev-snp-measure-0.0.8/tests/test_guest.py
--rw-r--r--   0 dovmurik   (502) staff       (20)     1203 2023-12-08 14:28:12.000000 sev-snp-measure-0.0.8/tests/test_id_block.py
--rw-r--r--   0 dovmurik   (502) staff       (20)     1264 2024-01-23 18:25:34.000000 sev-snp-measure-0.0.8/tests/test_sev_mode.py
--rw-r--r--   0 dovmurik   (502) staff       (20)      480 2023-09-13 01:50:22.000000 sev-snp-measure-0.0.8/tests/test_vcpu_types.py
+drwxr-xr-x   0 dovmurik   (502) staff       (20)        0 2024-02-09 15:24:42.995343 sev-snp-measure-0.0.9/
+-rw-r--r--   0 dovmurik   (502) staff       (20)    11358 2023-09-13 01:50:22.000000 sev-snp-measure-0.0.9/LICENSE
+-rw-r--r--   0 dovmurik   (502) staff       (20)     9588 2024-02-09 15:24:42.995203 sev-snp-measure-0.0.9/PKG-INFO
+-rw-r--r--   0 dovmurik   (502) staff       (20)     8758 2024-02-06 14:29:10.000000 sev-snp-measure-0.0.9/README.md
+-rw-r--r--   0 dovmurik   (502) staff       (20)       85 2023-09-13 01:50:22.000000 sev-snp-measure-0.0.9/pyproject.toml
+-rw-r--r--   0 dovmurik   (502) staff       (20)     1040 2024-02-09 15:24:42.995633 sev-snp-measure-0.0.9/setup.cfg
+drwxr-xr-x   0 dovmurik   (502) staff       (20)        0 2024-02-09 15:24:42.994825 sev-snp-measure-0.0.9/sev_snp_measure.egg-info/
+-rw-r--r--   0 dovmurik   (502) staff       (20)     9588 2024-02-09 15:24:42.000000 sev-snp-measure-0.0.9/sev_snp_measure.egg-info/PKG-INFO
+-rw-r--r--   0 dovmurik   (502) staff       (20)      640 2024-02-09 15:24:42.000000 sev-snp-measure-0.0.9/sev_snp_measure.egg-info/SOURCES.txt
+-rw-r--r--   0 dovmurik   (502) staff       (20)        1 2024-02-09 15:24:42.000000 sev-snp-measure-0.0.9/sev_snp_measure.egg-info/dependency_links.txt
+-rw-r--r--   0 dovmurik   (502) staff       (20)      109 2024-02-09 15:24:42.000000 sev-snp-measure-0.0.9/sev_snp_measure.egg-info/entry_points.txt
+-rw-r--r--   0 dovmurik   (502) staff       (20)       40 2024-02-09 15:24:42.000000 sev-snp-measure-0.0.9/sev_snp_measure.egg-info/requires.txt
+-rw-r--r--   0 dovmurik   (502) staff       (20)       14 2024-02-09 15:24:42.000000 sev-snp-measure-0.0.9/sev_snp_measure.egg-info/top_level.txt
+drwxr-xr-x   0 dovmurik   (502) staff       (20)        0 2024-02-09 15:24:42.992692 sev-snp-measure-0.0.9/sevsnpmeasure/
+-rw-r--r--   0 dovmurik   (502) staff       (20)       89 2023-09-13 01:50:22.000000 sev-snp-measure-0.0.9/sevsnpmeasure/__init__.py
+-rw-r--r--   0 dovmurik   (502) staff       (20)     6606 2024-02-09 15:20:23.000000 sev-snp-measure-0.0.9/sevsnpmeasure/cli.py
+-rw-r--r--   0 dovmurik   (502) staff       (20)     2462 2023-09-13 01:50:22.000000 sev-snp-measure-0.0.9/sevsnpmeasure/gctx.py
+-rw-r--r--   0 dovmurik   (502) staff       (20)     6856 2024-02-02 02:55:12.000000 sev-snp-measure-0.0.9/sevsnpmeasure/guest.py
+-rw-r--r--   0 dovmurik   (502) staff       (20)     5813 2023-12-08 14:28:12.000000 sev-snp-measure-0.0.9/sevsnpmeasure/id_block.py
+-rw-r--r--   0 dovmurik   (502) staff       (20)     5748 2024-01-23 18:25:34.000000 sev-snp-measure-0.0.9/sevsnpmeasure/ovmf.py
+-rw-r--r--   0 dovmurik   (502) staff       (20)     3488 2023-09-13 01:50:22.000000 sev-snp-measure-0.0.9/sevsnpmeasure/sev_hashes.py
+-rw-r--r--   0 dovmurik   (502) staff       (20)      727 2024-01-23 18:25:34.000000 sev-snp-measure-0.0.9/sevsnpmeasure/sev_mode.py
+-rw-r--r--   0 dovmurik   (502) staff       (20)     1732 2023-09-13 01:50:22.000000 sev-snp-measure-0.0.9/sevsnpmeasure/vcpu_types.py
+-rw-r--r--   0 dovmurik   (502) staff       (20)       70 2023-09-13 01:50:22.000000 sev-snp-measure-0.0.9/sevsnpmeasure/vmm_types.py
+-rw-r--r--   0 dovmurik   (502) staff       (20)     7660 2024-02-02 02:55:12.000000 sev-snp-measure-0.0.9/sevsnpmeasure/vmsa.py
+drwxr-xr-x   0 dovmurik   (502) staff       (20)        0 2024-02-09 15:24:42.994367 sev-snp-measure-0.0.9/tests/
+-rw-r--r--   0 dovmurik   (502) staff       (20)    17710 2024-02-02 02:55:12.000000 sev-snp-measure-0.0.9/tests/test_guest.py
+-rw-r--r--   0 dovmurik   (502) staff       (20)     1203 2023-12-08 14:28:12.000000 sev-snp-measure-0.0.9/tests/test_id_block.py
+-rw-r--r--   0 dovmurik   (502) staff       (20)     1264 2024-01-23 18:25:34.000000 sev-snp-measure-0.0.9/tests/test_sev_mode.py
+-rw-r--r--   0 dovmurik   (502) staff       (20)      480 2023-09-13 01:50:22.000000 sev-snp-measure-0.0.9/tests/test_vcpu_types.py
```

### Comparing `sev-snp-measure-0.0.8/LICENSE` & `sev-snp-measure-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.8/PKG-INFO` & `sev-snp-measure-0.0.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: sev-snp-measure
-Version: 0.0.8
-Summary: Calculate expected measurement of an AMD SEV/SEV-ES/SEV-SNP guest VM for confidential computing
-Home-page: https://github.com/virtee/sev-snp-measure
-Author: Dov Murik
-Author-email: dov.murik@gmail.com
-Project-URL: Bug Tracker, https://github.com/virtee/sev-snp-measure/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Security
-Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: cryptography>=39.0.1
-Requires-Dist: types-cryptography
-
 # sev-snp-measure
 
 ## Scope
 
 Command-line tool and Python library to calculate expected measurement of an
 AMD SEV/SEV-ES/SEV-SNP guest VM for confidential computing.
 
@@ -50,16 +29,17 @@
 ### sev-snp-measure
 ```
 $ sev-snp-measure --help
 usage: sev-snp-measure [-h] [--version] [-v] --mode {sev,seves,snp,snp:ovmf-hash,snp:svsm}
                        [--vcpus N] [--vcpu-type CPUTYPE] [--vcpu-sig VALUE] [--vcpu-family FAMILY]
                        [--vcpu-model MODEL] [--vcpu-stepping STEPPING] [--vmm-type VMMTYPE] --ovmf
                        PATH [--kernel PATH] [--initrd PATH] [--append CMDLINE]
-                       [--output-format {hex,base64}] [--snp-ovmf-hash HASH] [--dump-vmsa]
-                       [--vars-size VARS_SIZE] [--svsm SVSM]
+                       [--guest-features VALUE] [--output-format {hex,base64}]
+                       [--snp-ovmf-hash HASH] [--dump-vmsa] [--svsm PATH]
+                       [--vars-size SIZE | --vars-file PATH]
 
 Calculate AMD SEV/SEV-ES/SEV-SNP guest launch measurement
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose
@@ -75,27 +55,50 @@
   --vcpu-stepping STEPPING
                         Guest vcpu stepping
   --vmm-type VMMTYPE    Type of guest vmm (QEMU, ec2)
   --ovmf PATH           OVMF file to calculate hash from
   --kernel PATH         Kernel file to calculate hash from
   --initrd PATH         Initrd file to calculate hash from (use with --kernel)
   --append CMDLINE      Kernel command line to calculate hash from (use with --kernel)
+  --guest-features VALUE
+                        Hex representation of the guest kernel features expected to be included
+                        (defaults to 0x21); see README.md for possible values
   --output-format {hex,base64}
                         Measurement output format
   --snp-ovmf-hash HASH  Precalculated hash of the OVMF binary (hex string)
   --dump-vmsa           Write measured VMSAs to vmsa<N>.bin (seves, snp, and snp:svsm modes only)
-  --vars-size VARS_SIZE
-                        OVMF_VARS size in bytes (snp:svsm mode only)
-  --svsm SVSM           SVSM binary (snp:svsm mode only)
+
+snp:svsm Mode:
+  AMD SEV-SNP with Coconut-SVSM. This mode additionally requires --svsm and either --vars-file
+  or --vars-size to be set.
+
+  --svsm PATH           SVSM binary
+  --vars-size SIZE      Size of the OVMF_VARS file in bytes (conflicts with --vars-file)
+  --vars-file PATH      OVMF_VARS file (conflicts with --vars-size)
 ```
 
-For example:
+### Example: SNP mode
+
+```
+$ sev-snp-measure --mode snp --vcpus=1 --vcpu-type=EPYC-v4 --ovmf=OVMF.fd --kernel=vmlinuz --initrd=initrd.img --append="console=ttyS0 loglevel=7"
+1c8bf2f320add50cb22ca824c17f3fa51a7a4296a4a3113698c2e31b50c2dcfa7e36dea3ebc3a9411061c30acffc6d5a
+```
 
-    $ sev-snp-measure --mode snp --vcpus=1 --vcpu-type=EPYC-v4 --ovmf=OVMF.fd --kernel=vmlinuz --initrd=initrd.img --append="console=ttyS0 loglevel=7"
-    1c8bf2f320add50cb22ca824c17f3fa51a7a4296a4a3113698c2e31b50c2dcfa7e36dea3ebc3a9411061c30acffc6d5a
+### Example: SNP:SVSM mode
+
+```
+$ sev-snp-measure \
+    --mode snp:svsm \
+    --vmm-type=QEMU \
+    --vcpus=4 \
+    --vcpu-type=EPYC-v4 \
+    --ovmf=OVMF_CODE.fd \
+    --svsm=svsm.bin --vars-file=OVMF_VARS.fd
+3447e476b226e317890a350003b56ee17becb48d1dc25dd6b5819a1192df3238f50cda0f0216bd5ae2a992ad7ab961c4
+```
 
 ### snp-create-id-block
 ```
 $ snp-create-id-block --help
 usage: snp-create-id-block [-h] [--measurement VALUE] [--idkey PATH] [--authorkey PATH]
 
 Calculate AMD SEV-SNP guest id block
@@ -114,15 +117,15 @@
 
 ```python3
 from sevsnpmeasure import guest,id_block
 from sevsnpmeasure import vcpu_types
 from sevsnpmeasure.sev_mode import SevMode
 
 ld = guest.calc_launch_digest(SevMode.SEV_SNP, vcpus_num, vcpu_types.CPU_SIGS["EPYC-v4"],
-                              ovmf_path, kernel_path, initrd_path, cmdline_str)
+                              ovmf_path, kernel_path, initrd_path, cmdline_str, guest_features)
 print("Calculated measurement:", ld.hex())
 
 block = id_block.snp_calc_id_block(ld,"id_key_file","author_key_file")
 print("Calculated id block in base64", block)
 ```
 
 ## Choosing guest CPU type
@@ -136,14 +139,38 @@
 combination of `--vcpu-family`, `--vcpu-model`, and `--vcpu-stepping`. For
 example, the following 3 invocations are identical:
 
 1. `sev-snp-measure --vcpu-type=EPYC-v4 ...`
 2. `sev-snp-measure --vcpu-sig=0x800f12 ...`
 3. `sev-snp-measure --vcpu-family=23 --vcpu-model=1 --vcpu-stepping=2 ...`
 
+## SEV-SNP Guest Feature Field Values
+Prior to Linux Kernel version 6.6, the default value was always calculated to `0x1`, as the kernel only supported `SNPActive`. After the release of Linux Kernel 6.6, additional features were made available some of them enabled by default. Because of this, the new default value is `0x21` which is `SNPActive + DebugSwap`. Other possible combinations my be derived by generating a 64-bit hex value from the following chart:
+
+| BIT FIELD | Description |
+|:---------:|:------------:|
+| 0 | SNPActive |
+| 1 | vTOM |
+| 2 | ReflectVC |
+| 3 | RestrictedInjection |
+| 4 | AlternateInjection |
+| 5 | DebugSwap |
+| 6 | PreventHostIBS |
+| 7 | BTBIsolation |
+| 8 | VmplSSS |
+| 9 | SecureTSC |
+| 10 | VmgexitParameter |
+| 11 | Reserved, SBZ |
+| 12 | IbsVirtualization |
+| 13 | Reserved, SBZ |
+| 14 | VmsaRegProt |
+| 15 | SmtProtection |
+| 63:16 | Reserved, SBZ |
+
+
 ## Precalculated OVMF hashes
 
 The SEV-SNP digest gets generated in multiple steps that each have a digest as output. With that digest output, you can stop at any of these steps and continue generation of the full digest later. These are the steps:
 
 1. OVMF
 2. (optional) -kernel, -initrd, -append arguments
 3. Initial state of all vCPUs
```

### Comparing `sev-snp-measure-0.0.8/README.md` & `sev-snp-measure-0.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: sev-snp-measure
+Version: 0.0.9
+Summary: Calculate expected measurement of an AMD SEV/SEV-ES/SEV-SNP guest VM for confidential computing
+Home-page: https://github.com/virtee/sev-snp-measure
+Author: Dov Murik
+Author-email: dov.murik@gmail.com
+Project-URL: Bug Tracker, https://github.com/virtee/sev-snp-measure/issues
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Security
+Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cryptography>=39.0.1
+Requires-Dist: types-cryptography
+
 # sev-snp-measure
 
 ## Scope
 
 Command-line tool and Python library to calculate expected measurement of an
 AMD SEV/SEV-ES/SEV-SNP guest VM for confidential computing.
 
@@ -29,16 +50,17 @@
 ### sev-snp-measure
 ```
 $ sev-snp-measure --help
 usage: sev-snp-measure [-h] [--version] [-v] --mode {sev,seves,snp,snp:ovmf-hash,snp:svsm}
                        [--vcpus N] [--vcpu-type CPUTYPE] [--vcpu-sig VALUE] [--vcpu-family FAMILY]
                        [--vcpu-model MODEL] [--vcpu-stepping STEPPING] [--vmm-type VMMTYPE] --ovmf
                        PATH [--kernel PATH] [--initrd PATH] [--append CMDLINE]
-                       [--output-format {hex,base64}] [--snp-ovmf-hash HASH] [--dump-vmsa]
-                       [--vars-size VARS_SIZE] [--svsm SVSM]
+                       [--guest-features VALUE] [--output-format {hex,base64}]
+                       [--snp-ovmf-hash HASH] [--dump-vmsa] [--svsm PATH]
+                       [--vars-size SIZE | --vars-file PATH]
 
 Calculate AMD SEV/SEV-ES/SEV-SNP guest launch measurement
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose
@@ -54,27 +76,50 @@
   --vcpu-stepping STEPPING
                         Guest vcpu stepping
   --vmm-type VMMTYPE    Type of guest vmm (QEMU, ec2)
   --ovmf PATH           OVMF file to calculate hash from
   --kernel PATH         Kernel file to calculate hash from
   --initrd PATH         Initrd file to calculate hash from (use with --kernel)
   --append CMDLINE      Kernel command line to calculate hash from (use with --kernel)
+  --guest-features VALUE
+                        Hex representation of the guest kernel features expected to be included
+                        (defaults to 0x21); see README.md for possible values
   --output-format {hex,base64}
                         Measurement output format
   --snp-ovmf-hash HASH  Precalculated hash of the OVMF binary (hex string)
   --dump-vmsa           Write measured VMSAs to vmsa<N>.bin (seves, snp, and snp:svsm modes only)
-  --vars-size VARS_SIZE
-                        OVMF_VARS size in bytes (snp:svsm mode only)
-  --svsm SVSM           SVSM binary (snp:svsm mode only)
+
+snp:svsm Mode:
+  AMD SEV-SNP with Coconut-SVSM. This mode additionally requires --svsm and either --vars-file
+  or --vars-size to be set.
+
+  --svsm PATH           SVSM binary
+  --vars-size SIZE      Size of the OVMF_VARS file in bytes (conflicts with --vars-file)
+  --vars-file PATH      OVMF_VARS file (conflicts with --vars-size)
 ```
 
-For example:
+### Example: SNP mode
+
+```
+$ sev-snp-measure --mode snp --vcpus=1 --vcpu-type=EPYC-v4 --ovmf=OVMF.fd --kernel=vmlinuz --initrd=initrd.img --append="console=ttyS0 loglevel=7"
+1c8bf2f320add50cb22ca824c17f3fa51a7a4296a4a3113698c2e31b50c2dcfa7e36dea3ebc3a9411061c30acffc6d5a
+```
 
-    $ sev-snp-measure --mode snp --vcpus=1 --vcpu-type=EPYC-v4 --ovmf=OVMF.fd --kernel=vmlinuz --initrd=initrd.img --append="console=ttyS0 loglevel=7"
-    1c8bf2f320add50cb22ca824c17f3fa51a7a4296a4a3113698c2e31b50c2dcfa7e36dea3ebc3a9411061c30acffc6d5a
+### Example: SNP:SVSM mode
+
+```
+$ sev-snp-measure \
+    --mode snp:svsm \
+    --vmm-type=QEMU \
+    --vcpus=4 \
+    --vcpu-type=EPYC-v4 \
+    --ovmf=OVMF_CODE.fd \
+    --svsm=svsm.bin --vars-file=OVMF_VARS.fd
+3447e476b226e317890a350003b56ee17becb48d1dc25dd6b5819a1192df3238f50cda0f0216bd5ae2a992ad7ab961c4
+```
 
 ### snp-create-id-block
 ```
 $ snp-create-id-block --help
 usage: snp-create-id-block [-h] [--measurement VALUE] [--idkey PATH] [--authorkey PATH]
 
 Calculate AMD SEV-SNP guest id block
@@ -93,15 +138,15 @@
 
 ```python3
 from sevsnpmeasure import guest,id_block
 from sevsnpmeasure import vcpu_types
 from sevsnpmeasure.sev_mode import SevMode
 
 ld = guest.calc_launch_digest(SevMode.SEV_SNP, vcpus_num, vcpu_types.CPU_SIGS["EPYC-v4"],
-                              ovmf_path, kernel_path, initrd_path, cmdline_str)
+                              ovmf_path, kernel_path, initrd_path, cmdline_str, guest_features)
 print("Calculated measurement:", ld.hex())
 
 block = id_block.snp_calc_id_block(ld,"id_key_file","author_key_file")
 print("Calculated id block in base64", block)
 ```
 
 ## Choosing guest CPU type
@@ -115,14 +160,38 @@
 combination of `--vcpu-family`, `--vcpu-model`, and `--vcpu-stepping`. For
 example, the following 3 invocations are identical:
 
 1. `sev-snp-measure --vcpu-type=EPYC-v4 ...`
 2. `sev-snp-measure --vcpu-sig=0x800f12 ...`
 3. `sev-snp-measure --vcpu-family=23 --vcpu-model=1 --vcpu-stepping=2 ...`
 
+## SEV-SNP Guest Feature Field Values
+Prior to Linux Kernel version 6.6, the default value was always calculated to `0x1`, as the kernel only supported `SNPActive`. After the release of Linux Kernel 6.6, additional features were made available some of them enabled by default. Because of this, the new default value is `0x21` which is `SNPActive + DebugSwap`. Other possible combinations my be derived by generating a 64-bit hex value from the following chart:
+
+| BIT FIELD | Description |
+|:---------:|:------------:|
+| 0 | SNPActive |
+| 1 | vTOM |
+| 2 | ReflectVC |
+| 3 | RestrictedInjection |
+| 4 | AlternateInjection |
+| 5 | DebugSwap |
+| 6 | PreventHostIBS |
+| 7 | BTBIsolation |
+| 8 | VmplSSS |
+| 9 | SecureTSC |
+| 10 | VmgexitParameter |
+| 11 | Reserved, SBZ |
+| 12 | IbsVirtualization |
+| 13 | Reserved, SBZ |
+| 14 | VmsaRegProt |
+| 15 | SmtProtection |
+| 63:16 | Reserved, SBZ |
+
+
 ## Precalculated OVMF hashes
 
 The SEV-SNP digest gets generated in multiple steps that each have a digest as output. With that digest output, you can stop at any of these steps and continue generation of the full digest later. These are the steps:
 
 1. OVMF
 2. (optional) -kernel, -initrd, -append arguments
 3. Initial state of all vCPUs
```

### Comparing `sev-snp-measure-0.0.8/setup.cfg` & `sev-snp-measure-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sev-snp-measure
-version = 0.0.8
+version = 0.0.9
 author = Dov Murik
 author_email = dov.murik@gmail.com
 description = Calculate expected measurement of an AMD SEV/SEV-ES/SEV-SNP guest VM for confidential computing
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/virtee/sev-snp-measure
 project_urls = 
@@ -27,14 +27,14 @@
 
 [options.entry_points]
 console_scripts = 
 	sev-snp-measure = sevsnpmeasure.cli:main
 	snp-create-id-block = sevsnpmeasure.id_block:main
 
 [flake8]
-max-complexity = 10
+max-complexity = 12
 max-line-length = 127
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sev-snp-measure-0.0.8/sev_snp_measure.egg-info/PKG-INFO` & `sev-snp-measure-0.0.9/sev_snp_measure.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sev-snp-measure
-Version: 0.0.8
+Version: 0.0.9
 Summary: Calculate expected measurement of an AMD SEV/SEV-ES/SEV-SNP guest VM for confidential computing
 Home-page: https://github.com/virtee/sev-snp-measure
 Author: Dov Murik
 Author-email: dov.murik@gmail.com
 Project-URL: Bug Tracker, https://github.com/virtee/sev-snp-measure/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -50,16 +50,17 @@
 ### sev-snp-measure
 ```
 $ sev-snp-measure --help
 usage: sev-snp-measure [-h] [--version] [-v] --mode {sev,seves,snp,snp:ovmf-hash,snp:svsm}
                        [--vcpus N] [--vcpu-type CPUTYPE] [--vcpu-sig VALUE] [--vcpu-family FAMILY]
                        [--vcpu-model MODEL] [--vcpu-stepping STEPPING] [--vmm-type VMMTYPE] --ovmf
                        PATH [--kernel PATH] [--initrd PATH] [--append CMDLINE]
-                       [--output-format {hex,base64}] [--snp-ovmf-hash HASH] [--dump-vmsa]
-                       [--vars-size VARS_SIZE] [--svsm SVSM]
+                       [--guest-features VALUE] [--output-format {hex,base64}]
+                       [--snp-ovmf-hash HASH] [--dump-vmsa] [--svsm PATH]
+                       [--vars-size SIZE | --vars-file PATH]
 
 Calculate AMD SEV/SEV-ES/SEV-SNP guest launch measurement
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose
@@ -75,27 +76,50 @@
   --vcpu-stepping STEPPING
                         Guest vcpu stepping
   --vmm-type VMMTYPE    Type of guest vmm (QEMU, ec2)
   --ovmf PATH           OVMF file to calculate hash from
   --kernel PATH         Kernel file to calculate hash from
   --initrd PATH         Initrd file to calculate hash from (use with --kernel)
   --append CMDLINE      Kernel command line to calculate hash from (use with --kernel)
+  --guest-features VALUE
+                        Hex representation of the guest kernel features expected to be included
+                        (defaults to 0x21); see README.md for possible values
   --output-format {hex,base64}
                         Measurement output format
   --snp-ovmf-hash HASH  Precalculated hash of the OVMF binary (hex string)
   --dump-vmsa           Write measured VMSAs to vmsa<N>.bin (seves, snp, and snp:svsm modes only)
-  --vars-size VARS_SIZE
-                        OVMF_VARS size in bytes (snp:svsm mode only)
-  --svsm SVSM           SVSM binary (snp:svsm mode only)
+
+snp:svsm Mode:
+  AMD SEV-SNP with Coconut-SVSM. This mode additionally requires --svsm and either --vars-file
+  or --vars-size to be set.
+
+  --svsm PATH           SVSM binary
+  --vars-size SIZE      Size of the OVMF_VARS file in bytes (conflicts with --vars-file)
+  --vars-file PATH      OVMF_VARS file (conflicts with --vars-size)
+```
+
+### Example: SNP mode
+
+```
+$ sev-snp-measure --mode snp --vcpus=1 --vcpu-type=EPYC-v4 --ovmf=OVMF.fd --kernel=vmlinuz --initrd=initrd.img --append="console=ttyS0 loglevel=7"
+1c8bf2f320add50cb22ca824c17f3fa51a7a4296a4a3113698c2e31b50c2dcfa7e36dea3ebc3a9411061c30acffc6d5a
 ```
 
-For example:
+### Example: SNP:SVSM mode
 
-    $ sev-snp-measure --mode snp --vcpus=1 --vcpu-type=EPYC-v4 --ovmf=OVMF.fd --kernel=vmlinuz --initrd=initrd.img --append="console=ttyS0 loglevel=7"
-    1c8bf2f320add50cb22ca824c17f3fa51a7a4296a4a3113698c2e31b50c2dcfa7e36dea3ebc3a9411061c30acffc6d5a
+```
+$ sev-snp-measure \
+    --mode snp:svsm \
+    --vmm-type=QEMU \
+    --vcpus=4 \
+    --vcpu-type=EPYC-v4 \
+    --ovmf=OVMF_CODE.fd \
+    --svsm=svsm.bin --vars-file=OVMF_VARS.fd
+3447e476b226e317890a350003b56ee17becb48d1dc25dd6b5819a1192df3238f50cda0f0216bd5ae2a992ad7ab961c4
+```
 
 ### snp-create-id-block
 ```
 $ snp-create-id-block --help
 usage: snp-create-id-block [-h] [--measurement VALUE] [--idkey PATH] [--authorkey PATH]
 
 Calculate AMD SEV-SNP guest id block
@@ -114,15 +138,15 @@
 
 ```python3
 from sevsnpmeasure import guest,id_block
 from sevsnpmeasure import vcpu_types
 from sevsnpmeasure.sev_mode import SevMode
 
 ld = guest.calc_launch_digest(SevMode.SEV_SNP, vcpus_num, vcpu_types.CPU_SIGS["EPYC-v4"],
-                              ovmf_path, kernel_path, initrd_path, cmdline_str)
+                              ovmf_path, kernel_path, initrd_path, cmdline_str, guest_features)
 print("Calculated measurement:", ld.hex())
 
 block = id_block.snp_calc_id_block(ld,"id_key_file","author_key_file")
 print("Calculated id block in base64", block)
 ```
 
 ## Choosing guest CPU type
@@ -136,14 +160,38 @@
 combination of `--vcpu-family`, `--vcpu-model`, and `--vcpu-stepping`. For
 example, the following 3 invocations are identical:
 
 1. `sev-snp-measure --vcpu-type=EPYC-v4 ...`
 2. `sev-snp-measure --vcpu-sig=0x800f12 ...`
 3. `sev-snp-measure --vcpu-family=23 --vcpu-model=1 --vcpu-stepping=2 ...`
 
+## SEV-SNP Guest Feature Field Values
+Prior to Linux Kernel version 6.6, the default value was always calculated to `0x1`, as the kernel only supported `SNPActive`. After the release of Linux Kernel 6.6, additional features were made available some of them enabled by default. Because of this, the new default value is `0x21` which is `SNPActive + DebugSwap`. Other possible combinations my be derived by generating a 64-bit hex value from the following chart:
+
+| BIT FIELD | Description |
+|:---------:|:------------:|
+| 0 | SNPActive |
+| 1 | vTOM |
+| 2 | ReflectVC |
+| 3 | RestrictedInjection |
+| 4 | AlternateInjection |
+| 5 | DebugSwap |
+| 6 | PreventHostIBS |
+| 7 | BTBIsolation |
+| 8 | VmplSSS |
+| 9 | SecureTSC |
+| 10 | VmgexitParameter |
+| 11 | Reserved, SBZ |
+| 12 | IbsVirtualization |
+| 13 | Reserved, SBZ |
+| 14 | VmsaRegProt |
+| 15 | SmtProtection |
+| 63:16 | Reserved, SBZ |
+
+
 ## Precalculated OVMF hashes
 
 The SEV-SNP digest gets generated in multiple steps that each have a digest as output. With that digest output, you can stop at any of these steps and continue generation of the full digest later. These are the steps:
 
 1. OVMF
 2. (optional) -kernel, -initrd, -append arguments
 3. Initial state of all vCPUs
```

### Comparing `sev-snp-measure-0.0.8/sev_snp_measure.egg-info/SOURCES.txt` & `sev-snp-measure-0.0.9/sev_snp_measure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.8/sevsnpmeasure/cli.py` & `sev-snp-measure-0.0.9/sevsnpmeasure/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 # Copyright 2022- IBM Inc. All rights reserved
 # SPDX-License-Identifier: Apache-2.0
 #
 
 import argparse
 import base64
 import sys
+import pathlib
 
 from sevsnpmeasure import guest
 from sevsnpmeasure import vcpu_types
 from sevsnpmeasure import vmm_types
 from .sev_mode import SevMode
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 
 
 def auto_base_int(s: str) -> int:
     return int(s, 0)
 
 
 def print_measurement(ld: bytes, sev_mode: SevMode, output_format: str, verbose: bool):
@@ -65,20 +66,33 @@
                         help='OVMF file to calculate hash from', required=True)
     parser.add_argument('--kernel', metavar='PATH',
                         help='Kernel file to calculate hash from')
     parser.add_argument('--initrd', metavar='PATH',
                         help='Initrd file to calculate hash from (use with --kernel)')
     parser.add_argument('--append', metavar='CMDLINE',
                         help='Kernel command line to calculate hash from (use with --kernel)')
+    parser.add_argument('--guest-features', metavar='VALUE', type=lambda x: int(x, 0),
+                        default=0x21,
+                        help="Hex representation of the guest kernel features expected to be included "
+                             "(defaults to 0x21); see README.md for possible values"),
     parser.add_argument('--output-format', choices=['hex', 'base64'], help='Measurement output format', default='hex')
     parser.add_argument('--snp-ovmf-hash', metavar='HASH', help='Precalculated hash of the OVMF binary (hex string)')
     parser.add_argument('--dump-vmsa', action='store_true',
                         help='Write measured VMSAs to vmsa<N>.bin (seves, snp, and snp:svsm modes only)')
-    parser.add_argument('--vars-size', type=int, help='OVMF_VARS size in bytes (snp:svsm mode only)')
-    parser.add_argument('--svsm', type=str, help='SVSM binary (snp:svsm mode only)')
+
+    arg_group_svsm = parser.add_argument_group(title='snp:svsm Mode',
+                                               description='AMD SEV-SNP with Coconut-SVSM. This mode additionally requires '
+                                               '--svsm and either --vars-file or --vars-size to be set.')
+    arg_group_svsm.add_argument('--svsm', type=str, metavar='PATH', help='SVSM binary')
+    arg_group_ovmf_vars = arg_group_svsm.add_mutually_exclusive_group(required=False)
+    arg_group_ovmf_vars.add_argument('--vars-size', type=int, metavar='SIZE', help='Size of the OVMF_VARS file in bytes '
+                                     '(conflicts with --vars-file)')
+    arg_group_ovmf_vars.add_argument('--vars-file', type=str, metavar='PATH', help='OVMF_VARS file '
+                                     '(conflicts with --vars-size)')
+
     args = parser.parse_args()
 
     if args.mode == 'snp:ovmf-hash':
         print(guest.calc_snp_ovmf_hash(args.ovmf).hex())
         return 0
 
     if args.initrd and args.kernel is None:
@@ -94,21 +108,32 @@
         vmm_type = vmm_types.VMMType[args.vmm_type]
     else:
         parser.error(f"unknown VMM type '{args.vmm_type}'")
 
     vcpu_sig = get_vcpu_sig(parser, args, vmm_type)
 
     try:
+        vars_size = 0
         sev_mode = SevMode.from_str(args.mode)
 
+        if sev_mode == SevMode.SEV_SNP_SVSM:
+
+            if args.vars_file:
+                vars_size = pathlib.Path(args.vars_file).stat().st_size
+            elif args.vars_size:
+                vars_size = args.vars_size
+            else:
+                parser.error("snp:svsm mode requires --vars-size or --vars-file")
+
         if args.dump_vmsa is True and sev_mode not in [SevMode.SEV_ES, SevMode.SEV_SNP, SevMode.SEV_SNP_SVSM]:
             parser.error("--dump-vmsa is not availibe in the selected mode")
 
         ld = guest.calc_launch_digest(sev_mode, args.vcpus, vcpu_sig, args.ovmf, args.kernel, args.initrd, args.append,
-                                      args.snp_ovmf_hash, vmm_type, args.dump_vmsa, args.svsm, args.vars_size)
+                                      args.guest_features, args.snp_ovmf_hash, vmm_type, args.dump_vmsa,
+                                      args.svsm, vars_size)
 
         print_measurement(ld, sev_mode, args.output_format, args.verbose)
     except RuntimeError as e:
         print(f"Error: {e}", file=sys.stderr)
         return 1
 
     return 0
```

### Comparing `sev-snp-measure-0.0.8/sevsnpmeasure/gctx.py` & `sev-snp-measure-0.0.9/sevsnpmeasure/gctx.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.8/sevsnpmeasure/guest.py` & `sev-snp-measure-0.0.9/sevsnpmeasure/guest.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 from .sev_mode import SevMode
 from .vmm_types import VMMType
 
 PAGE_MASK = 0xfff
 
 
 def calc_launch_digest(mode: SevMode, vcpus: int, vcpu_sig: int, ovmf_file: str,
-                       kernel: str, initrd: str, append: str, snp_ovmf_hash_str: str = '',
+                       kernel: str, initrd: str, append: str, guest_features: int, snp_ovmf_hash_str: str = '',
                        vmm_type: VMMType = VMMType.QEMU, dump_vmsa: bool = False, svsm_file: str = '',
                        ovmf_vars_size: int = 0) -> bytes:
     if snp_ovmf_hash_str and mode != SevMode.SEV_SNP:
         raise ValueError("SNP OVMF hash only works with SNP")
 
     if mode == SevMode.SEV_SNP:
-        return snp_calc_launch_digest(vcpus, vcpu_sig, ovmf_file, kernel, initrd, append, snp_ovmf_hash_str, vmm_type,
-                                      dump_vmsa=dump_vmsa)
+        return snp_calc_launch_digest(vcpus, vcpu_sig, ovmf_file, kernel, initrd, append, guest_features,
+                                      snp_ovmf_hash_str, vmm_type, dump_vmsa=dump_vmsa)
     elif mode == SevMode.SEV_ES:
-        return seves_calc_launch_digest(vcpus, vcpu_sig, ovmf_file, kernel, initrd, append, vmm_type=vmm_type,
-                                        dump_vmsa=dump_vmsa)
+        return seves_calc_launch_digest(vcpus, vcpu_sig, ovmf_file, kernel, initrd, append,
+                                        vmm_type=vmm_type, dump_vmsa=dump_vmsa)
     elif mode == SevMode.SEV:
         return sev_calc_launch_digest(ovmf_file, kernel, initrd, append)
     elif mode == SevMode.SEV_SNP_SVSM:
         if vmm_type != VMMType.QEMU:
             raise AssertionError("SVSM mode is only implemented for Qemu.")
         return svsm_calc_launch_digest(vcpus, vcpu_sig, ovmf_file, ovmf_vars_size, svsm_file, dump_vmsa)
     else:
@@ -84,16 +84,16 @@
 
     gctx = GCTX()
     gctx.update_normal_pages(ovmf.gpa(), ovmf.data())
     return gctx.ld()
 
 
 def snp_calc_launch_digest(vcpus: int, vcpu_sig: int, ovmf_file: str,
-                           kernel: str, initrd: str, append: str, ovmf_hash_str: str,
-                           vmm_type: VMMType = VMMType.QEMU, dump_vmsa: bool = False) -> bytes:
+                           kernel: str, initrd: str, append: str, guest_features: int,
+                           ovmf_hash_str: str, vmm_type: VMMType = VMMType.QEMU, dump_vmsa: bool = False) -> bytes:
 
     gctx = GCTX()
     ovmf = OVMF(ovmf_file)
 
     # Allow users to provide a precalculated OVMF hash.
     # Ignores the contents of the OVMF file in front of us.
     if ovmf_hash_str:
@@ -104,15 +104,15 @@
 
     sev_hashes = None
     if kernel:
         sev_hashes = SevHashes(kernel, initrd, append)
 
     snp_update_metadata_pages(gctx, ovmf, sev_hashes, vmm_type)
 
-    vmsa = VMSA(SevMode.SEV_SNP, ovmf.sev_es_reset_eip(), vcpu_sig, vmm_type)
+    vmsa = VMSA(SevMode.SEV_SNP, ovmf.sev_es_reset_eip(), vcpu_sig, guest_features, vmm_type)
     for i, vmsa_page in enumerate(vmsa.pages(vcpus)):
         gctx.update_vmsa_page(vmsa_page)
         if dump_vmsa:
             pathlib.Path(f"vmsa{i}.bin").write_bytes(vmsa_page)
 
     return gctx.ld()
 
@@ -145,15 +145,15 @@
     ovmf = OVMF(ovmf_file)
     launch_hash = hashlib.sha256(ovmf.data())
     if kernel:
         if not ovmf.is_sev_hashes_table_supported():
             raise RuntimeError("Kernel specified but OVMF doesn't support kernel/initrd/cmdline measurement")
         sev_hashes_table = SevHashes(kernel, initrd, append).construct_table()
         launch_hash.update(sev_hashes_table)
-    vmsa = VMSA(SevMode.SEV_ES, ovmf.sev_es_reset_eip(), vcpu_sig, vmm_type)
+    vmsa = VMSA(SevMode.SEV_ES, ovmf.sev_es_reset_eip(), vcpu_sig, 0x0, vmm_type)
     for i, vmsa_page in enumerate(vmsa.pages(vcpus)):
         launch_hash.update(vmsa_page)
         if dump_vmsa:
             pathlib.Path(f"vmsa{i}.bin").write_bytes(vmsa_page)
     return launch_hash.digest()
```

### Comparing `sev-snp-measure-0.0.8/sevsnpmeasure/id_block.py` & `sev-snp-measure-0.0.9/sevsnpmeasure/id_block.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.8/sevsnpmeasure/ovmf.py` & `sev-snp-measure-0.0.9/sevsnpmeasure/ovmf.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.8/sevsnpmeasure/sev_hashes.py` & `sev-snp-measure-0.0.9/sevsnpmeasure/sev_hashes.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.8/sevsnpmeasure/sev_mode.py` & `sev-snp-measure-0.0.9/sevsnpmeasure/sev_mode.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.8/sevsnpmeasure/vcpu_types.py` & `sev-snp-measure-0.0.9/sevsnpmeasure/vcpu_types.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.8/sevsnpmeasure/vmsa.py` & `sev-snp-measure-0.0.9/sevsnpmeasure/vmsa.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,23 +178,19 @@
             rip=eip & 0xffff,
             g_pat=0x7040600070406,  # PAT MSR: See AMD APM Vol 2, Section A.3
             rdx=rdx,
             sev_features=sev_features,
             xcr0=0x1,
         )
 
-    def __init__(self, sev_mode: SevMode, ap_eip: int, vcpu_sig: int, vmm_type: VMMType = VMMType.QEMU):
-        if sev_mode == SevMode.SEV_SNP:
-            sev_features = 0x1
-        else:
-            sev_features = 0x0
-
-        self.bsp_save_area = VMSA.build_save_area(self.BSP_EIP, sev_features, vcpu_sig, vmm_type)
+    def __init__(self, sev_mode: SevMode, ap_eip: int, vcpu_sig: int, guest_features: int,
+                 vmm_type: VMMType = VMMType.QEMU):
+        self.bsp_save_area = VMSA.build_save_area(self.BSP_EIP, guest_features, vcpu_sig, vmm_type)
         if ap_eip:
-            self.ap_save_area = VMSA.build_save_area(ap_eip, sev_features, vcpu_sig, vmm_type)
+            self.ap_save_area = VMSA.build_save_area(ap_eip, guest_features, vcpu_sig, vmm_type)
 
     def pages(self, vcpus: int) -> Iterator[bytes]:
         """
         Generate VMSA pages
         """
         for i in range(vcpus):
             if i == 0:
```

### Comparing `sev-snp-measure-0.0.8/tests/test_guest.py` & `sev-snp-measure-0.0.9/tests/test_guest.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,158 +13,284 @@
 import contextlib
 import os
 
 
 class TestGuest(unittest.TestCase):
 
     # Test of we can generate a good OVMF hash
-    def test_snp_ovmf_hash_gen(self):
+    def test_snp_ovmf_hash_gen_default(self):
         ovmf_hash = 'cab7e085874b3acfdbe2d96dcaa3125111f00c35c6fc9708464c2ae74bfdb048a198cb9a9ccae0b3e5e1a33f5f249819'
         ld = guest.calc_launch_digest(
                 SevMode.SEV_SNP,
                 1,
                 vcpu_types.CPU_SIGS["EPYC-v4"],
                 "tests/fixtures/ovmf_AmdSev_suffix.bin",
                 "/dev/null",
                 "/dev/null",
                 "",
+                0x21,
+                snp_ovmf_hash_str=ovmf_hash)
+        self.assertEqual(
+                ld.hex(),
+                'a076e1b0e6cf55fd94c82e2c25245f8c15f76690b941ba37'
+                '9b31527f82eafe7ad489777ff510d080bac9cd14d41bc205')
+
+    def test_snp_ovmf_hash_gen_feature_snp_only(self):
+        ovmf_hash = 'cab7e085874b3acfdbe2d96dcaa3125111f00c35c6fc9708464c2ae74bfdb048a198cb9a9ccae0b3e5e1a33f5f249819'
+        ld = guest.calc_launch_digest(
+                SevMode.SEV_SNP,
+                1,
+                vcpu_types.CPU_SIGS["EPYC-v4"],
+                "tests/fixtures/ovmf_AmdSev_suffix.bin",
+                "/dev/null",
+                "/dev/null",
+                "",
+                0x1,
                 snp_ovmf_hash_str=ovmf_hash)
         self.assertEqual(
                 ld.hex(),
                 'db06fb267824b1ccb56edbe2a9c2ce88841bca5090dc6dac'
                 '91d9cd30f3c2c0bf42daccb30d55d6625bfbf0dae5c50c6d')
 
     # Test of we can a full LD from the OVMF hash
-    def test_snp_ovmf_hash_full(self):
+    def test_snp_ovmf_hash_full_default(self):
         ovmf_hash = guest.calc_snp_ovmf_hash("tests/fixtures/ovmf_AmdSev_suffix.bin").hex()
         self.assertEqual(
                 ovmf_hash,
                 'edcf6d1c57ce868a167c990f58c8667c698269ef9e080324'
                 '6419eea914186343054d557e1f17acd93b032c106bc70d25')
 
         ld = guest.calc_launch_digest(
                 SevMode.SEV_SNP,
                 1,
                 vcpu_types.CPU_SIGS["EPYC-v4"],
                 "tests/fixtures/ovmf_AmdSev_suffix.bin",
                 "/dev/null",
                 "/dev/null",
                 "console=ttyS0 loglevel=7",
+                0x21,
+                snp_ovmf_hash_str=ovmf_hash)
+        self.assertEqual(
+                ld.hex(),
+                '314e4f0794187ffef05702a36546ea5fe02698041b7f7f17'
+                'd9f418da2d5e4d5cff25256cef9d34888a0dd64dea438780')
+
+    def test_snp_ovmf_hash_full_feature_snp_only(self):
+        ovmf_hash = guest.calc_snp_ovmf_hash("tests/fixtures/ovmf_AmdSev_suffix.bin").hex()
+        self.assertEqual(
+                ovmf_hash,
+                'edcf6d1c57ce868a167c990f58c8667c698269ef9e080324'
+                '6419eea914186343054d557e1f17acd93b032c106bc70d25')
+
+        ld = guest.calc_launch_digest(
+                SevMode.SEV_SNP,
+                1,
+                vcpu_types.CPU_SIGS["EPYC-v4"],
+                "tests/fixtures/ovmf_AmdSev_suffix.bin",
+                "/dev/null",
+                "/dev/null",
+                "console=ttyS0 loglevel=7",
+                0x1,
                 snp_ovmf_hash_str=ovmf_hash)
         self.assertEqual(
                 ld.hex(),
                 'f07864303ad8243132029e8110b92805c78d1135a15da75f'
-                '67abb9a711d78740347f24ee76f603e650ec4adf3611cc1e')
+                '67abb9a711d78740347f24ee76f603e650ec4adf3611cc1e'
+            )
+
+    def test_snp_ec2_default(self):
+        ld = guest.calc_launch_digest(
+                SevMode.SEV_SNP,
+                1,
+                vcpu_types.CPU_SIGS["EPYC-v4"],
+                "tests/fixtures/ovmf_AmdSev_suffix.bin",
+                "/dev/null",
+                "/dev/null",
+                "",
+                0x21,
+                vmm_type=vmm_types.VMMType.ec2)
+        self.assertEqual(
+                ld.hex(),
+                'cd4a4690a1f679ac8f3d6e446aab8d0061d535cc94615d98'
+                'c7d7dbe4b16dbceeaf7fc7944e7874b202e27041f179e7e6')
 
-    def test_snp_ec2(self):
+    def test_snp_ec2_feature_snp_only(self):
         ld = guest.calc_launch_digest(
                 SevMode.SEV_SNP,
                 1,
                 vcpu_types.CPU_SIGS["EPYC-v4"],
                 "tests/fixtures/ovmf_AmdSev_suffix.bin",
                 "/dev/null",
                 "/dev/null",
                 "",
+                0x1,
                 vmm_type=vmm_types.VMMType.ec2)
         self.assertEqual(
                 ld.hex(),
                 '760b6e51039d2d6c1fc6d38ca5c387967d158e0294883e45'
                 '22c36f89bd61bfc9cdb975cd1ceedffbe1b23b1daf4e3f42')
 
-    def test_snp(self):
+    def test_snp_default(self):
         ld = guest.calc_launch_digest(
                 SevMode.SEV_SNP,
                 1,
                 vcpu_types.CPU_SIGS["EPYC-v4"],
                 "tests/fixtures/ovmf_AmdSev_suffix.bin",
                 "/dev/null",
                 "/dev/null",
-                "console=ttyS0 loglevel=7")
+                "console=ttyS0 loglevel=7",
+                0x21)
+        self.assertEqual(
+                ld.hex(),
+                '314e4f0794187ffef05702a36546ea5fe02698041b7f7f17'
+                'd9f418da2d5e4d5cff25256cef9d34888a0dd64dea438780')
+
+    def test_snp_guest_feature_snp_only(self):
+        ld = guest.calc_launch_digest(
+                SevMode.SEV_SNP,
+                1,
+                vcpu_types.CPU_SIGS["EPYC-v4"],
+                "tests/fixtures/ovmf_AmdSev_suffix.bin",
+                "/dev/null",
+                "/dev/null",
+                "console=ttyS0 loglevel=7",
+                0x1)
         self.assertEqual(
                 ld.hex(),
                 'f07864303ad8243132029e8110b92805c78d1135a15da75f'
                 '67abb9a711d78740347f24ee76f603e650ec4adf3611cc1e')
 
-    def test_snp_without_kernel(self):
+    def test_snp_without_kernel_default(self):
+        ld = guest.calc_launch_digest(
+                SevMode.SEV_SNP,
+                1,
+                vcpu_types.CPU_SIGS["EPYC-v4"],
+                "tests/fixtures/ovmf_AmdSev_suffix.bin",
+                None,
+                None,
+                None,
+                0x21)
+        self.assertEqual(
+                ld.hex(),
+                '6d9054ed9872a64c968cfbcfa1247cafa792e3f9a395306d'
+                '95c9937aaa081c643d25f369ccbd34409dafcae90bff55f3')
+
+    def test_snp_without_kernel_feature_snp_only(self):
         ld = guest.calc_launch_digest(
                 SevMode.SEV_SNP,
                 1,
                 vcpu_types.CPU_SIGS["EPYC-v4"],
                 "tests/fixtures/ovmf_AmdSev_suffix.bin",
                 None,
                 None,
-                None)
+                None,
+                0x1)
         self.assertEqual(
                 ld.hex(),
                 'e5e6be5a8fa6256f0245666bb237e2d028b7928148ce78d5'
                 '1b8a64dc9506c377709a5b5d7ab75554593bced304fcff93')
 
-    def test_snp_with_multiple_vcpus(self):
+    def test_snp_with_multiple_vcpus_default(self):
+        ld = guest.calc_launch_digest(
+                SevMode.SEV_SNP,
+                4,
+                vcpu_types.CPU_SIGS["EPYC-v4"],
+                "tests/fixtures/ovmf_AmdSev_suffix.bin",
+                "/dev/null",
+                "/dev/null",
+                "",
+                0x21)
+        self.assertEqual(
+                ld.hex(),
+                '3aa1bdf5a87fad15960f099e82a09e428901c590f2b68d71'
+                'aa246c168db5e75daf4819d017a9530c56bed2da5c0cdbd7')
+
+    def test_snp_with_multiple_vcpus_feature_snp_only(self):
         ld = guest.calc_launch_digest(
                 SevMode.SEV_SNP,
                 4,
                 vcpu_types.CPU_SIGS["EPYC-v4"],
                 "tests/fixtures/ovmf_AmdSev_suffix.bin",
                 "/dev/null",
                 "/dev/null",
-                "")
+                "",
+                0x1)
         self.assertEqual(
                 ld.hex(),
                 '1c784beb8c49aa604b7fd57fbc73b36ec53a3f5fb48a2b89'
                 '5ad6cc2ea15d18ee7cc15e3e57c792766b45f944c3e81cfe')
 
-    def test_snp_with_ovmfx64_without_kernel(self):
+    def test_snp_with_ovmfx64_without_default(self):
+        ld = guest.calc_launch_digest(
+                SevMode.SEV_SNP,
+                1,
+                vcpu_types.CPU_SIGS["EPYC-v4"],
+                "tests/fixtures/ovmf_OvmfX64_suffix.bin",
+                None,
+                None,
+                None,
+                0x21)
+        self.assertEqual(
+                ld.hex(),
+                '37a9efc939f360a9ccfaaf1a7702137b81ea00c38d0361c8'
+                '523285fad1b10e94ad8c1ecd7c82ff589cb120670be74a99')
+
+    def test_snp_with_ovmfx64_without_kernel_feature_snp_only(self):
         ld = guest.calc_launch_digest(
                 SevMode.SEV_SNP,
                 1,
                 vcpu_types.CPU_SIGS["EPYC-v4"],
                 "tests/fixtures/ovmf_OvmfX64_suffix.bin",
                 None,
                 None,
-                None)
+                None,
+                0x1)
         self.assertEqual(
                 ld.hex(),
                 '7ef631fa7f659f7250de96c456a0eb7354bd3b9461982f38'
                 '6a41c6a6aede87870ad020552a5a0716672d5d6e5b86b8f9')
 
     def test_snp_with_ovmfx64_and_kernel_should_fail(self):
         with self.assertRaises(RuntimeError) as c:
             guest.calc_launch_digest(
                     SevMode.SEV_SNP,
                     1,
                     vcpu_types.CPU_SIGS["EPYC-v4"],
                     "tests/fixtures/ovmf_OvmfX64_suffix.bin",
                     "/dev/null",
                     "/dev/null",
-                    "")
+                    "",
+                    0x21)
         self.assertEqual(str(c.exception),
                          "Kernel specified but OVMF metadata doesn't include SNP_KERNEL_HASHES section")
 
     def test_seves(self):
         ld = guest.calc_launch_digest(
                 SevMode.SEV_ES,
                 1,
                 vcpu_types.CPU_SIGS["EPYC-v4"],
                 "tests/fixtures/ovmf_AmdSev_suffix.bin",
                 "/dev/null",
                 "/dev/null",
-                "")
+                "",
+                0x21)
         self.assertEqual(
                 ld.hex(),
                 '2e91d54814445ad178180af09f881efe4079fc54bfddd0ec1179ecd3cdbdf772')
 
     def test_seves_with_multiple_vcpus(self):
         ld = guest.calc_launch_digest(
                 SevMode.SEV_ES,
                 4,
                 vcpu_types.CPU_SIGS["EPYC-v4"],
                 "tests/fixtures/ovmf_AmdSev_suffix.bin",
                 "/dev/null",
                 "/dev/null",
-                "")
+                "",
+                0x21)
         self.assertEqual(
                 ld.hex(),
                 'c05d37600072dc5ff24bafc49410f0369ba3a37c130a7bb7055ac6878be300f7')
 
     def test_seves_dump_vmsa(self):
         """Test that SEV-ES mode creates vmsa files if requrested."""
         fixtures_dir = pathlib.Path('tests/fixtures').absolute()
@@ -174,14 +300,15 @@
                         SevMode.SEV_ES,
                         4,
                         vcpu_types.CPU_SIGS["EPYC-v4"],
                         fixtures_dir / "ovmf_AmdSev_suffix.bin",
                         "/dev/null",
                         "/dev/null",
                         "",
+                        0x21,
                         dump_vmsa=True)
                 self.assertTrue(pathlib.Path("vmsa0.bin").exists())
                 self.assertTrue(pathlib.Path("vmsa1.bin").exists())
                 self.assertTrue(pathlib.Path("vmsa2.bin").exists())
                 self.assertTrue(pathlib.Path("vmsa3.bin").exists())
                 self.assertFalse(pathlib.Path("vmsa4.bin").exists())
 
@@ -190,54 +317,58 @@
             guest.calc_launch_digest(
                     SevMode.SEV_ES,
                     1,
                     None,
                     "tests/fixtures/ovmf_OvmfX64_suffix.bin",
                     "/dev/null",
                     "/dev/null",
-                    "")
+                    "",
+                    0x21)
         self.assertEqual(str(c.exception),
                          "Kernel specified but OVMF doesn't support kernel/initrd/cmdline measurement")
 
     def test_sev(self):
         ld = guest.calc_launch_digest(
                 SevMode.SEV,
                 1,
                 None,
                 "tests/fixtures/ovmf_AmdSev_suffix.bin",
                 "/dev/null",
                 "/dev/null",
-                "console=ttyS0 loglevel=7")
+                "console=ttyS0 loglevel=7",
+                0x21)
         self.assertEqual(
                 ld.hex(),
                 'f0d92a1fda00249e008820bd40def6abbed2ee65fea8a8bc47e532863ca0cc6a')
 
     def test_sev_with_kernel_without_initrd_and_append(self):
         ld = guest.calc_launch_digest(
                 SevMode.SEV,
                 1,
                 None,
                 "tests/fixtures/ovmf_AmdSev_suffix.bin",
                 "/dev/null",
                 None,
-                None)
+                None,
+                0x21)
         self.assertEqual(
                 ld.hex(),
                 '7332f6ef294f79919b46302e4541900a2dfc96714e2b7b4b5ccdc1899b78a195')
 
     def test_sev_with_ovmfx64_and_kernel_should_fail(self):
         with self.assertRaises(RuntimeError) as c:
             guest.calc_launch_digest(
                     SevMode.SEV,
                     1,
                     None,
                     "tests/fixtures/ovmf_OvmfX64_suffix.bin",
                     "/dev/null",
                     "/dev/null",
-                    "")
+                    "",
+                    0x21)
         self.assertEqual(str(c.exception),
                          "Kernel specified but OVMF doesn't support kernel/initrd/cmdline measurement")
 
     def test_snp_dump_vmsa(self):
         """Test that SEV-SNP mode creates vmsa files if requrested."""
         fixtures_dir = pathlib.Path('tests/fixtures').absolute()
         with tempfile.TemporaryDirectory() as tmp:
@@ -247,42 +378,45 @@
                         SevMode.SEV_SNP,
                         1,
                         vcpu_types.CPU_SIGS["EPYC-v4"],
                         fixtures_dir / "ovmf_AmdSev_suffix.bin",
                         "/dev/null",
                         "/dev/null",
                         "",
+                        0x21,
                         snp_ovmf_hash_str=ovmf_hash,
                         dump_vmsa=True)
                 self.assertTrue(pathlib.Path("vmsa0.bin").exists())
                 self.assertFalse(pathlib.Path("vmsa1.bin").exists())
 
     def test_sev_with_ovmfx64_without_kernel(self):
         ld = guest.calc_launch_digest(
                 SevMode.SEV,
                 1,
                 None,
                 "tests/fixtures/ovmf_OvmfX64_suffix.bin",
                 None,
                 None,
-                None)
+                None,
+                0x21)
         self.assertEqual(
                 ld.hex(),
                 'af9d6c674b1ff04937084c98c99ca106b25c37b2c9541ac313e6e0c54426314f')
 
     def test_snp_svsm_4_vcpus(self):
         """Test that SNP-SVSM mode produces correct measurement value when using 4 vCPUs"""
         ld = guest.calc_launch_digest(
                 SevMode.SEV_SNP_SVSM,
                 4,
                 vcpu_types.CPU_SIGS["EPYC-v4"],
                 'tests/fixtures/svsm_ovmf.fd',
                 None,
                 None,
                 None,
+                0x21,
                 None,
                 vmm_types.VMMType.QEMU,
                 False,
                 'tests/fixtures/svsm.bin',
                 540672)
         self.assertEqual(
                 ld.hex(),
@@ -294,14 +428,15 @@
                 SevMode.SEV_SNP_SVSM,
                 2,
                 vcpu_types.CPU_SIGS["EPYC-v4"],
                 'tests/fixtures/svsm_ovmf.fd',
                 None,
                 None,
                 None,
+                0x21,
                 None,
                 vmm_types.VMMType.QEMU,
                 False,
                 'tests/fixtures/svsm.bin',
                 540672)
         self.assertEqual(
                 ld.hex(),
@@ -316,14 +451,15 @@
                         SevMode.SEV_SNP_SVSM,
                         2,
                         vcpu_types.CPU_SIGS["EPYC-v4"],
                         fixtures_dir / 'svsm_ovmf.fd',
                         None,
                         None,
                         None,
+                        0x21,
                         None,
                         vmm_types.VMMType.QEMU,
                         True,
                         fixtures_dir / 'svsm.bin',
                         540672)
                 self.assertTrue(pathlib.Path("vmsa0.bin").exists())
                 self.assertTrue(pathlib.Path("vmsa1.bin").exists())
```

### Comparing `sev-snp-measure-0.0.8/tests/test_id_block.py` & `sev-snp-measure-0.0.9/tests/test_id_block.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.8/tests/test_sev_mode.py` & `sev-snp-measure-0.0.9/tests/test_sev_mode.py`

 * *Files identical despite different names*

