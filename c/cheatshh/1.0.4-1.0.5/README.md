# Comparing `tmp/cheatshh-1.0.4.tar.gz` & `tmp/cheatshh-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheatshh-1.0.4.tar", last modified: Sat May 18 11:30:33 2024, max compression
+gzip compressed data, was "cheatshh-1.0.5.tar", last modified: Fri May 24 18:31:19 2024, max compression
```

## Comparing `cheatshh-1.0.4.tar` & `cheatshh-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-18 11:30:33.981696 cheatshh-1.0.4/
--rw-r--r--   0 root         (0) staff       (20)    11357 2024-05-09 07:38:12.000000 cheatshh-1.0.4/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     1411 2024-05-18 11:30:33.981427 cheatshh-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     4844 2024-05-18 11:22:35.000000 cheatshh-1.0.4/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-18 11:30:33.980885 cheatshh-1.0.4/cheatshh.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     1411 2024-05-18 11:30:33.000000 cheatshh-1.0.4/cheatshh.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      256 2024-05-18 11:30:33.000000 cheatshh-1.0.4/cheatshh.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-05-18 11:30:33.000000 cheatshh-1.0.4/cheatshh.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       51 2024-05-18 11:30:33.000000 cheatshh-1.0.4/cheatshh.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)       21 2024-05-18 11:30:33.000000 cheatshh-1.0.4/cheatshh.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        4 2024-05-18 11:30:33.000000 cheatshh-1.0.4/cheatshh.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2024-05-18 11:30:33.981742 cheatshh-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     3250 2024-05-18 11:27:52.000000 cheatshh-1.0.4/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-18 11:30:33.981102 cheatshh-1.0.4/src/
--rw-r--r--   0 root         (0) staff       (20)        0 2024-05-09 09:59:20.000000 cheatshh-1.0.4/src/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      222 2024-05-18 10:34:26.000000 cheatshh-1.0.4/src/run_cheatshh.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-24 18:31:19.674085 cheatshh-1.0.5/
+-rw-r--r--   0 root         (0) staff       (20)    11357 2024-05-09 07:38:12.000000 cheatshh-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     1552 2024-05-24 18:31:19.673874 cheatshh-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     5815 2024-05-24 18:25:19.000000 cheatshh-1.0.5/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-24 18:31:19.673301 cheatshh-1.0.5/cheatshh.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     1552 2024-05-24 18:31:19.000000 cheatshh-1.0.5/cheatshh.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      256 2024-05-24 18:31:19.000000 cheatshh-1.0.5/cheatshh.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-05-24 18:31:19.000000 cheatshh-1.0.5/cheatshh.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       51 2024-05-24 18:31:19.000000 cheatshh-1.0.5/cheatshh.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)       21 2024-05-24 18:31:19.000000 cheatshh-1.0.5/cheatshh.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        4 2024-05-24 18:31:19.000000 cheatshh-1.0.5/cheatshh.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2024-05-24 18:31:19.674125 cheatshh-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     3391 2024-05-24 18:23:49.000000 cheatshh-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-24 18:31:19.673520 cheatshh-1.0.5/src/
+-rw-r--r--   0 root         (0) staff       (20)        0 2024-05-09 09:59:20.000000 cheatshh-1.0.5/src/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      222 2024-05-18 10:34:26.000000 cheatshh-1.0.5/src/run_cheatshh.py
```

### Comparing `cheatshh-1.0.4/LICENSE` & `cheatshh-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cheatshh-1.0.4/PKG-INFO` & `cheatshh-1.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: cheatshh
-Version: 1.0.4
+Version: 1.0.5
+Home-page: https://github.com/AnirudhG07/cheatshh
 Author: Anirudh Gupta
 Keywords: cheatsheet, cheat, command-line, cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fuzzyfinder
 Requires-Dist: whiptail
 
@@ -17,21 +18,22 @@
 
 - Comprehensive cheatsheets for various command-line utilities and tools.
 - Easy-to-use interface for quickly accessing and executing commands, powered by fuzzy finder(fzf) and whiptail.
 - Customizable cheatshheets and groups to suit your needs.
 - TLDR and MAN pages visible in the preview.
 - Easy to add, edit, delete commands and groups and playing around.
 - Press Enter on a command to copy it to clipboard and exit.
+- Bookmark your favourite commands and view them in main preview despite being in a group.
 
 Visit the Github Repository for more details: https://github.com/AnirudhG07/cheatshh
 
 # Version
-1.0.4
+1.0.5
 
 ## Note:
 - This package is best used in Unix based systems, like linux and MacOS. For Windows, see the github repository for more details.
 - The package is installed in ~/.config/cheatshh directory.
 
-## Bugs fixed in 1.0.4
+## Bugs fixed in 1.0.5
 - Path configuration for Linux has been fixed.
 - group names will be displayed whenever asked to enter a group name in option functionalities.
```

### Comparing `cheatshh-1.0.4/README.md` & `cheatshh-1.0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,114 +1,162 @@
-# cheatshh ![Static Badge](https://img.shields.io/badge/version-1.0.4-blue)
+# cheatshh ![Static Badge](https://img.shields.io/badge/version-1.0.5-blue)
 
 Cheatshh is an interactive CLI meant for managing command line cheatshheets, written in shell script. Now you don't have to remember CLI commands and just refer your cheatshhet. You can group commands and view their TLDR and MAN pages along with a custom description for the command.
 
 # Preview/Screenshots 
 
 https://github.com/AnirudhG07/cheatshh/assets/146579014/831405bb-aba4-461f-9ca9-e0f75d74155d
 
-
 # Features
 
 - Comprehensive cheatsheets for various command-line utilities and tools.
 - Easy-to-use interface for quickly accessing and executing commands, powered by fuzzy finder(fzf) and whiptail.
 - Customizable cheatshheets and groups to suit your needs.
 - TLDR and MAN pages visible in the preview.
-- Easy to add, edit, delete commands and groups and playing around.
+- Easy to add, edit, delete commands & groups and play around.
+- Bookmark commands to access them outside of group as well.
+
+# Installation
 
-# Installation 
 The following installation guidelines hold for Linux and MacOS.<br>
 You can download cheatshh through following ways- (more will be added soon)
 
-## Pip Installation 
+## Pip Installation
+
 Before running the below commands, make sure your dependencies are satisfied. See the DEPENDENCIES section for more info.
 From your command line, run-
+
 ```bash
 pip install cheatshh
 ```
+
 This will create ~/.config/cheatshh in your home directory. Now simply run-
+
 ```bash
 cheatshh
 ```
+
 and you are done. Use various options to add, edit and delete commands and groups.
 
 ## Manual Installation through git clone
+
 You can setup manual installation with the following guidelines-
 
 ### For MacOS and Linux
+
 1. Clone the repository
+
 ```bash
 git clone https://github.com/AnirudhG07/cheatshh
 ```
+
 2. Navigate to the project directory run below if downloaded in home directory
+
 ```bash
 cd ~/cheatshh
 ```
+
 3. Install the requirements through
+
 ```
 pip install -r requirements.txt
 ```
+
 4. Run the `setup.py` code to set cheatshh
+
 ```bash
 python setup.py install
 ```
-Now you should be able to use the tool by running ```cheatshh``` in your terminal. Feel free to raise an issue if any error comes up.
+
+Now you should be able to use the tool by running `cheatshh` in your terminal. Feel free to raise an issue if any error comes up.
 
 ## For Windows
+
 For Windows, you can use Virtual Machines of Linux, or change configurations manually.<br>
+
 - Change the path to directory `~/.config/cheatshh` to `/path/to/your/directory/cheatshh`, by using grep command
-in the cheatshh directory, in `setup.py`,`cheats.sh` and manually setting up `./src/run_cheatshh.py`.
+  in the cheatshh directory, in `setup.py`,`cheats.sh` and manually setting up `./src/run_cheatshh.py`.
 
-- This should run cheatshh appropriately. Make sure the dependencies are installed, since they are easy available for Unix applications.
+- This should run cheatshh appropriately. Make sure the dependencies are installed, since they are easily available for Unix applications.
 
 # Libraries and Groups
-You can create custom groups usig-
+
+You can create custom groups using-
+
 ```bash
 cheatshh -g
 ```
+
 We also have premade libraries of groups <a href="https://github.com/AnirudhG07/cheatshh/tree/main/library"> here </a> which you can download with the instructions given there itself. <br>
 We welcome you to publish your own libraries for everyone to see.
 
+# Bookmarking
+Bookmarking let's you save your command in the main preview despite them being present in a group.<br>
+You can bookmark a command by pressing Enter and selecting `Bookmark`. Now you don't need to find it in a group and access it in the main preview.<br>You can always remove Bookmark of a command by pressing Enter and selecting `Remove Bookmark`.
+
 # Dependencies
+
 Cheatshh uses the following as its main tools. Ensure that these are pre-installed in your computer.
+
 - fuzzy finder
 - whiptail
 - jq
 
 In MacOS, you can use HomeBrew to install the above packages with-
+
 ```bash
 brew install <package>
 ```
+
 For MacOS & Linux both, you can run the following command to download the packages.
+
 ```bash
 sudo apt install <package>
 ```
-For Windows, you can use your favourite package manager to download the packages,
+
+For Windows, you can use your favourite package manager or download from their website itself.
 
 # Trouble-shooting
-1) If permission denial error shows upm run the same command using sudo. You will have to provide password in this case. 
+
+1. If permission denial error shows up, run the same command using sudo. You will have to provide password in this case.
+
 ```bash
 sudo <command-name>
 ```
-    This might be needed in the case for man page display or maybe for installation of dependency.
-2) If `WARNING: The script cheatshh is installed in '/home/admin/.local/bin' which is not on PATH.` error comes, then cheatshh script has to be included in the system PATH, you can add the following lines to the appropriate shell configuration.
-- BASH: Add the following at the end of ~/.bashrc 
+
+This might be needed in the case for man page display or maybe for installation of dependency.
+
+2. If `WARNING: The script cheatshh is installed in '/home/admin/.local/bin' which is not on PATH.` error comes, then cheatshh script has to be included in the system PATH, you can add the following lines to the appropriate shell configuration.
+
+- BASH: Add the following at the end of ~/.bashrc
+
 ```bash
 export PATH="$HOME/.local/bin:$PATH"
 ```
+
 - ZSH: Add the following at the end of ~/.zshrc
+
 ```bash
 export PATH="$HOME/.local/bin:$PATH"
 ```
+
 After adding these lines, either restart your terminal or run source on the respective configuration file to apply the changes. For example:
+
 ```bash
 source ~/.bashrc  # For Bash
 source ~/.zshrc   # For Zsh
 ```
-This should add the path in your shell-rc file and you should be able to run.<br>
-Note: If you are using some other shell like fish or any other, configure the settings accordingly. Using Fish is not recommended for this tool.
+
+This should add the path in your `shell-rc` file and you should be able to run.<br>
+Note: If you are using some other shell like fish or any similar other, configure the settings accordingly. Using Fish is not recommended for this tool.
 
 # Documentation
-Cheatshh is an interactive, easy CLI tool to maintain your custom cheatshheets. You can check our the <a href="https://github.com/AnirudhG07/cheatshh/tree/1.0.4/docs"> docs </a> to see how to use cheatshh.
+
+Cheatshh is an interactive, easy CLI tool to maintain your custom cheatshheets. You can check our the <a href="https://github.com/AnirudhG07/cheatshh/tree/1.0.5/docs"> docs </a> to see how to use cheatshh.
 
 # Contributing
-I would love to take contributions from the community! If you have suggestions for new cheatsheets, improvements to existing ones, or bug fixes, please feel free to submit a pull request.
+
+I would love to take contributions from the community! If you have suggestions for new cheatsheets, improvements to existing ones, or bug fixes, please feel free to submit a pull request. 
+### Contribution Guidelines
+1) For contribution of a library, it should have a suitable folder name(max 3 words) with commands.json and groups.json, similar to the format in other libraries. The `group` field should be "yes", `bookmark` field should be "no".
+2) For bug fixes, it will be great if you could discuss first in Issues before directly putting a PR. 
+3) It would be great to publish this in other package managers. So I would request help for publishing to different package managers.
```

#### html2text {}

```diff
@@ -1,62 +1,76 @@
-# cheatshh ![Static Badge](https://img.shields.io/badge/version-1.0.4-blue)
+# cheatshh ![Static Badge](https://img.shields.io/badge/version-1.0.5-blue)
 Cheatshh is an interactive CLI meant for managing command line cheatshheets,
 written in shell script. Now you don't have to remember CLI commands and just
 refer your cheatshhet. You can group commands and view their TLDR and MAN pages
 along with a custom description for the command. # Preview/ScreenshotsÂ  https:
 //github.com/AnirudhG07/cheatshh/assets/146579014/831405bb-aba4-461f-9ca9-
 e0f75d74155d # Features - Comprehensive cheatsheets for various command-line
 utilities and tools. - Easy-to-use interface for quickly accessing and
 executing commands, powered by fuzzy finder(fzf) and whiptail. - Customizable
 cheatshheets and groups to suit your needs. - TLDR and MAN pages visible in the
-preview. - Easy to add, edit, delete commands and groups and playing around. #
-Installation The following installation guidelines hold for Linux and MacOS.
+preview. - Easy to add, edit, delete commands & groups and play around. -
+Bookmark commands to access them outside of group as well. # Installation The
+following installation guidelines hold for Linux and MacOS.
 You can download cheatshh through following ways- (more will be added soon) ##
 Pip Installation Before running the below commands, make sure your dependencies
 are satisfied. See the DEPENDENCIES section for more info. From your command
 line, run- ```bash pip install cheatshh ``` This will create ~/.config/cheatshh
 in your home directory. Now simply run- ```bash cheatshh ``` and you are done.
 Use various options to add, edit and delete commands and groups. ## Manual
 Installation through git clone You can setup manual installation with the
 following guidelines- ### For MacOS and Linux 1. Clone the repository ```bash
 git clone https://github.com/AnirudhG07/cheatshh ``` 2. Navigate to the project
 directory run below if downloaded in home directory ```bash cd ~/cheatshh ```
 3. Install the requirements through ``` pip install -r requirements.txt ``` 4.
 Run the `setup.py` code to set cheatshh ```bash python setup.py install ``` Now
-you should be able to use the tool by running ```cheatshh``` in your terminal.
-Feel free to raise an issue if any error comes up. ## For Windows For Windows,
-you can use Virtual Machines of Linux, or change configurations manually.
+you should be able to use the tool by running `cheatshh` in your terminal. Feel
+free to raise an issue if any error comes up. ## For Windows For Windows, you
+can use Virtual Machines of Linux, or change configurations manually.
 - Change the path to directory `~/.config/cheatshh` to `/path/to/your/
 directory/cheatshh`, by using grep command in the cheatshh directory, in
 `setup.py`,`cheats.sh` and manually setting up `./src/run_cheatshh.py`. - This
 should run cheatshh appropriately. Make sure the dependencies are installed,
-since they are easy available for Unix applications. # Libraries and Groups You
-can create custom groups usig- ```bash cheatshh -g ``` We also have premade
-libraries of groups _h_e_r_e_ which you can download with the instructions given
-there itself.
-We welcome you to publish your own libraries for everyone to see. #
-Dependencies Cheatshh uses the following as its main tools. Ensure that these
-are pre-installed in your computer. - fuzzy finder - whiptail - jq In MacOS,
-you can use HomeBrew to install the above packages with- ```bash brew install
-``` For MacOS & Linux both, you can run the following command to download the
-packages. ```bash sudo apt install ``` For Windows, you can use your favourite
-package manager to download the packages, # Trouble-shooting 1) If permission
-denial error shows upm run the same command using sudo. You will have to
-provide password in this case. ```bash sudo ``` This might be needed in the
-case for man page display or maybe for installation of dependency. 2) If
-`WARNING: The script cheatshh is installed in '/home/admin/.local/bin' which is
-not on PATH.` error comes, then cheatshh script has to be included in the
-system PATH, you can add the following lines to the appropriate shell
-configuration. - BASH: Add the following at the end of ~/.bashrc ```bash export
-PATH="$HOME/.local/bin:$PATH" ``` - ZSH: Add the following at the end of
-~/.zshrc ```bash export PATH="$HOME/.local/bin:$PATH" ``` After adding these
-lines, either restart your terminal or run source on the respective
-configuration file to apply the changes. For example: ```bash source ~/.bashrc
-# For Bash source ~/.zshrc # For Zsh ``` This should add the path in your
-shell-rc file and you should be able to run.
-Note: If you are using some other shell like fish or any other, configure the
-settings accordingly. Using Fish is not recommended for this tool. #
-Documentation Cheatshh is an interactive, easy CLI tool to maintain your custom
-cheatshheets. You can check our the _d_o_c_s_ to see how to use cheatshh. #
-Contributing I would love to take contributions from the community! If you have
-suggestions for new cheatsheets, improvements to existing ones, or bug fixes,
-please feel free to submit a pull request.
+since they are easily available for Unix applications. # Libraries and Groups
+You can create custom groups using- ```bash cheatshh -g ``` We also have
+premade libraries of groups _h_e_r_e_ which you can download with the instructions
+given there itself.
+We welcome you to publish your own libraries for everyone to see. # Bookmarking
+Bookmarking let's you save your command in the main preview despite them being
+present in a group.
+You can bookmark a command by pressing Enter and selecting `Bookmark`. Now you
+don't need to find it in a group and access it in the main preview.
+You can always remove Bookmark of a command by pressing Enter and selecting
+`Remove Bookmark`. # Dependencies Cheatshh uses the following as its main
+tools. Ensure that these are pre-installed in your computer. - fuzzy finder -
+whiptail - jq In MacOS, you can use HomeBrew to install the above packages
+with- ```bash brew install ``` For MacOS & Linux both, you can run the
+following command to download the packages. ```bash sudo apt install ``` For
+Windows, you can use your favourite package manager or download from their
+website itself. # Trouble-shooting 1. If permission denial error shows up, run
+the same command using sudo. You will have to provide password in this case.
+```bash sudo ``` This might be needed in the case for man page display or maybe
+for installation of dependency. 2. If `WARNING: The script cheatshh is
+installed in '/home/admin/.local/bin' which is not on PATH.` error comes, then
+cheatshh script has to be included in the system PATH, you can add the
+following lines to the appropriate shell configuration. - BASH: Add the
+following at the end of ~/.bashrc ```bash export PATH="$HOME/.local/bin:$PATH"
+``` - ZSH: Add the following at the end of ~/.zshrc ```bash export
+PATH="$HOME/.local/bin:$PATH" ``` After adding these lines, either restart your
+terminal or run source on the respective configuration file to apply the
+changes. For example: ```bash source ~/.bashrc # For Bash source ~/.zshrc # For
+Zsh ``` This should add the path in your `shell-rc` file and you should be able
+to run.
+Note: If you are using some other shell like fish or any similar other,
+configure the settings accordingly. Using Fish is not recommended for this
+tool. # Documentation Cheatshh is an interactive, easy CLI tool to maintain
+your custom cheatshheets. You can check our the _d_o_c_s_ to see how to use
+cheatshh. # Contributing I would love to take contributions from the community!
+If you have suggestions for new cheatsheets, improvements to existing ones, or
+bug fixes, please feel free to submit a pull request. ### Contribution
+Guidelines 1) For contribution of a library, it should have a suitable folder
+name(max 3 words) with commands.json and groups.json, similar to the format in
+other libraries. The `group` field should be "yes", `bookmark` field should be
+"no". 2) For bug fixes, it will be great if you could discuss first in Issues
+before directly putting a PR. 3) It would be great to publish this in other
+package managers. So I would request help for publishing to different package
+managers.
```

### Comparing `cheatshh-1.0.4/cheatshh.egg-info/PKG-INFO` & `cheatshh-1.0.5/cheatshh.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: cheatshh
-Version: 1.0.4
+Version: 1.0.5
+Home-page: https://github.com/AnirudhG07/cheatshh
 Author: Anirudh Gupta
 Keywords: cheatsheet, cheat, command-line, cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fuzzyfinder
 Requires-Dist: whiptail
 
@@ -17,21 +18,22 @@
 
 - Comprehensive cheatsheets for various command-line utilities and tools.
 - Easy-to-use interface for quickly accessing and executing commands, powered by fuzzy finder(fzf) and whiptail.
 - Customizable cheatshheets and groups to suit your needs.
 - TLDR and MAN pages visible in the preview.
 - Easy to add, edit, delete commands and groups and playing around.
 - Press Enter on a command to copy it to clipboard and exit.
+- Bookmark your favourite commands and view them in main preview despite being in a group.
 
 Visit the Github Repository for more details: https://github.com/AnirudhG07/cheatshh
 
 # Version
-1.0.4
+1.0.5
 
 ## Note:
 - This package is best used in Unix based systems, like linux and MacOS. For Windows, see the github repository for more details.
 - The package is installed in ~/.config/cheatshh directory.
 
-## Bugs fixed in 1.0.4
+## Bugs fixed in 1.0.5
 - Path configuration for Linux has been fixed.
 - group names will be displayed whenever asked to enter a group name in option functionalities.
```

### Comparing `cheatshh-1.0.4/setup.py` & `cheatshh-1.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,46 +45,48 @@
         dest_path = os.path.join(config_dir, file_name)
         shutil.copy(src_path, dest_path)
     print("Cheatshh installed successfully!")
 
 def run_cheatshh():
     subprocess.run(["bash", os.path.expanduser("~/.config/cheatshh/cheats.sh")])
 
-setup(name="cheatshh", version="1.0.4", cmdclass={"install": CustomInstallCommand},
+setup(name="cheatshh", version="1.0.5", cmdclass={"install": CustomInstallCommand},
       long_description="""
 # cheatshh
 
 Cheatshh is an interactive CLI meant for managing command line cheatshheets. Now you don't have to remember CLI commands and just refer your cheatshhet. You can group commands and view their TLDR and MAN pages along with a custom description for the command.
 
 # Features
 
 - Comprehensive cheatsheets for various command-line utilities and tools.
 - Easy-to-use interface for quickly accessing and executing commands, powered by fuzzy finder(fzf) and whiptail.
 - Customizable cheatshheets and groups to suit your needs.
 - TLDR and MAN pages visible in the preview.
 - Easy to add, edit, delete commands and groups and playing around.
 - Press Enter on a command to copy it to clipboard and exit.
+- Bookmark your favourite commands and view them in main preview despite being in a group.
 
 Visit the Github Repository for more details: https://github.com/AnirudhG07/cheatshh
 
 # Version
-1.0.4
+1.0.5
 
 ## Note:
 - This package is best used in Unix based systems, like linux and MacOS. For Windows, see the github repository for more details.
 - The package is installed in ~/.config/cheatshh directory.
 
-## Bugs fixed in 1.0.4
+## Bugs fixed in 1.0.5
 - Path configuration for Linux has been fixed.
 - group names will be displayed whenever asked to enter a group name in option functionalities.
 
 """,
     long_description_content_type="text/markdown",
     keywords=["cheatsheet, cheat, command-line, cli"],
     install_requires=["fuzzyfinder", "whiptail"],
+    url="https://github.com/AnirudhG07/cheatshh",
     author="Anirudh Gupta",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "cheatshh=src.run_cheatshh:main",
         ],
     },
```

