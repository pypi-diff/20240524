# Comparing `tmp/neofbs-1.2.4.tar.gz` & `tmp/neofbs-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neofbs-1.2.4.tar", last modified: Fri May 24 15:11:23 2024, max compression
+gzip compressed data, was "neofbs-1.2.5.tar", last modified: Fri May 24 15:12:44 2024, max compression
```

## Comparing `neofbs-1.2.4.tar` & `neofbs-1.2.5.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.603874 neofbs-1.2.4/
--rw-rw-rw-   0        0        0    35821 2024-05-24 14:55:11.000000 neofbs-1.2.4/LICENSE
--rw-rw-rw-   0        0        0    12994 2024-05-24 14:55:11.000000 neofbs-1.2.4/NOTICE
--rw-rw-rw-   0        0        0     1341 2024-05-24 15:11:23.602873 neofbs-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       94 2024-05-24 14:55:11.000000 neofbs-1.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.512556 neofbs-1.2.4/fbs/
--rw-rw-rw-   0        0        0     2452 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/__init__.py
--rw-rw-rw-   0        0        0     1755 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/__main__.py
--rw-rw-rw-   0        0        0     1080 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_aws.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.491544 neofbs-1.2.4/fbs/_defaults/
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.516556 neofbs-1.2.4/fbs/_defaults/requirements/
--rw-rw-rw-   0        0        0      138 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/requirements/arch.txt
--rw-rw-rw-   0        0        0       10 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/requirements/base.txt
--rw-rw-rw-   0        0        0      112 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/requirements/fedora.txt
--rw-rw-rw-   0        0        0       11 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/requirements/linux.txt
--rw-rw-rw-   0        0        0       26 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/requirements/ubuntu.txt
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.495556 neofbs-1.2.4/fbs/_defaults/src/
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.492556 neofbs-1.2.4/fbs/_defaults/src/build/
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.492556 neofbs-1.2.4/fbs/_defaults/src/build/docker/
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.519556 neofbs-1.2.4/fbs/_defaults/src/build/docker/arch/
--rw-rw-rw-   0        0        0      176 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/build/docker/arch/.bashrc
--rw-rw-rw-   0        0        0     1696 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/build/docker/arch/Dockerfile
--rw-rw-rw-   0        0        0      104 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/build/docker/arch/gpg-agent.conf
--rw-rw-rw-   0        0        0      396 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/build/docker/arch/motd
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.523556 neofbs-1.2.4/fbs/_defaults/src/build/docker/fedora/
--rw-rw-rw-   0        0        0       98 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/build/docker/fedora/.bashrc
--rw-rw-rw-   0        0        0       87 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/build/docker/fedora/.rpmmacros
--rw-rw-rw-   0        0        0     1904 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/build/docker/fedora/Dockerfile
--rw-rw-rw-   0        0        0      104 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/build/docker/fedora/gpg-agent.conf
--rw-rw-rw-   0        0        0      400 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/build/docker/fedora/motd
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.526556 neofbs-1.2.4/fbs/_defaults/src/build/docker/ubuntu/
--rw-rw-rw-   0        0        0       98 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/build/docker/ubuntu/.bashrc
--rw-rw-rw-   0        0        0     1805 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/build/docker/ubuntu/Dockerfile
--rw-rw-rw-   0        0        0      104 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/build/docker/ubuntu/gpg-agent.conf
--rw-rw-rw-   0        0        0      367 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/build/docker/ubuntu/gpg.conf
--rw-rw-rw-   0        0        0      400 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/build/docker/ubuntu/motd
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.532556 neofbs-1.2.4/fbs/_defaults/src/build/settings/
--rw-rw-rw-   0        0        0      199 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/build/settings/arch.json
--rw-rw-rw-   0        0        0     1246 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/build/settings/base.json
--rw-rw-rw-   0        0        0      285 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/build/settings/fedora.json
--rw-rw-rw-   0        0        0      301 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/build/settings/linux.json
--rw-rw-rw-   0        0        0      234 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/build/settings/mac.json
--rw-rw-rw-   0        0        0       59 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/build/settings/release.json
--rw-rw-rw-   0        0        0      138 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/build/settings/ubuntu.json
--rw-rw-rw-   0        0        0      224 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/build/settings/windows.json
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.493556 neofbs-1.2.4/fbs/_defaults/src/freeze/
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.493556 neofbs-1.2.4/fbs/_defaults/src/freeze/mac/
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.533556 neofbs-1.2.4/fbs/_defaults/src/freeze/mac/Contents/
--rw-rw-rw-   0        0        0      997 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/freeze/mac/Contents/Info.plist
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.533556 neofbs-1.2.4/fbs/_defaults/src/freeze/windows/
--rw-rw-rw-   0        0        0     1834 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/freeze/windows/version_info.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.495556 neofbs-1.2.4/fbs/_defaults/src/installer/
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.494557 neofbs-1.2.4/fbs/_defaults/src/installer/linux/
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.494557 neofbs-1.2.4/fbs/_defaults/src/installer/linux/usr/
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.494557 neofbs-1.2.4/fbs/_defaults/src/installer/linux/usr/share/
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.534556 neofbs-1.2.4/fbs/_defaults/src/installer/linux/usr/share/applications/
--rw-rw-rw-   0        0        0      176 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/installer/linux/usr/share/applications/AppName.desktop
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.535556 neofbs-1.2.4/fbs/_defaults/src/installer/windows/
--rw-rw-rw-   0        0        0     3510 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/installer/windows/Installer.nsi
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.495556 neofbs-1.2.4/fbs/_defaults/src/repo/
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.536556 neofbs-1.2.4/fbs/_defaults/src/repo/fedora/
--rw-rw-rw-   0        0        0       97 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/repo/fedora/AppName.repo
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.536556 neofbs-1.2.4/fbs/_defaults/src/repo/ubuntu/
--rw-rw-rw-   0        0        0      150 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_defaults/src/repo/ubuntu/distributions
--rw-rw-rw-   0        0        0     2129 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_gpg.py
--rw-rw-rw-   0        0        0      782 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_server.py
--rw-rw-rw-   0        0        0      598 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/_state.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.540557 neofbs-1.2.4/fbs/builtin_commands/
--rw-rw-rw-   0        0        0    19939 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/__init__.py
--rw-rw-rw-   0        0        0     1310 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/_account.py
--rw-rw-rw-   0        0        0     3675 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/_docker.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.543557 neofbs-1.2.4/fbs/builtin_commands/_gpg/
--rw-rw-rw-   0        0        0      296 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/_gpg/Dockerfile
--rw-rw-rw-   0        0        0     2968 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/_gpg/__init__.py
--rw-rw-rw-   0        0        0      449 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/_gpg/genkey.sh
--rw-rw-rw-   0        0        0      145 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/_gpg/gpg-agent.conf
--rw-rw-rw-   0        0        0     2256 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/_licensing.py
--rw-rw-rw-   0        0        0     2768 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/_util.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.496556 neofbs-1.2.4/fbs/builtin_commands/project_template/
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.497556 neofbs-1.2.4/fbs/builtin_commands/project_template/src/
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.497556 neofbs-1.2.4/fbs/builtin_commands/project_template/src/build/
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.545556 neofbs-1.2.4/fbs/builtin_commands/project_template/src/build/settings/
--rw-rw-rw-   0        0        0      135 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/project_template/src/build/settings/base.json
--rw-rw-rw-   0        0        0       99 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/project_template/src/build/settings/linux.json
--rw-rw-rw-   0        0        0       61 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/project_template/src/build/settings/mac.json
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.498560 neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.547556 neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/
--rw-rw-rw-   0        0        0   168229 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/Icon.ico
--rw-rw-rw-   0        0        0      570 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.551556 neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/base/
--rw-rw-rw-   0        0        0      544 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/base/16.png
--rw-rw-rw-   0        0        0      783 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/base/24.png
--rw-rw-rw-   0        0        0      912 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/base/32.png
--rw-rw-rw-   0        0        0     1497 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/base/48.png
--rw-rw-rw-   0        0        0     1657 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/base/64.png
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.554558 neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/linux/
--rw-rw-rw-   0        0        0    26841 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/linux/1024.png
--rw-rw-rw-   0        0        0     3177 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/linux/128.png
--rw-rw-rw-   0        0        0     5641 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/linux/256.png
--rw-rw-rw-   0        0        0    11653 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/linux/512.png
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.557556 neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/mac/
--rw-rw-rw-   0        0        0    47311 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/mac/1024.png
--rw-rw-rw-   0        0        0     4978 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/mac/128.png
--rw-rw-rw-   0        0        0    10278 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/mac/256.png
--rw-rw-rw-   0        0        0    21699 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/mac/512.png
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.558556 neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/python/
--rw-rw-rw-   0        0        0      432 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/python/main.py
--rw-rw-rw-   0        0        0     3234 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/cmdline.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.563305 neofbs-1.2.4/fbs/freeze/
--rw-rw-rw-   0        0        0     3460 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/freeze/__init__.py
--rw-rw-rw-   0        0        0       99 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/freeze/arch.py
--rw-rw-rw-   0        0        0      761 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/freeze/fedora.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.566316 neofbs-1.2.4/fbs/freeze/hooks/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/freeze/hooks/__init__.py
--rw-rw-rw-   0        0        0     1282 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/freeze/hooks/hook-PySide2.py
--rw-rw-rw-   0        0        0     1123 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/freeze/hooks/hook-shiboken2.py
--rw-rw-rw-   0        0        0     1019 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/freeze/linux.py
--rw-rw-rw-   0        0        0     2340 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/freeze/mac.py
--rw-rw-rw-   0        0        0     1483 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/freeze/ubuntu.py
--rw-rw-rw-   0        0        0     4010 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/freeze/windows.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.570315 neofbs-1.2.4/fbs/installer/
--rw-rw-rw-   0        0        0      319 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/installer/__init__.py
--rw-rw-rw-   0        0        0      349 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/installer/arch.py
--rw-rw-rw-   0        0        0      151 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/installer/fedora.py
--rw-rw-rw-   0        0        0     3276 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/installer/linux.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.571315 neofbs-1.2.4/fbs/installer/mac/
--rw-rw-rw-   0        0        0     1156 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/installer/mac/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.573748 neofbs-1.2.4/fbs/installer/mac/create-dmg/
--rw-rw-rw-   0        0        0     1109 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/installer/mac/create-dmg/LICENSE
--rw-rw-rw-   0        0        0     3583 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/installer/mac/create-dmg/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.574761 neofbs-1.2.4/fbs/installer/mac/create-dmg/builder/
--rw-rw-rw-   0        0        0      542 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/installer/mac/create-dmg/builder/create-dmg.builder
--rw-rw-rw-   0        0        0    12081 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/installer/mac/create-dmg/create-dmg
--rw-rw-rw-   0        0        0      523 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/installer/mac/create-dmg/sample
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.576760 neofbs-1.2.4/fbs/installer/mac/create-dmg/support/
--rw-rw-rw-   0        0        0      718 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/installer/mac/create-dmg/support/brew-me.sh
--rw-rw-rw-   0        0        0     6442 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/installer/mac/create-dmg/support/dmg-license.py
--rw-rw-rw-   0        0        0     1902 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/installer/mac/create-dmg/support/template.applescript
--rw-rw-rw-   0        0        0      151 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/installer/ubuntu.py
--rw-rw-rw-   0        0        0      586 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/installer/windows.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.579763 neofbs-1.2.4/fbs/repo/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/repo/__init__.py
--rw-rw-rw-   0        0        0     1099 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/repo/arch.py
--rw-rw-rw-   0        0        0      987 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/repo/fedora.py
--rw-rw-rw-   0        0        0      941 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/repo/ubuntu.py
--rw-rw-rw-   0        0        0     4640 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/resources.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.580764 neofbs-1.2.4/fbs/sign/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/sign/__init__.py
--rw-rw-rw-   0        0        0     4029 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/sign/windows.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.583760 neofbs-1.2.4/fbs/sign_installer/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/sign_installer/__init__.py
--rw-rw-rw-   0        0        0      473 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/sign_installer/arch.py
--rw-rw-rw-   0        0        0      338 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/sign_installer/fedora.py
--rw-rw-rw-   0        0        0      224 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/sign_installer/windows.py
--rw-rw-rw-   0        0        0     1705 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs/upload.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.590873 neofbs-1.2.4/fbs_runtime/
--rw-rw-rw-   0        0        0       36 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs_runtime/__init__.py
--rw-rw-rw-   0        0        0      960 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs_runtime/_fbs.py
--rw-rw-rw-   0        0        0      556 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs_runtime/_frozen.py
--rw-rw-rw-   0        0        0      515 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs_runtime/_resources.py
--rw-rw-rw-   0        0        0     1918 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs_runtime/_settings.py
--rw-rw-rw-   0        0        0     2690 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs_runtime/_signal.py
--rw-rw-rw-   0        0        0     1979 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs_runtime/_source.py
--rw-rw-rw-   0        0        0      657 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs_runtime/_state.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.592873 neofbs-1.2.4/fbs_runtime/application_context/
--rw-rw-rw-   0        0        0     1256 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs_runtime/application_context/PyQt5.py
--rw-rw-rw-   0        0        0     1262 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs_runtime/application_context/PySide2.py
--rw-rw-rw-   0        0        0     5938 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs_runtime/application_context/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.594872 neofbs-1.2.4/fbs_runtime/excepthook/
--rw-rw-rw-   0        0        0     5373 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs_runtime/excepthook/__init__.py
--rw-rw-rw-   0        0        0      613 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs_runtime/excepthook/_util.py
--rw-rw-rw-   0        0        0      458 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs_runtime/excepthook/sentry.py
--rw-rw-rw-   0        0        0     3211 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs_runtime/licensing.py
--rw-rw-rw-   0        0        0     2552 2024-05-24 14:55:11.000000 neofbs-1.2.4/fbs_runtime/platform.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:11:23.601873 neofbs-1.2.4/neofbs.egg-info/
--rw-rw-rw-   0        0        0     1341 2024-05-24 15:11:23.000000 neofbs-1.2.4/neofbs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4900 2024-05-24 15:11:23.000000 neofbs-1.2.4/neofbs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 15:11:23.000000 neofbs-1.2.4/neofbs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-05-24 15:11:23.000000 neofbs-1.2.4/neofbs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       88 2024-05-24 15:11:23.000000 neofbs-1.2.4/neofbs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-24 15:11:23.000000 neofbs-1.2.4/neofbs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-24 15:11:23.607872 neofbs-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0     3058 2024-05-24 15:10:53.000000 neofbs-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.939981 neofbs-1.2.5/
+-rw-rw-rw-   0        0        0    35821 2024-05-24 14:55:11.000000 neofbs-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0    12994 2024-05-24 14:55:11.000000 neofbs-1.2.5/NOTICE
+-rw-rw-rw-   0        0        0     1908 2024-05-24 15:12:44.939981 neofbs-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       94 2024-05-24 14:55:11.000000 neofbs-1.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.841710 neofbs-1.2.5/fbs/
+-rw-rw-rw-   0        0        0     2452 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/__init__.py
+-rw-rw-rw-   0        0        0     1755 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/__main__.py
+-rw-rw-rw-   0        0        0     1080 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_aws.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.819662 neofbs-1.2.5/fbs/_defaults/
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.845711 neofbs-1.2.5/fbs/_defaults/requirements/
+-rw-rw-rw-   0        0        0      138 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/requirements/arch.txt
+-rw-rw-rw-   0        0        0       10 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/requirements/base.txt
+-rw-rw-rw-   0        0        0      112 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/requirements/fedora.txt
+-rw-rw-rw-   0        0        0       11 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/requirements/linux.txt
+-rw-rw-rw-   0        0        0       26 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/requirements/ubuntu.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.823691 neofbs-1.2.5/fbs/_defaults/src/
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.821660 neofbs-1.2.5/fbs/_defaults/src/build/
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.820660 neofbs-1.2.5/fbs/_defaults/src/build/docker/
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.849709 neofbs-1.2.5/fbs/_defaults/src/build/docker/arch/
+-rw-rw-rw-   0        0        0      176 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/build/docker/arch/.bashrc
+-rw-rw-rw-   0        0        0     1696 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/build/docker/arch/Dockerfile
+-rw-rw-rw-   0        0        0      104 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/build/docker/arch/gpg-agent.conf
+-rw-rw-rw-   0        0        0      396 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/build/docker/arch/motd
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.853648 neofbs-1.2.5/fbs/_defaults/src/build/docker/fedora/
+-rw-rw-rw-   0        0        0       98 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/build/docker/fedora/.bashrc
+-rw-rw-rw-   0        0        0       87 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/build/docker/fedora/.rpmmacros
+-rw-rw-rw-   0        0        0     1904 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/build/docker/fedora/Dockerfile
+-rw-rw-rw-   0        0        0      104 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/build/docker/fedora/gpg-agent.conf
+-rw-rw-rw-   0        0        0      400 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/build/docker/fedora/motd
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.858659 neofbs-1.2.5/fbs/_defaults/src/build/docker/ubuntu/
+-rw-rw-rw-   0        0        0       98 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/build/docker/ubuntu/.bashrc
+-rw-rw-rw-   0        0        0     1805 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/build/docker/ubuntu/Dockerfile
+-rw-rw-rw-   0        0        0      104 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/build/docker/ubuntu/gpg-agent.conf
+-rw-rw-rw-   0        0        0      367 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/build/docker/ubuntu/gpg.conf
+-rw-rw-rw-   0        0        0      400 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/build/docker/ubuntu/motd
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.864659 neofbs-1.2.5/fbs/_defaults/src/build/settings/
+-rw-rw-rw-   0        0        0      199 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/build/settings/arch.json
+-rw-rw-rw-   0        0        0     1246 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/build/settings/base.json
+-rw-rw-rw-   0        0        0      285 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/build/settings/fedora.json
+-rw-rw-rw-   0        0        0      301 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/build/settings/linux.json
+-rw-rw-rw-   0        0        0      234 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/build/settings/mac.json
+-rw-rw-rw-   0        0        0       59 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/build/settings/release.json
+-rw-rw-rw-   0        0        0      138 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/build/settings/ubuntu.json
+-rw-rw-rw-   0        0        0      224 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/build/settings/windows.json
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.822661 neofbs-1.2.5/fbs/_defaults/src/freeze/
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.821660 neofbs-1.2.5/fbs/_defaults/src/freeze/mac/
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.864659 neofbs-1.2.5/fbs/_defaults/src/freeze/mac/Contents/
+-rw-rw-rw-   0        0        0      997 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/freeze/mac/Contents/Info.plist
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.865659 neofbs-1.2.5/fbs/_defaults/src/freeze/windows/
+-rw-rw-rw-   0        0        0     1834 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/freeze/windows/version_info.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.823691 neofbs-1.2.5/fbs/_defaults/src/installer/
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.822661 neofbs-1.2.5/fbs/_defaults/src/installer/linux/
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.823691 neofbs-1.2.5/fbs/_defaults/src/installer/linux/usr/
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.823691 neofbs-1.2.5/fbs/_defaults/src/installer/linux/usr/share/
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.866659 neofbs-1.2.5/fbs/_defaults/src/installer/linux/usr/share/applications/
+-rw-rw-rw-   0        0        0      176 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/installer/linux/usr/share/applications/AppName.desktop
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.866659 neofbs-1.2.5/fbs/_defaults/src/installer/windows/
+-rw-rw-rw-   0        0        0     3510 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/installer/windows/Installer.nsi
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.824690 neofbs-1.2.5/fbs/_defaults/src/repo/
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.867658 neofbs-1.2.5/fbs/_defaults/src/repo/fedora/
+-rw-rw-rw-   0        0        0       97 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/repo/fedora/AppName.repo
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.868659 neofbs-1.2.5/fbs/_defaults/src/repo/ubuntu/
+-rw-rw-rw-   0        0        0      150 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_defaults/src/repo/ubuntu/distributions
+-rw-rw-rw-   0        0        0     2129 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_gpg.py
+-rw-rw-rw-   0        0        0      782 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_server.py
+-rw-rw-rw-   0        0        0      598 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/_state.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.872658 neofbs-1.2.5/fbs/builtin_commands/
+-rw-rw-rw-   0        0        0    19939 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/__init__.py
+-rw-rw-rw-   0        0        0     1310 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/_account.py
+-rw-rw-rw-   0        0        0     3675 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/_docker.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.875659 neofbs-1.2.5/fbs/builtin_commands/_gpg/
+-rw-rw-rw-   0        0        0      296 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/_gpg/Dockerfile
+-rw-rw-rw-   0        0        0     2968 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/_gpg/__init__.py
+-rw-rw-rw-   0        0        0      449 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/_gpg/genkey.sh
+-rw-rw-rw-   0        0        0      145 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/_gpg/gpg-agent.conf
+-rw-rw-rw-   0        0        0     2256 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/_licensing.py
+-rw-rw-rw-   0        0        0     2768 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/_util.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.825691 neofbs-1.2.5/fbs/builtin_commands/project_template/
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.826691 neofbs-1.2.5/fbs/builtin_commands/project_template/src/
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.825691 neofbs-1.2.5/fbs/builtin_commands/project_template/src/build/
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.877658 neofbs-1.2.5/fbs/builtin_commands/project_template/src/build/settings/
+-rw-rw-rw-   0        0        0      135 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/project_template/src/build/settings/base.json
+-rw-rw-rw-   0        0        0       99 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/project_template/src/build/settings/linux.json
+-rw-rw-rw-   0        0        0       61 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/project_template/src/build/settings/mac.json
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.827691 neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.879658 neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/
+-rw-rw-rw-   0        0        0   168229 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/Icon.ico
+-rw-rw-rw-   0        0        0      570 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.883659 neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/base/
+-rw-rw-rw-   0        0        0      544 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/base/16.png
+-rw-rw-rw-   0        0        0      783 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/base/24.png
+-rw-rw-rw-   0        0        0      912 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/base/32.png
+-rw-rw-rw-   0        0        0     1497 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/base/48.png
+-rw-rw-rw-   0        0        0     1657 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/base/64.png
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.886658 neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/linux/
+-rw-rw-rw-   0        0        0    26841 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/linux/1024.png
+-rw-rw-rw-   0        0        0     3177 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/linux/128.png
+-rw-rw-rw-   0        0        0     5641 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/linux/256.png
+-rw-rw-rw-   0        0        0    11653 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/linux/512.png
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.889659 neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/mac/
+-rw-rw-rw-   0        0        0    47311 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/mac/1024.png
+-rw-rw-rw-   0        0        0     4978 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/mac/128.png
+-rw-rw-rw-   0        0        0    10278 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/mac/256.png
+-rw-rw-rw-   0        0        0    21699 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/mac/512.png
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.890658 neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/python/
+-rw-rw-rw-   0        0        0      432 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/python/main.py
+-rw-rw-rw-   0        0        0     3234 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/cmdline.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.895824 neofbs-1.2.5/fbs/freeze/
+-rw-rw-rw-   0        0        0     3460 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/freeze/__init__.py
+-rw-rw-rw-   0        0        0       99 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/freeze/arch.py
+-rw-rw-rw-   0        0        0      761 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/freeze/fedora.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.897835 neofbs-1.2.5/fbs/freeze/hooks/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/freeze/hooks/__init__.py
+-rw-rw-rw-   0        0        0     1282 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/freeze/hooks/hook-PySide2.py
+-rw-rw-rw-   0        0        0     1123 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/freeze/hooks/hook-shiboken2.py
+-rw-rw-rw-   0        0        0     1019 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/freeze/linux.py
+-rw-rw-rw-   0        0        0     2340 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/freeze/mac.py
+-rw-rw-rw-   0        0        0     1483 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/freeze/ubuntu.py
+-rw-rw-rw-   0        0        0     4010 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/freeze/windows.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.902835 neofbs-1.2.5/fbs/installer/
+-rw-rw-rw-   0        0        0      319 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/installer/__init__.py
+-rw-rw-rw-   0        0        0      349 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/installer/arch.py
+-rw-rw-rw-   0        0        0      151 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/installer/fedora.py
+-rw-rw-rw-   0        0        0     3276 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/installer/linux.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.902835 neofbs-1.2.5/fbs/installer/mac/
+-rw-rw-rw-   0        0        0     1156 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/installer/mac/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.906835 neofbs-1.2.5/fbs/installer/mac/create-dmg/
+-rw-rw-rw-   0        0        0     1109 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/installer/mac/create-dmg/LICENSE
+-rw-rw-rw-   0        0        0     3583 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/installer/mac/create-dmg/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.906835 neofbs-1.2.5/fbs/installer/mac/create-dmg/builder/
+-rw-rw-rw-   0        0        0      542 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/installer/mac/create-dmg/builder/create-dmg.builder
+-rw-rw-rw-   0        0        0    12081 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/installer/mac/create-dmg/create-dmg
+-rw-rw-rw-   0        0        0      523 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/installer/mac/create-dmg/sample
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.908840 neofbs-1.2.5/fbs/installer/mac/create-dmg/support/
+-rw-rw-rw-   0        0        0      718 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/installer/mac/create-dmg/support/brew-me.sh
+-rw-rw-rw-   0        0        0     6442 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/installer/mac/create-dmg/support/dmg-license.py
+-rw-rw-rw-   0        0        0     1902 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/installer/mac/create-dmg/support/template.applescript
+-rw-rw-rw-   0        0        0      151 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/installer/ubuntu.py
+-rw-rw-rw-   0        0        0      586 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/installer/windows.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.911841 neofbs-1.2.5/fbs/repo/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/repo/__init__.py
+-rw-rw-rw-   0        0        0     1099 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/repo/arch.py
+-rw-rw-rw-   0        0        0      987 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/repo/fedora.py
+-rw-rw-rw-   0        0        0      941 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/repo/ubuntu.py
+-rw-rw-rw-   0        0        0     4640 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/resources.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.912841 neofbs-1.2.5/fbs/sign/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/sign/__init__.py
+-rw-rw-rw-   0        0        0     4029 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/sign/windows.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.915840 neofbs-1.2.5/fbs/sign_installer/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/sign_installer/__init__.py
+-rw-rw-rw-   0        0        0      473 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/sign_installer/arch.py
+-rw-rw-rw-   0        0        0      338 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/sign_installer/fedora.py
+-rw-rw-rw-   0        0        0      224 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/sign_installer/windows.py
+-rw-rw-rw-   0        0        0     1705 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs/upload.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.922849 neofbs-1.2.5/fbs_runtime/
+-rw-rw-rw-   0        0        0       36 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs_runtime/__init__.py
+-rw-rw-rw-   0        0        0      960 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs_runtime/_fbs.py
+-rw-rw-rw-   0        0        0      556 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs_runtime/_frozen.py
+-rw-rw-rw-   0        0        0      515 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs_runtime/_resources.py
+-rw-rw-rw-   0        0        0     1918 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs_runtime/_settings.py
+-rw-rw-rw-   0        0        0     2690 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs_runtime/_signal.py
+-rw-rw-rw-   0        0        0     1979 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs_runtime/_source.py
+-rw-rw-rw-   0        0        0      657 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs_runtime/_state.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.924982 neofbs-1.2.5/fbs_runtime/application_context/
+-rw-rw-rw-   0        0        0     1256 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs_runtime/application_context/PyQt5.py
+-rw-rw-rw-   0        0        0     1262 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs_runtime/application_context/PySide2.py
+-rw-rw-rw-   0        0        0     5938 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs_runtime/application_context/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.926982 neofbs-1.2.5/fbs_runtime/excepthook/
+-rw-rw-rw-   0        0        0     5373 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs_runtime/excepthook/__init__.py
+-rw-rw-rw-   0        0        0      613 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs_runtime/excepthook/_util.py
+-rw-rw-rw-   0        0        0      458 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs_runtime/excepthook/sentry.py
+-rw-rw-rw-   0        0        0     3211 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs_runtime/licensing.py
+-rw-rw-rw-   0        0        0     2552 2024-05-24 14:55:11.000000 neofbs-1.2.5/fbs_runtime/platform.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:12:44.938981 neofbs-1.2.5/neofbs.egg-info/
+-rw-rw-rw-   0        0        0     1908 2024-05-24 15:12:44.000000 neofbs-1.2.5/neofbs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4900 2024-05-24 15:12:44.000000 neofbs-1.2.5/neofbs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 15:12:44.000000 neofbs-1.2.5/neofbs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-24 15:12:44.000000 neofbs-1.2.5/neofbs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       88 2024-05-24 15:12:44.000000 neofbs-1.2.5/neofbs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-24 15:12:44.000000 neofbs-1.2.5/neofbs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-24 15:12:44.943981 neofbs-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     2853 2024-05-24 15:12:41.000000 neofbs-1.2.5/setup.py
```

### Comparing `neofbs-1.2.4/LICENSE` & `neofbs-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/NOTICE` & `neofbs-1.2.5/NOTICE`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/__init__.py` & `neofbs-1.2.5/fbs/__init__.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/__main__.py` & `neofbs-1.2.5/fbs/__main__.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/_aws.py` & `neofbs-1.2.5/fbs/_aws.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/_defaults/src/build/docker/arch/Dockerfile` & `neofbs-1.2.5/fbs/_defaults/src/build/docker/arch/Dockerfile`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/_defaults/src/build/docker/fedora/Dockerfile` & `neofbs-1.2.5/fbs/_defaults/src/build/docker/fedora/Dockerfile`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/_defaults/src/build/docker/ubuntu/Dockerfile` & `neofbs-1.2.5/fbs/_defaults/src/build/docker/ubuntu/Dockerfile`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/_defaults/src/build/settings/base.json` & `neofbs-1.2.5/fbs/_defaults/src/build/settings/base.json`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/_defaults/src/freeze/mac/Contents/Info.plist` & `neofbs-1.2.5/fbs/_defaults/src/freeze/mac/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/_defaults/src/freeze/windows/version_info.py` & `neofbs-1.2.5/fbs/_defaults/src/freeze/windows/version_info.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/_defaults/src/installer/windows/Installer.nsi` & `neofbs-1.2.5/fbs/_defaults/src/installer/windows/Installer.nsi`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/_gpg.py` & `neofbs-1.2.5/fbs/_gpg.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/_server.py` & `neofbs-1.2.5/fbs/_server.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/_state.py` & `neofbs-1.2.5/fbs/_state.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/builtin_commands/__init__.py` & `neofbs-1.2.5/fbs/builtin_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/builtin_commands/_account.py` & `neofbs-1.2.5/fbs/builtin_commands/_account.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/builtin_commands/_docker.py` & `neofbs-1.2.5/fbs/builtin_commands/_docker.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/builtin_commands/_gpg/__init__.py` & `neofbs-1.2.5/fbs/builtin_commands/_gpg/__init__.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/builtin_commands/_licensing.py` & `neofbs-1.2.5/fbs/builtin_commands/_licensing.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/builtin_commands/_util.py` & `neofbs-1.2.5/fbs/builtin_commands/_util.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/Icon.ico` & `neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/Icon.ico`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/README.md` & `neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/README.md`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/base/16.png` & `neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/base/16.png`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/base/24.png` & `neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/base/24.png`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/base/32.png` & `neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/base/32.png`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/base/48.png` & `neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/base/48.png`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/base/64.png` & `neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/base/64.png`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/linux/1024.png` & `neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/linux/1024.png`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/linux/128.png` & `neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/linux/128.png`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/linux/256.png` & `neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/linux/256.png`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/linux/512.png` & `neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/linux/512.png`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/mac/1024.png` & `neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/mac/1024.png`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/mac/128.png` & `neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/mac/128.png`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/mac/256.png` & `neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/mac/256.png`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/builtin_commands/project_template/src/main/icons/mac/512.png` & `neofbs-1.2.5/fbs/builtin_commands/project_template/src/main/icons/mac/512.png`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/cmdline.py` & `neofbs-1.2.5/fbs/cmdline.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/freeze/__init__.py` & `neofbs-1.2.5/fbs/freeze/__init__.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/freeze/fedora.py` & `neofbs-1.2.5/fbs/freeze/fedora.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/freeze/hooks/hook-PySide2.py` & `neofbs-1.2.5/fbs/freeze/hooks/hook-PySide2.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/freeze/hooks/hook-shiboken2.py` & `neofbs-1.2.5/fbs/freeze/hooks/hook-shiboken2.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/freeze/linux.py` & `neofbs-1.2.5/fbs/freeze/linux.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/freeze/mac.py` & `neofbs-1.2.5/fbs/freeze/mac.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/freeze/ubuntu.py` & `neofbs-1.2.5/fbs/freeze/ubuntu.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/freeze/windows.py` & `neofbs-1.2.5/fbs/freeze/windows.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/installer/linux.py` & `neofbs-1.2.5/fbs/installer/linux.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/installer/mac/__init__.py` & `neofbs-1.2.5/fbs/installer/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/installer/mac/create-dmg/LICENSE` & `neofbs-1.2.5/fbs/installer/mac/create-dmg/LICENSE`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/installer/mac/create-dmg/README.md` & `neofbs-1.2.5/fbs/installer/mac/create-dmg/README.md`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/installer/mac/create-dmg/builder/create-dmg.builder` & `neofbs-1.2.5/fbs/installer/mac/create-dmg/builder/create-dmg.builder`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/installer/mac/create-dmg/create-dmg` & `neofbs-1.2.5/fbs/installer/mac/create-dmg/create-dmg`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/installer/mac/create-dmg/sample` & `neofbs-1.2.5/fbs/installer/mac/create-dmg/sample`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/installer/mac/create-dmg/support/brew-me.sh` & `neofbs-1.2.5/fbs/installer/mac/create-dmg/support/brew-me.sh`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/installer/mac/create-dmg/support/dmg-license.py` & `neofbs-1.2.5/fbs/installer/mac/create-dmg/support/dmg-license.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/installer/mac/create-dmg/support/template.applescript` & `neofbs-1.2.5/fbs/installer/mac/create-dmg/support/template.applescript`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/installer/windows.py` & `neofbs-1.2.5/fbs/installer/windows.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/repo/arch.py` & `neofbs-1.2.5/fbs/repo/arch.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/repo/fedora.py` & `neofbs-1.2.5/fbs/repo/fedora.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/repo/ubuntu.py` & `neofbs-1.2.5/fbs/repo/ubuntu.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/resources.py` & `neofbs-1.2.5/fbs/resources.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/sign/windows.py` & `neofbs-1.2.5/fbs/sign/windows.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs/upload.py` & `neofbs-1.2.5/fbs/upload.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs_runtime/_fbs.py` & `neofbs-1.2.5/fbs_runtime/_fbs.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs_runtime/_frozen.py` & `neofbs-1.2.5/fbs_runtime/_frozen.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs_runtime/_resources.py` & `neofbs-1.2.5/fbs_runtime/_resources.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs_runtime/_settings.py` & `neofbs-1.2.5/fbs_runtime/_settings.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs_runtime/_signal.py` & `neofbs-1.2.5/fbs_runtime/_signal.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs_runtime/_source.py` & `neofbs-1.2.5/fbs_runtime/_source.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs_runtime/_state.py` & `neofbs-1.2.5/fbs_runtime/_state.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs_runtime/application_context/PyQt5.py` & `neofbs-1.2.5/fbs_runtime/application_context/PyQt5.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs_runtime/application_context/PySide2.py` & `neofbs-1.2.5/fbs_runtime/application_context/PySide2.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs_runtime/application_context/__init__.py` & `neofbs-1.2.5/fbs_runtime/application_context/__init__.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs_runtime/excepthook/__init__.py` & `neofbs-1.2.5/fbs_runtime/excepthook/__init__.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs_runtime/excepthook/_util.py` & `neofbs-1.2.5/fbs_runtime/excepthook/_util.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs_runtime/licensing.py` & `neofbs-1.2.5/fbs_runtime/licensing.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/fbs_runtime/platform.py` & `neofbs-1.2.5/fbs_runtime/platform.py`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/neofbs.egg-info/SOURCES.txt` & `neofbs-1.2.5/neofbs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neofbs-1.2.4/setup.py` & `neofbs-1.2.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Create cross-platform desktop applications with Python and Qt with support for the most recent Python versions.
-
+long_de = """
 Neofbs is a fork of fbs. The original project is locked to Python 3.5 and 3.6, which are not supported anymore. To have the more recent versions, you have to pay €50.
 Obviously, the paid versions have a lot more features, but atleast with neofbs you can start a project, package it into a .exe and then package it into an installer.
 
 To download it, simply use pip:
 
 ```
 pip install neofbs
@@ -20,66 +18,59 @@
 """
 
 from os.path import relpath, join
 from setuptools import setup, find_packages
 
 import os
 
+
 def _get_package_data(pkg_dir, data_subdir):
     result = []
     for dirpath, _, filenames in os.walk(join(pkg_dir, data_subdir)):
         for filename in filenames:
             filepath = join(dirpath, filename)
             result.append(relpath(filepath, pkg_dir))
     return result
 
-description = 'Create cross-platform desktop applications with Python and Qt with support for the most recent Python versions'
+
+description = "Create cross-platform desktop applications with Python and Qt with support for the most recent Python versions"
 setup(
-    name='neofbs',
+    name="neofbs",
     # Also update fbs/_defaults/requirements/base.txt when you change this:
-    version='1.2.4',
+    version="1.2.5",
     description=description,
-    long_description=
-        description + '\n\nHome page: https://build-system.fman.io',
-    author='Andre Albano',
-    author_email='geof.aalbano@gmail.com',
-    url='https://albano-dev.netlify.app',
-    packages=find_packages(exclude=('tests', 'tests.*')),
+    long_description=description + long_de,
+    author="Andre Albano",
+    author_email="geof.aalbano@gmail.com",
+    url="https://albano-dev.netlify.app",
+    packages=find_packages(exclude=("tests", "tests.*")),
     package_data={
-        'fbs': _get_package_data('fbs', '_defaults'),
-        'fbs.builtin_commands':
-            _get_package_data('fbs/builtin_commands', 'project_template'),
-        'fbs.builtin_commands._gpg':
-            ['Dockerfile', 'genkey.sh', 'gpg-agent.conf'],
-        'fbs.installer.mac': _get_package_data(
-            'fbs/installer/mac', 'create-dmg'
-        )
+        "fbs": _get_package_data("fbs", "_defaults"),
+        "fbs.builtin_commands": _get_package_data(
+            "fbs/builtin_commands", "project_template"
+        ),
+        "fbs.builtin_commands._gpg": ["Dockerfile", "genkey.sh", "gpg-agent.conf"],
+        "fbs.installer.mac": _get_package_data("fbs/installer/mac", "create-dmg"),
     },
-    install_requires=['PyInstaller==5.13.2'],
+    install_requires=["PyInstaller==5.13.2"],
     extras_require={
         # Also update requirements.txt when you change this:
-        'licensing': ['rsa>=3.4.2'],
-        'sentry': ['sentry-sdk>=0.6.6'],
-        'upload': ['boto3']
+        "licensing": ["rsa>=3.4.2"],
+        "sentry": ["sentry-sdk>=0.6.6"],
+        "upload": ["boto3"],
     },
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-    
-        'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
-    
-        'Operating System :: OS Independent',
-    
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules'
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: Software Development :: Libraries :: Python Modules",
     ],
-    entry_points={
-        'console_scripts': ['fbs=fbs.__main__:_main']
-    },
-    license='GPLv3 or later',
-    keywords='PyQt',
-    platforms=['MacOS', 'Windows', 'Debian', 'Fedora', 'CentOS', 'Arch'],
-    test_suite='tests'
-)
+    entry_points={"console_scripts": ["fbs=fbs.__main__:_main"]},
+    license="GPLv3 or later",
+    keywords="PyQt",
+    platforms=["MacOS", "Windows", "Debian", "Fedora", "CentOS", "Arch"],
+    test_suite="tests",
+)
```

