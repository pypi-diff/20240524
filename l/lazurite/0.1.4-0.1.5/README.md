# Comparing `tmp/lazurite-0.1.4.tar.gz` & `tmp/lazurite-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazurite-0.1.4.tar", last modified: Thu May 16 12:09:08 2024, max compression
+gzip compressed data, was "lazurite-0.1.5.tar", last modified: Fri May 24 12:19:38 2024, max compression
```

## Comparing `lazurite-0.1.4.tar` & `lazurite-0.1.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:09:08.627611 lazurite-0.1.4/
--rw-rw-rw-   0        0        0    35823 2024-05-03 11:00:28.000000 lazurite-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     1820 2024-05-16 12:09:08.626612 lazurite-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      730 2024-05-16 12:03:06.000000 lazurite-0.1.4/README.md
--rw-rw-rw-   0        0        0     1216 2024-05-16 12:07:15.000000 lazurite-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 12:09:08.627611 lazurite-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-16 12:09:08.574102 lazurite-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-16 12:09:08.583100 lazurite-0.1.4/src/lazurite/
--rw-rw-rw-   0        0        0        0 2024-02-13 20:06:38.000000 lazurite-0.1.4/src/lazurite/__init__.py
--rw-rw-rw-   0        0        0       73 2024-05-03 09:54:14.000000 lazurite-0.1.4/src/lazurite/__main__.py
--rw-rw-rw-   0        0        0    12806 2024-05-09 21:47:12.000000 lazurite-0.1.4/src/lazurite/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:09:08.603126 lazurite-0.1.4/src/lazurite/compiler/
--rw-rw-rw-   0        0        0       68 2024-02-13 21:47:08.000000 lazurite-0.1.4/src/lazurite/compiler/__init__.py
--rw-rw-rw-   0        0        0     2645 2024-04-30 10:45:06.000000 lazurite-0.1.4/src/lazurite/compiler/dxc.py
--rw-rw-rw-   0        0        0      766 2024-04-01 13:25:10.000000 lazurite-0.1.4/src/lazurite/compiler/macro_define.py
--rw-rw-rw-   0        0        0     6461 2024-05-03 11:38:02.000000 lazurite-0.1.4/src/lazurite/compiler/shaderc.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:09:08.605147 lazurite-0.1.4/src/lazurite/decompiler/
--rw-rw-rw-   0        0        0        0 2023-07-31 21:03:18.000000 lazurite-0.1.4/src/lazurite/decompiler/__init__.py
--rw-rw-rw-   0        0        0    25267 2024-03-31 20:06:22.000000 lazurite-0.1.4/src/lazurite/decompiler/macro_decompiler.py
--rw-rw-rw-   0        0        0     3448 2024-03-31 20:05:52.000000 lazurite-0.1.4/src/lazurite/decompiler/varying_decompiler.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:09:08.613095 lazurite-0.1.4/src/lazurite/material/
--rw-rw-rw-   0        0        0       32 2024-02-13 21:47:22.000000 lazurite-0.1.4/src/lazurite/material/__init__.py
--rw-rw-rw-   0        0        0     6210 2024-05-15 17:13:46.000000 lazurite-0.1.4/src/lazurite/material/buffer.py
--rw-rw-rw-   0        0        0      359 2024-03-20 14:54:26.000000 lazurite-0.1.4/src/lazurite/material/encryption.py
--rw-rw-rw-   0        0        0    21695 2024-04-29 14:03:32.000000 lazurite-0.1.4/src/lazurite/material/material.py
--rw-rw-rw-   0        0        0      750 2024-02-13 20:38:24.000000 lazurite-0.1.4/src/lazurite/material/platform.py
--rw-rw-rw-   0        0        0      114 2023-10-07 14:20:58.000000 lazurite-0.1.4/src/lazurite/material/precision.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:09:08.619611 lazurite-0.1.4/src/lazurite/material/shader_pass/
--rw-rw-rw-   0        0        0       28 2024-02-13 21:07:36.000000 lazurite-0.1.4/src/lazurite/material/shader_pass/__init__.py
--rw-rw-rw-   0        0        0     5398 2024-04-06 20:22:04.000000 lazurite-0.1.4/src/lazurite/material/shader_pass/bgfx_shader.py
--rw-rw-rw-   0        0        0      377 2024-02-18 16:33:18.000000 lazurite-0.1.4/src/lazurite/material/shader_pass/blend_mode.py
--rw-rw-rw-   0        0        0     4192 2024-04-06 20:22:08.000000 lazurite-0.1.4/src/lazurite/material/shader_pass/shader_definition.py
--rw-rw-rw-   0        0        0     5119 2024-04-29 18:12:28.000000 lazurite-0.1.4/src/lazurite/material/shader_pass/shader_input.py
--rw-rw-rw-   0        0        0     6354 2024-05-05 22:06:01.000000 lazurite-0.1.4/src/lazurite/material/shader_pass/shader_pass.py
--rw-rw-rw-   0        0        0     1595 2024-03-01 01:21:50.000000 lazurite-0.1.4/src/lazurite/material/shader_pass/supported_platforms.py
--rw-rw-rw-   0        0        0     3871 2024-04-06 20:22:20.000000 lazurite-0.1.4/src/lazurite/material/shader_pass/variant.py
--rw-rw-rw-   0        0        0      121 2023-09-24 16:30:26.000000 lazurite-0.1.4/src/lazurite/material/stage.py
--rw-rw-rw-   0        0        0     2502 2024-04-13 17:47:30.000000 lazurite-0.1.4/src/lazurite/material/uniform.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:09:08.624611 lazurite-0.1.4/src/lazurite/project/
--rw-rw-rw-   0        0        0        0 2024-02-13 20:05:48.000000 lazurite-0.1.4/src/lazurite/project/__init__.py
--rw-rw-rw-   0        0        0      273 2024-04-01 22:39:38.000000 lazurite-0.1.4/src/lazurite/project/compiler_type.py
--rw-rw-rw-   0        0        0     3067 2024-04-06 20:35:26.000000 lazurite-0.1.4/src/lazurite/project/material_config.py
--rw-rw-rw-   0        0        0    13693 2024-05-16 11:55:24.000000 lazurite-0.1.4/src/lazurite/project/project.py
--rw-rw-rw-   0        0        0     5513 2024-04-06 20:35:26.000000 lazurite-0.1.4/src/lazurite/project/project_config.py
--rw-rw-rw-   0        0        0     1271 2024-04-01 22:38:14.000000 lazurite-0.1.4/src/lazurite/project/shader_file_overwrite.py
--rw-rw-rw-   0        0        0      838 2024-04-29 18:29:54.000000 lazurite-0.1.4/src/lazurite/tempfile.py
--rw-rw-rw-   0        0        0     2260 2024-02-24 14:42:42.000000 lazurite-0.1.4/src/lazurite/util.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:09:08.625612 lazurite-0.1.4/src/lazurite.egg-info/
--rw-rw-rw-   0        0        0     1820 2024-05-16 12:09:08.000000 lazurite-0.1.4/src/lazurite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1522 2024-05-16 12:09:08.000000 lazurite-0.1.4/src/lazurite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:09:08.000000 lazurite-0.1.4/src/lazurite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-16 12:09:08.000000 lazurite-0.1.4/src/lazurite.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2024-05-16 12:09:08.000000 lazurite-0.1.4/src/lazurite.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-16 12:09:08.000000 lazurite-0.1.4/src/lazurite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:19:38.252045 lazurite-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-24 12:19:24.000000 lazurite-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-24 12:19:38.252045 lazurite-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-24 12:19:24.000000 lazurite-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-24 12:19:24.000000 lazurite-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 12:19:38.252045 lazurite-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:19:38.244045 lazurite-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:19:38.244045 lazurite-0.1.5/src/lazurite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13643 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:19:38.248045 lazurite-0.1.5/src/lazurite/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/compiler/dxc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/compiler/macro_define.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/compiler/shaderc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:19:38.248045 lazurite-0.1.5/src/lazurite/decompiler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/decompiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24554 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/decompiler/macro_decompiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/decompiler/varying_decompiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:19:38.248045 lazurite-0.1.5/src/lazurite/material/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/material/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/material/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/material/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20828 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/material/material.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/material/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/material/precision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:19:38.248045 lazurite-0.1.5/src/lazurite/material/shader_pass/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/material/shader_pass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/material/shader_pass/bgfx_shader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/material/shader_pass/blend_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/material/shader_pass/shader_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/material/shader_pass/shader_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/material/shader_pass/shader_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/material/shader_pass/supported_platforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/material/shader_pass/variant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/material/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/material/uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:19:38.252045 lazurite-0.1.5/src/lazurite/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/project/compiler_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/project/material_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13326 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/project/project_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/project/shader_file_overwrite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/tempfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-24 12:19:24.000000 lazurite-0.1.5/src/lazurite/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:19:38.252045 lazurite-0.1.5/src/lazurite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-24 12:19:38.000000 lazurite-0.1.5/src/lazurite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-24 12:19:38.000000 lazurite-0.1.5/src/lazurite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 12:19:38.000000 lazurite-0.1.5/src/lazurite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-24 12:19:38.000000 lazurite-0.1.5/src/lazurite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 12:19:38.000000 lazurite-0.1.5/src/lazurite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 12:19:38.000000 lazurite-0.1.5/src/lazurite.egg-info/top_level.txt
```

### Comparing `lazurite-0.1.4/LICENSE` & `lazurite-0.1.5/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `lazurite-0.1.4/PKG-INFO` & `lazurite-0.1.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-Metadata-Version: 2.1
-Name: lazurite
-Version: 0.1.4
-Summary: Unofficial shader development tool for Minecraft: Bedrock Edition with RenderDragon graphics engine
-Author: veka0
-Project-URL: Documentation, https://veka0.github.io/lazurite
-Project-URL: Repository, https://github.com/veka0/lazurite
-Keywords: shader,minecraft,bedrock,renderdragon
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: Android
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Topic :: Software Development :: Compilers
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pyjson5
-Requires-Dist: myers
-Requires-Dist: pcpp
-Requires-Dist: pycryptodome
-Requires-Dist: sympy
-
-# Lazurite
-
-Unofficial shader development tool for Minecraft: Bedrock Edition with RenderDragon graphics engine.
-
-Documentation: <https://veka0.github.io/lazurite>
-
-PyPi page: <https://pypi.org/project/lazurite>
-
-## Installation
-
-Lazurite requires to have Python 3.10+ installed, but 3.12 is recommended.
-
-Official python installation page: <https://www.python.org/downloads>.
-Windows users are recommended to install Python from Microsoft Store.
-
-After installing python, you can install lazurite package from pypi repository, with a command
-
-```sh
-pip install lazurite
-```
-
-or
-
-```sh
-python -m pip install lazurite
-```
-
-## Next steps
-
-Read the documentation here <https://veka0.github.io/lazurite>
+Metadata-Version: 2.1
+Name: lazurite
+Version: 0.1.5
+Summary: Unofficial shader development tool for Minecraft: Bedrock Edition with RenderDragon graphics engine
+Author: veka0
+Project-URL: Documentation, https://veka0.github.io/lazurite
+Project-URL: Repository, https://github.com/veka0/lazurite
+Keywords: shader,minecraft,bedrock,renderdragon
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Operating System :: Android
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Compilers
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pyjson5
+Requires-Dist: myers
+Requires-Dist: pcpp
+Requires-Dist: pycryptodome
+Requires-Dist: sympy
+
+# Lazurite
+
+Unofficial shader development tool for Minecraft: Bedrock Edition with RenderDragon graphics engine.
+
+Documentation: <https://veka0.github.io/lazurite>
+
+PyPi page: <https://pypi.org/project/lazurite>
+
+## Installation
+
+Lazurite requires to have Python 3.10+ installed, but 3.12 is recommended.
+
+Official python installation page: <https://www.python.org/downloads>.
+Windows users are recommended to install Python from Microsoft Store.
+
+After installing python, you can install lazurite package from pypi repository, with a command
+
+```sh
+pip install lazurite
+```
+
+or
+
+```sh
+python -m pip install lazurite
+```
+
+## Next steps
+
+Read the documentation here <https://veka0.github.io/lazurite>
```

### Comparing `lazurite-0.1.4/README.md` & `lazurite-0.1.5/README.md`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Lazurite
-
-Unofficial shader development tool for Minecraft: Bedrock Edition with RenderDragon graphics engine.
-
-Documentation: <https://veka0.github.io/lazurite>
-
-PyPi page: <https://pypi.org/project/lazurite>
-
-## Installation
-
-Lazurite requires to have Python 3.10+ installed, but 3.12 is recommended.
-
-Official python installation page: <https://www.python.org/downloads>.
-Windows users are recommended to install Python from Microsoft Store.
-
-After installing python, you can install lazurite package from pypi repository, with a command
-
-```sh
-pip install lazurite
-```
-
-or
-
-```sh
-python -m pip install lazurite
-```
-
-## Next steps
-
-Read the documentation here <https://veka0.github.io/lazurite>
+# Lazurite
+
+Unofficial shader development tool for Minecraft: Bedrock Edition with RenderDragon graphics engine.
+
+Documentation: <https://veka0.github.io/lazurite>
+
+PyPi page: <https://pypi.org/project/lazurite>
+
+## Installation
+
+Lazurite requires to have Python 3.10+ installed, but 3.12 is recommended.
+
+Official python installation page: <https://www.python.org/downloads>.
+Windows users are recommended to install Python from Microsoft Store.
+
+After installing python, you can install lazurite package from pypi repository, with a command
+
+```sh
+pip install lazurite
+```
+
+or
+
+```sh
+python -m pip install lazurite
+```
+
+## Next steps
+
+Read the documentation here <https://veka0.github.io/lazurite>
```

### Comparing `lazurite-0.1.4/pyproject.toml` & `lazurite-0.1.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-
-[project]
-name = "lazurite"
-description = "Unofficial shader development tool for Minecraft: Bedrock Edition with RenderDragon graphics engine"
-keywords = ["shader", "minecraft", "bedrock", "renderdragon"]
-version = "0.1.4"
-readme = "README.md"
-requires-python = ">=3.10"
-authors = [{ name = "veka0" }]
-
-classifiers = [
-    # General
-    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    # Python Versions
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
-    # OS
-    "Operating System :: Android",
-    "Operating System :: MacOS",
-    "Operating System :: Microsoft :: Windows",
-    "Operating System :: POSIX :: Linux",
-    # Topics
-    "Topic :: Software Development :: Build Tools",
-    "Topic :: Software Development :: Compilers",
-]
-dependencies = ["pyjson5", "myers", "pcpp", "pycryptodome", "sympy"]
-
-
-[project.urls]
-Documentation = "https://veka0.github.io/lazurite"
-Repository = "https://github.com/veka0/lazurite"
-
-
-[project.scripts]
-lazurite = "lazurite.cli:main"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+
+[project]
+name = "lazurite"
+description = "Unofficial shader development tool for Minecraft: Bedrock Edition with RenderDragon graphics engine"
+keywords = ["shader", "minecraft", "bedrock", "renderdragon"]
+version = "0.1.5"
+readme = "README.md"
+requires-python = ">=3.10"
+authors = [{ name = "veka0" }]
+
+classifiers = [
+    # General
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    # Python Versions
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    # OS
+    "Operating System :: Android",
+    "Operating System :: MacOS",
+    "Operating System :: Microsoft :: Windows",
+    "Operating System :: POSIX :: Linux",
+    # Topics
+    "Topic :: Software Development :: Build Tools",
+    "Topic :: Software Development :: Compilers",
+]
+dependencies = ["pyjson5", "myers", "pcpp", "pycryptodome", "sympy"]
+
+
+[project.urls]
+Documentation = "https://veka0.github.io/lazurite"
+Repository = "https://github.com/veka0/lazurite"
+
+
+[project.scripts]
+lazurite = "lazurite.cli:main"
```

### Comparing `lazurite-0.1.4/src/lazurite/compiler/dxc.py` & `lazurite-0.1.5/src/lazurite/compiler/dxc.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-import subprocess
-from lazurite.material.stage import ShaderStage
-from lazurite.material.platform import ShaderPlatform
-from lazurite.tempfile import CustomTempFile
-
-from .macro_define import MacroDefine
-
-
-class DxcCompiler:
-    dxc_path: str
-
-    def __init__(self, dxc_paths: list[str] | str = None) -> None:
-        if dxc_paths is None:
-            dxc_paths = ["dxc", "./dxc"]
-        elif isinstance(dxc_paths, str):
-            dxc_paths = [dxc_paths]
-
-        self.dxc_path = ""
-
-        for path in dxc_paths:
-            try:
-                result = subprocess.run([path, "-help"], capture_output=True)
-            except FileNotFoundError:
-                pass
-            else:
-                self.dxc_path = path
-                break
-
-        if not self.dxc_path:
-            raise Exception(
-                f"Error! No valid DXC compiler was found in the list {dxc_paths}"
-            )
-
-        if result.returncode:
-            print(result.stdout.decode())
-            print(result.stderr.decode())
-            result.check_returncode()
-
-    def compile(
-        self,
-        file: str,
-        platform: ShaderPlatform = ShaderPlatform.Direct3D_SM65,
-        stage: ShaderStage = ShaderStage.Compute,
-        entry_point: str = None,
-        defines: list[MacroDefine] = None,
-        options: list[str] = None,
-    ):
-        if not platform.name.startswith("Direct3D_SM"):
-            raise Exception(
-                f"{platform.name} shaders cannot be compiled with DXC compiler!"
-            )
-
-        args = [self.dxc_path, file]
-
-        if stage == ShaderStage.Compute:
-            profile = "cs"  # Compute Shader
-        elif stage == ShaderStage.Vertex:
-            profile = "vs"  # Vertex Shader
-        else:
-            profile = "ps"  # Pixel Shader
-        version = platform.name.removeprefix("Direct3D_SM")
-        args.extend(("-T", "_".join((profile, *version))))
-
-        if entry_point:
-            args.extend(("-E", entry_point))
-
-        if defines:
-            for define in defines:
-                args.extend(("-D", define.format_dxc()))
-
-        if options:
-            args.extend(options)
-
-        with CustomTempFile() as f:
-            f.close()
-            args.extend(("-Fo", f.name))
-
-            result = subprocess.run(args)
-
-            if result.stderr:
-                print(result.stderr.decode())
-            if result.stdout:
-                print(result.stdout.decode())
-
-            result.check_returncode()
-
-            with open(f.name, "rb") as f:
-                return f.read()
+import subprocess
+from lazurite.material.stage import ShaderStage
+from lazurite.material.platform import ShaderPlatform
+from lazurite.tempfile import CustomTempFile
+
+from .macro_define import MacroDefine
+
+
+class DxcCompiler:
+    dxc_path: str
+
+    def __init__(self, dxc_paths: list[str] | str = None) -> None:
+        if dxc_paths is None:
+            dxc_paths = ["dxc", "./dxc"]
+        elif isinstance(dxc_paths, str):
+            dxc_paths = [dxc_paths]
+
+        self.dxc_path = ""
+
+        for path in dxc_paths:
+            try:
+                result = subprocess.run([path, "-help"], capture_output=True)
+            except FileNotFoundError:
+                pass
+            else:
+                self.dxc_path = path
+                break
+
+        if not self.dxc_path:
+            raise Exception(
+                f"Error! No valid DXC compiler was found in the list {dxc_paths}"
+            )
+
+        if result.returncode:
+            print(result.stdout.decode())
+            print(result.stderr.decode())
+            result.check_returncode()
+
+    def compile(
+        self,
+        file: str,
+        platform: ShaderPlatform = ShaderPlatform.Direct3D_SM65,
+        stage: ShaderStage = ShaderStage.Compute,
+        entry_point: str = None,
+        defines: list[MacroDefine] = None,
+        options: list[str] = None,
+    ):
+        if not platform.name.startswith("Direct3D_SM"):
+            raise Exception(
+                f"{platform.name} shaders cannot be compiled with DXC compiler!"
+            )
+
+        args = [self.dxc_path, file]
+
+        if stage == ShaderStage.Compute:
+            profile = "cs"  # Compute Shader
+        elif stage == ShaderStage.Vertex:
+            profile = "vs"  # Vertex Shader
+        else:
+            profile = "ps"  # Pixel Shader
+        version = platform.name.removeprefix("Direct3D_SM")
+        args.extend(("-T", "_".join((profile, *version))))
+
+        if entry_point:
+            args.extend(("-E", entry_point))
+
+        if defines:
+            for define in defines:
+                args.extend(("-D", define.format_dxc()))
+
+        if options:
+            args.extend(options)
+
+        with CustomTempFile() as f:
+            f.close()
+            args.extend(("-Fo", f.name))
+
+            result = subprocess.run(args)
+
+            if result.stderr:
+                print(result.stderr.decode())
+            if result.stdout:
+                print(result.stdout.decode())
+
+            result.check_returncode()
+
+            with open(f.name, "rb") as f:
+                return f.read()
```

### Comparing `lazurite-0.1.4/src/lazurite/compiler/macro_define.py` & `lazurite-0.1.5/src/lazurite/compiler/macro_define.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-class MacroDefine:
-    name: str
-    value: int | None
-
-    def __init__(self, name: str = "", value: int = None) -> None:
-        self.name = name
-        self.value = value
-
-    def format_bgfx(self):
-        if self.value is None:
-            return self.name
-        return f"{self.name}={self.value}"
-
-    def format_dxc(self):
-        if self.value is None:
-            return self.name
-        return f"{self.name}={self.value}"
-
-    def format_cpp(self):
-        if self.value is None:
-            return self.name
-        return f"{self.name} {self.value}"
-
-    @classmethod
-    def from_string(cls, string: str):
-        elements = string.split(" ", 1)
-        return cls(elements[0], elements[1] if len(elements) > 1 else None)
+class MacroDefine:
+    name: str
+    value: int | None
+
+    def __init__(self, name: str = "", value: int = None) -> None:
+        self.name = name
+        self.value = value
+
+    def format_bgfx(self):
+        if self.value is None:
+            return self.name
+        return f"{self.name}={self.value}"
+
+    def format_dxc(self):
+        if self.value is None:
+            return self.name
+        return f"{self.name}={self.value}"
+
+    def format_cpp(self):
+        if self.value is None:
+            return self.name
+        return f"{self.name} {self.value}"
+
+    @classmethod
+    def from_string(cls, string: str):
+        elements = string.split(" ", 1)
+        return cls(elements[0], elements[1] if len(elements) > 1 else None)
```

### Comparing `lazurite-0.1.4/src/lazurite/compiler/shaderc.py` & `lazurite-0.1.5/src/lazurite/compiler/shaderc.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-import subprocess
-
-from lazurite.material.stage import ShaderStage
-from lazurite.material.platform import ShaderPlatform
-from lazurite.material.shader_pass.bgfx_shader import BgfxShader
-from lazurite.tempfile import CustomTempFile
-
-from .macro_define import MacroDefine
-
-
-class ShadercCompiler:
-    shaderc_path: str
-
-    def __init__(self, shaderc_paths: list[str] | str = None) -> None:
-        if shaderc_paths is None:
-            shaderc_paths = ["shaderc", "./shaderc"]
-        elif isinstance(shaderc_paths, str):
-            shaderc_paths = [shaderc_paths]
-
-        self.shaderc_path = ""
-
-        for path in shaderc_paths:
-            try:
-                result = subprocess.run([path, "-v"], capture_output=True)
-            except FileNotFoundError:
-                pass
-            else:
-                self.shaderc_path = path
-                break
-
-        if not self.shaderc_path:
-            raise Exception(
-                f"Error! No valid SHADERC compiler was found in the list {shaderc_paths}"
-            )
-
-        if result.returncode:
-            print(result.stdout.decode())
-            print(result.stderr.decode())
-            result.check_returncode()
-
-    def compile(
-        self,
-        file: str,
-        platform: ShaderPlatform = ShaderPlatform.ESSL_310,
-        stage: ShaderStage = ShaderStage.Fragment,
-        varying_def: str = None,
-        include: list[str] = None,
-        defines: list[MacroDefine] = None,
-        options: list[str] = None,
-    ) -> BgfxShader:
-        args = [self.shaderc_path]
-
-        args.extend(("-f", file))
-
-        device = ""
-        if platform == ShaderPlatform.Metal:
-            device = "ios"
-        elif platform.name.startswith("ESSL"):
-            device = "android"
-        elif platform.name.startswith("GLSL"):
-            device = "linux"
-        elif platform.name.startswith("Direct3D"):
-            device = "windows"
-        if device:
-            args.extend(("--platform", device))
-
-        profile = ""
-        if platform == ShaderPlatform.Direct3D_SM40:
-            profile = "s_4_0"
-        elif platform == ShaderPlatform.Vulkan:
-            profile = "spirv"
-        elif platform in {ShaderPlatform.Metal, ShaderPlatform.PSSL}:
-            profile = platform.name.lower()
-        elif platform.name.startswith("Direct3D_SM"):
-            profile = "s_5_0"
-        elif platform.name.startswith("GLSL"):
-            profile = platform.name.removeprefix("GLSL_")
-        elif platform.name.startswith("ESSL"):
-            profile = platform.name.removeprefix("ESSL_") + "_es"
-        if profile:
-            args.extend(("-p", profile))
-
-        args.append("--type")
-        if stage == ShaderStage.Compute:
-            args.append("compute")
-        elif stage == ShaderStage.Vertex:
-            args.append("vertex")
-        else:
-            args.append("fragment")
-
-        if varying_def is not None:
-            args.extend(("--varyingdef", varying_def))
-
-        if include:
-            for item in include:
-                args.extend(("-i", item))
-
-        if defines:
-            args.extend(("--define", ";".join(d.format_bgfx() for d in defines)))
-
-        if options:
-            args.extend(options)
-
-        with CustomTempFile() as f:
-            args.extend(("-o", f.name))
-
-            result = subprocess.run(args, capture_output=True)
-
-            if result.stderr:
-                print(result.stderr.decode())
-            if result.stdout:
-                print(result.stdout.decode())
-
-            result.check_returncode()
-
-            bgfx_shader = BgfxShader()
-            bgfx_shader.read(f, platform, stage)
-
-        return bgfx_shader
-
-
-def generate_bgfx_defines(platform: ShaderPlatform, stage: ShaderStage):
-    keys = [
-        # Platform
-        "BX_PLATFORM_ANDROID",
-        "BX_PLATFORM_EMSCRIPTEN",
-        "BX_PLATFORM_IOS",
-        "BX_PLATFORM_LINUX",
-        "BX_PLATFORM_OSX",
-        "BX_PLATFORM_PS4",
-        "BX_PLATFORM_WINDOWS",
-        "BX_PLATFORM_XBOXONE",
-        # Language
-        "BGFX_SHADER_LANGUAGE_GLSL",
-        "BGFX_SHADER_LANGUAGE_HLSL",
-        "BGFX_SHADER_LANGUAGE_METAL",
-        "BGFX_SHADER_LANGUAGE_PSSL",
-        "BGFX_SHADER_LANGUAGE_SPIRV",
-        # Stage
-        "BGFX_SHADER_TYPE_COMPUTE",
-        "BGFX_SHADER_TYPE_FRAGMENT",
-        "BGFX_SHADER_TYPE_VERTEX",
-    ]
-
-    defines = {key: 0 for key in keys}
-
-    # Stage
-    if stage == ShaderStage.Compute:
-        defines["BGFX_SHADER_TYPE_COMPUTE"] = 1
-    elif stage == ShaderStage.Vertex:
-        defines["BGFX_SHADER_TYPE_VERTEX"] = 1
-    else:
-        defines["BGFX_SHADER_TYPE_FRAGMENT"] = 1
-
-    # Platform & language
-    if platform == ShaderPlatform.Metal:
-        defines["BX_PLATFORM_IOS"] = 1
-        defines["BGFX_SHADER_LANGUAGE_METAL"] = 1
-
-    elif platform.name.startswith("ESSL"):
-        defines["BX_PLATFORM_ANDROID"] = 1
-        defines["BGFX_SHADER_LANGUAGE_GLSL"] = int(platform.name.removeprefix("ESSL_"))
-
-    elif platform.name.startswith("GLSL"):
-        defines["BX_PLATFORM_LINUX"] = 1
-        defines["BGFX_SHADER_LANGUAGE_GLSL"] = int(platform.name.removeprefix("GLSL_"))
-
-    elif platform.name.startswith("Direct3D"):
-        defines["BX_PLATFORM_WINDOWS"] = 1
-        defines["BGFX_SHADER_LANGUAGE_HLSL"] = (
-            400 if platform == ShaderPlatform.Direct3D_SM40 else 500
-        )
-
-    elif platform == ShaderPlatform.PSSL:
-        defines["BX_PLATFORM_PS4"] = 1
-        defines["BGFX_SHADER_LANGUAGE_PSSL"] = 1
-
-    elif platform == ShaderPlatform.Vulkan:
-        defines["BGFX_SHADER_LANGUAGE_SPIRV"] = 1
-
-    return [MacroDefine(key, value) for key, value in defines.items()]
-
-
-# BX_PLATFORM_ANDROID 0 1
-# BX_PLATFORM_EMSCRIPTEN 0 1
-# BX_PLATFORM_IOS 0 1
-# BX_PLATFORM_LINUX 0 1
-# BX_PLATFORM_OSX 0 1
-# BX_PLATFORM_PS4 0 1
-# BX_PLATFORM_WINDOWS 0 1
-# BX_PLATFORM_XBOXONE 0 1
-
-# BGFX_SHADER_LANGUAGE_GLSL (ESSL) id [120] 130 140 150 330 400 410 420 [430] 440 ESSL [100] [300] [310] 320
-# BGFX_SHADER_LANGUAGE_HLSL id 300 [400] [500]
-# BGFX_SHADER_LANGUAGE_METAL 0 1 for ios id for osx 1000
-# BGFX_SHADER_LANGUAGE_PSSL 0 1 1000
-# BGFX_SHADER_LANGUAGE_SPIRV 0 1 id [1010] 1311 1411 1512 1613
-
-# BGFX_SHADER_TYPE_COMPUTE 0 1
-# BGFX_SHADER_TYPE_FRAGMENT 0 1
-# BGFX_SHADER_TYPE_VERTEX 0 1
+import subprocess
+
+from lazurite.material.stage import ShaderStage
+from lazurite.material.platform import ShaderPlatform
+from lazurite.material.shader_pass.bgfx_shader import BgfxShader
+from lazurite.tempfile import CustomTempFile
+
+from .macro_define import MacroDefine
+
+
+class ShadercCompiler:
+    shaderc_path: str
+
+    def __init__(self, shaderc_paths: list[str] | str = None) -> None:
+        if shaderc_paths is None:
+            shaderc_paths = ["shaderc", "./shaderc"]
+        elif isinstance(shaderc_paths, str):
+            shaderc_paths = [shaderc_paths]
+
+        self.shaderc_path = ""
+
+        for path in shaderc_paths:
+            try:
+                result = subprocess.run([path, "-v"], capture_output=True)
+            except FileNotFoundError:
+                pass
+            else:
+                self.shaderc_path = path
+                break
+
+        if not self.shaderc_path:
+            raise Exception(
+                f"Error! No valid SHADERC compiler was found in the list {shaderc_paths}"
+            )
+
+        if result.returncode:
+            print(result.stdout.decode())
+            print(result.stderr.decode())
+            result.check_returncode()
+
+    def compile(
+        self,
+        file: str,
+        platform: ShaderPlatform = ShaderPlatform.ESSL_310,
+        stage: ShaderStage = ShaderStage.Fragment,
+        varying_def: str = None,
+        include: list[str] = None,
+        defines: list[MacroDefine] = None,
+        options: list[str] = None,
+    ) -> BgfxShader:
+        args = [self.shaderc_path]
+
+        args.extend(("-f", file))
+
+        device = ""
+        if platform == ShaderPlatform.Metal:
+            device = "ios"
+        elif platform.name.startswith("ESSL"):
+            device = "android"
+        elif platform.name.startswith("GLSL"):
+            device = "linux"
+        elif platform.name.startswith("Direct3D"):
+            device = "windows"
+        if device:
+            args.extend(("--platform", device))
+
+        profile = ""
+        if platform == ShaderPlatform.Direct3D_SM40:
+            profile = "s_4_0"
+        elif platform == ShaderPlatform.Vulkan:
+            profile = "spirv"
+        elif platform in {ShaderPlatform.Metal, ShaderPlatform.PSSL}:
+            profile = platform.name.lower()
+        elif platform.name.startswith("Direct3D_SM"):
+            profile = "s_5_0"
+        elif platform.name.startswith("GLSL"):
+            profile = platform.name.removeprefix("GLSL_")
+        elif platform.name.startswith("ESSL"):
+            profile = platform.name.removeprefix("ESSL_") + "_es"
+        if profile:
+            args.extend(("-p", profile))
+
+        args.append("--type")
+        if stage == ShaderStage.Compute:
+            args.append("compute")
+        elif stage == ShaderStage.Vertex:
+            args.append("vertex")
+        else:
+            args.append("fragment")
+
+        if varying_def is not None:
+            args.extend(("--varyingdef", varying_def))
+
+        if include:
+            for item in include:
+                args.extend(("-i", item))
+
+        if defines:
+            args.extend(("--define", ";".join(d.format_bgfx() for d in defines)))
+
+        if options:
+            args.extend(options)
+
+        with CustomTempFile() as f:
+            args.extend(("-o", f.name))
+
+            result = subprocess.run(args, capture_output=True)
+
+            if result.stderr:
+                print(result.stderr.decode())
+            if result.stdout:
+                print(result.stdout.decode())
+
+            result.check_returncode()
+
+            bgfx_shader = BgfxShader()
+            bgfx_shader.read(f, platform, stage)
+
+        return bgfx_shader
+
+
+def generate_bgfx_defines(platform: ShaderPlatform, stage: ShaderStage):
+    keys = [
+        # Platform
+        "BX_PLATFORM_ANDROID",
+        "BX_PLATFORM_EMSCRIPTEN",
+        "BX_PLATFORM_IOS",
+        "BX_PLATFORM_LINUX",
+        "BX_PLATFORM_OSX",
+        "BX_PLATFORM_PS4",
+        "BX_PLATFORM_WINDOWS",
+        "BX_PLATFORM_XBOXONE",
+        # Language
+        "BGFX_SHADER_LANGUAGE_GLSL",
+        "BGFX_SHADER_LANGUAGE_HLSL",
+        "BGFX_SHADER_LANGUAGE_METAL",
+        "BGFX_SHADER_LANGUAGE_PSSL",
+        "BGFX_SHADER_LANGUAGE_SPIRV",
+        # Stage
+        "BGFX_SHADER_TYPE_COMPUTE",
+        "BGFX_SHADER_TYPE_FRAGMENT",
+        "BGFX_SHADER_TYPE_VERTEX",
+    ]
+
+    defines = {key: 0 for key in keys}
+
+    # Stage
+    if stage == ShaderStage.Compute:
+        defines["BGFX_SHADER_TYPE_COMPUTE"] = 1
+    elif stage == ShaderStage.Vertex:
+        defines["BGFX_SHADER_TYPE_VERTEX"] = 1
+    else:
+        defines["BGFX_SHADER_TYPE_FRAGMENT"] = 1
+
+    # Platform & language
+    if platform == ShaderPlatform.Metal:
+        defines["BX_PLATFORM_IOS"] = 1
+        defines["BGFX_SHADER_LANGUAGE_METAL"] = 1
+
+    elif platform.name.startswith("ESSL"):
+        defines["BX_PLATFORM_ANDROID"] = 1
+        defines["BGFX_SHADER_LANGUAGE_GLSL"] = int(platform.name.removeprefix("ESSL_"))
+
+    elif platform.name.startswith("GLSL"):
+        defines["BX_PLATFORM_LINUX"] = 1
+        defines["BGFX_SHADER_LANGUAGE_GLSL"] = int(platform.name.removeprefix("GLSL_"))
+
+    elif platform.name.startswith("Direct3D"):
+        defines["BX_PLATFORM_WINDOWS"] = 1
+        defines["BGFX_SHADER_LANGUAGE_HLSL"] = (
+            400 if platform == ShaderPlatform.Direct3D_SM40 else 500
+        )
+
+    elif platform == ShaderPlatform.PSSL:
+        defines["BX_PLATFORM_PS4"] = 1
+        defines["BGFX_SHADER_LANGUAGE_PSSL"] = 1
+
+    elif platform == ShaderPlatform.Vulkan:
+        defines["BGFX_SHADER_LANGUAGE_SPIRV"] = 1
+
+    return [MacroDefine(key, value) for key, value in defines.items()]
+
+
+# BX_PLATFORM_ANDROID 0 1
+# BX_PLATFORM_EMSCRIPTEN 0 1
+# BX_PLATFORM_IOS 0 1
+# BX_PLATFORM_LINUX 0 1
+# BX_PLATFORM_OSX 0 1
+# BX_PLATFORM_PS4 0 1
+# BX_PLATFORM_WINDOWS 0 1
+# BX_PLATFORM_XBOXONE 0 1
+
+# BGFX_SHADER_LANGUAGE_GLSL (ESSL) id [120] 130 140 150 330 400 410 420 [430] 440 ESSL [100] [300] [310] 320
+# BGFX_SHADER_LANGUAGE_HLSL id 300 [400] [500]
+# BGFX_SHADER_LANGUAGE_METAL 0 1 for ios id for osx 1000
+# BGFX_SHADER_LANGUAGE_PSSL 0 1 1000
+# BGFX_SHADER_LANGUAGE_SPIRV 0 1 id [1010] 1311 1411 1512 1613
+
+# BGFX_SHADER_TYPE_COMPUTE 0 1
+# BGFX_SHADER_TYPE_FRAGMENT 0 1
+# BGFX_SHADER_TYPE_VERTEX 0 1
```

### Comparing `lazurite-0.1.4/src/lazurite/decompiler/macro_decompiler.py` & `lazurite-0.1.5/src/lazurite/decompiler/macro_decompiler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,770 +1,773 @@
-from dataclasses import dataclass
-import myers
-import sympy
-import time
-import copy
-import io
-import re
-
-
-from lazurite import util
-
-
-@dataclass
-class Variant:
-    """
-    Decompiler input struct, containing code and flags.
-    """
-
-    flags: dict[str, str]
-    code: str
-
-
-class Shader:
-    """
-    Class, responsible for storing intermediate representations of a shader.
-    """
-
-    codes: list[list[int]] | list[str]
-    flags: list[set[int]]
-    combined_code: list[int]
-    line_conditions: list[set[int]]
-    chunks: list[tuple[int, int]] | list[tuple[int, int, int]]
-    is_struct: bool
-    all_flags: set[int]
-
-    def __init__(self) -> None:
-        self.codes = []
-        self.flags = []
-        self.chunks = []
-        self.is_struct = False
-        self.combined_code = []
-        self.line_conditions = []
-
-    def load(
-        self,
-        variants: list[Variant],
-        remove_comments=True,
-        preprocess=True,
-    ):
-        """
-        Loads and processes shader variants into codes and flags arrays.
-        """
-        self.codes = []
-        self.flags = []
-        for i, variant in enumerate(variants):
-            code = variant.code
-            if remove_comments:
-                code = re.sub(r"//.*\n", "", code)
-                code = re.sub(r"/\*.*?\*/", "", code, flags=re.DOTALL)
-                code = re.sub(r"\n\n+", "\n", code)
-            if preprocess:
-                code = _preprocess_shader(code)
-            self.codes.append(code)
-            self.flags.append({i})
-
-    def uniquify(self):
-        """
-        Removes duplicate codes and combines their flags, also creates `all_flags` array with all flags.
-        """
-        codes: list[str] = []
-        flags: list[set[int]] = []
-        all_flags = set()
-        for index, code in enumerate(self.codes):
-            try:
-                i = codes.index(code)
-            except ValueError:
-                i = len(codes)
-                codes.append(code)
-                flags.append(set())
-            flags[i].update(self.flags[index])
-            all_flags.update(self.flags[index])
-        self.all_flags = all_flags
-        self.codes = codes
-        self.flags = flags
-
-    def encode(self, line_decode_table: dict[str, int]):
-        """
-        Encodes shader as an array of line indices, while saving line-index mapping in `line_decode_table`.
-        """
-        for i, code in enumerate(self.codes):
-            lines = code.splitlines()
-            encoded_shader = []
-            for line in lines:
-                line_index = line_decode_table.get(line)
-                if line_index is None:
-                    line_index = len(line_decode_table)
-                    line_decode_table[line] = line_index
-                encoded_shader.append(line_index)
-            self.codes[i] = encoded_shader
-
-    def diff(self):
-        """
-        Compute combined diff of all shader variants. Populates `combined_code` and `line_conditions`.
-        """
-        combined_code: list[int] = []
-        line_conditions: list[set[int]] = []
-        for i, code in enumerate(self.codes):
-            diff = myers.diff(combined_code, code)
-            combined_code = []
-            new_conditions = []
-            current_index = 0
-            for op, val in diff:
-                combined_code.append(val)
-                if op == "i":
-                    new_conditions.append(copy.copy(self.flags[i]))
-                elif op == "r":
-                    new_conditions.append(line_conditions[current_index])
-                    current_index += 1
-                elif op == "k":
-                    condition_set = line_conditions[current_index]
-                    condition_set.update(self.flags[i])
-                    new_conditions.append(condition_set)
-                    current_index += 1
-
-            line_conditions = new_conditions
-        self.combined_code = combined_code
-        self.line_conditions = line_conditions
-
-    def group_lines(self):
-        """
-        Groups lines with the same condition into chunks, populates `Shader.chunks` list.
-        """
-        start = 0
-        chunks: list[tuple[int, int]] = []
-        end = len(self.line_conditions) - 1
-        current_condition = self.line_conditions[0]
-        for i, condition in enumerate(self.line_conditions):
-            if i == end:
-                if current_condition != condition:
-                    chunks.append((start, i))
-                    chunks.append((i, i + 1))
-                else:
-                    chunks.append((start, i + 1))
-            elif current_condition != condition:
-                chunks.append((start, i))
-                start = i
-                current_condition = condition
-        self.chunks = chunks
-
-    def generate_calc_list(self, calc_list: list[tuple[set[int], set[int]]]):
-        """
-        Populates `calc_list` with unique calculations that need to be performed, adds calculation index to each chunk.
-        """
-        for index, (start, end) in enumerate(self.chunks):
-            condition = self.line_conditions[start]
-            found = False
-            try:
-                calc_index = calc_list.index((self.all_flags, condition))
-            except ValueError:
-                calc_index = len(calc_list)
-            else:
-                found = True
-
-            if len(condition) == len(self.all_flags):
-                calc_index = -1  # This line is always unconditionally present.
-            elif not found:
-                calc_list.append((self.all_flags, condition))
-
-            self.chunks[index] = (start, end, calc_index)
-
-    def assemble_code(self, calc_final, line_decode_table):
-        """
-        Creates a final code string with macros.
-        """
-        string_pipe = io.StringIO()
-        for start, end, calc in self.chunks:
-            has_condition = calc != -1
-
-            if has_condition:
-                string_pipe.write(calc_final[calc] + "\n")
-
-            for i in range(start, end):
-                string_pipe.write(line_decode_table[self.combined_code[i]] + "\n")
-
-            if has_condition:
-                string_pipe.write("#endif\n")
-        string_pipe.seek(0)
-        return string_pipe.read()
-
-
-def _extract_functions(
-    code: str, functions: dict[str, tuple[bool, Shader]], flags: set[int]
-):
-    """
-    Extracts functions and structs from shader, storing them as separate individual shaders and replacing them in main shader.
-    """
-    re_func_start = re.compile(
-        r"^[\s]*?([^#\s][\w]+)[\s]+([\w]+)[\s]*\(([^;]*?)\)[\s]*{",
-        re.DOTALL | re.MULTILINE,
-    )
-    func_start = re.search(re_func_start, code)
-    modified_text = ""
-
-    # Extract functions.
-    while func_start:
-        groups = func_start.groups()
-        args = groups[2].replace("\n", "")
-        name = f"{groups[0]} {groups[1]}({args})"
-
-        modified_text += code[: func_start.start()]
-
-        bracket_balance = 1
-        for i in range(func_start.end(), len(code)):
-            c = code[i]
-            if c == "{":
-                bracket_balance += 1
-            elif c == "}":
-                bracket_balance -= 1
-
-            if not bracket_balance:
-                content = code[func_start.end() : i]
-                code = code[i + 1 :]
-                break
-        if bracket_balance:
-            break
-
-        func = functions.get(name)
-
-        if not func:
-            func = Shader()
-            functions[name] = func
-
-        modified_text += f"START_NAME|||{name}|||END_NAME\n"
-
-        func.codes.append(content)
-        func.flags.append(copy.copy(flags))
-
-        func_start = re.search(re_func_start, code)
-
-    code = modified_text + code
-
-    # Extract structs.
-    match: re.Match
-    for match in re.finditer(
-        r"^[\s]*?struct[\s]+([\w]+)[\s]*{(.*?)};", code, re.DOTALL | re.MULTILINE
-    ):
-        name, contents = match.groups()
-        name = "struct " + name
-
-        struct = functions.get(name)
-        if not struct:
-            struct = Shader()
-            struct.is_struct = True
-            functions[name] = struct
-
-        struct.codes.append(contents)
-        struct.flags.append(copy.copy(flags))
-
-        code = code.replace(match.group(), f"START_NAME|||{name}|||END_NAME\n")
-
-    return code
-
-
-def _evaluate_condition(condition: list[set[bool, bool, int, int]], flag: list[int]):
-    value = False
-    for c in condition:
-        a = flag[c[2]] == c[3]
-        if c[0]:
-            a = not a
-        if c[1]:
-            value = value and a
-        else:
-            value = value or a
-
-    return value
-
-
-def _calculate_condition_score(
-    expr: list[set[bool, bool, int, int]],
-    conditions: tuple[set[int], set[int]],
-    flags: list[list[int]],
-):
-    score = 0
-    for flag in conditions[0]:
-        goal = flag in conditions[1]
-
-        score += 1 if goal == _evaluate_condition(expr, flags[flag]) else -1
-
-    return score
-
-
-def _increment_expr(expr: list[list[bool, bool, int, int]], flag_def: list[int]):
-    for i, val in enumerate(expr):
-        if not val[1] and i:
-            val[1] = True
-            return
-        val[1] = False
-
-        if val[3] + 1 < flag_def[val[2]]:
-            val[3] += 1
-            return
-        val[3] = 0
-
-        if not val[0]:
-            val[0] = True
-            return
-        val[0] = False
-
-        if val[2] + 1 < len(flag_def):
-            val[2] += 1
-            return
-        val[2] = 0
-
-    expr.append([False, False, 0, 0])
-
-
-def _slow_search(
-    conditions: tuple[set[int], set[int]],
-    flags: list[list[int]],
-    flag_def: list[int],
-    timeout: float = 10,
-):
-    """
-    Slow brute-force search that scores all possible expression combinations.
-    """
-    # (bool NOT, bool AND/OR, flag_index, flag_value)
-
-    expression = [[False, False, 0, 0]]
-    best_score = -10000
-    best_expr = []
-
-    t = time.perf_counter()
-    while len(expression) <= len(flag_def) + 5:
-        score = _calculate_condition_score(expression, conditions, flags)
-
-        if score > best_score:
-            best_score = score
-            best_expr = copy.deepcopy(expression)
-
-        if score == len(conditions[0]):
-            return True, expression, score
-
-        _increment_expr(expression, flag_def)
-
-        if time.perf_counter() - t > timeout:
-            break
-
-    return False, best_expr, best_score
-
-
-def _fast_search(
-    conditions: tuple[set[int], set[int]], flags: list[list[int]], flag_def: list[int]
-) -> tuple[bool, list, int]:
-    """
-    Fast search that calculates best score for each new token.
-    """
-    # (bool NOT, bool AND/OR, flag_index, flag_value)
-
-    best = -10000
-    best_expr = []
-    local_best_expr = []
-    expression = []
-    for _ in range(len(flag_def) + 5):
-        expression = copy.deepcopy(local_best_expr)
-        expression.append([False, False, 0, 0])
-
-        local_best = -10000
-        local_best_expr = []
-
-        for i in range(4):
-            if len(expression) == 1 and i >= 2:
-                break
-            expression[-1][0] = i % 2 == 1
-            expression[-1][1] = i / 2 >= 1
-            for flag_index, flag in enumerate(flag_def):
-                expression[-1][2] = flag_index
-                for value in range(flag):
-                    expression[-1][3] = value
-
-                    score = _calculate_condition_score(expression, conditions, flags)
-                    if score > local_best:
-                        local_best = score
-                        local_best_expr = copy.deepcopy(expression)
-
-        if local_best > best:
-            best = local_best
-            best_expr = copy.deepcopy(local_best_expr)
-            if best == len(conditions[0]):
-                return True, best_expr, best
-    return False, best_expr, best
-
-
-def _convert_to_sympy_expression(
-    expression: list[set[bool, bool, int, int]],
-    inverse_flag_def: list[tuple[str, list[str]]],
-):
-    expr = sympy.false
-    for e in expression:
-        flag, values = inverse_flag_def[e[2]]
-        value = values[e[3]]
-        is_pass = flag == "pass"
-        if is_pass:
-            flag = util.generate_pass_name_macro(value)
-        else:
-            is_bool = False
-            # is_bool = set(values) in [
-            #     {"On", "Off"},
-            #     {"Enabled", "Disabled"},
-            # ]
-            if flag.startswith("f_"):
-                flag = flag.removeprefix("f_")
-                flag = util.generate_flag_name_macro(flag, value, is_bool)
-            else:
-                flag = util.format_definition_name(flag + value)
-
-        a = sympy.symbols(flag)
-
-        # if not is_pass and is_bool and value in {"Off", "Disabled"}:
-        #     a = ~a
-
-        if e[0]:
-            a = ~a
-        if e[1]:
-            expr = expr & a
-        else:
-            expr = expr | a
-
-    return expr
-
-
-def _format_expression(expr: str):
-    """
-    Formats stringified sympy expression according to GLSL macro format.
-    """
-    expr = expr.replace("~", "!").replace("|", "||").replace("&", "&&")
-    expr = re.sub(r"(\w+)", r"defined(\1)", expr)
-    return expr
-
-
-def _convert_from_dict_to_list(line_decode_table: dict[str, int]):
-    l = [""] * len(line_decode_table)
-    for line, i in line_decode_table.items():
-        l[i] = line
-    return l
-
-
-def restore_code(
-    variants: list[Variant],
-    remove_comments=True,
-    process_shaders=False,
-    search_timeout: float = 10,
-) -> tuple[set[str], str]:
-    """
-    Attempts to restore original shader source, by combining variants while adding missing macros.
-    """
-    main_shader = Shader()
-    main_shader.load(variants, remove_comments, process_shaders)
-    main_shader.uniquify()
-
-    functions: dict[str, Shader] = {}
-    for i, (code, flags) in enumerate(zip(main_shader.codes, main_shader.flags)):
-        main_shader.codes[i] = _extract_functions(code, functions, flags)
-
-    for _, func in functions.items():
-        func.uniquify()
-
-    code_flag_list = [copy.copy(v.flags) for v in variants]
-
-    line_decode_table = {}
-    main_shader.encode(line_decode_table)
-
-    for _, func in functions.items():
-        func.encode(line_decode_table)
-
-    line_decode_table = _convert_from_dict_to_list(line_decode_table)
-
-    # { name: (index, [values]) }
-    flag_definition: dict[str, tuple[int, list[str]]] = {}
-    for variant in variants:
-        for name, value in variant.flags.items():
-            definition = flag_definition.get(name)
-            if definition is None:
-                flag_definition[name] = (len(flag_definition), [value])
-            else:
-                value_list = definition[1]
-                if value not in value_list:
-                    value_list.append(value)
-
-    keys_to_remove = []
-    for name, (_, value_list) in flag_definition.items():
-        # Remove flags with a single value.
-        if len(value_list) <= 1:
-            keys_to_remove.append(name)
-        # Bias against disabling
-        for i in {"Off", "Disabled"}:
-            if i in value_list:
-                value_list.remove(i)
-                value_list.append(i)
-        # Bias towards enabling
-        for i in {"On", "Enabled"}:
-            if i in value_list:
-                value_list.remove(i)
-                value_list.insert(0, i)
-    for key in keys_to_remove:
-        flag_definition.pop(key)
-    for flags in code_flag_list:
-        for key in keys_to_remove:
-            flags.pop(key)
-
-    # Re-populate flag indices.
-    for index, (flag, (_, values)) in enumerate(flag_definition.items()):
-        flag_definition[flag] = (index, values)
-
-    main_shader.diff()
-    main_shader.group_lines()
-
-    for _, func in functions.items():
-        func.diff()
-        func.group_lines()
-
-    calc_list: list[tuple[set[int], set[int]]] = []
-    main_shader.generate_calc_list(calc_list)
-    for _, func in functions.items():
-        func.generate_calc_list(calc_list)
-
-    encoded_flags: list[list[int]] = []
-    for flags in code_flag_list:
-        encoded_flag = [-1] * len(flag_definition)
-        for name, value in flags.items():
-            name_index, value_list = flag_definition[name]
-            encoded_flag[name_index] = value_list.index(value)
-        encoded_flags.append(encoded_flag)
-
-    encoded_flag_def = [0] * len(flag_definition)
-    for _, (index, values) in flag_definition.items():
-        encoded_flag_def[index] = len(values)
-
-    inverse_flag_def: list[tuple[str, list[str]]] = [0] * len(flag_definition)
-    for flag, (index, values) in flag_definition.items():
-        inverse_flag_def[index] = (flag, values)
-
-    macro_pattern = re.compile(r"\w+")
-    macro_set = set()
-    calc_result = []
-    calc_result_formatted = []
-    calc_final = []
-    for i, calc in enumerate(calc_list):
-        success, expr, score = _fast_search(calc, encoded_flags, encoded_flag_def)
-        if not success:
-            print("slow search")
-            success, expr_slow, score_slow = _slow_search(
-                calc, encoded_flags, encoded_flag_def, search_timeout
-            )
-            if not success:
-                print("not found")
-            if success or score_slow > score:
-                expr = expr_slow
-                score = score_slow
-
-        result = _convert_to_sympy_expression(expr, inverse_flag_def)
-        try:
-            index = calc_result.index(result)
-        except ValueError:
-            index = len(calc_result)
-            calc_result.append(result)
-            result = sympy.simplify_logic(result, force=True)
-            str_result = str(result)
-            macro_set.update(set(re.findall(macro_pattern, str_result)))
-            if len(result.atoms()) == 1:
-                if str_result.startswith("~"):
-                    str_result = "#ifndef " + str_result.removeprefix("~")
-                else:
-                    str_result = "#ifdef " + str_result
-            else:
-                str_result = "#if " + _format_expression(str_result)
-            if not success:
-                str_result = f"// Approximation, matches {score} cases out of {len(calc[0])}\n{str_result}"
-
-            calc_result_formatted.append(str_result)
-
-        calc_final.append(calc_result_formatted[index])
-
-    main_code = main_shader.assemble_code(calc_final, line_decode_table)
-
-    for name, func in functions.items():
-        code = func.assemble_code(calc_final, line_decode_table)
-        if not code.startswith("\n"):
-            code = "\n" + code
-
-        main_code = main_code.replace(
-            f"START_NAME|||{name}|||END_NAME",
-            f"{name} {{{code}}}" + (";" if func.is_struct else ""),
-        )
-
-    if process_shaders:
-        main_code = _postprocess_shader(main_code)
-
-    return macro_set, main_code
-
-
-def _preprocess_shader(shader: str):
-    """
-    Pre-processes plain text shader code to convert it from GLSL to BGFX SC.\n
-    Removes built-in `u_` uniforms, replaces `gl_FragColor` and `gl_FragData`,
-    replaces attributes and varyings with `$input` and `$output`, removes macros,
-    replaces samplers with BGFX AUTOREG macros, adds NUM_THREADS to compute shaders.
-    """
-    shader = re.sub(r"^uniform\s+\w+\s+u_[\w[\]]+;\n", "", shader, flags=re.MULTILINE)
-
-    shader = re.sub(r"(\W)bgfx_FragColor(\W)", r"\1gl_FragColor\2", shader)
-    shader = re.sub(r"(\W)bgfx_FragData(\W)", r"\1gl_FragData\2", shader)
-
-    shader = re.sub(r"^out\s.+?;\n", "", shader, flags=re.MULTILINE)
-
-    is_vertex_stage = bool(
-        re.search(r"^#define varying out$", shader, flags=re.MULTILINE)
-    )
-
-    shader = re.sub(r"^#define\s.+?\n", "", shader, flags=re.MULTILINE)
-    shader = re.sub(r"^#if\s.+?#endif\n", "", shader, flags=re.MULTILINE | re.DOTALL)
-    shader = re.sub(r"^#extension\s.+?\n", "", shader, flags=re.MULTILINE)
-
-    shader = re.sub(
-        r"^[\s\w]*?varying\s.+? (\w+);$",
-        r"$output \1" if is_vertex_stage else r"$input \1",
-        shader,
-        flags=re.MULTILINE,
-    )
-    shader = re.sub(
-        r"^[\s\w]*?attribute\s.+? (\w+);$", r"$input \1", shader, flags=re.MULTILINE
-    )
-
-    shader = re.sub(r"^#version\s.+?\n", "", shader)
-
-    samplers = [
-        (r"lowp sampler2D", r"SAMPLER2D"),
-        (r"highp sampler2DMS", r"SAMPLER2DMS"),
-        (r"highp sampler3D", r"SAMPLER3D"),
-        (r"lowp samplerCube", r"SAMPLERCUBE"),
-        (r"highp sampler2DShadow", r"SAMPLER2DSHADOW"),
-        (r"highp sampler2D", r"SAMPLER2D_HIGHP"),
-        (r"highp samplerCube", r"SAMPLERCUBE_HIGHP"),
-        (r"highp sampler2DArray", r"SAMPLER2DARRAY"),
-        (r"highp sampler2DMSArray", r"SAMPLER2DMSARRAY"),
-        (r"highp samplerCubeArray", r"SAMPLERCUBEARRAY"),
-        (r"highp sampler2DArrayShadow", r"SAMPLER2DARRAYSHADOW"),
-        (r"highp isampler2D", r"ISAMPLER2D"),
-        (r"highp usampler2D", r"USAMPLER2D"),
-        (r"highp isampler3D", r"ISAMPLER3D"),
-    ]
-
-    for pattern, repl in samplers:
-        pattern = r"^uniform " + pattern + r" (\w+);"
-        repl = repl + r"_AUTOREG(\1);"
-        shader = shader = re.sub(pattern, repl, shader, flags=re.MULTILINE)
-
-    shader = shader = re.sub(
-        r"^layout\(std430, .+?\) readonly buffer (\w+) { (\w+) .+? }",
-        r"BUFFER_RO_AUTOREG(\1, \2);",
-        shader,
-        flags=re.MULTILINE,
-    )
-    shader = shader = re.sub(
-        r"^layout\(std430, .+?\) writeonly buffer (\w+) { (\w+) .+? }",
-        r"BUFFER_WR_AUTOREG(\1, \2);",
-        shader,
-        flags=re.MULTILINE,
-    )
-    shader = shader = re.sub(
-        r"^layout\(std430, .+?\) buffer (\w+) { (\w+) .+? }",
-        r"BUFFER_RW_AUTOREG(\1, \2)",
-        shader,
-        flags=re.MULTILINE,
-    )
-
-    for i, access in enumerate(("readonly ", "writeonly ", "")):
-        for prefix in "iu":
-            prefix = "u" if prefix == "u" else ""
-            access_id = ("RO", "WR", "RW")[i]
-
-            name = f"{prefix.upper()}IMAGE2D_{access_id}_AUTOREG"
-            shader = re.sub(
-                r"^layout\((.+?), .+?\) "
-                + access
-                + "uniform highp "
-                + prefix
-                + r"image2D (\w+)",
-                name + r"(\2, \1)",
-                shader,
-                flags=re.MULTILINE,
-            )
-
-            name = f"{prefix.upper()}IMAGE2D_ARRAY_{access_id}_AUTOREG"
-            shader = re.sub(
-                r"^layout\((.+?), .+?\) "
-                + access
-                + "uniform highp "
-                + prefix
-                + r"image2DArray (\w+)",
-                name + r"(\2, \1)",
-                shader,
-                flags=re.MULTILINE,
-            )
-
-            name = f"{prefix.upper()}IMAGE3D_{access_id}_AUTOREG"
-            shader = re.sub(
-                r"^layout\((.+?), .+?\) "
-                + access
-                + "uniform highp "
-                + prefix
-                + r"image3D (\w+)",
-                name + r"(\2, \1)",
-                shader,
-                flags=re.MULTILINE,
-            )
-
-    shader = re.sub(
-        r"^layout \(local_size_x = (\d+), local_size_y = (\d+), local_size_z = (\d+)\) in;",
-        r"NUM_THREADS(\1, \2, \3)",
-        shader,
-        flags=re.MULTILINE,
-    )
-
-    return shader
-
-
-def _postprocess_shader(shader: str):
-    """
-    Post-processes plain text shader code to convert it from GLSL to BGFX SC.\n
-    Merges `$input` and `$output` declarations together and adds `// Attention!`
-    comment to potential array access and matrix multiplication operations.
-    """
-    shader = shader.splitlines(keepends=True)
-
-    new_shader = []
-    args = []
-    line_type = 0  # 0 - none, 1 - input, 2 = output
-    line_prefix = ""
-    for line in shader:
-        if line.startswith("$input "):
-            current_line_type = 1
-            line_prefix = "$input "
-        elif line.startswith("$output "):
-            current_line_type = 2
-            line_prefix = "$output "
-        else:
-            current_line_type = 0
-
-        if line_type:
-            if line_type == current_line_type:
-                args.append(line.removeprefix(line_prefix).removesuffix("\n"))
-            else:
-                new_shader.append(", ".join(args) + "\n")
-        if not line_type or line_type != current_line_type:
-            if current_line_type:
-                args = [line.removesuffix("\n")]
-            else:
-                new_shader.append(line)
-
-        line_type = current_line_type
-    shader = new_shader
-
-    for i, line in enumerate(shader):
-        if ") * (" in line or "][" in line:
-            line = line[:-1] + " // Attention!\n"
-            shader[i] = line
-
-    shader = "".join(shader)
-
-    return shader
+from dataclasses import dataclass
+import myers
+import sympy
+import time
+import copy
+import io
+import re
+
+
+from lazurite import util
+
+
+@dataclass
+class Variant:
+    """
+    Decompiler input struct, containing code and flags.
+    """
+
+    flags: dict[str, str]
+    code: str
+
+
+class Shader:
+    """
+    Class, responsible for storing intermediate representations of a shader.
+    """
+
+    codes: list[list[int]] | list[str]
+    flags: list[set[int]]
+    combined_code: list[int]
+    line_conditions: list[set[int]]
+    chunks: list[tuple[int, int]] | list[tuple[int, int, int]]
+    is_struct: bool
+    all_flags: set[int]
+
+    def __init__(self) -> None:
+        self.codes = []
+        self.flags = []
+        self.chunks = []
+        self.is_struct = False
+        self.combined_code = []
+        self.line_conditions = []
+
+    def load(
+        self,
+        variants: list[Variant],
+        remove_comments=True,
+        preprocess=True,
+    ):
+        """
+        Loads and processes shader variants into codes and flags arrays.
+        """
+        self.codes = []
+        self.flags = []
+        for i, variant in enumerate(variants):
+            code = variant.code
+            if remove_comments:
+                code = re.sub(r"//.*\n", "", code)
+                code = re.sub(r"/\*.*?\*/", "", code, flags=re.DOTALL)
+                code = re.sub(r"\n\n+", "\n", code)
+            if preprocess:
+                code = _preprocess_shader(code)
+            self.codes.append(code)
+            self.flags.append({i})
+
+    def uniquify(self):
+        """
+        Removes duplicate codes and combines their flags, also creates `all_flags` array with all flags.
+        """
+        codes: list[str] = []
+        flags: list[set[int]] = []
+        all_flags = set()
+        for index, code in enumerate(self.codes):
+            try:
+                i = codes.index(code)
+            except ValueError:
+                i = len(codes)
+                codes.append(code)
+                flags.append(set())
+            flags[i].update(self.flags[index])
+            all_flags.update(self.flags[index])
+        self.all_flags = all_flags
+        self.codes = codes
+        self.flags = flags
+
+    def encode(self, line_decode_table: dict[str, int]):
+        """
+        Encodes shader as an array of line indices, while saving line-index mapping in `line_decode_table`.
+        """
+        for i, code in enumerate(self.codes):
+            lines = code.splitlines()
+            encoded_shader = []
+            for line in lines:
+                line_index = line_decode_table.get(line)
+                if line_index is None:
+                    line_index = len(line_decode_table)
+                    line_decode_table[line] = line_index
+                encoded_shader.append(line_index)
+            self.codes[i] = encoded_shader
+
+    def diff(self):
+        """
+        Compute combined diff of all shader variants. Populates `combined_code` and `line_conditions`.
+        """
+        combined_code: list[int] = []
+        line_conditions: list[set[int]] = []
+        for i, code in enumerate(self.codes):
+            diff = myers.diff(combined_code, code)
+            combined_code = []
+            new_conditions = []
+            current_index = 0
+            for op, val in diff:
+                combined_code.append(val)
+                if op == "i":
+                    new_conditions.append(copy.copy(self.flags[i]))
+                elif op == "r":
+                    new_conditions.append(line_conditions[current_index])
+                    current_index += 1
+                elif op == "k":
+                    condition_set = line_conditions[current_index]
+                    condition_set.update(self.flags[i])
+                    new_conditions.append(condition_set)
+                    current_index += 1
+
+            line_conditions = new_conditions
+        self.combined_code = combined_code
+        self.line_conditions = line_conditions
+
+    def group_lines(self):
+        """
+        Groups lines with the same condition into chunks, populates `Shader.chunks` list.
+        """
+        if not self.line_conditions:
+            return
+
+        start = 0
+        chunks: list[tuple[int, int]] = []
+        end = len(self.line_conditions) - 1
+        current_condition = self.line_conditions[0]
+        for i, condition in enumerate(self.line_conditions):
+            if i == end:
+                if current_condition != condition:
+                    chunks.append((start, i))
+                    chunks.append((i, i + 1))
+                else:
+                    chunks.append((start, i + 1))
+            elif current_condition != condition:
+                chunks.append((start, i))
+                start = i
+                current_condition = condition
+        self.chunks = chunks
+
+    def generate_calc_list(self, calc_list: list[tuple[set[int], set[int]]]):
+        """
+        Populates `calc_list` with unique calculations that need to be performed, adds calculation index to each chunk.
+        """
+        for index, (start, end) in enumerate(self.chunks):
+            condition = self.line_conditions[start]
+            found = False
+            try:
+                calc_index = calc_list.index((self.all_flags, condition))
+            except ValueError:
+                calc_index = len(calc_list)
+            else:
+                found = True
+
+            if len(condition) == len(self.all_flags):
+                calc_index = -1  # This line is always unconditionally present.
+            elif not found:
+                calc_list.append((self.all_flags, condition))
+
+            self.chunks[index] = (start, end, calc_index)
+
+    def assemble_code(self, calc_final, line_decode_table):
+        """
+        Creates a final code string with macros.
+        """
+        string_pipe = io.StringIO()
+        for start, end, calc in self.chunks:
+            has_condition = calc != -1
+
+            if has_condition:
+                string_pipe.write(calc_final[calc] + "\n")
+
+            for i in range(start, end):
+                string_pipe.write(line_decode_table[self.combined_code[i]] + "\n")
+
+            if has_condition:
+                string_pipe.write("#endif\n")
+        string_pipe.seek(0)
+        return string_pipe.read()
+
+
+def _extract_functions(
+    code: str, functions: dict[str, tuple[bool, Shader]], flags: set[int]
+):
+    """
+    Extracts functions and structs from shader, storing them as separate individual shaders and replacing them in main shader.
+    """
+    re_func_start = re.compile(
+        r"^[\s]*?([^#\s][\w]+)[\s]+([\w]+)[\s]*\(([^;]*?)\)[\s]*{",
+        re.DOTALL | re.MULTILINE,
+    )
+    func_start = re.search(re_func_start, code)
+    modified_text = ""
+
+    # Extract functions.
+    while func_start:
+        groups = func_start.groups()
+        args = groups[2].replace("\n", "")
+        name = f"{groups[0]} {groups[1]}({args})"
+
+        modified_text += code[: func_start.start()]
+
+        bracket_balance = 1
+        for i in range(func_start.end(), len(code)):
+            c = code[i]
+            if c == "{":
+                bracket_balance += 1
+            elif c == "}":
+                bracket_balance -= 1
+
+            if not bracket_balance:
+                content = code[func_start.end() : i]
+                code = code[i + 1 :]
+                break
+        if bracket_balance:
+            break
+
+        func = functions.get(name)
+
+        if not func:
+            func = Shader()
+            functions[name] = func
+
+        modified_text += f"START_NAME|||{name}|||END_NAME\n"
+
+        func.codes.append(content)
+        func.flags.append(copy.copy(flags))
+
+        func_start = re.search(re_func_start, code)
+
+    code = modified_text + code
+
+    # Extract structs.
+    match: re.Match
+    for match in re.finditer(
+        r"^[\s]*?struct[\s]+([\w]+)[\s]*{(.*?)};", code, re.DOTALL | re.MULTILINE
+    ):
+        name, contents = match.groups()
+        name = "struct " + name
+
+        struct = functions.get(name)
+        if not struct:
+            struct = Shader()
+            struct.is_struct = True
+            functions[name] = struct
+
+        struct.codes.append(contents)
+        struct.flags.append(copy.copy(flags))
+
+        code = code.replace(match.group(), f"START_NAME|||{name}|||END_NAME\n")
+
+    return code
+
+
+def _evaluate_condition(condition: list[set[bool, bool, int, int]], flag: list[int]):
+    value = False
+    for c in condition:
+        a = flag[c[2]] == c[3]
+        if c[0]:
+            a = not a
+        if c[1]:
+            value = value and a
+        else:
+            value = value or a
+
+    return value
+
+
+def _calculate_condition_score(
+    expr: list[set[bool, bool, int, int]],
+    conditions: tuple[set[int], set[int]],
+    flags: list[list[int]],
+):
+    score = 0
+    for flag in conditions[0]:
+        goal = flag in conditions[1]
+
+        score += 1 if goal == _evaluate_condition(expr, flags[flag]) else -1
+
+    return score
+
+
+def _increment_expr(expr: list[list[bool, bool, int, int]], flag_def: list[int]):
+    for i, val in enumerate(expr):
+        if not val[1] and i:
+            val[1] = True
+            return
+        val[1] = False
+
+        if val[3] + 1 < flag_def[val[2]]:
+            val[3] += 1
+            return
+        val[3] = 0
+
+        if not val[0]:
+            val[0] = True
+            return
+        val[0] = False
+
+        if val[2] + 1 < len(flag_def):
+            val[2] += 1
+            return
+        val[2] = 0
+
+    expr.append([False, False, 0, 0])
+
+
+def _slow_search(
+    conditions: tuple[set[int], set[int]],
+    flags: list[list[int]],
+    flag_def: list[int],
+    timeout: float = 10,
+):
+    """
+    Slow brute-force search that scores all possible expression combinations.
+    """
+    # (bool NOT, bool AND/OR, flag_index, flag_value)
+
+    expression = [[False, False, 0, 0]]
+    best_score = -10000
+    best_expr = []
+
+    t = time.perf_counter()
+    while len(expression) <= len(flag_def) + 5:
+        score = _calculate_condition_score(expression, conditions, flags)
+
+        if score > best_score:
+            best_score = score
+            best_expr = copy.deepcopy(expression)
+
+        if score == len(conditions[0]):
+            return True, expression, score
+
+        _increment_expr(expression, flag_def)
+
+        if time.perf_counter() - t > timeout:
+            break
+
+    return False, best_expr, best_score
+
+
+def _fast_search(
+    conditions: tuple[set[int], set[int]], flags: list[list[int]], flag_def: list[int]
+) -> tuple[bool, list, int]:
+    """
+    Fast search that calculates best score for each new token.
+    """
+    # (bool NOT, bool AND/OR, flag_index, flag_value)
+
+    best = -10000
+    best_expr = []
+    local_best_expr = []
+    expression = []
+    for _ in range(len(flag_def) + 5):
+        expression = copy.deepcopy(local_best_expr)
+        expression.append([False, False, 0, 0])
+
+        local_best = -10000
+        local_best_expr = []
+
+        for i in range(4):
+            if len(expression) == 1 and i >= 2:
+                break
+            expression[-1][0] = i % 2 == 1
+            expression[-1][1] = i / 2 >= 1
+            for flag_index, flag in enumerate(flag_def):
+                expression[-1][2] = flag_index
+                for value in range(flag):
+                    expression[-1][3] = value
+
+                    score = _calculate_condition_score(expression, conditions, flags)
+                    if score > local_best:
+                        local_best = score
+                        local_best_expr = copy.deepcopy(expression)
+
+        if local_best > best:
+            best = local_best
+            best_expr = copy.deepcopy(local_best_expr)
+            if best == len(conditions[0]):
+                return True, best_expr, best
+    return False, best_expr, best
+
+
+def _convert_to_sympy_expression(
+    expression: list[set[bool, bool, int, int]],
+    inverse_flag_def: list[tuple[str, list[str]]],
+):
+    expr = sympy.false
+    for e in expression:
+        flag, values = inverse_flag_def[e[2]]
+        value = values[e[3]]
+        is_pass = flag == "pass"
+        if is_pass:
+            flag = util.generate_pass_name_macro(value)
+        else:
+            is_bool = False
+            # is_bool = set(values) in [
+            #     {"On", "Off"},
+            #     {"Enabled", "Disabled"},
+            # ]
+            if flag.startswith("f_"):
+                flag = flag.removeprefix("f_")
+                flag = util.generate_flag_name_macro(flag, value, is_bool)
+            else:
+                flag = util.format_definition_name(flag + value)
+
+        a = sympy.symbols(flag)
+
+        # if not is_pass and is_bool and value in {"Off", "Disabled"}:
+        #     a = ~a
+
+        if e[0]:
+            a = ~a
+        if e[1]:
+            expr = expr & a
+        else:
+            expr = expr | a
+
+    return expr
+
+
+def _format_expression(expr: str):
+    """
+    Formats stringified sympy expression according to GLSL macro format.
+    """
+    expr = expr.replace("~", "!").replace("|", "||").replace("&", "&&")
+    expr = re.sub(r"(\w+)", r"defined(\1)", expr)
+    return expr
+
+
+def _convert_from_dict_to_list(line_decode_table: dict[str, int]):
+    l = [""] * len(line_decode_table)
+    for line, i in line_decode_table.items():
+        l[i] = line
+    return l
+
+
+def restore_code(
+    variants: list[Variant],
+    remove_comments=True,
+    process_shaders=False,
+    search_timeout: float = 10,
+) -> tuple[set[str], str]:
+    """
+    Attempts to restore original shader source, by combining variants while adding missing macros.
+    """
+    main_shader = Shader()
+    main_shader.load(variants, remove_comments, process_shaders)
+    main_shader.uniquify()
+
+    functions: dict[str, Shader] = {}
+    for i, (code, flags) in enumerate(zip(main_shader.codes, main_shader.flags)):
+        main_shader.codes[i] = _extract_functions(code, functions, flags)
+
+    for _, func in functions.items():
+        func.uniquify()
+
+    code_flag_list = [copy.copy(v.flags) for v in variants]
+
+    line_decode_table = {}
+    main_shader.encode(line_decode_table)
+
+    for _, func in functions.items():
+        func.encode(line_decode_table)
+
+    line_decode_table = _convert_from_dict_to_list(line_decode_table)
+
+    # { name: (index, [values]) }
+    flag_definition: dict[str, tuple[int, list[str]]] = {}
+    for variant in variants:
+        for name, value in variant.flags.items():
+            definition = flag_definition.get(name)
+            if definition is None:
+                flag_definition[name] = (len(flag_definition), [value])
+            else:
+                value_list = definition[1]
+                if value not in value_list:
+                    value_list.append(value)
+
+    keys_to_remove = []
+    for name, (_, value_list) in flag_definition.items():
+        # Remove flags with a single value.
+        if len(value_list) <= 1:
+            keys_to_remove.append(name)
+        # Bias against disabling
+        for i in {"Off", "Disabled"}:
+            if i in value_list:
+                value_list.remove(i)
+                value_list.append(i)
+        # Bias towards enabling
+        for i in {"On", "Enabled"}:
+            if i in value_list:
+                value_list.remove(i)
+                value_list.insert(0, i)
+    for key in keys_to_remove:
+        flag_definition.pop(key)
+    for flags in code_flag_list:
+        for key in keys_to_remove:
+            flags.pop(key)
+
+    # Re-populate flag indices.
+    for index, (flag, (_, values)) in enumerate(flag_definition.items()):
+        flag_definition[flag] = (index, values)
+
+    main_shader.diff()
+    main_shader.group_lines()
+
+    for _, func in functions.items():
+        func.diff()
+        func.group_lines()
+
+    calc_list: list[tuple[set[int], set[int]]] = []
+    main_shader.generate_calc_list(calc_list)
+    for _, func in functions.items():
+        func.generate_calc_list(calc_list)
+
+    encoded_flags: list[list[int]] = []
+    for flags in code_flag_list:
+        encoded_flag = [-1] * len(flag_definition)
+        for name, value in flags.items():
+            name_index, value_list = flag_definition[name]
+            encoded_flag[name_index] = value_list.index(value)
+        encoded_flags.append(encoded_flag)
+
+    encoded_flag_def = [0] * len(flag_definition)
+    for _, (index, values) in flag_definition.items():
+        encoded_flag_def[index] = len(values)
+
+    inverse_flag_def: list[tuple[str, list[str]]] = [0] * len(flag_definition)
+    for flag, (index, values) in flag_definition.items():
+        inverse_flag_def[index] = (flag, values)
+
+    macro_pattern = re.compile(r"\w+")
+    macro_set = set()
+    calc_result = []
+    calc_result_formatted = []
+    calc_final = []
+    for i, calc in enumerate(calc_list):
+        success, expr, score = _fast_search(calc, encoded_flags, encoded_flag_def)
+        if not success:
+            print("slow search")
+            success, expr_slow, score_slow = _slow_search(
+                calc, encoded_flags, encoded_flag_def, search_timeout
+            )
+            if not success:
+                print("not found")
+            if success or score_slow > score:
+                expr = expr_slow
+                score = score_slow
+
+        result = _convert_to_sympy_expression(expr, inverse_flag_def)
+        try:
+            index = calc_result.index(result)
+        except ValueError:
+            index = len(calc_result)
+            calc_result.append(result)
+            result = sympy.simplify_logic(result, force=True)
+            str_result = str(result)
+            macro_set.update(set(re.findall(macro_pattern, str_result)))
+            if len(result.atoms()) == 1:
+                if str_result.startswith("~"):
+                    str_result = "#ifndef " + str_result.removeprefix("~")
+                else:
+                    str_result = "#ifdef " + str_result
+            else:
+                str_result = "#if " + _format_expression(str_result)
+            if not success:
+                str_result = f"// Approximation, matches {score} cases out of {len(calc[0])}\n{str_result}"
+
+            calc_result_formatted.append(str_result)
+
+        calc_final.append(calc_result_formatted[index])
+
+    main_code = main_shader.assemble_code(calc_final, line_decode_table)
+
+    for name, func in functions.items():
+        code = func.assemble_code(calc_final, line_decode_table)
+        if not code.startswith("\n"):
+            code = "\n" + code
+
+        main_code = main_code.replace(
+            f"START_NAME|||{name}|||END_NAME",
+            f"{name} {{{code}}}" + (";" if func.is_struct else ""),
+        )
+
+    if process_shaders:
+        main_code = _postprocess_shader(main_code)
+
+    return macro_set, main_code
+
+
+def _preprocess_shader(shader: str):
+    """
+    Pre-processes plain text shader code to convert it from GLSL to BGFX SC.\n
+    Removes built-in `u_` uniforms, replaces `gl_FragColor` and `gl_FragData`,
+    replaces attributes and varyings with `$input` and `$output`, removes macros,
+    replaces samplers with BGFX AUTOREG macros, adds NUM_THREADS to compute shaders.
+    """
+    shader = re.sub(r"^uniform\s+\w+\s+u_[\w[\]]+;\n", "", shader, flags=re.MULTILINE)
+
+    shader = re.sub(r"(\W)bgfx_FragColor(\W)", r"\1gl_FragColor\2", shader)
+    shader = re.sub(r"(\W)bgfx_FragData(\W)", r"\1gl_FragData\2", shader)
+
+    shader = re.sub(r"^out\s.+?;\n", "", shader, flags=re.MULTILINE)
+
+    is_vertex_stage = bool(
+        re.search(r"^#define varying out$", shader, flags=re.MULTILINE)
+    )
+
+    shader = re.sub(r"^#define\s.+?\n", "", shader, flags=re.MULTILINE)
+    shader = re.sub(r"^#if\s.+?#endif\n", "", shader, flags=re.MULTILINE | re.DOTALL)
+    shader = re.sub(r"^#extension\s.+?\n", "", shader, flags=re.MULTILINE)
+
+    shader = re.sub(
+        r"^[\s\w]*?varying\s.+? (\w+);$",
+        r"$output \1" if is_vertex_stage else r"$input \1",
+        shader,
+        flags=re.MULTILINE,
+    )
+    shader = re.sub(
+        r"^[\s\w]*?attribute\s.+? (\w+);$", r"$input \1", shader, flags=re.MULTILINE
+    )
+
+    shader = re.sub(r"^#version\s.+?\n", "", shader)
+
+    samplers = [
+        (r"lowp sampler2D", r"SAMPLER2D"),
+        (r"highp sampler2DMS", r"SAMPLER2DMS"),
+        (r"highp sampler3D", r"SAMPLER3D"),
+        (r"lowp samplerCube", r"SAMPLERCUBE"),
+        (r"highp sampler2DShadow", r"SAMPLER2DSHADOW"),
+        (r"highp sampler2D", r"SAMPLER2D_HIGHP"),
+        (r"highp samplerCube", r"SAMPLERCUBE_HIGHP"),
+        (r"highp sampler2DArray", r"SAMPLER2DARRAY"),
+        (r"highp sampler2DMSArray", r"SAMPLER2DMSARRAY"),
+        (r"highp samplerCubeArray", r"SAMPLERCUBEARRAY"),
+        (r"highp sampler2DArrayShadow", r"SAMPLER2DARRAYSHADOW"),
+        (r"highp isampler2D", r"ISAMPLER2D"),
+        (r"highp usampler2D", r"USAMPLER2D"),
+        (r"highp isampler3D", r"ISAMPLER3D"),
+    ]
+
+    for pattern, repl in samplers:
+        pattern = r"^uniform " + pattern + r" (\w+);"
+        repl = repl + r"_AUTOREG(\1);"
+        shader = shader = re.sub(pattern, repl, shader, flags=re.MULTILINE)
+
+    shader = shader = re.sub(
+        r"^layout\(std430, .+?\) readonly buffer (\w+) { (\w+) .+? }",
+        r"BUFFER_RO_AUTOREG(\1, \2);",
+        shader,
+        flags=re.MULTILINE,
+    )
+    shader = shader = re.sub(
+        r"^layout\(std430, .+?\) writeonly buffer (\w+) { (\w+) .+? }",
+        r"BUFFER_WR_AUTOREG(\1, \2);",
+        shader,
+        flags=re.MULTILINE,
+    )
+    shader = shader = re.sub(
+        r"^layout\(std430, .+?\) buffer (\w+) { (\w+) .+? }",
+        r"BUFFER_RW_AUTOREG(\1, \2)",
+        shader,
+        flags=re.MULTILINE,
+    )
+
+    for i, access in enumerate(("readonly ", "writeonly ", "")):
+        for prefix in "iu":
+            prefix = "u" if prefix == "u" else ""
+            access_id = ("RO", "WR", "RW")[i]
+
+            name = f"{prefix.upper()}IMAGE2D_{access_id}_AUTOREG"
+            shader = re.sub(
+                r"^layout\((.+?), .+?\) "
+                + access
+                + "uniform highp "
+                + prefix
+                + r"image2D (\w+)",
+                name + r"(\2, \1)",
+                shader,
+                flags=re.MULTILINE,
+            )
+
+            name = f"{prefix.upper()}IMAGE2D_ARRAY_{access_id}_AUTOREG"
+            shader = re.sub(
+                r"^layout\((.+?), .+?\) "
+                + access
+                + "uniform highp "
+                + prefix
+                + r"image2DArray (\w+)",
+                name + r"(\2, \1)",
+                shader,
+                flags=re.MULTILINE,
+            )
+
+            name = f"{prefix.upper()}IMAGE3D_{access_id}_AUTOREG"
+            shader = re.sub(
+                r"^layout\((.+?), .+?\) "
+                + access
+                + "uniform highp "
+                + prefix
+                + r"image3D (\w+)",
+                name + r"(\2, \1)",
+                shader,
+                flags=re.MULTILINE,
+            )
+
+    shader = re.sub(
+        r"^layout \(local_size_x = (\d+), local_size_y = (\d+), local_size_z = (\d+)\) in;",
+        r"NUM_THREADS(\1, \2, \3)",
+        shader,
+        flags=re.MULTILINE,
+    )
+
+    return shader
+
+
+def _postprocess_shader(shader: str):
+    """
+    Post-processes plain text shader code to convert it from GLSL to BGFX SC.\n
+    Merges `$input` and `$output` declarations together and adds `// Attention!`
+    comment to potential array access and matrix multiplication operations.
+    """
+    shader = shader.splitlines(keepends=True)
+
+    new_shader = []
+    args = []
+    line_type = 0  # 0 - none, 1 - input, 2 = output
+    line_prefix = ""
+    for line in shader:
+        if line.startswith("$input "):
+            current_line_type = 1
+            line_prefix = "$input "
+        elif line.startswith("$output "):
+            current_line_type = 2
+            line_prefix = "$output "
+        else:
+            current_line_type = 0
+
+        if line_type:
+            if line_type == current_line_type:
+                args.append(line.removeprefix(line_prefix).removesuffix("\n"))
+            else:
+                new_shader.append(", ".join(args) + "\n")
+        if not line_type or line_type != current_line_type:
+            if current_line_type:
+                args = [line.removesuffix("\n")]
+            else:
+                new_shader.append(line)
+
+        line_type = current_line_type
+    shader = new_shader
+
+    for i, line in enumerate(shader):
+        if ") * (" in line or "][" in line:
+            line = line[:-1] + " // Attention!\n"
+            shader[i] = line
+
+    shader = "".join(shader)
+
+    return shader
```

### Comparing `lazurite-0.1.4/src/lazurite/decompiler/varying_decompiler.py` & `lazurite-0.1.5/src/lazurite/decompiler/varying_decompiler.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-import re
-
-
-from .macro_decompiler import restore_code, Variant
-from lazurite import util
-from lazurite.material.stage import ShaderStage
-from lazurite.material.platform import ShaderPlatform
-from lazurite.material.shader_pass.shader_input import (
-    Interpolation,
-    Precision,
-    ShaderInput,
-)
-
-
-def generate_varying_line(shader_input: ShaderInput, stage: ShaderStage):
-    """
-    Creates a text line from varying.def.sc for a specific shader input and stage.
-    """
-    line = ""
-    is_instance_data = False
-
-    if shader_input.interpolation != Interpolation.none:
-        line += shader_input.interpolation.name + " "
-    if shader_input.precision != Precision.none:
-        line += shader_input.precision.name + " "
-    line += shader_input.type.name + " "
-    name = shader_input.name
-    if name.startswith("instanceData"):
-        name = f"i_data{int(name.removeprefix('instanceData'))+1}"
-        is_instance_data = True
-    elif stage == ShaderStage.Vertex:
-        name = "a_" + shader_input.semantic.get_variable_name()
-    else:
-        name = "v_" + name
-    line += f"{name} : {shader_input.semantic.get_name()};"
-
-    return is_instance_data, line
-
-
-def _postprocess_varying(code: str):
-    """
-    Formats generated varying.def code and corrects platform macros.
-    """
-    a_pattern = re.compile(r"^(.+? )(a_\w+)([\s]+: [\w]+;)", re.MULTILINE)
-    i_pattern = re.compile(r"^(.+? )(i_\w+)([\s]+: [\w]+;)", re.MULTILINE)
-    v_pattern = re.compile(r"^(.+? )(v_\w+)([\s]+: [\w]+;)", re.MULTILINE)
-
-    for pattern in [a_pattern, i_pattern, v_pattern]:
-        matches: list[re.Match] = re.findall(pattern, code)
-        if not matches:
-            continue
-        max_type_len = max((len(x[0]) for x in matches))
-        max_name_len = max((len(x[1]) for x in matches))
-
-        def replacement(m: re.Match):
-            g = m.groups()
-            txt = g[0] + (max_type_len - len(g[0])) * " "
-            txt += g[1] + (max_name_len - len(g[1])) * " "
-            return txt + g[2]
-
-        code = re.sub(pattern, replacement, code)
-
-    for platform in ShaderPlatform:
-        lang = "UNKNOWN"
-        version = 1
-        if platform.name.startswith("Direct3D_"):
-            lang = "HLSL"
-            if platform == ShaderPlatform.Direct3D_SM40:
-                version = 400
-            elif platform.name.startswith("Direct3D_SM"):
-                version = 500
-        elif platform.name.startswith("GLSL_") or platform.name.startswith("ESSL_"):
-            lang = "GLSL"
-            version = int(platform.name[-3:])
-        elif platform == ShaderPlatform.Vulkan:
-            lang = "SPIRV"
-        elif platform == ShaderPlatform.Nvn:
-            pass  # Don't know what should be used here.
-        else:
-            lang = platform.name.upper()
-
-        lang = f"BGFX_SHADER_LANGUAGE_{lang}"
-        macro = util.generate_flag_name_macro("platform", platform.name)
-        code = (
-            code.replace(f"defined({macro})", f"({lang} == {version})")
-            .replace(f"#ifdef {macro}", f"#if {lang} == {version}")
-            .replace(f"#ifndef {macro}", f"#if {lang} != {version}")
-        )
-    return code
-
-
-def restore_varying(permutations: list[Variant], search_timeout: float = 10):
-    _, code = restore_code(permutations, False, search_timeout=search_timeout)
-
-    return _postprocess_varying(code)
+import re
+
+
+from .macro_decompiler import restore_code, Variant
+from lazurite import util
+from lazurite.material.stage import ShaderStage
+from lazurite.material.platform import ShaderPlatform
+from lazurite.material.shader_pass.shader_input import (
+    Interpolation,
+    Precision,
+    ShaderInput,
+)
+
+
+def generate_varying_line(shader_input: ShaderInput, stage: ShaderStage):
+    """
+    Creates a text line from varying.def.sc for a specific shader input and stage.
+    """
+    line = ""
+    is_instance_data = False
+
+    if shader_input.interpolation != Interpolation.none:
+        line += shader_input.interpolation.name + " "
+    if shader_input.precision != Precision.none:
+        line += shader_input.precision.name + " "
+    line += shader_input.type.name + " "
+    name = shader_input.name
+    if name.startswith("instanceData"):
+        name = f"i_data{int(name.removeprefix('instanceData'))+1}"
+        is_instance_data = True
+    elif stage == ShaderStage.Vertex:
+        name = "a_" + shader_input.semantic.get_variable_name()
+    else:
+        name = "v_" + name
+    line += f"{name} : {shader_input.semantic.get_name()};"
+
+    return is_instance_data, line
+
+
+def _postprocess_varying(code: str):
+    """
+    Formats generated varying.def code and corrects platform macros.
+    """
+    a_pattern = re.compile(r"^(.+? )(a_\w+)([\s]+: [\w]+;)", re.MULTILINE)
+    i_pattern = re.compile(r"^(.+? )(i_\w+)([\s]+: [\w]+;)", re.MULTILINE)
+    v_pattern = re.compile(r"^(.+? )(v_\w+)([\s]+: [\w]+;)", re.MULTILINE)
+
+    for pattern in [a_pattern, i_pattern, v_pattern]:
+        matches: list[re.Match] = re.findall(pattern, code)
+        if not matches:
+            continue
+        max_type_len = max((len(x[0]) for x in matches))
+        max_name_len = max((len(x[1]) for x in matches))
+
+        def replacement(m: re.Match):
+            g = m.groups()
+            txt = g[0] + (max_type_len - len(g[0])) * " "
+            txt += g[1] + (max_name_len - len(g[1])) * " "
+            return txt + g[2]
+
+        code = re.sub(pattern, replacement, code)
+
+    for platform in ShaderPlatform:
+        lang = "UNKNOWN"
+        version = 1
+        if platform.name.startswith("Direct3D_"):
+            lang = "HLSL"
+            if platform == ShaderPlatform.Direct3D_SM40:
+                version = 400
+            elif platform.name.startswith("Direct3D_SM"):
+                version = 500
+        elif platform.name.startswith("GLSL_") or platform.name.startswith("ESSL_"):
+            lang = "GLSL"
+            version = int(platform.name[-3:])
+        elif platform == ShaderPlatform.Vulkan:
+            lang = "SPIRV"
+        elif platform == ShaderPlatform.Nvn:
+            pass  # Don't know what should be used here.
+        else:
+            lang = platform.name.upper()
+
+        lang = f"BGFX_SHADER_LANGUAGE_{lang}"
+        macro = util.generate_flag_name_macro("platform", platform.name)
+        code = (
+            code.replace(f"defined({macro})", f"({lang} == {version})")
+            .replace(f"#ifdef {macro}", f"#if {lang} == {version}")
+            .replace(f"#ifndef {macro}", f"#if {lang} != {version}")
+        )
+    return code
+
+
+def restore_varying(permutations: list[Variant], search_timeout: float = 10):
+    _, code = restore_code(permutations, False, search_timeout=search_timeout)
+
+    return _postprocess_varying(code)
```

### Comparing `lazurite-0.1.4/src/lazurite/material/buffer.py` & `lazurite-0.1.5/src/lazurite/material/buffer.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,176 +1,176 @@
-import json, os
-from io import BytesIO
-from enum import Enum
-
-from lazurite import util
-from .precision import Precision
-
-
-class BufferAccess(Enum):
-    undefined = 0
-    readonly = 1
-    writeonly = 2
-    readwrite = 3
-
-
-class BufferType(Enum):
-    texture2D = 0
-    texture2DArray = 1
-    external2D = 2  # ?
-    texture3D = 3  # ?
-    textureCube = 4
-    structBuffer = 5
-    rawBuffer = 6
-    accelerationStructure = 7  # ?
-    shadow2D = 8
-    shadow2DArray = 9
-
-    # ? -> never observed in-game
-
-
-class Buffer:
-    class CustomTypeInfo:
-        struct: str
-        size: int
-
-        def __init__(self, name="", size=0):
-            self.struct = name
-            self.size = size
-
-    name: str
-    reg1: int
-    access: BufferAccess
-    precision: Precision
-    unordered_access: bool
-    type: BufferType
-    texture_format: str
-    always_one: int
-    reg2: int
-    default_texture: str
-    unknown_string: str
-    custom_type_info: CustomTypeInfo | None
-
-    def __init__(self):
-        self.name = ""
-        self.reg1 = 0
-        self.access = BufferAccess.readonly
-        self.precision = Precision.lowp
-        self.unordered_access = False
-        self.type = BufferType.texture2D
-        self.texture_format = ""
-        self.always_one = 1
-        self.reg2 = 0
-        self.default_texture = ""
-        self.unknown_string = ""
-        self.custom_type_info = None
-
-    def read(self, file: BytesIO):
-        self.name = util.read_string(file)
-        self.reg1 = util.read_ushort(file)
-        self.access = BufferAccess(util.read_ubyte(file))  # 1 2 3
-        self.precision = Precision(util.read_ubyte(file))  # 0 2
-        self.unordered_access = util.read_bool(file)
-        self.type = BufferType(util.read_ubyte(file))  # 0 - 9
-        # Values according to bgfx_compute.sh: (empty string) r32ui rg32ui rgba32ui r32f r16f rg16f rgba16f rgba8 rg8 r8 rgba32f
-        self.texture_format = util.read_string(file)
-        self.always_one = util.read_ulong(file)  # 1
-        self.reg2 = util.read_ubyte(file)  # same as reg1
-
-        if util.read_bool(file):
-            self.default_texture = util.read_string(file)  # white
-        else:
-            self.default_texture = ""
-
-        if util.read_bool(file):
-            self.unknown_string = util.read_string(file)
-            # print(self.unknown_string)  # TODO: remove
-
-        if util.read_bool(file):  # CustomTypeInfo
-            self.custom_type_info = self.CustomTypeInfo()
-            self.custom_type_info.struct = util.read_string(file)
-            self.custom_type_info.size = util.read_ulong(file)
-
-        return self
-
-    def write(self, file: BytesIO):
-        util.write_string(file, self.name)
-        util.write_ushort(file, self.reg1)
-        util.write_ubyte(file, self.access.value)
-        util.write_ubyte(file, self.precision.value)
-        util.write_bool(file, self.unordered_access)
-        util.write_ubyte(file, self.type.value)
-        util.write_string(file, self.texture_format)
-        util.write_ulong(file, self.always_one)
-        util.write_ubyte(file, self.reg2)
-
-        util.write_bool(file, self.default_texture != "")
-        if self.default_texture != "":
-            util.write_string(file, self.default_texture)
-
-        util.write_bool(file, self.unknown_string != "")
-        if self.unknown_string != "":
-            util.write_string(file, self.unknown_string)
-
-        util.write_bool(file, self.custom_type_info != None)
-        if self.custom_type_info != None:
-            util.write_string(file, self.custom_type_info.struct)
-            util.write_ulong(file, self.custom_type_info.size)
-
-        return self
-
-    def serialize_properties(self):
-        obj = {
-            "name": self.name,
-            "reg1": self.reg1,
-            "reg2": self.reg2,
-            "type": self.type.name,
-            "precision": self.precision.name,
-            "access": self.access.name,
-            "texture_format": self.texture_format,
-            "default_texture": self.default_texture,
-            "unordered_access": self.unordered_access,
-            "always_one": self.always_one,
-            "unknown_string": self.unknown_string,
-            "custom_type_info": {},
-        }
-        if self.custom_type_info != None:
-            obj["custom_type_info"]["struct"] = self.custom_type_info.struct
-            obj["custom_type_info"]["size"] = self.custom_type_info.size
-
-        return obj
-
-    def store(self, path: str = "."):
-        with open(os.path.join(path, f"{self.name}.json"), "w") as f:
-            json.dump(self.serialize_properties(), f, indent=4)
-
-        return self
-
-    def load(self, object: dict, path: str):
-        self.name = object.get("name", self.name)
-        self.reg1 = object.get("reg1", self.reg1)
-        self.access = BufferAccess[object.get("access", self.access.name)]
-        self.precision = Precision[object.get("precision", self.precision.name)]
-        self.unordered_access = object.get("unordered_access", self.unordered_access)
-        self.type = BufferType[object.get("type", self.type.name)]
-        self.texture_format = object.get("texture_format", self.texture_format)
-        self.always_one = object.get("always_one", self.always_one)
-        self.unknown_string = object.get("unknown_string", self.unknown_string)
-        self.reg2 = object.get("reg2", self.reg2)
-        self.default_texture = object.get("default_texture", self.default_texture)
-
-        if "custom_type_info" in object:
-            if len(object["custom_type_info"]) > 0:
-                if self.custom_type_info == None:
-                    self.custom_type_info = self.CustomTypeInfo()
-
-                self.custom_type_info.struct = object["custom_type_info"].get(
-                    "struct", self.custom_type_info.struct
-                )
-                self.custom_type_info.size = object["custom_type_info"].get(
-                    "size", self.custom_type_info.size
-                )
-
-            else:
-                self.custom_type_info = None
-
-        return self
+import json, os
+from io import BytesIO
+from enum import Enum
+
+from lazurite import util
+from .precision import Precision
+
+
+class BufferAccess(Enum):
+    undefined = 0
+    readonly = 1
+    writeonly = 2
+    readwrite = 3
+
+
+class BufferType(Enum):
+    texture2D = 0
+    texture2DArray = 1
+    external2D = 2  # ?
+    texture3D = 3  # ?
+    textureCube = 4
+    structBuffer = 5
+    rawBuffer = 6
+    accelerationStructure = 7  # ?
+    shadow2D = 8
+    shadow2DArray = 9
+
+    # ? -> never observed in-game
+
+
+class Buffer:
+    class CustomTypeInfo:
+        struct: str
+        size: int
+
+        def __init__(self, name="", size=0):
+            self.struct = name
+            self.size = size
+
+    name: str
+    reg1: int
+    access: BufferAccess
+    precision: Precision
+    unordered_access: bool
+    type: BufferType
+    texture_format: str
+    always_one: int
+    reg2: int
+    default_texture: str
+    unknown_string: str
+    custom_type_info: CustomTypeInfo | None
+
+    def __init__(self):
+        self.name = ""
+        self.reg1 = 0
+        self.access = BufferAccess.readonly
+        self.precision = Precision.lowp
+        self.unordered_access = False
+        self.type = BufferType.texture2D
+        self.texture_format = ""
+        self.always_one = 1
+        self.reg2 = 0
+        self.default_texture = ""
+        self.unknown_string = ""
+        self.custom_type_info = None
+
+    def read(self, file: BytesIO):
+        self.name = util.read_string(file)
+        self.reg1 = util.read_ushort(file)
+        self.access = BufferAccess(util.read_ubyte(file))  # 1 2 3
+        self.precision = Precision(util.read_ubyte(file))  # 0 2
+        self.unordered_access = util.read_bool(file)
+        self.type = BufferType(util.read_ubyte(file))  # 0 - 9
+        # Values according to bgfx_compute.sh: (empty string) r32ui rg32ui rgba32ui r32f r16f rg16f rgba16f rgba8 rg8 r8 rgba32f
+        self.texture_format = util.read_string(file)
+        self.always_one = util.read_ulong(file)  # 1
+        self.reg2 = util.read_ubyte(file)  # same as reg1
+
+        if util.read_bool(file):
+            self.default_texture = util.read_string(file)  # white
+        else:
+            self.default_texture = ""
+
+        if util.read_bool(file):
+            self.unknown_string = util.read_string(file)
+            # print(self.unknown_string)  # TODO: remove
+
+        if util.read_bool(file):  # CustomTypeInfo
+            self.custom_type_info = self.CustomTypeInfo()
+            self.custom_type_info.struct = util.read_string(file)
+            self.custom_type_info.size = util.read_ulong(file)
+
+        return self
+
+    def write(self, file: BytesIO):
+        util.write_string(file, self.name)
+        util.write_ushort(file, self.reg1)
+        util.write_ubyte(file, self.access.value)
+        util.write_ubyte(file, self.precision.value)
+        util.write_bool(file, self.unordered_access)
+        util.write_ubyte(file, self.type.value)
+        util.write_string(file, self.texture_format)
+        util.write_ulong(file, self.always_one)
+        util.write_ubyte(file, self.reg2)
+
+        util.write_bool(file, self.default_texture != "")
+        if self.default_texture != "":
+            util.write_string(file, self.default_texture)
+
+        util.write_bool(file, self.unknown_string != "")
+        if self.unknown_string != "":
+            util.write_string(file, self.unknown_string)
+
+        util.write_bool(file, self.custom_type_info != None)
+        if self.custom_type_info != None:
+            util.write_string(file, self.custom_type_info.struct)
+            util.write_ulong(file, self.custom_type_info.size)
+
+        return self
+
+    def serialize_properties(self):
+        obj = {
+            "name": self.name,
+            "reg1": self.reg1,
+            "reg2": self.reg2,
+            "type": self.type.name,
+            "precision": self.precision.name,
+            "access": self.access.name,
+            "texture_format": self.texture_format,
+            "default_texture": self.default_texture,
+            "unordered_access": self.unordered_access,
+            "always_one": self.always_one,
+            "unknown_string": self.unknown_string,
+            "custom_type_info": {},
+        }
+        if self.custom_type_info != None:
+            obj["custom_type_info"]["struct"] = self.custom_type_info.struct
+            obj["custom_type_info"]["size"] = self.custom_type_info.size
+
+        return obj
+
+    def store(self, path: str = "."):
+        with open(os.path.join(path, f"{self.name}.json"), "w") as f:
+            json.dump(self.serialize_properties(), f, indent=4)
+
+        return self
+
+    def load(self, object: dict, path: str):
+        self.name = object.get("name", self.name)
+        self.reg1 = object.get("reg1", self.reg1)
+        self.access = BufferAccess[object.get("access", self.access.name)]
+        self.precision = Precision[object.get("precision", self.precision.name)]
+        self.unordered_access = object.get("unordered_access", self.unordered_access)
+        self.type = BufferType[object.get("type", self.type.name)]
+        self.texture_format = object.get("texture_format", self.texture_format)
+        self.always_one = object.get("always_one", self.always_one)
+        self.unknown_string = object.get("unknown_string", self.unknown_string)
+        self.reg2 = object.get("reg2", self.reg2)
+        self.default_texture = object.get("default_texture", self.default_texture)
+
+        if "custom_type_info" in object:
+            if len(object["custom_type_info"]) > 0:
+                if self.custom_type_info == None:
+                    self.custom_type_info = self.CustomTypeInfo()
+
+                self.custom_type_info.struct = object["custom_type_info"].get(
+                    "struct", self.custom_type_info.struct
+                )
+                self.custom_type_info.size = object["custom_type_info"].get(
+                    "size", self.custom_type_info.size
+                )
+
+            else:
+                self.custom_type_info = None
+
+        return self
```

### Comparing `lazurite-0.1.4/src/lazurite/material/platform.py` & `lazurite-0.1.5/src/lazurite/material/platform.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from enum import Enum
-
-
-class ShaderPlatform(Enum):
-    Direct3D_SM40 = 0
-    Direct3D_SM50 = 1
-    Direct3D_SM60 = 2
-    Direct3D_SM65 = 3
-    Direct3D_XB1 = 4
-    Direct3D_XBX = 5
-    GLSL_120 = 6
-    GLSL_430 = 7
-    ESSL_100 = 8
-    ESSL_300 = 9
-    ESSL_310 = 10
-    Metal = 11
-    Vulkan = 12
-    Nvn = 13
-    PSSL = 14
-    Unknown = 15
-
-    def file_extension(self):
-        if self.name.startswith("Direct3D"):
-            return "dxbc"
-
-        elif self.name.startswith("GLSL") or self.name.startswith("ESSL"):
-            return "glsl"
-
-        elif self.name == "Metal":
-            return "metal"
-
-        elif self.name == "Vulkan":
-            return "spirv"
-
-        else:
-            return "bin"
+from enum import Enum
+
+
+class ShaderPlatform(Enum):
+    Direct3D_SM40 = 0
+    Direct3D_SM50 = 1
+    Direct3D_SM60 = 2
+    Direct3D_SM65 = 3
+    Direct3D_XB1 = 4
+    Direct3D_XBX = 5
+    GLSL_120 = 6
+    GLSL_430 = 7
+    ESSL_100 = 8
+    ESSL_300 = 9
+    ESSL_310 = 10
+    Metal = 11
+    Vulkan = 12
+    Nvn = 13
+    PSSL = 14
+    Unknown = 15
+
+    def file_extension(self):
+        if self.name.startswith("Direct3D"):
+            return "dxbc"
+
+        elif self.name.startswith("GLSL") or self.name.startswith("ESSL"):
+            return "glsl"
+
+        elif self.name == "Metal":
+            return "metal"
+
+        elif self.name == "Vulkan":
+            return "spirv"
+
+        else:
+            return "bin"
```

### Comparing `lazurite-0.1.4/src/lazurite/material/shader_pass/bgfx_shader.py` & `lazurite-0.1.5/src/lazurite/material/shader_pass/bgfx_shader.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,168 +1,168 @@
-from lazurite import util
-from ..platform import ShaderPlatform
-from ..stage import ShaderStage
-from io import BytesIO
-import struct, os
-
-
-class BgfxUniform:
-    name: str
-    type_bits: int
-    count: int
-    reg_index: int
-    reg_count: int
-
-    def read(self, file: BytesIO):
-        self.name = file.read(util.read_ubyte(file)).decode()
-        self.type_bits = util.read_ubyte(file)
-        self.count = util.read_ubyte(file)
-        self.reg_index = util.read_ushort(file)
-        self.reg_count = util.read_ushort(file)
-
-        return self
-
-    def write(self, file: BytesIO):
-        util.write_ubyte(file, len(self.name))
-        file.write(self.name.encode())
-        util.write_ubyte(file, self.type_bits)
-        util.write_ubyte(file, self.count)
-        util.write_ushort(file, self.reg_index)
-        util.write_ushort(file, self.reg_count)
-        return self
-
-    def serialize_properties(self):
-        obj = {}
-        obj["name"] = self.name
-        obj["type_bits"] = self.type_bits
-        obj["count"] = self.count
-        obj["reg_index"] = self.reg_index
-        obj["reg_count"] = self.reg_count
-        return obj
-
-    def load(self, object: dict):
-        self.name = object["name"]
-        self.type_bits = object["type_bits"]
-        self.count = object["count"]
-        self.reg_index = object["reg_index"]
-        self.reg_count = object["reg_count"]
-        return self
-
-
-class BgfxShader:
-    hash: int
-    uniforms: list[BgfxUniform]
-    group_size: list[int]
-    shader_bytes: bytes
-    attributes: list[int]  # Array of attribute IDs
-    size: int
-
-    def __init__(self) -> None:
-        self.hash = 0
-        self.uniforms = []
-        self.group_size = []
-        self.shader_bytes = b""
-        self.attributes = []
-        self.size = 0
-
-    def read(self, file: BytesIO, platform: ShaderPlatform, stage: ShaderStage):
-        header = file.read(3).decode()
-        if not header in ["VSH", "FSH", "CSH"]:
-            raise Exception(f'Unrecognized BGFX shader bin header "{header}"')
-
-        version = util.read_ubyte(file)
-        if not (version == 5 or version == 3 and header == "CSH"):
-            raise Exception(f"Unsupported BGFX shader bin version: {version}")
-
-        self.hash = util.read_ulong(file)
-        self.uniforms = [
-            BgfxUniform().read(file) for _ in range(util.read_ushort(file))
-        ]
-
-        if platform == ShaderPlatform.Metal and stage == ShaderStage.Compute:
-            self.group_size = [
-                util.read_ushort(file),
-                util.read_ushort(file),
-                util.read_ushort(file),
-            ]
-        else:
-            self.group_size = []
-
-        self.shader_bytes = file.read(util.read_ulong(file))
-        util.read_ubyte(file)  # Padding (always 0)
-
-        attribute_count = file.read(1)
-        if len(attribute_count) != 0:
-            self.attributes = [
-                util.read_ushort(file)
-                for _ in range(struct.unpack("<B", attribute_count)[0])
-            ]
-            self.size = util.read_ushort(file)
-        else:
-            self.attributes = []
-            self.size = -1
-
-        return self
-
-    def write(self, file: BytesIO, platform: ShaderPlatform, stage: ShaderStage):
-        bgfx_file = BytesIO()
-
-        header = "FSH"
-        version = 5
-        if stage == ShaderStage.Vertex:
-            header = "VSH"
-        elif stage == ShaderStage.Compute:
-            header = "CSH"
-            version = 3
-
-        bgfx_file.write(header.encode())
-        util.write_ubyte(bgfx_file, version)
-
-        util.write_ulong(bgfx_file, self.hash)
-
-        util.write_ushort(bgfx_file, len(self.uniforms))
-        for uniform in self.uniforms:
-            uniform.write(bgfx_file)
-
-        if platform == ShaderPlatform.Metal and stage == ShaderStage.Compute:
-            for i in range(3):
-                util.write_ushort(bgfx_file, self.group_size[i])
-
-        util.write_ulong(bgfx_file, len(self.shader_bytes))
-        bgfx_file.write(self.shader_bytes)
-
-        util.write_ubyte(bgfx_file, 0)  # Padding
-
-        if self.size != -1:
-            util.write_ubyte(bgfx_file, len(self.attributes))
-            for attribute in self.attributes:
-                util.write_ushort(bgfx_file, attribute)
-
-            util.write_ushort(bgfx_file, self.size)
-
-        bgfx_file.seek(0)
-        util.write_array(file, bgfx_file.read())
-        return self
-
-    def serialize_properties(self):
-        obj = {}
-        obj["hash"] = self.hash
-        obj["uniforms"] = [uniform.serialize_properties() for uniform in self.uniforms]
-        obj["group_size"] = self.group_size
-        obj["attributes"] = self.attributes
-        obj["size"] = self.size
-        return obj
-
-    def load(self, object: dict, path: str):
-        bgfx_obj = object["bgfx_shader"]
-        self.hash = bgfx_obj["hash"]
-        self.uniforms = [
-            BgfxUniform().load(uniform) for uniform in bgfx_obj["uniforms"]
-        ]
-        self.group_size = bgfx_obj["group_size"]
-        self.attributes = bgfx_obj["attributes"]
-        self.size = bgfx_obj["size"]
-
-        with open(os.path.join(path, object["file_name"]), "rb") as f:
-            self.shader_bytes = f.read()
-
-        return self
+from lazurite import util
+from ..platform import ShaderPlatform
+from ..stage import ShaderStage
+from io import BytesIO
+import struct, os
+
+
+class BgfxUniform:
+    name: str
+    type_bits: int
+    count: int
+    reg_index: int
+    reg_count: int
+
+    def read(self, file: BytesIO):
+        self.name = file.read(util.read_ubyte(file)).decode()
+        self.type_bits = util.read_ubyte(file)
+        self.count = util.read_ubyte(file)
+        self.reg_index = util.read_ushort(file)
+        self.reg_count = util.read_ushort(file)
+
+        return self
+
+    def write(self, file: BytesIO):
+        util.write_ubyte(file, len(self.name))
+        file.write(self.name.encode())
+        util.write_ubyte(file, self.type_bits)
+        util.write_ubyte(file, self.count)
+        util.write_ushort(file, self.reg_index)
+        util.write_ushort(file, self.reg_count)
+        return self
+
+    def serialize_properties(self):
+        obj = {}
+        obj["name"] = self.name
+        obj["type_bits"] = self.type_bits
+        obj["count"] = self.count
+        obj["reg_index"] = self.reg_index
+        obj["reg_count"] = self.reg_count
+        return obj
+
+    def load(self, object: dict):
+        self.name = object["name"]
+        self.type_bits = object["type_bits"]
+        self.count = object["count"]
+        self.reg_index = object["reg_index"]
+        self.reg_count = object["reg_count"]
+        return self
+
+
+class BgfxShader:
+    hash: int
+    uniforms: list[BgfxUniform]
+    group_size: list[int]
+    shader_bytes: bytes
+    attributes: list[int]  # Array of attribute IDs
+    size: int
+
+    def __init__(self) -> None:
+        self.hash = 0
+        self.uniforms = []
+        self.group_size = []
+        self.shader_bytes = b""
+        self.attributes = []
+        self.size = 0
+
+    def read(self, file: BytesIO, platform: ShaderPlatform, stage: ShaderStage):
+        header = file.read(3).decode()
+        if not header in ["VSH", "FSH", "CSH"]:
+            raise Exception(f'Unrecognized BGFX shader bin header "{header}"')
+
+        version = util.read_ubyte(file)
+        if not (version == 5 or version == 3 and header == "CSH"):
+            raise Exception(f"Unsupported BGFX shader bin version: {version}")
+
+        self.hash = util.read_ulong(file)
+        self.uniforms = [
+            BgfxUniform().read(file) for _ in range(util.read_ushort(file))
+        ]
+
+        if platform == ShaderPlatform.Metal and stage == ShaderStage.Compute:
+            self.group_size = [
+                util.read_ushort(file),
+                util.read_ushort(file),
+                util.read_ushort(file),
+            ]
+        else:
+            self.group_size = []
+
+        self.shader_bytes = file.read(util.read_ulong(file))
+        util.read_ubyte(file)  # Padding (always 0)
+
+        attribute_count = file.read(1)
+        if len(attribute_count) != 0:
+            self.attributes = [
+                util.read_ushort(file)
+                for _ in range(struct.unpack("<B", attribute_count)[0])
+            ]
+            self.size = util.read_ushort(file)
+        else:
+            self.attributes = []
+            self.size = -1
+
+        return self
+
+    def write(self, file: BytesIO, platform: ShaderPlatform, stage: ShaderStage):
+        bgfx_file = BytesIO()
+
+        header = "FSH"
+        version = 5
+        if stage == ShaderStage.Vertex:
+            header = "VSH"
+        elif stage == ShaderStage.Compute:
+            header = "CSH"
+            version = 3
+
+        bgfx_file.write(header.encode())
+        util.write_ubyte(bgfx_file, version)
+
+        util.write_ulong(bgfx_file, self.hash)
+
+        util.write_ushort(bgfx_file, len(self.uniforms))
+        for uniform in self.uniforms:
+            uniform.write(bgfx_file)
+
+        if platform == ShaderPlatform.Metal and stage == ShaderStage.Compute:
+            for i in range(3):
+                util.write_ushort(bgfx_file, self.group_size[i])
+
+        util.write_ulong(bgfx_file, len(self.shader_bytes))
+        bgfx_file.write(self.shader_bytes)
+
+        util.write_ubyte(bgfx_file, 0)  # Padding
+
+        if self.size != -1:
+            util.write_ubyte(bgfx_file, len(self.attributes))
+            for attribute in self.attributes:
+                util.write_ushort(bgfx_file, attribute)
+
+            util.write_ushort(bgfx_file, self.size)
+
+        bgfx_file.seek(0)
+        util.write_array(file, bgfx_file.read())
+        return self
+
+    def serialize_properties(self):
+        obj = {}
+        obj["hash"] = self.hash
+        obj["uniforms"] = [uniform.serialize_properties() for uniform in self.uniforms]
+        obj["group_size"] = self.group_size
+        obj["attributes"] = self.attributes
+        obj["size"] = self.size
+        return obj
+
+    def load(self, object: dict, path: str):
+        bgfx_obj = object["bgfx_shader"]
+        self.hash = bgfx_obj["hash"]
+        self.uniforms = [
+            BgfxUniform().load(uniform) for uniform in bgfx_obj["uniforms"]
+        ]
+        self.group_size = bgfx_obj["group_size"]
+        self.attributes = bgfx_obj["attributes"]
+        self.size = bgfx_obj["size"]
+
+        with open(os.path.join(path, object["file_name"]), "rb") as f:
+            self.shader_bytes = f.read()
+
+        return self
```

### Comparing `lazurite-0.1.4/src/lazurite/material/shader_pass/shader_definition.py` & `lazurite-0.1.5/src/lazurite/material/shader_pass/shader_definition.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-from io import BytesIO
-
-from lazurite import util
-from ..platform import ShaderPlatform
-from ..stage import ShaderStage
-from .bgfx_shader import BgfxShader
-from .shader_input import ShaderInput
-
-
-class ShaderDefinition:
-    stage: ShaderStage
-    platform: ShaderPlatform
-    inputs: list[ShaderInput]
-    hash: int
-    bgfx_shader: BgfxShader
-
-    def __init__(self) -> None:
-        self.stage = ShaderStage.Unknown
-        self.platform = ShaderPlatform.Unknown
-        self.inputs = []
-        self.hash = 0
-        self.bgfx_shader = BgfxShader()
-
-    def read(self, file: BytesIO):
-        self.stage = ShaderStage[util.read_string(file)]
-        self.platform = ShaderPlatform[util.read_string(file)]
-
-        stage_index = util.read_ubyte(file)
-        if self.stage.value != stage_index:
-            raise Exception(
-                f'Stage name "{self.stage.name}" and index "{stage_index}" do not match! Index "{self.stage.value}" was expected.'
-            )
-
-        platform_index = util.read_ubyte(file)
-        if self.platform.value != platform_index:
-            raise Exception(
-                f'Platform name "{self.platform.name}" and index "{platform_index}" do not match! Index "{self.platform.value}" was expected.'
-            )
-
-        self.inputs = [ShaderInput().read(file) for _ in range(util.read_ushort(file))]
-        self.hash = util.read_ulonglong(file)
-        bgfx_shader_bytes = BytesIO(util.read_array(file))
-        self.bgfx_shader.read(bgfx_shader_bytes, self.platform, self.stage)
-
-        return self
-
-    def write(self, file: BytesIO):
-        util.write_string(file, self.stage.name)
-        util.write_string(file, self.platform.name)
-        util.write_ubyte(file, self.stage.value)
-        util.write_ubyte(file, self.platform.value)
-
-        util.write_ushort(file, len(self.inputs))
-        for inp in self.inputs:
-            inp.write(file)
-
-        util.write_ulonglong(file, self.hash)
-        self.bgfx_shader.write(file, self.platform, self.stage)
-
-        return self
-
-    def get_shader_file_name(self, index: int):
-        return f"{index}.{self.platform.name}.{self.stage.name}.{self.platform.file_extension()}"
-
-    def serialize_properties(self, index: int):
-        obj = {}
-        if index != None:
-            obj["file_name"] = self.get_shader_file_name(index)
-        obj["stage"] = self.stage.name
-        obj["platform"] = self.platform.name
-        obj["inputs"] = [
-            shaderInput.serialize_properties() for shaderInput in self.inputs
-        ]
-        obj["hash"] = self.hash
-        obj["bgfx_shader"] = self.bgfx_shader.serialize_properties()
-        return obj
-
-    def load(self, object: dict, path: str):
-        self.stage = ShaderStage[object["stage"]]
-        self.platform = ShaderPlatform[object["platform"]]
-        self.inputs = [ShaderInput().load(inp) for inp in object["inputs"]]
-        self.hash = object["hash"]
-        self.bgfx_shader = BgfxShader().load(object, path)
-        return self
-
-    def label(
-        self,
-        material_name: str,
-        pass_name: str,
-        variant_index: int,
-        is_supported: bool,
-        flags: dict,
-    ):
-        if not any(
-            self.platform.name.startswith(platform_prefix)
-            for platform_prefix in ["ESSL", "GLSL", "Metal"]
-        ):
-            return self
-
-        comment = (
-            "// Shader Information:\n"
-            f"// - Name: {material_name}\n"
-            f"// - Pass: {pass_name}\n"
-            f"// - Platform: {self.platform.name}\n"
-            f"// - Stage: {self.stage.name}\n"
-            f"// - Variant: {variant_index}\n"
-            f"// - Variant Supported: {is_supported}\n"
-        )
-
-        if flags:
-            comment += "// - Variant Flags: \n"
-            comment += "\n".join(
-                [f"//    - {flag}: {value}" for flag, value in flags.items()]
-            )
-
-        code = self.bgfx_shader.shader_bytes.decode()
-        code = util.insert_header_comment(code, comment)
-        self.bgfx_shader.shader_bytes = code.encode()
-
-        return self
+from io import BytesIO
+
+from lazurite import util
+from ..platform import ShaderPlatform
+from ..stage import ShaderStage
+from .bgfx_shader import BgfxShader
+from .shader_input import ShaderInput
+
+
+class ShaderDefinition:
+    stage: ShaderStage
+    platform: ShaderPlatform
+    inputs: list[ShaderInput]
+    hash: int
+    bgfx_shader: BgfxShader
+
+    def __init__(self) -> None:
+        self.stage = ShaderStage.Unknown
+        self.platform = ShaderPlatform.Unknown
+        self.inputs = []
+        self.hash = 0
+        self.bgfx_shader = BgfxShader()
+
+    def read(self, file: BytesIO):
+        self.stage = ShaderStage[util.read_string(file)]
+        self.platform = ShaderPlatform[util.read_string(file)]
+
+        stage_index = util.read_ubyte(file)
+        if self.stage.value != stage_index:
+            raise Exception(
+                f'Stage name "{self.stage.name}" and index "{stage_index}" do not match! Index "{self.stage.value}" was expected.'
+            )
+
+        platform_index = util.read_ubyte(file)
+        if self.platform.value != platform_index:
+            raise Exception(
+                f'Platform name "{self.platform.name}" and index "{platform_index}" do not match! Index "{self.platform.value}" was expected.'
+            )
+
+        self.inputs = [ShaderInput().read(file) for _ in range(util.read_ushort(file))]
+        self.hash = util.read_ulonglong(file)
+        bgfx_shader_bytes = BytesIO(util.read_array(file))
+        self.bgfx_shader.read(bgfx_shader_bytes, self.platform, self.stage)
+
+        return self
+
+    def write(self, file: BytesIO):
+        util.write_string(file, self.stage.name)
+        util.write_string(file, self.platform.name)
+        util.write_ubyte(file, self.stage.value)
+        util.write_ubyte(file, self.platform.value)
+
+        util.write_ushort(file, len(self.inputs))
+        for inp in self.inputs:
+            inp.write(file)
+
+        util.write_ulonglong(file, self.hash)
+        self.bgfx_shader.write(file, self.platform, self.stage)
+
+        return self
+
+    def get_shader_file_name(self, index: int):
+        return f"{index}.{self.platform.name}.{self.stage.name}.{self.platform.file_extension()}"
+
+    def serialize_properties(self, index: int):
+        obj = {}
+        if index != None:
+            obj["file_name"] = self.get_shader_file_name(index)
+        obj["stage"] = self.stage.name
+        obj["platform"] = self.platform.name
+        obj["inputs"] = [
+            shaderInput.serialize_properties() for shaderInput in self.inputs
+        ]
+        obj["hash"] = self.hash
+        obj["bgfx_shader"] = self.bgfx_shader.serialize_properties()
+        return obj
+
+    def load(self, object: dict, path: str):
+        self.stage = ShaderStage[object["stage"]]
+        self.platform = ShaderPlatform[object["platform"]]
+        self.inputs = [ShaderInput().load(inp) for inp in object["inputs"]]
+        self.hash = object["hash"]
+        self.bgfx_shader = BgfxShader().load(object, path)
+        return self
+
+    def label(
+        self,
+        material_name: str,
+        pass_name: str,
+        variant_index: int,
+        is_supported: bool,
+        flags: dict,
+    ):
+        if not any(
+            self.platform.name.startswith(platform_prefix)
+            for platform_prefix in ["ESSL", "GLSL", "Metal"]
+        ):
+            return self
+
+        comment = (
+            "// Shader Information:\n"
+            f"// - Name: {material_name}\n"
+            f"// - Pass: {pass_name}\n"
+            f"// - Platform: {self.platform.name}\n"
+            f"// - Stage: {self.stage.name}\n"
+            f"// - Variant: {variant_index}\n"
+            f"// - Variant Supported: {is_supported}\n"
+        )
+
+        if flags:
+            comment += "// - Variant Flags: \n"
+            comment += "\n".join(
+                [f"//    - {flag}: {value}" for flag, value in flags.items()]
+            )
+
+        code = self.bgfx_shader.shader_bytes.decode()
+        code = util.insert_header_comment(code, comment)
+        self.bgfx_shader.shader_bytes = code.encode()
+
+        return self
```

### Comparing `lazurite-0.1.4/src/lazurite/material/shader_pass/shader_pass.py` & `lazurite-0.1.5/src/lazurite/material/shader_pass/shader_pass.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,178 +1,178 @@
-from io import BytesIO
-import os, json
-
-from lazurite import util
-from .variant import Variant
-from ..platform import ShaderPlatform
-from ..stage import ShaderStage
-from .blend_mode import BlendMode
-from .supported_platforms import SupportedPlatforms
-
-
-class Pass:
-    name: str
-    supported_platforms: SupportedPlatforms
-    fallback_pass: str
-    default_blend_mode: BlendMode
-    default_variant: dict[str, str]
-    variants: list[Variant]
-
-    def __init__(self):
-        self.name = ""
-        self.supported_platforms = SupportedPlatforms()
-        self.fallback_pass = ""
-        self.default_blend_mode = BlendMode.Unspecified
-        self.default_variant = {}
-        self.variants = []
-
-    def read(self, file: BytesIO):
-        self.name = util.read_string(file)
-        self.supported_platforms = SupportedPlatforms(util.read_string(file))
-        self.fallback_pass = util.read_string(
-            file
-        )  # (empty string) Fallback DoCheckerboarding DepthOnlyFallback
-
-        if util.read_bool(file):  # Has default blend mode
-            self.default_blend_mode = BlendMode[util.read_ushort(file)]
-
-        self.default_variant = {}
-        default_flag_count = util.read_ushort(file)
-        for _ in range(default_flag_count):
-            key = util.read_string(file)
-            self.default_variant[key] = util.read_string(file)
-
-        self.variants = [Variant().read(file) for _ in range(util.read_ushort(file))]
-
-        return self
-
-    def write(self, file: BytesIO):
-        util.write_string(file, self.name)
-        util.write_string(file, self.supported_platforms.get_bit_string())
-        util.write_string(file, self.fallback_pass)
-
-        util.write_bool(file, self.default_blend_mode != BlendMode.Unspecified)
-        if self.default_blend_mode != BlendMode.Unspecified:
-            util.write_ushort(file, self.default_blend_mode.value)
-
-        util.write_ushort(file, len(self.default_variant))
-        for key in self.default_variant:
-            util.write_string(file, key)
-            util.write_string(file, self.default_variant[key])
-
-        util.write_ushort(file, len(self.variants))
-        for variant in self.variants:
-            variant.write(file)
-        return self
-
-    def serialize_properties(self):
-        obj = {}
-        obj["name"] = self.name
-        obj["supported_platforms"] = self.supported_platforms.serialize()
-        obj["fallback_pass"] = self.fallback_pass
-        obj["default_blend_mode"] = (
-            self.default_blend_mode.name
-            if self.default_blend_mode != BlendMode.Unspecified
-            else ""
-        )
-        obj["default_variant"] = self.default_variant
-        obj["variants"] = []
-
-        for i in range(len(self.variants)):
-            obj["variants"].append(self.variants[i].serialize_properties(i))
-
-        return obj
-
-    def store(self, path: str = ".", skip_shaders=False):
-        pass_dir = os.path.join(path, self.name)
-
-        with open(os.path.join(path, f"{self.name}.json"), "w") as f:
-            json.dump(self.serialize_properties(), f, indent=4)
-
-        if skip_shaders:
-            return self
-
-        os.mkdir(pass_dir)
-
-        for i in range(len(self.variants)):
-            for shader in self.variants[i].shaders:
-                with open(
-                    os.path.join(pass_dir, shader.get_shader_file_name(i)), "wb"
-                ) as f:
-                    f.write(shader.bgfx_shader.shader_bytes)
-
-        return self
-
-    def load(self, object: dict, path: str):
-        self.name = object.get("name", self.name)
-        self.supported_platforms.load(object.get("supported_platforms", {}))
-        self.fallback_pass = object.get("fallback_pass", self.fallback_pass)
-        mode = object.get("default_blend_mode", None)
-        if mode != None:
-            self.default_blend_mode = BlendMode[mode] if mode else BlendMode.Unspecified
-        self.default_variant = object.get("default_variant", self.default_variant)
-
-        if "variants" in object:
-            self.variants = [
-                Variant().load(variant, os.path.join(path, self.name))
-                for variant in object["variants"]
-            ]
-        return self
-
-    def label(self, material_name: str):
-        for variant_index, variant in enumerate(self.variants):
-            variant.label(material_name, self.name, variant_index)
-
-        return self
-
-    def sort_variants(self):
-        self.default_variant = dict(sorted(self.default_variant.items()))
-
-        for variant in self.variants:
-            variant.flags = dict(sorted(variant.flags.items()))
-
-        self.variants.sort(key=lambda x: str(x.flags))
-
-    def get_platforms(self):
-        platforms: set[ShaderPlatform] = set()
-        for variant in self.variants:
-            platforms.update(variant.get_platforms())
-
-        return platforms
-
-    def get_stages(self):
-        stages: set[ShaderStage] = set()
-        for variant in self.variants:
-            stages.update(variant.get_stages())
-
-        return stages
-
-    def merge_variants(self, other: "Pass"):
-        for other_variant in other.variants:
-            matching_variant = next(
-                (v for v in self.variants if v.flags == other_variant.flags), None
-            )
-            if matching_variant is None:
-                self.variants.append(other_variant)
-            else:
-                matching_variant.merge_variant(other_variant)
-
-    def get_flag_definitions(self):
-        """
-        Returns a dict of all possible flag keys and their values.
-        """
-        definitions = {key: {value} for key, value in self.default_variant.items()}
-
-        for variant in self.variants:
-            for key, value in variant.flags.items():
-                if key not in definitions:
-                    definitions[key] = set()
-                definitions[key].add(value)
-        return definitions
-
-    def add_platforms(self, platforms: set[ShaderPlatform]):
-        for variant in self.variants:
-            variant.add_platforms(platforms)
-
-    def remove_platforms(self, platforms: set[ShaderPlatform]):
-        for variant in self.variants:
-            variant.remove_platforms(platforms)
+from io import BytesIO
+import os, json
+
+from lazurite import util
+from .variant import Variant
+from ..platform import ShaderPlatform
+from ..stage import ShaderStage
+from .blend_mode import BlendMode
+from .supported_platforms import SupportedPlatforms
+
+
+class Pass:
+    name: str
+    supported_platforms: SupportedPlatforms
+    fallback_pass: str
+    default_blend_mode: BlendMode
+    default_variant: dict[str, str]
+    variants: list[Variant]
+
+    def __init__(self):
+        self.name = ""
+        self.supported_platforms = SupportedPlatforms()
+        self.fallback_pass = ""
+        self.default_blend_mode = BlendMode.Unspecified
+        self.default_variant = {}
+        self.variants = []
+
+    def read(self, file: BytesIO):
+        self.name = util.read_string(file)
+        self.supported_platforms = SupportedPlatforms(util.read_string(file))
+        self.fallback_pass = util.read_string(
+            file
+        )  # (empty string) Fallback DoCheckerboarding DepthOnlyFallback
+
+        if util.read_bool(file):  # Has default blend mode
+            self.default_blend_mode = BlendMode[util.read_ushort(file)]
+
+        self.default_variant = {}
+        default_flag_count = util.read_ushort(file)
+        for _ in range(default_flag_count):
+            key = util.read_string(file)
+            self.default_variant[key] = util.read_string(file)
+
+        self.variants = [Variant().read(file) for _ in range(util.read_ushort(file))]
+
+        return self
+
+    def write(self, file: BytesIO):
+        util.write_string(file, self.name)
+        util.write_string(file, self.supported_platforms.get_bit_string())
+        util.write_string(file, self.fallback_pass)
+
+        util.write_bool(file, self.default_blend_mode != BlendMode.Unspecified)
+        if self.default_blend_mode != BlendMode.Unspecified:
+            util.write_ushort(file, self.default_blend_mode.value)
+
+        util.write_ushort(file, len(self.default_variant))
+        for key in self.default_variant:
+            util.write_string(file, key)
+            util.write_string(file, self.default_variant[key])
+
+        util.write_ushort(file, len(self.variants))
+        for variant in self.variants:
+            variant.write(file)
+        return self
+
+    def serialize_properties(self):
+        obj = {}
+        obj["name"] = self.name
+        obj["supported_platforms"] = self.supported_platforms.serialize()
+        obj["fallback_pass"] = self.fallback_pass
+        obj["default_blend_mode"] = (
+            self.default_blend_mode.name
+            if self.default_blend_mode != BlendMode.Unspecified
+            else ""
+        )
+        obj["default_variant"] = self.default_variant
+        obj["variants"] = []
+
+        for i in range(len(self.variants)):
+            obj["variants"].append(self.variants[i].serialize_properties(i))
+
+        return obj
+
+    def store(self, path: str = ".", skip_shaders=False):
+        pass_dir = os.path.join(path, self.name)
+
+        with open(os.path.join(path, f"{self.name}.json"), "w") as f:
+            json.dump(self.serialize_properties(), f, indent=4)
+
+        if skip_shaders:
+            return self
+
+        os.mkdir(pass_dir)
+
+        for i in range(len(self.variants)):
+            for shader in self.variants[i].shaders:
+                with open(
+                    os.path.join(pass_dir, shader.get_shader_file_name(i)), "wb"
+                ) as f:
+                    f.write(shader.bgfx_shader.shader_bytes)
+
+        return self
+
+    def load(self, object: dict, path: str):
+        self.name = object.get("name", self.name)
+        self.supported_platforms.load(object.get("supported_platforms", {}))
+        self.fallback_pass = object.get("fallback_pass", self.fallback_pass)
+        mode = object.get("default_blend_mode", None)
+        if mode != None:
+            self.default_blend_mode = BlendMode[mode] if mode else BlendMode.Unspecified
+        self.default_variant = object.get("default_variant", self.default_variant)
+
+        if "variants" in object:
+            self.variants = [
+                Variant().load(variant, os.path.join(path, self.name))
+                for variant in object["variants"]
+            ]
+        return self
+
+    def label(self, material_name: str):
+        for variant_index, variant in enumerate(self.variants):
+            variant.label(material_name, self.name, variant_index)
+
+        return self
+
+    def sort_variants(self):
+        self.default_variant = dict(sorted(self.default_variant.items()))
+
+        for variant in self.variants:
+            variant.flags = dict(sorted(variant.flags.items()))
+
+        self.variants.sort(key=lambda x: str(x.flags))
+
+    def get_platforms(self):
+        platforms: set[ShaderPlatform] = set()
+        for variant in self.variants:
+            platforms.update(variant.get_platforms())
+
+        return platforms
+
+    def get_stages(self):
+        stages: set[ShaderStage] = set()
+        for variant in self.variants:
+            stages.update(variant.get_stages())
+
+        return stages
+
+    def merge_variants(self, other: "Pass"):
+        for other_variant in other.variants:
+            matching_variant = next(
+                (v for v in self.variants if v.flags == other_variant.flags), None
+            )
+            if matching_variant is None:
+                self.variants.append(other_variant)
+            else:
+                matching_variant.merge_variant(other_variant)
+
+    def get_flag_definitions(self):
+        """
+        Returns a dict of all possible flag keys and their values.
+        """
+        definitions = {key: {value} for key, value in self.default_variant.items()}
+
+        for variant in self.variants:
+            for key, value in variant.flags.items():
+                if key not in definitions:
+                    definitions[key] = set()
+                definitions[key].add(value)
+        return definitions
+
+    def add_platforms(self, platforms: set[ShaderPlatform]):
+        for variant in self.variants:
+            variant.add_platforms(platforms)
+
+    def remove_platforms(self, platforms: set[ShaderPlatform]):
+        for variant in self.variants:
+            variant.remove_platforms(platforms)
```

### Comparing `lazurite-0.1.4/src/lazurite/material/shader_pass/supported_platforms.py` & `lazurite-0.1.5/src/lazurite/material/shader_pass/supported_platforms.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from ..platform import ShaderPlatform
-
-
-class SupportedPlatforms:
-    platforms: dict[ShaderPlatform, bool]
-
-    def _validate_bit_string(self, platforms_bit_string: str) -> str:
-        if any(c not in "01" for c in platforms_bit_string):
-            print(
-                f"Warning: Invalid supported platforms bit field {platforms_bit_string}"
-            )
-            return "1" * len(ShaderPlatform)
-        return platforms_bit_string
-
-    def _format_bit_string(self, platforms_bit_string: str):
-        # Truncate everything after 16 symbols.
-        platforms_bit_string = platforms_bit_string[: len(ShaderPlatform)]
-
-        # In case there are less than 16, add leading zeros.
-        platforms_bit_string = platforms_bit_string.zfill(len(ShaderPlatform))
-
-        return platforms_bit_string
-
-    def __init__(self, platforms_bit_string: str = "1" * len(ShaderPlatform)) -> None:
-        platforms_bit_string = self._validate_bit_string(platforms_bit_string)
-        platforms_bit_string = self._format_bit_string(platforms_bit_string)
-
-        self.platforms = {
-            platform: bit == "1"
-            for platform, bit in zip(ShaderPlatform, platforms_bit_string)
-        }
-
-    def get_bit_string(self) -> str:
-        return "".join("1" if self.platforms[p] else "0" for p in ShaderPlatform)
-
-    def load(self, json_data: dict[str, bool]):
-        for key, value in json_data.items():
-            self.platforms[ShaderPlatform[key]] = value
-
-    def serialize(self):
-        return {p.name: v for p, v in self.platforms.items()}
+from ..platform import ShaderPlatform
+
+
+class SupportedPlatforms:
+    platforms: dict[ShaderPlatform, bool]
+
+    def _validate_bit_string(self, platforms_bit_string: str) -> str:
+        if any(c not in "01" for c in platforms_bit_string):
+            print(
+                f"Warning: Invalid supported platforms bit field {platforms_bit_string}"
+            )
+            return "1" * len(ShaderPlatform)
+        return platforms_bit_string
+
+    def _format_bit_string(self, platforms_bit_string: str):
+        # Truncate everything after 16 symbols.
+        platforms_bit_string = platforms_bit_string[: len(ShaderPlatform)]
+
+        # In case there are less than 16, add leading zeros.
+        platforms_bit_string = platforms_bit_string.zfill(len(ShaderPlatform))
+
+        return platforms_bit_string
+
+    def __init__(self, platforms_bit_string: str = "1" * len(ShaderPlatform)) -> None:
+        platforms_bit_string = self._validate_bit_string(platforms_bit_string)
+        platforms_bit_string = self._format_bit_string(platforms_bit_string)
+
+        self.platforms = {
+            platform: bit == "1"
+            for platform, bit in zip(ShaderPlatform, platforms_bit_string)
+        }
+
+    def get_bit_string(self) -> str:
+        return "".join("1" if self.platforms[p] else "0" for p in ShaderPlatform)
+
+    def load(self, json_data: dict[str, bool]):
+        for key, value in json_data.items():
+            self.platforms[ShaderPlatform[key]] = value
+
+    def serialize(self):
+        return {p.name: v for p, v in self.platforms.items()}
```

### Comparing `lazurite-0.1.4/src/lazurite/material/shader_pass/variant.py` & `lazurite-0.1.5/src/lazurite/material/shader_pass/variant.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-import copy
-from io import BytesIO
-
-from lazurite import util
-from .shader_definition import ShaderDefinition
-from ..platform import ShaderPlatform
-from ..stage import ShaderStage
-from .bgfx_shader import BgfxShader
-
-
-class Variant:
-    is_supported: bool
-    flags: dict[str, str]
-    shaders: list[ShaderDefinition]
-
-    def __init__(self) -> None:
-        self.is_supported = False
-        self.flags = {}
-        self.shaders = []
-
-    def read(self, file: BytesIO):
-        self.is_supported = util.read_bool(file)
-        flag_count = util.read_ushort(file)
-        shader_count = util.read_ushort(file)
-
-        self.flags = {}
-        for _ in range(flag_count):
-            key = util.read_string(file)
-            self.flags[key] = util.read_string(file)
-
-        self.shaders = [ShaderDefinition().read(file) for _ in range(shader_count)]
-
-        return self
-
-    def write(self, file: BytesIO):
-        util.write_bool(file, self.is_supported)
-        util.write_ushort(file, len(self.flags))
-        util.write_ushort(file, len(self.shaders))
-
-        for key in self.flags:
-            util.write_string(file, key)
-            util.write_string(file, self.flags[key])
-
-        for shader in self.shaders:
-            shader.write(file)
-
-        return self
-
-    def serialize_properties(self, index: int):
-        obj = {}
-        obj["is_supported"] = self.is_supported
-        obj["flags"] = self.flags
-        obj["shaders"] = [shader.serialize_properties(index) for shader in self.shaders]
-
-        return obj
-
-    def load(self, object: dict, path: str):
-        self.is_supported = object.get("is_supported", self.is_supported)
-        self.flags = object.get("flags", self.flags)
-
-        if "shaders" in object:
-            self.shaders = [
-                ShaderDefinition().load(shader, path) for shader in object["shaders"]
-            ]
-        return self
-
-    def label(self, material_name: str, pass_name: str, variant_index: int):
-        for shader in self.shaders:
-            shader.label(
-                material_name, pass_name, variant_index, self.is_supported, self.flags
-            )
-
-        return self
-
-    def get_platforms(self):
-        platforms: set[ShaderPlatform] = set()
-        for shader in self.shaders:
-            platforms.add(shader.platform)
-
-        return platforms
-
-    def get_stages(self):
-        stages: set[ShaderStage] = set()
-        for shader in self.shaders:
-            stages.add(shader.stage)
-
-        return stages
-
-    def merge_variant(self, other: "Variant"):
-        for other_shader in other.shaders:
-            matching_shader = next(
-                (
-                    v
-                    for v in self.shaders
-                    if v.platform == other_shader.platform
-                    and v.stage == other_shader.stage
-                ),
-                None,
-            )
-            if matching_shader is None:
-                self.shaders.append(other_shader)
-
-    def add_platforms(self, platforms: set[ShaderPlatform]):
-        current_platforms = self.get_platforms()
-        missing_platforms = platforms.difference(current_platforms)
-        stages = self.get_stages()
-
-        for platform in missing_platforms:
-            for stage in stages:
-                shader = next(
-                    (x for x in self.shaders if x.stage == stage), ShaderDefinition()
-                )
-                shader = copy.deepcopy(shader)
-                shader.stage = stage
-                shader.platform = platform
-                shader.bgfx_shader = BgfxShader()
-                self.shaders.append(shader)
-
-    def remove_platforms(self, platforms: set[ShaderPlatform]):
-        self.shaders = [s for s in self.shaders if s.platform not in platforms]
+import copy
+from io import BytesIO
+
+from lazurite import util
+from .shader_definition import ShaderDefinition
+from ..platform import ShaderPlatform
+from ..stage import ShaderStage
+from .bgfx_shader import BgfxShader
+
+
+class Variant:
+    is_supported: bool
+    flags: dict[str, str]
+    shaders: list[ShaderDefinition]
+
+    def __init__(self) -> None:
+        self.is_supported = False
+        self.flags = {}
+        self.shaders = []
+
+    def read(self, file: BytesIO):
+        self.is_supported = util.read_bool(file)
+        flag_count = util.read_ushort(file)
+        shader_count = util.read_ushort(file)
+
+        self.flags = {}
+        for _ in range(flag_count):
+            key = util.read_string(file)
+            self.flags[key] = util.read_string(file)
+
+        self.shaders = [ShaderDefinition().read(file) for _ in range(shader_count)]
+
+        return self
+
+    def write(self, file: BytesIO):
+        util.write_bool(file, self.is_supported)
+        util.write_ushort(file, len(self.flags))
+        util.write_ushort(file, len(self.shaders))
+
+        for key in self.flags:
+            util.write_string(file, key)
+            util.write_string(file, self.flags[key])
+
+        for shader in self.shaders:
+            shader.write(file)
+
+        return self
+
+    def serialize_properties(self, index: int):
+        obj = {}
+        obj["is_supported"] = self.is_supported
+        obj["flags"] = self.flags
+        obj["shaders"] = [shader.serialize_properties(index) for shader in self.shaders]
+
+        return obj
+
+    def load(self, object: dict, path: str):
+        self.is_supported = object.get("is_supported", self.is_supported)
+        self.flags = object.get("flags", self.flags)
+
+        if "shaders" in object:
+            self.shaders = [
+                ShaderDefinition().load(shader, path) for shader in object["shaders"]
+            ]
+        return self
+
+    def label(self, material_name: str, pass_name: str, variant_index: int):
+        for shader in self.shaders:
+            shader.label(
+                material_name, pass_name, variant_index, self.is_supported, self.flags
+            )
+
+        return self
+
+    def get_platforms(self):
+        platforms: set[ShaderPlatform] = set()
+        for shader in self.shaders:
+            platforms.add(shader.platform)
+
+        return platforms
+
+    def get_stages(self):
+        stages: set[ShaderStage] = set()
+        for shader in self.shaders:
+            stages.add(shader.stage)
+
+        return stages
+
+    def merge_variant(self, other: "Variant"):
+        for other_shader in other.shaders:
+            matching_shader = next(
+                (
+                    v
+                    for v in self.shaders
+                    if v.platform == other_shader.platform
+                    and v.stage == other_shader.stage
+                ),
+                None,
+            )
+            if matching_shader is None:
+                self.shaders.append(other_shader)
+
+    def add_platforms(self, platforms: set[ShaderPlatform]):
+        current_platforms = self.get_platforms()
+        missing_platforms = platforms.difference(current_platforms)
+        stages = self.get_stages()
+
+        for platform in missing_platforms:
+            for stage in stages:
+                shader = next(
+                    (x for x in self.shaders if x.stage == stage), ShaderDefinition()
+                )
+                shader = copy.deepcopy(shader)
+                shader.stage = stage
+                shader.platform = platform
+                shader.bgfx_shader = BgfxShader()
+                self.shaders.append(shader)
+
+    def remove_platforms(self, platforms: set[ShaderPlatform]):
+        self.shaders = [s for s in self.shaders if s.platform not in platforms]
```

### Comparing `lazurite-0.1.4/src/lazurite/project/material_config.py` & `lazurite-0.1.5/src/lazurite/project/material_config.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-import pyjson5, copy, os
-from .compiler_type import CompilerType
-from lazurite.compiler.macro_define import MacroDefine
-from .shader_file_overwrite import ShaderFileOverwrite
-from lazurite.material.shader_pass.shader_definition import ShaderPlatform
-
-
-class MaterialConfig:
-    compiler_type: CompilerType
-    compiler_options: list[str]
-    macro_overwrite_pass: dict[str, list[MacroDefine]]
-    macro_overwrite_flags: dict[str, dict[str, list[MacroDefine]]]
-    file_overwrite_default: ShaderFileOverwrite
-    file_overwrite_pass: dict[str, ShaderFileOverwrite]
-    supported_platforms: set[ShaderPlatform]
-
-    def __init__(self) -> None:
-        self.compiler_type = CompilerType.SHADERC
-        self.compiler_options = []
-        self.macro_overwrite_pass = {}
-        self.macro_overwrite_flags = {}
-        self.file_overwrite_default = ShaderFileOverwrite()
-        self.file_overwrite_pass = {}
-        self.supported_platforms = set(ShaderPlatform)
-
-    def read_from_json_file(self, file_path: str):
-        if not os.path.isfile(file_path):
-            return
-
-        with open(file_path) as f:
-            mat_json = pyjson5.load(f)
-        self.read_json(mat_json)
-
-    def read_json(self, json_data: dict):
-        # Compiler config
-        compiler_config: dict = json_data.get("compiler", {})
-
-        self.compiler_type = (
-            CompilerType.from_name(compiler_config.get("type", ""))
-            or self.compiler_type
-        )
-        self.compiler_options = compiler_config.get("options", self.compiler_options)
-
-        # Macro overwrite
-        macro_overwrite: dict = json_data.get("macro_overwrite", {})
-        flags: dict[str, dict[str, list[str]]] = macro_overwrite.get("flags", {})
-        for _, values in flags.items():
-            for key, macros in values.items():
-                if type(macros) == str:
-                    macros = [macros]
-                values[key] = [MacroDefine.from_string(x) for x in macros]
-        self.macro_overwrite_flags = flags
-
-        passes: dict = macro_overwrite.get("passes", {})
-        for key, value in passes.items():
-            if type(value) == str:
-                value = [value]
-            passes[key] = [MacroDefine.from_string(m) for m in value]
-
-        self.macro_overwrite_pass = passes
-
-        # File overwrite
-        file_overwrite: dict = json_data.get("file_overwrite", {})
-        self.file_overwrite_default.read_json(file_overwrite.get("default", {}))
-        if "passes" in file_overwrite:
-            self.file_overwrite_pass = {}
-        for key, value in file_overwrite.get("passes", {}).items():
-            file_overwrite_pass = copy.copy(self.file_overwrite_default)
-            file_overwrite_pass.read_json(value)
-            self.file_overwrite_pass[key] = file_overwrite_pass
-
-        # Platforms
-        if "supported_platforms" in json_data:
-            self.supported_platforms = {
-                ShaderPlatform[x] for x in json_data["supported_platforms"]
-            }
+import pyjson5, copy, os
+from .compiler_type import CompilerType
+from lazurite.compiler.macro_define import MacroDefine
+from .shader_file_overwrite import ShaderFileOverwrite
+from lazurite.material.shader_pass.shader_definition import ShaderPlatform
+
+
+class MaterialConfig:
+    compiler_type: CompilerType
+    compiler_options: list[str]
+    macro_overwrite_pass: dict[str, list[MacroDefine]]
+    macro_overwrite_flags: dict[str, dict[str, list[MacroDefine]]]
+    file_overwrite_default: ShaderFileOverwrite
+    file_overwrite_pass: dict[str, ShaderFileOverwrite]
+    supported_platforms: set[ShaderPlatform]
+
+    def __init__(self) -> None:
+        self.compiler_type = CompilerType.SHADERC
+        self.compiler_options = []
+        self.macro_overwrite_pass = {}
+        self.macro_overwrite_flags = {}
+        self.file_overwrite_default = ShaderFileOverwrite()
+        self.file_overwrite_pass = {}
+        self.supported_platforms = set(ShaderPlatform)
+
+    def read_from_json_file(self, file_path: str):
+        if not os.path.isfile(file_path):
+            return
+
+        with open(file_path) as f:
+            mat_json = pyjson5.load(f)
+        self.read_json(mat_json)
+
+    def read_json(self, json_data: dict):
+        # Compiler config
+        compiler_config: dict = json_data.get("compiler", {})
+
+        self.compiler_type = (
+            CompilerType.from_name(compiler_config.get("type", ""))
+            or self.compiler_type
+        )
+        self.compiler_options = compiler_config.get("options", self.compiler_options)
+
+        # Macro overwrite
+        macro_overwrite: dict = json_data.get("macro_overwrite", {})
+        flags: dict[str, dict[str, list[str]]] = macro_overwrite.get("flags", {})
+        for _, values in flags.items():
+            for key, macros in values.items():
+                if type(macros) == str:
+                    macros = [macros]
+                values[key] = [MacroDefine.from_string(x) for x in macros]
+        self.macro_overwrite_flags = flags
+
+        passes: dict = macro_overwrite.get("passes", {})
+        for key, value in passes.items():
+            if type(value) == str:
+                value = [value]
+            passes[key] = [MacroDefine.from_string(m) for m in value]
+
+        self.macro_overwrite_pass = passes
+
+        # File overwrite
+        file_overwrite: dict = json_data.get("file_overwrite", {})
+        self.file_overwrite_default.read_json(file_overwrite.get("default", {}))
+        if "passes" in file_overwrite:
+            self.file_overwrite_pass = {}
+        for key, value in file_overwrite.get("passes", {}).items():
+            file_overwrite_pass = copy.copy(self.file_overwrite_default)
+            file_overwrite_pass.read_json(value)
+            self.file_overwrite_pass[key] = file_overwrite_pass
+
+        # Platforms
+        if "supported_platforms" in json_data:
+            self.supported_platforms = {
+                ShaderPlatform[x] for x in json_data["supported_platforms"]
+            }
```

### Comparing `lazurite-0.1.4/src/lazurite/project/project.py` & `lazurite-0.1.5/src/lazurite/project/project.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,367 +1,367 @@
-import os, pyjson5, pcpp, pathlib
-from concurrent.futures import ThreadPoolExecutor
-
-from .material_config import MaterialConfig
-from .compiler_type import CompilerType
-from .project_config import ProjectConfig
-
-from lazurite import util
-from lazurite.material import Material
-from lazurite.material.shader_pass.shader_definition import ShaderPlatform
-from lazurite.material.stage import ShaderStage
-from lazurite.compiler.shaderc import ShadercCompiler, generate_bgfx_defines
-from lazurite.compiler.dxc import DxcCompiler
-from lazurite.compiler.macro_define import MacroDefine
-from lazurite.material.shader_pass import Pass
-from lazurite.material.shader_pass.variant import Variant
-from lazurite.material.shader_pass.shader_definition import ShaderDefinition
-from lazurite.tempfile import CustomTempFile
-
-
-def _merge_source_by_name(
-    name: str,
-    platforms: list[ShaderPlatform],
-    merge_source: list[str],
-    cache: dict[str, tuple[str, set[ShaderPlatform]]],
-):
-    mat = None
-    for platform in platforms:
-        for path in merge_source:
-            found_platform = False
-            if path in cache:
-                cache_name, cache_platforms = cache[path]
-                if cache_name == name and platform in cache_platforms:
-                    found_platform = True
-                    temp_mat = Material.load_bin_file(path)
-                    if mat is None:
-                        mat = temp_mat
-                    else:
-                        mat.merge_variants(temp_mat)
-            else:
-                temp_mat = Material.load_bin_file(path)
-                mat_platforms = temp_mat.get_platforms()
-                if temp_mat.name == name and platform in mat_platforms:
-                    found_platform = True
-                    if mat is None:
-                        mat = temp_mat
-                    else:
-                        mat.merge_variants(temp_mat)
-                cache[path] = (temp_mat.name, mat_platforms)
-            if found_platform:
-                break
-    return mat
-
-
-def _merge_source_by_path(
-    name: str,
-    platforms: list[ShaderPlatform],
-    merge_source: list[str],
-    cache: dict[str, tuple[str, set[ShaderPlatform]]],
-):
-    mat = None
-    for platform in platforms:
-        for path in merge_source:
-            if os.path.basename(path) != name:
-                continue
-            found_platform = False
-            if path in cache:
-                if platform in cache[path][1]:
-                    found_platform = True
-                    temp_mat = Material.load_bin_file(path)
-                    if mat is None:
-                        mat = temp_mat
-                    else:
-                        mat.merge_variants(temp_mat)
-            else:
-                temp_mat = Material.load_bin_file(path)
-                mat_platforms = temp_mat.get_platforms()
-                if platform in mat_platforms:
-                    found_platform = True
-                    if mat is None:
-                        mat = temp_mat
-                    else:
-                        mat.merge_variants(temp_mat)
-                cache[path] = (temp_mat.name, mat_platforms)
-            if found_platform:
-                break
-    return mat
-
-
-def _merge_source_materials(
-    mat_dir: os.DirEntry,
-    platforms: list[ShaderPlatform],
-    merge_source: list[str],
-    material_cache: dict[str, tuple[str, set[ShaderPlatform]]],
-):
-    name = mat_dir.name + Material.EXTENSION
-    use_name = False
-    path = os.path.join(mat_dir, "material.json")
-    if os.path.isfile(path):
-        with open(path) as f:
-            json_data = pyjson5.load(f)
-        if "name" in json_data:
-            name = json_data["name"]
-            use_name = True
-
-    if use_name:
-        return _merge_source_by_name(name, platforms, merge_source, material_cache)
-    else:
-        return _merge_source_by_path(name, platforms, merge_source, material_cache)
-
-
-def _generate_defines(
-    config: ProjectConfig,
-    material: Material,
-    mat_config: MaterialConfig,
-    shader_pass: Pass,
-    variant: Variant,
-):
-    defines = config.macros[:]
-    if mat_config.compiler_type is CompilerType.SHADERC:
-        defines.append(MacroDefine("BGFX_CONFIG_MAX_BONES", 4))
-
-    defines.extend(MacroDefine(f"s_{s.name}_REG", s.reg1) for s in material.buffers)
-
-    if shader_pass.name in mat_config.macro_overwrite_pass:
-        defines.extend(mat_config.macro_overwrite_pass[shader_pass.name])
-    else:
-        defines.append(MacroDefine(util.generate_pass_name_macro(shader_pass.name)))
-
-    for key, value in variant.flags.items():
-        if (
-            key in mat_config.macro_overwrite_flags
-            and value in mat_config.macro_overwrite_flags[key]
-        ):
-            defines.extend(mat_config.macro_overwrite_flags[key][value])
-        else:
-            defines.append(MacroDefine(util.generate_flag_name_macro(key, value)))
-
-    return defines
-
-
-def _compile_bgfx_shader_async(
-    shaderc_compiler: ShadercCompiler,
-    code_path: str,
-    stage: ShaderStage,
-    platform: ShaderPlatform,
-    varying_path: str,
-    defines: list[MacroDefine],
-    options: list[str],
-):
-    if stage == ShaderStage.Compute:
-        compiled_shader = shaderc_compiler.compile(
-            code_path, platform, stage, None, None, defines, options
-        )
-    else:
-        parser = pcpp.Preprocessor()
-        parser.line_directive = None
-
-        varying_defines = defines + generate_bgfx_defines(platform, stage)
-        for macro in varying_defines:
-            parser.define(macro.format_cpp())
-
-        with open(varying_path) as f:
-            parser.parse(f)
-
-        with CustomTempFile("w+") as f:
-            parser.write(f)
-            f.close()
-            # f.flush()
-
-            compiled_shader = shaderc_compiler.compile(
-                code_path, platform, stage, f.name, None, defines, options
-            )
-
-    return compiled_shader
-
-
-def _get_material_folders(proj_config: ProjectConfig, project_path: str):
-    material_folders: set[pathlib.Path] = set()
-    proj_path = pathlib.Path(project_path)
-    for pattern in proj_config.include_patterns:
-        for path in proj_path.glob(pattern):
-            if path.is_dir() and not any(
-                path.match(p) for p in proj_config.exclude_patterns
-            ):
-                material_folders.add(path)
-    return sorted(list(material_folders))
-
-
-def compile(
-    project_path: str,
-    profiles: list[str],
-    output_folder: str = "",
-    defines: list[MacroDefine] = None,
-    shaderc_path: str = None,
-    dxc_path: str = None,
-    shaderc_args: list[str] = None,
-    dxc_args: list[str] = None,
-    max_workers: int = None,
-):
-    if not os.path.isdir(project_path):
-        raise Exception(f'Failed to compile project: "{project_path}" is not a folder.')
-
-    if profiles is None:
-        profiles = []
-
-    if shaderc_args is None:
-        shaderc_args = []
-
-    if dxc_args is None:
-        dxc_args = []
-
-    proj_config = ProjectConfig()
-    proj_config.read_json_file(os.path.join(project_path, "project.json"), profiles)
-    platforms_set = set(proj_config.platforms)
-
-    shaderc_compiler: ShadercCompiler = None
-    dxc_compiler: DxcCompiler = None
-
-    # {path: (name, {platforms})}
-    material_cache: dict[str, tuple[str, set[ShaderPlatform]]] = {}
-
-    for mat_dir in _get_material_folders(proj_config, project_path):
-        shaders: list[ShaderDefinition] = []
-        arg_defines: list[list[MacroDefine]] = []
-        arg_code_path: list[str] = []
-        arg_stage: list[ShaderStage] = []
-        arg_platform: list[ShaderPlatform] = []
-        arg_varying: list[str] = []
-        arg_entry_point: list[str] = []
-
-        print(mat_dir.name)
-
-        mat_config = MaterialConfig()
-        mat_config.read_from_json_file(os.path.join(mat_dir, "config.json"))
-
-        # Target platforms AND platforms supported by material.
-        compilable_platforms = platforms_set.intersection(
-            mat_config.supported_platforms
-        )
-
-        # Load and merge vanilla target platform materials.
-        material = (
-            _merge_source_materials(
-                mat_dir, proj_config.platforms, proj_config.merge_source, material_cache
-            )
-            or Material()
-        )
-
-        # If it failed to load any source materials.
-        if not material.get_platforms():
-            # Load and merge vanilla materials with any platforms.
-            temp_mat = _merge_source_materials(
-                mat_dir,
-                set(ShaderPlatform),
-                proj_config.merge_source,
-                material_cache,
-            )
-
-            if temp_mat:
-                material = temp_mat
-            elif proj_config.merge_source:
-                # Display a warning if no valid merge source was ever found
-                # but merge_source in project config is not empty.
-                print(f"Warning! Failed to find merge source for {mat_dir.name}")
-
-            # Add necessary platforms.
-            material.add_platforms(compilable_platforms)
-            # Remove other unwanted platforms.
-            material.remove_platforms(
-                set(ShaderPlatform).difference(compilable_platforms)
-            )
-        else:
-            material.add_platforms(compilable_platforms)
-
-        material.load_unpacked_material(mat_dir)
-
-        # Gather shaders for compilation.
-        for shader_pass in material.passes:
-            for variant in shader_pass.variants:
-                for shader in variant.shaders:
-                    if shader.platform not in compilable_platforms:
-                        continue
-
-                    file_overwrite = mat_config.file_overwrite_pass.get(
-                        shader_pass.name, mat_config.file_overwrite_default
-                    )
-                    code_path = os.path.normpath(
-                        os.path.join(mat_dir, file_overwrite.get_stage(shader.stage))
-                    )
-                    if not os.path.isfile(code_path):
-                        continue
-
-                    if mat_config.compiler_type is CompilerType.SHADERC:
-                        varying_path = None
-                        if shaderc_compiler is None:
-                            shaderc_compiler = ShadercCompiler(shaderc_path)
-                        if shader.stage is not ShaderStage.Compute:
-                            varying_path = os.path.normpath(
-                                os.path.join(mat_dir, file_overwrite.varying)
-                            )
-                            if not os.path.isfile(varying_path):
-                                print(
-                                    f'Varying file "{varying_path}" was not found! Skipping current shader.'
-                                )
-                                continue
-                        arg_varying.append(varying_path)
-                    else:
-                        if dxc_compiler is None:
-                            dxc_compiler = DxcCompiler(dxc_path)
-                        arg_entry_point.append(
-                            file_overwrite.entry_point or shader_pass.name
-                        )
-
-                    shaders.append(shader)
-                    arg_code_path.append(code_path)
-                    arg_stage.append(shader.stage)
-                    arg_platform.append(shader.platform)
-                    arg_defines.append(
-                        _generate_defines(
-                            proj_config, material, mat_config, shader_pass, variant
-                        )
-                        + defines
-                    )
-
-        with ThreadPoolExecutor(max_workers=max_workers) as executor:
-            if mat_config.compiler_type is CompilerType.SHADERC:
-                results = executor.map(
-                    _compile_bgfx_shader_async,
-                    len(shaders) * [shaderc_compiler],
-                    arg_code_path,
-                    arg_stage,
-                    arg_platform,
-                    arg_varying,
-                    arg_defines,
-                    len(shaders) * [mat_config.compiler_options + shaderc_args],
-                )
-            else:
-                results = executor.map(
-                    dxc_compiler.compile,
-                    arg_code_path,
-                    arg_platform,
-                    arg_stage,
-                    arg_entry_point,
-                    arg_defines,
-                    len(shaders) * [mat_config.compiler_options + dxc_args],
-                )
-
-        for shader, result in zip(shaders, results):
-            if mat_config.compiler_type is CompilerType.SHADERC:
-                shader.bgfx_shader = result
-            else:
-                shader.bgfx_shader.shader_bytes = result
-
-        # Filter empty shaders.
-        for shader_pass in material.passes:
-            for variant in shader_pass.variants:
-                new_shaders = []
-                for shader in variant.shaders:
-                    if shader.bgfx_shader.shader_bytes:
-                        new_shaders.append(shader)
-                variant.shaders = new_shaders
-
-        filepath = output_folder or os.path.dirname(project_path)
-        filepath = os.path.join(filepath, mat_dir.name + Material.EXTENSION)
-        with open(filepath, "wb") as f:
-            material.write(f)
+import os, pyjson5, pcpp, pathlib
+from concurrent.futures import ThreadPoolExecutor
+
+from .material_config import MaterialConfig
+from .compiler_type import CompilerType
+from .project_config import ProjectConfig
+
+from lazurite import util
+from lazurite.material import Material
+from lazurite.material.shader_pass.shader_definition import ShaderPlatform
+from lazurite.material.stage import ShaderStage
+from lazurite.compiler.shaderc import ShadercCompiler, generate_bgfx_defines
+from lazurite.compiler.dxc import DxcCompiler
+from lazurite.compiler.macro_define import MacroDefine
+from lazurite.material.shader_pass import Pass
+from lazurite.material.shader_pass.variant import Variant
+from lazurite.material.shader_pass.shader_definition import ShaderDefinition
+from lazurite.tempfile import CustomTempFile
+
+
+def _merge_source_by_name(
+    name: str,
+    platforms: list[ShaderPlatform],
+    merge_source: list[str],
+    cache: dict[str, tuple[str, set[ShaderPlatform]]],
+):
+    mat = None
+    for platform in platforms:
+        for path in merge_source:
+            found_platform = False
+            if path in cache:
+                cache_name, cache_platforms = cache[path]
+                if cache_name == name and platform in cache_platforms:
+                    found_platform = True
+                    temp_mat = Material.load_bin_file(path)
+                    if mat is None:
+                        mat = temp_mat
+                    else:
+                        mat.merge_variants(temp_mat)
+            else:
+                temp_mat = Material.load_bin_file(path)
+                mat_platforms = temp_mat.get_platforms()
+                if temp_mat.name == name and platform in mat_platforms:
+                    found_platform = True
+                    if mat is None:
+                        mat = temp_mat
+                    else:
+                        mat.merge_variants(temp_mat)
+                cache[path] = (temp_mat.name, mat_platforms)
+            if found_platform:
+                break
+    return mat
+
+
+def _merge_source_by_path(
+    name: str,
+    platforms: list[ShaderPlatform],
+    merge_source: list[str],
+    cache: dict[str, tuple[str, set[ShaderPlatform]]],
+):
+    mat = None
+    for platform in platforms:
+        for path in merge_source:
+            if os.path.basename(path) != name:
+                continue
+            found_platform = False
+            if path in cache:
+                if platform in cache[path][1]:
+                    found_platform = True
+                    temp_mat = Material.load_bin_file(path)
+                    if mat is None:
+                        mat = temp_mat
+                    else:
+                        mat.merge_variants(temp_mat)
+            else:
+                temp_mat = Material.load_bin_file(path)
+                mat_platforms = temp_mat.get_platforms()
+                if platform in mat_platforms:
+                    found_platform = True
+                    if mat is None:
+                        mat = temp_mat
+                    else:
+                        mat.merge_variants(temp_mat)
+                cache[path] = (temp_mat.name, mat_platforms)
+            if found_platform:
+                break
+    return mat
+
+
+def _merge_source_materials(
+    mat_dir: os.DirEntry,
+    platforms: list[ShaderPlatform],
+    merge_source: list[str],
+    material_cache: dict[str, tuple[str, set[ShaderPlatform]]],
+):
+    name = mat_dir.name + Material.EXTENSION
+    use_name = False
+    path = os.path.join(mat_dir, "material.json")
+    if os.path.isfile(path):
+        with open(path) as f:
+            json_data = pyjson5.load(f)
+        if "name" in json_data:
+            name = json_data["name"]
+            use_name = True
+
+    if use_name:
+        return _merge_source_by_name(name, platforms, merge_source, material_cache)
+    else:
+        return _merge_source_by_path(name, platforms, merge_source, material_cache)
+
+
+def _generate_defines(
+    config: ProjectConfig,
+    material: Material,
+    mat_config: MaterialConfig,
+    shader_pass: Pass,
+    variant: Variant,
+):
+    defines = config.macros[:]
+    if mat_config.compiler_type is CompilerType.SHADERC:
+        defines.append(MacroDefine("BGFX_CONFIG_MAX_BONES", 4))
+
+    defines.extend(MacroDefine(f"s_{s.name}_REG", s.reg1) for s in material.buffers)
+
+    if shader_pass.name in mat_config.macro_overwrite_pass:
+        defines.extend(mat_config.macro_overwrite_pass[shader_pass.name])
+    else:
+        defines.append(MacroDefine(util.generate_pass_name_macro(shader_pass.name)))
+
+    for key, value in variant.flags.items():
+        if (
+            key in mat_config.macro_overwrite_flags
+            and value in mat_config.macro_overwrite_flags[key]
+        ):
+            defines.extend(mat_config.macro_overwrite_flags[key][value])
+        else:
+            defines.append(MacroDefine(util.generate_flag_name_macro(key, value)))
+
+    return defines
+
+
+def _compile_bgfx_shader_async(
+    shaderc_compiler: ShadercCompiler,
+    code_path: str,
+    stage: ShaderStage,
+    platform: ShaderPlatform,
+    varying_path: str,
+    defines: list[MacroDefine],
+    options: list[str],
+):
+    if stage == ShaderStage.Compute:
+        compiled_shader = shaderc_compiler.compile(
+            code_path, platform, stage, None, None, defines, options
+        )
+    else:
+        parser = pcpp.Preprocessor()
+        parser.line_directive = None
+
+        varying_defines = defines + generate_bgfx_defines(platform, stage)
+        for macro in varying_defines:
+            parser.define(macro.format_cpp())
+
+        with open(varying_path) as f:
+            parser.parse(f)
+
+        with CustomTempFile("w+") as f:
+            parser.write(f)
+            f.close()
+            # f.flush()
+
+            compiled_shader = shaderc_compiler.compile(
+                code_path, platform, stage, f.name, None, defines, options
+            )
+
+    return compiled_shader
+
+
+def _get_material_folders(proj_config: ProjectConfig, project_path: str):
+    material_folders: set[pathlib.Path] = set()
+    proj_path = pathlib.Path(project_path)
+    for pattern in proj_config.include_patterns:
+        for path in proj_path.glob(pattern):
+            if path.is_dir() and not any(
+                path.match(p) for p in proj_config.exclude_patterns
+            ):
+                material_folders.add(path)
+    return sorted(list(material_folders))
+
+
+def compile(
+    project_path: str,
+    profiles: list[str],
+    output_folder: str = "",
+    defines: list[MacroDefine] = None,
+    shaderc_path: str = None,
+    dxc_path: str = None,
+    shaderc_args: list[str] = None,
+    dxc_args: list[str] = None,
+    max_workers: int = None,
+):
+    if not os.path.isdir(project_path):
+        raise Exception(f'Failed to compile project: "{project_path}" is not a folder.')
+
+    if profiles is None:
+        profiles = []
+
+    if shaderc_args is None:
+        shaderc_args = []
+
+    if dxc_args is None:
+        dxc_args = []
+
+    proj_config = ProjectConfig()
+    proj_config.read_json_file(os.path.join(project_path, "project.json"), profiles)
+    platforms_set = set(proj_config.platforms)
+
+    shaderc_compiler: ShadercCompiler = None
+    dxc_compiler: DxcCompiler = None
+
+    # {path: (name, {platforms})}
+    material_cache: dict[str, tuple[str, set[ShaderPlatform]]] = {}
+
+    for mat_dir in _get_material_folders(proj_config, project_path):
+        shaders: list[ShaderDefinition] = []
+        arg_defines: list[list[MacroDefine]] = []
+        arg_code_path: list[str] = []
+        arg_stage: list[ShaderStage] = []
+        arg_platform: list[ShaderPlatform] = []
+        arg_varying: list[str] = []
+        arg_entry_point: list[str] = []
+
+        print(mat_dir.name)
+
+        mat_config = MaterialConfig()
+        mat_config.read_from_json_file(os.path.join(mat_dir, "config.json"))
+
+        # Target platforms AND platforms supported by material.
+        compilable_platforms = platforms_set.intersection(
+            mat_config.supported_platforms
+        )
+
+        # Load and merge vanilla target platform materials.
+        material = (
+            _merge_source_materials(
+                mat_dir, proj_config.platforms, proj_config.merge_source, material_cache
+            )
+            or Material()
+        )
+
+        # If it failed to load any source materials.
+        if not material.get_platforms():
+            # Load and merge vanilla materials with any platforms.
+            temp_mat = _merge_source_materials(
+                mat_dir,
+                set(ShaderPlatform),
+                proj_config.merge_source,
+                material_cache,
+            )
+
+            if temp_mat:
+                material = temp_mat
+            elif proj_config.merge_source:
+                # Display a warning if no valid merge source was ever found
+                # but merge_source in project config is not empty.
+                print(f"Warning! Failed to find merge source for {mat_dir.name}")
+
+            # Add necessary platforms.
+            material.add_platforms(compilable_platforms)
+            # Remove other unwanted platforms.
+            material.remove_platforms(
+                set(ShaderPlatform).difference(compilable_platforms)
+            )
+        else:
+            material.add_platforms(compilable_platforms)
+
+        material.load_unpacked_material(mat_dir)
+
+        # Gather shaders for compilation.
+        for shader_pass in material.passes:
+            for variant in shader_pass.variants:
+                for shader in variant.shaders:
+                    if shader.platform not in compilable_platforms:
+                        continue
+
+                    file_overwrite = mat_config.file_overwrite_pass.get(
+                        shader_pass.name, mat_config.file_overwrite_default
+                    )
+                    code_path = os.path.normpath(
+                        os.path.join(mat_dir, file_overwrite.get_stage(shader.stage))
+                    )
+                    if not os.path.isfile(code_path):
+                        continue
+
+                    if mat_config.compiler_type is CompilerType.SHADERC:
+                        varying_path = None
+                        if shaderc_compiler is None:
+                            shaderc_compiler = ShadercCompiler(shaderc_path)
+                        if shader.stage is not ShaderStage.Compute:
+                            varying_path = os.path.normpath(
+                                os.path.join(mat_dir, file_overwrite.varying)
+                            )
+                            if not os.path.isfile(varying_path):
+                                print(
+                                    f'Varying file "{varying_path}" was not found! Skipping current shader.'
+                                )
+                                continue
+                        arg_varying.append(varying_path)
+                    else:
+                        if dxc_compiler is None:
+                            dxc_compiler = DxcCompiler(dxc_path)
+                        arg_entry_point.append(
+                            file_overwrite.entry_point or shader_pass.name
+                        )
+
+                    shaders.append(shader)
+                    arg_code_path.append(code_path)
+                    arg_stage.append(shader.stage)
+                    arg_platform.append(shader.platform)
+                    arg_defines.append(
+                        _generate_defines(
+                            proj_config, material, mat_config, shader_pass, variant
+                        )
+                        + defines
+                    )
+
+        with ThreadPoolExecutor(max_workers=max_workers) as executor:
+            if mat_config.compiler_type is CompilerType.SHADERC:
+                results = executor.map(
+                    _compile_bgfx_shader_async,
+                    len(shaders) * [shaderc_compiler],
+                    arg_code_path,
+                    arg_stage,
+                    arg_platform,
+                    arg_varying,
+                    arg_defines,
+                    len(shaders) * [mat_config.compiler_options + shaderc_args],
+                )
+            else:
+                results = executor.map(
+                    dxc_compiler.compile,
+                    arg_code_path,
+                    arg_platform,
+                    arg_stage,
+                    arg_entry_point,
+                    arg_defines,
+                    len(shaders) * [mat_config.compiler_options + dxc_args],
+                )
+
+        for shader, result in zip(shaders, results):
+            if mat_config.compiler_type is CompilerType.SHADERC:
+                shader.bgfx_shader = result
+            else:
+                shader.bgfx_shader.shader_bytes = result
+
+        # Filter empty shaders.
+        for shader_pass in material.passes:
+            for variant in shader_pass.variants:
+                new_shaders = []
+                for shader in variant.shaders:
+                    if shader.bgfx_shader.shader_bytes:
+                        new_shaders.append(shader)
+                variant.shaders = new_shaders
+
+        filepath = output_folder or os.path.dirname(project_path)
+        filepath = os.path.join(filepath, mat_dir.name + Material.EXTENSION)
+        with open(filepath, "wb") as f:
+            material.write(f)
```

### Comparing `lazurite-0.1.4/src/lazurite/project/project_config.py` & `lazurite-0.1.5/src/lazurite/project/project_config.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-import os, pyjson5
-from lazurite.material import Material
-from lazurite.material.shader_pass.shader_definition import ShaderPlatform
-from lazurite.compiler.macro_define import MacroDefine
-
-
-class ProjectConfig:
-    macros: list[MacroDefine]
-    platforms: list[ShaderPlatform]
-    merge_source: list[str]
-    include_patterns: list[str]
-    exclude_patterns: list[str]
-
-    def __init__(self) -> None:
-        self.macros = []
-        self.platforms = []
-        self.merge_source = []
-        self.include_patterns = ["*"]
-        self.exclude_patterns = [".*", "_*"]
-
-    def read_json_file(self, path: str, profiles: list[str]):
-        def append_unique(target: list, source: list):
-            """
-            Appends elements from source to target, if they aren't in target list already.
-            """
-            target.extend((item for item in source if item not in target))
-
-        if not os.path.isfile(path):
-            return
-        with open(path) as f:
-            json_data = pyjson5.load(f)
-        has_macros = False
-        has_platforms = False
-        has_merge = False
-        has_include_pattern = False
-        has_exclude_pattern = False
-        if "profiles" in json_data:
-            json_profiles = json_data["profiles"]
-            for profile in profiles:
-                if profile not in json_profiles:
-                    print(f'Warning: profile "{profile}" was not found!')
-                    continue
-                profile = json_profiles[profile]
-
-                if "macros" in profile:
-                    if not has_macros:
-                        self.macros = []
-                        has_macros = True
-                    append_unique(
-                        self.macros,
-                        [MacroDefine.from_string(m) for m in profile["macros"]],
-                    )
-
-                if "platforms" in profile:
-                    if not has_platforms:
-                        self.platforms = []
-                        has_platforms = True
-                    append_unique(
-                        self.platforms,
-                        (ShaderPlatform[p] for p in profile["platforms"]),
-                    )
-
-                if "merge_source" in profile:
-                    if not has_merge:
-                        self.merge_source = []
-                        has_merge = True
-                    append_unique(self.merge_source, profile["merge_source"])
-
-                if "include_patterns" in profile:
-                    if not has_include_pattern:
-                        self.include_patterns = []
-                        has_include_pattern = True
-                    patterns = profile["include_patterns"]
-                    append_unique(
-                        self.include_patterns,
-                        [patterns] if type(patterns) == str else patterns,
-                    )
-
-                if "exclude_patterns" in profile:
-                    if not has_exclude_pattern:
-                        self.exclude_patterns = []
-                        has_exclude_pattern = True
-                    patterns = profile["exclude_patterns"]
-                    append_unique(
-                        self.exclude_patterns,
-                        [patterns] if type(patterns) == str else patterns,
-                    )
-
-        if "base_profile" in json_data:
-            base_profile = json_data["base_profile"]
-            if "macros" in base_profile and not has_macros:
-                self.macros = [
-                    MacroDefine.from_string(m) for m in base_profile["macros"]
-                ]
-
-            if "platforms" in base_profile and not has_platforms:
-                self.platforms = [ShaderPlatform[p] for p in base_profile["platforms"]]
-
-            if "merge_source" in base_profile and not has_merge:
-                self.merge_source = base_profile["merge_source"]
-
-            if "include_patterns" in base_profile and not has_include_pattern:
-                patterns = base_profile["include_patterns"]
-                self.include_patterns = (
-                    [patterns] if type(patterns) == str else patterns
-                )
-
-            if "exclude_patterns" in base_profile and not has_exclude_pattern:
-                patterns = base_profile["exclude_patterns"]
-                self.exclude_patterns = (
-                    [patterns] if type(patterns) == str else patterns
-                )
-
-        new_merge_source = []
-        for merge_path in self.merge_source:
-            merge_path = os.path.normpath(
-                os.path.join(os.path.split(path)[0], merge_path)
-            )
-            if (
-                os.path.isfile(merge_path)
-                and merge_path not in new_merge_source
-                and merge_path.endswith(Material.EXTENSION)
-            ):
-                new_merge_source.append(merge_path)
-            elif os.path.isdir(merge_path):
-                for mat_dir in os.scandir(merge_path):
-                    if (
-                        mat_dir.is_file()
-                        and mat_dir.path not in new_merge_source
-                        and mat_dir.path.endswith(Material.EXTENSION)
-                    ):
-                        new_merge_source.append(mat_dir.path)
-            else:
-                print(f'Warning: merge path "{merge_path}" was not found')
-        self.merge_source = new_merge_source
+import os, pyjson5
+from lazurite.material import Material
+from lazurite.material.shader_pass.shader_definition import ShaderPlatform
+from lazurite.compiler.macro_define import MacroDefine
+
+
+class ProjectConfig:
+    macros: list[MacroDefine]
+    platforms: list[ShaderPlatform]
+    merge_source: list[str]
+    include_patterns: list[str]
+    exclude_patterns: list[str]
+
+    def __init__(self) -> None:
+        self.macros = []
+        self.platforms = []
+        self.merge_source = []
+        self.include_patterns = ["*"]
+        self.exclude_patterns = [".*", "_*"]
+
+    def read_json_file(self, path: str, profiles: list[str]):
+        def append_unique(target: list, source: list):
+            """
+            Appends elements from source to target, if they aren't in target list already.
+            """
+            target.extend((item for item in source if item not in target))
+
+        if not os.path.isfile(path):
+            return
+        with open(path) as f:
+            json_data = pyjson5.load(f)
+        has_macros = False
+        has_platforms = False
+        has_merge = False
+        has_include_pattern = False
+        has_exclude_pattern = False
+        if "profiles" in json_data:
+            json_profiles = json_data["profiles"]
+            for profile in profiles:
+                if profile not in json_profiles:
+                    print(f'Warning: profile "{profile}" was not found!')
+                    continue
+                profile = json_profiles[profile]
+
+                if "macros" in profile:
+                    if not has_macros:
+                        self.macros = []
+                        has_macros = True
+                    append_unique(
+                        self.macros,
+                        [MacroDefine.from_string(m) for m in profile["macros"]],
+                    )
+
+                if "platforms" in profile:
+                    if not has_platforms:
+                        self.platforms = []
+                        has_platforms = True
+                    append_unique(
+                        self.platforms,
+                        (ShaderPlatform[p] for p in profile["platforms"]),
+                    )
+
+                if "merge_source" in profile:
+                    if not has_merge:
+                        self.merge_source = []
+                        has_merge = True
+                    append_unique(self.merge_source, profile["merge_source"])
+
+                if "include_patterns" in profile:
+                    if not has_include_pattern:
+                        self.include_patterns = []
+                        has_include_pattern = True
+                    patterns = profile["include_patterns"]
+                    append_unique(
+                        self.include_patterns,
+                        [patterns] if type(patterns) == str else patterns,
+                    )
+
+                if "exclude_patterns" in profile:
+                    if not has_exclude_pattern:
+                        self.exclude_patterns = []
+                        has_exclude_pattern = True
+                    patterns = profile["exclude_patterns"]
+                    append_unique(
+                        self.exclude_patterns,
+                        [patterns] if type(patterns) == str else patterns,
+                    )
+
+        if "base_profile" in json_data:
+            base_profile = json_data["base_profile"]
+            if "macros" in base_profile and not has_macros:
+                self.macros = [
+                    MacroDefine.from_string(m) for m in base_profile["macros"]
+                ]
+
+            if "platforms" in base_profile and not has_platforms:
+                self.platforms = [ShaderPlatform[p] for p in base_profile["platforms"]]
+
+            if "merge_source" in base_profile and not has_merge:
+                self.merge_source = base_profile["merge_source"]
+
+            if "include_patterns" in base_profile and not has_include_pattern:
+                patterns = base_profile["include_patterns"]
+                self.include_patterns = (
+                    [patterns] if type(patterns) == str else patterns
+                )
+
+            if "exclude_patterns" in base_profile and not has_exclude_pattern:
+                patterns = base_profile["exclude_patterns"]
+                self.exclude_patterns = (
+                    [patterns] if type(patterns) == str else patterns
+                )
+
+        new_merge_source = []
+        for merge_path in self.merge_source:
+            merge_path = os.path.normpath(
+                os.path.join(os.path.split(path)[0], merge_path)
+            )
+            if (
+                os.path.isfile(merge_path)
+                and merge_path not in new_merge_source
+                and merge_path.endswith(Material.EXTENSION)
+            ):
+                new_merge_source.append(merge_path)
+            elif os.path.isdir(merge_path):
+                for mat_dir in os.scandir(merge_path):
+                    if (
+                        mat_dir.is_file()
+                        and mat_dir.path not in new_merge_source
+                        and mat_dir.path.endswith(Material.EXTENSION)
+                    ):
+                        new_merge_source.append(mat_dir.path)
+            else:
+                print(f'Warning: merge path "{merge_path}" was not found')
+        self.merge_source = new_merge_source
```

### Comparing `lazurite-0.1.4/src/lazurite/project/shader_file_overwrite.py` & `lazurite-0.1.5/src/lazurite/project/shader_file_overwrite.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from lazurite.material.stage import ShaderStage
-
-
-class ShaderFileOverwrite:
-    entry_point: str
-    fragment: str
-    vertex: str
-    compute: str
-    unknown: str
-    varying: str
-
-    def __init__(self) -> None:
-        self.entry_point = ""
-        self.fragment = "shaders/fragment.sc"
-        self.vertex = "shaders/vertex.sc"
-        self.compute = "shaders/compute.sc"
-        self.unknown = "shaders/unknown.sc"
-        self.varying = "shaders/varying.def.sc"
-
-    def read_json(self, json_data: dict):
-        self.entry_point = json_data.get("entry_point", self.entry_point)
-        self.fragment = json_data.get("fragment", self.fragment)
-        self.vertex = json_data.get("vertex", self.vertex)
-        self.compute = json_data.get("compute", self.compute)
-        self.unknown = json_data.get("unknown", self.unknown)
-        self.varying = json_data.get("varying", self.varying)
-
-    def get_stage(self, stage: ShaderStage):
-        if stage == ShaderStage.Fragment:
-            return self.fragment
-        if stage == ShaderStage.Vertex:
-            return self.vertex
-        if stage == ShaderStage.Compute:
-            return self.compute
-        if stage == ShaderStage.Unknown:
-            return self.unknown
+from lazurite.material.stage import ShaderStage
+
+
+class ShaderFileOverwrite:
+    entry_point: str
+    fragment: str
+    vertex: str
+    compute: str
+    unknown: str
+    varying: str
+
+    def __init__(self) -> None:
+        self.entry_point = ""
+        self.fragment = "shaders/fragment.sc"
+        self.vertex = "shaders/vertex.sc"
+        self.compute = "shaders/compute.sc"
+        self.unknown = "shaders/unknown.sc"
+        self.varying = "shaders/varying.def.sc"
+
+    def read_json(self, json_data: dict):
+        self.entry_point = json_data.get("entry_point", self.entry_point)
+        self.fragment = json_data.get("fragment", self.fragment)
+        self.vertex = json_data.get("vertex", self.vertex)
+        self.compute = json_data.get("compute", self.compute)
+        self.unknown = json_data.get("unknown", self.unknown)
+        self.varying = json_data.get("varying", self.varying)
+
+    def get_stage(self, stage: ShaderStage):
+        if stage == ShaderStage.Fragment:
+            return self.fragment
+        if stage == ShaderStage.Vertex:
+            return self.vertex
+        if stage == ShaderStage.Compute:
+            return self.compute
+        if stage == ShaderStage.Unknown:
+            return self.unknown
```

### Comparing `lazurite-0.1.4/src/lazurite/tempfile.py` & `lazurite-0.1.5/src/lazurite/tempfile.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import contextlib, tempfile, os
-
-# from typing import TypeVar, Callable, Any, Generic
-
-# F = TypeVar("F", bound=Callable[..., Any])
-
-
-# class copy_signature(Generic[F]):
-#     def __init__(self, target: F) -> None: ...
-#     def __call__(self, wrapped: Callable[..., Any]) -> F: ...
-
-
-# this is a backport of delete_on_close functionality from 3.12
-@contextlib.contextmanager
-# @copy_signature(tempfile.NamedTemporaryFile)
-def CustomTempFile(*args, **kwargs):
-    """
-    Context manager for tempfile.NamedTemporaryFile which implements automatic file deletion on exit.
-    """
-    kwargs["delete"] = False
-    file = tempfile.NamedTemporaryFile(*args, **kwargs)
-    try:
-        yield file
-    finally:
-        file.close()
-        with contextlib.suppress(FileNotFoundError):
-            os.remove(file.name)
+import contextlib, tempfile, os
+
+# from typing import TypeVar, Callable, Any, Generic
+
+# F = TypeVar("F", bound=Callable[..., Any])
+
+
+# class copy_signature(Generic[F]):
+#     def __init__(self, target: F) -> None: ...
+#     def __call__(self, wrapped: Callable[..., Any]) -> F: ...
+
+
+# this is a backport of delete_on_close functionality from 3.12
+@contextlib.contextmanager
+# @copy_signature(tempfile.NamedTemporaryFile)
+def CustomTempFile(*args, **kwargs):
+    """
+    Context manager for tempfile.NamedTemporaryFile which implements automatic file deletion on exit.
+    """
+    kwargs["delete"] = False
+    file = tempfile.NamedTemporaryFile(*args, **kwargs)
+    try:
+        yield file
+    finally:
+        file.close()
+        with contextlib.suppress(FileNotFoundError):
+            os.remove(file.name)
```

### Comparing `lazurite-0.1.4/src/lazurite/util.py` & `lazurite-0.1.5/src/lazurite/util.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-from io import BytesIO
-import struct
-import re
-
-
-# Reading binary files.
-def read_ulonglong(f: BytesIO) -> int:
-    return struct.unpack("<Q", f.read(8))[0]
-
-
-def read_ulong(f: BytesIO) -> int:
-    return struct.unpack("<L", f.read(4))[0]
-
-
-def read_bool(f: BytesIO) -> bool:
-    return struct.unpack("<?", f.read(1))[0]
-
-
-def read_ubyte(f: BytesIO) -> int:
-    return struct.unpack("<B", f.read(1))[0]
-
-
-def read_ushort(f: BytesIO) -> int:
-    return struct.unpack("<H", f.read(2))[0]
-
-
-def read_array(f: BytesIO) -> bytes:
-    return f.read(struct.unpack("<I", f.read(4))[0])
-
-
-def read_string(f: BytesIO) -> str:
-    return read_array(f).decode()
-
-
-# writing binary files.
-def write_ulonglong(f: BytesIO, val: int):
-    f.write(struct.pack("<Q", val))
-
-
-def write_ulong(f: BytesIO, val: int):
-    f.write(struct.pack("<L", val))
-
-
-def write_bool(f: BytesIO, val: bool):
-    f.write(struct.pack("<?", val))
-
-
-def write_ubyte(f: BytesIO, val: int):
-    f.write(struct.pack("<B", val))
-
-
-def write_ushort(f: BytesIO, val: int):
-    f.write(struct.pack("<H", val))
-
-
-def write_array(f: BytesIO, val: bytes):
-    f.write(struct.pack("<I", len(val)))
-    f.write(val)
-
-
-def write_string(f: BytesIO, val: str):
-    write_array(f, val.encode())
-
-
-def format_definition_name(name: str):
-    # aA -> a_A
-    name = re.sub(r"([a-z]+)([A-Z])", r"\1_\2", name)
-    # AAa -> A_Aa
-    name = re.sub(r"([A-Z]+)([A-Z][a-z])", r"\1_\2", name)
-    # X00 -> X_00
-    # name = re.sub(r"([a-zA-Z])(\d+)", r"\1_\2", name)
-    # 00X -> 00_X
-    name = re.sub(r"(\d+)([a-zA-Z])", r"\1_\2", name)
-    return name.upper()
-
-
-def generate_flag_name_macro(key: str, value: str, is_bool: bool = False):
-    if is_bool:
-        return format_definition_name(key)
-    else:
-        return format_definition_name(key + "__" + value)
-
-
-def generate_pass_name_macro(name: str):
-    name = format_definition_name(name)
-    if name.endswith("_PASS"):
-        return name
-    return name + "_PASS"
-
-
-def insert_header_comment(code: str, comment: str):
-    if code.startswith("#version"):
-        return code.replace("\n", "\n\n" + comment + "\n\n", 1)
-    else:
-        return comment + "\n\n" + code
+from io import BytesIO
+import struct
+import re
+
+
+# Reading binary files.
+def read_ulonglong(f: BytesIO) -> int:
+    return struct.unpack("<Q", f.read(8))[0]
+
+
+def read_ulong(f: BytesIO) -> int:
+    return struct.unpack("<L", f.read(4))[0]
+
+
+def read_bool(f: BytesIO) -> bool:
+    return struct.unpack("<?", f.read(1))[0]
+
+
+def read_ubyte(f: BytesIO) -> int:
+    return struct.unpack("<B", f.read(1))[0]
+
+
+def read_ushort(f: BytesIO) -> int:
+    return struct.unpack("<H", f.read(2))[0]
+
+
+def read_array(f: BytesIO) -> bytes:
+    return f.read(struct.unpack("<I", f.read(4))[0])
+
+
+def read_string(f: BytesIO) -> str:
+    return read_array(f).decode()
+
+
+# writing binary files.
+def write_ulonglong(f: BytesIO, val: int):
+    f.write(struct.pack("<Q", val))
+
+
+def write_ulong(f: BytesIO, val: int):
+    f.write(struct.pack("<L", val))
+
+
+def write_bool(f: BytesIO, val: bool):
+    f.write(struct.pack("<?", val))
+
+
+def write_ubyte(f: BytesIO, val: int):
+    f.write(struct.pack("<B", val))
+
+
+def write_ushort(f: BytesIO, val: int):
+    f.write(struct.pack("<H", val))
+
+
+def write_array(f: BytesIO, val: bytes):
+    f.write(struct.pack("<I", len(val)))
+    f.write(val)
+
+
+def write_string(f: BytesIO, val: str):
+    write_array(f, val.encode())
+
+
+def format_definition_name(name: str):
+    # aA -> a_A
+    name = re.sub(r"([a-z]+)([A-Z])", r"\1_\2", name)
+    # AAa -> A_Aa
+    name = re.sub(r"([A-Z]+)([A-Z][a-z])", r"\1_\2", name)
+    # X00 -> X_00
+    # name = re.sub(r"([a-zA-Z])(\d+)", r"\1_\2", name)
+    # 00X -> 00_X
+    name = re.sub(r"(\d+)([a-zA-Z])", r"\1_\2", name)
+    return name.upper()
+
+
+def generate_flag_name_macro(key: str, value: str, is_bool: bool = False):
+    if is_bool:
+        return format_definition_name(key)
+    else:
+        return format_definition_name(key + "__" + value)
+
+
+def generate_pass_name_macro(name: str):
+    name = format_definition_name(name)
+    if name.endswith("_PASS"):
+        return name
+    return name + "_PASS"
+
+
+def insert_header_comment(code: str, comment: str):
+    if code.startswith("#version"):
+        return code.replace("\n", "\n\n" + comment + "\n\n", 1)
+    else:
+        return comment + "\n\n" + code
```

### Comparing `lazurite-0.1.4/src/lazurite.egg-info/PKG-INFO` & `lazurite-0.1.5/src/lazurite.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-Metadata-Version: 2.1
-Name: lazurite
-Version: 0.1.4
-Summary: Unofficial shader development tool for Minecraft: Bedrock Edition with RenderDragon graphics engine
-Author: veka0
-Project-URL: Documentation, https://veka0.github.io/lazurite
-Project-URL: Repository, https://github.com/veka0/lazurite
-Keywords: shader,minecraft,bedrock,renderdragon
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: Android
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Topic :: Software Development :: Compilers
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pyjson5
-Requires-Dist: myers
-Requires-Dist: pcpp
-Requires-Dist: pycryptodome
-Requires-Dist: sympy
-
-# Lazurite
-
-Unofficial shader development tool for Minecraft: Bedrock Edition with RenderDragon graphics engine.
-
-Documentation: <https://veka0.github.io/lazurite>
-
-PyPi page: <https://pypi.org/project/lazurite>
-
-## Installation
-
-Lazurite requires to have Python 3.10+ installed, but 3.12 is recommended.
-
-Official python installation page: <https://www.python.org/downloads>.
-Windows users are recommended to install Python from Microsoft Store.
-
-After installing python, you can install lazurite package from pypi repository, with a command
-
-```sh
-pip install lazurite
-```
-
-or
-
-```sh
-python -m pip install lazurite
-```
-
-## Next steps
-
-Read the documentation here <https://veka0.github.io/lazurite>
+Metadata-Version: 2.1
+Name: lazurite
+Version: 0.1.5
+Summary: Unofficial shader development tool for Minecraft: Bedrock Edition with RenderDragon graphics engine
+Author: veka0
+Project-URL: Documentation, https://veka0.github.io/lazurite
+Project-URL: Repository, https://github.com/veka0/lazurite
+Keywords: shader,minecraft,bedrock,renderdragon
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Operating System :: Android
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Compilers
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pyjson5
+Requires-Dist: myers
+Requires-Dist: pcpp
+Requires-Dist: pycryptodome
+Requires-Dist: sympy
+
+# Lazurite
+
+Unofficial shader development tool for Minecraft: Bedrock Edition with RenderDragon graphics engine.
+
+Documentation: <https://veka0.github.io/lazurite>
+
+PyPi page: <https://pypi.org/project/lazurite>
+
+## Installation
+
+Lazurite requires to have Python 3.10+ installed, but 3.12 is recommended.
+
+Official python installation page: <https://www.python.org/downloads>.
+Windows users are recommended to install Python from Microsoft Store.
+
+After installing python, you can install lazurite package from pypi repository, with a command
+
+```sh
+pip install lazurite
+```
+
+or
+
+```sh
+python -m pip install lazurite
+```
+
+## Next steps
+
+Read the documentation here <https://veka0.github.io/lazurite>
```

### Comparing `lazurite-0.1.4/src/lazurite.egg-info/SOURCES.txt` & `lazurite-0.1.5/src/lazurite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

