# Comparing `tmp/odoo_addon_upgrade_analysis-16.0.1.0.2-py3-none-any.whl.zip` & `tmp/odoo_addon_upgrade_analysis-17.0.1.0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,57 +1,56 @@
-Zip file size: 66326 bytes, number of entries: 55
--rw-r--r--  2.0 unx     4561 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/README.rst
--rw-r--r--  2.0 unx      140 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/__init__.py
--rw-r--r--  2.0 unx     1077 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/__manifest__.py
--rw-r--r--  2.0 unx      362 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/blacklist.py
--rw-r--r--  2.0 unx    20132 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/compare.py
--rw-r--r--  2.0 unx     8297 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/upgrade_log.py
--rw-r--r--  2.0 unx    22496 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/i18n/es_AR.po
--rw-r--r--  2.0 unx    20161 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/i18n/fr.po
--rw-r--r--  2.0 unx    19925 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/i18n/upgrade_analysis.pot
--rw-r--r--  2.0 unx      163 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/models/__init__.py
--rw-r--r--  2.0 unx     1031 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/models/ir_module_module.py
--rw-r--r--  2.0 unx    22546 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/models/upgrade_analysis.py
--rw-r--r--  2.0 unx      536 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/models/upgrade_attribute.py
--rw-r--r--  2.0 unx     3098 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/models/upgrade_comparison_config.py
--rw-r--r--  2.0 unx     6006 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/models/upgrade_record.py
--rw-r--r--  2.0 unx       65 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/odoo_patch/__init__.py
--rw-r--r--  2.0 unx     1843 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/odoo_patch/odoo_patch.py
--rw-r--r--  2.0 unx      103 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/odoo_patch/addons/__init__.py
--rw-r--r--  2.0 unx      270 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/odoo_patch/addons/mrp/__init__.py
--rw-r--r--  2.0 unx      371 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/odoo_patch/addons/point_of_sale/__init__.py
--rw-r--r--  2.0 unx      341 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/odoo_patch/addons/sale_quotation_builder/__init__.py
--rw-r--r--  2.0 unx      259 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/odoo_patch/addons/stock/__init__.py
--rw-r--r--  2.0 unx       84 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/odoo_patch/odoo/__init__.py
--rw-r--r--  2.0 unx      739 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/odoo_patch/odoo/models.py
--rw-r--r--  2.0 unx       19 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/__init__.py
--rw-r--r--  2.0 unx       21 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/__init__.py
--rw-r--r--  2.0 unx       23 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/__init__.py
--rw-r--r--  2.0 unx     1482 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/ir_model.py
--rw-r--r--  2.0 unx       23 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/__init__.py
--rw-r--r--  2.0 unx     1112 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/registry.py
--rw-r--r--  2.0 unx       22 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/__init__.py
--rw-r--r--  2.0 unx      397 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/convert.py
--rw-r--r--  2.0 unx      308 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/readme/CONTRIBUTORS.rst
--rw-r--r--  2.0 unx      675 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/readme/DESCRIPTION.rst
--rw-r--r--  2.0 unx      263 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/readme/ROADMAP.rst
--rw-r--r--  2.0 unx       71 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/readme/USAGE.rst
--rw-r--r--  2.0 unx      696 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/security/ir.model.access.csv
--rw-r--r--  2.0 unx     9455 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/static/description/icon.png
--rw-r--r--  2.0 unx    15067 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/static/description/index.html
--rw-r--r--  2.0 unx      744 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/static/src/module_coverage_template.rst.mako
--rw-r--r--  2.0 unx       26 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/tests/__init__.py
--rw-r--r--  2.0 unx     1787 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/tests/test_module.py
--rw-r--r--  2.0 unx      200 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/views/menu.xml
--rw-r--r--  2.0 unx     2640 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/views/view_upgrade_analysis.xml
--rw-r--r--  2.0 unx     2826 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/views/view_upgrade_comparison_config.xml
--rw-r--r--  2.0 unx     2834 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/views/view_upgrade_record.xml
--rw-r--r--  2.0 unx       82 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/wizards/__init__.py
--rw-r--r--  2.0 unx     4527 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/wizards/upgrade_generate_record_wizard.py
--rw-r--r--  2.0 unx     4040 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/wizards/upgrade_install_wizard.py
--rw-r--r--  2.0 unx     1787 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/wizards/view_upgrade_generate_record_wizard.xml
--rw-r--r--  2.0 unx     3289 b- defN 24-Feb-02 21:10 odoo/addons/upgrade_analysis/wizards/view_upgrade_install_wizard.xml
--rw-r--r--  2.0 unx     5278 b- defN 24-Feb-02 21:10 odoo_addon_upgrade_analysis-16.0.1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-02 21:10 odoo_addon_upgrade_analysis-16.0.1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-Feb-02 21:10 odoo_addon_upgrade_analysis-16.0.1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     6155 b- defN 24-Feb-02 21:10 odoo_addon_upgrade_analysis-16.0.1.0.2.dist-info/RECORD
-55 files, 200552 bytes uncompressed, 55904 bytes compressed:  72.1%
+Zip file size: 65856 bytes, number of entries: 54
+-rw-r--r--  2.0 unx     4578 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/README.rst
+-rw-r--r--  2.0 unx      140 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/__init__.py
+-rw-r--r--  2.0 unx     1077 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/__manifest__.py
+-rw-r--r--  2.0 unx      456 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/blacklist.py
+-rw-r--r--  2.0 unx    19987 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/compare.py
+-rw-r--r--  2.0 unx     8286 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/upgrade_log.py
+-rw-r--r--  2.0 unx    22496 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/i18n/es_AR.po
+-rw-r--r--  2.0 unx    20161 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/i18n/fr.po
+-rw-r--r--  2.0 unx    18533 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/i18n/upgrade_analysis.pot
+-rw-r--r--  2.0 unx      163 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/models/__init__.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/models/ir_module_module.py
+-rw-r--r--  2.0 unx    22565 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/models/upgrade_analysis.py
+-rw-r--r--  2.0 unx      536 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/models/upgrade_attribute.py
+-rw-r--r--  2.0 unx     3098 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/models/upgrade_comparison_config.py
+-rw-r--r--  2.0 unx     5998 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/models/upgrade_record.py
+-rw-r--r--  2.0 unx       65 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/__init__.py
+-rw-r--r--  2.0 unx     1835 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/odoo_patch.py
+-rw-r--r--  2.0 unx       66 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/addons/__init__.py
+-rw-r--r--  2.0 unx      270 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/addons/mrp/__init__.py
+-rw-r--r--  2.0 unx      371 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/addons/point_of_sale/__init__.py
+-rw-r--r--  2.0 unx      259 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/addons/stock/__init__.py
+-rw-r--r--  2.0 unx       84 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/odoo/__init__.py
+-rw-r--r--  2.0 unx      729 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/odoo/models.py
+-rw-r--r--  2.0 unx       19 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/__init__.py
+-rw-r--r--  2.0 unx       21 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/__init__.py
+-rw-r--r--  2.0 unx       23 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/__init__.py
+-rw-r--r--  2.0 unx     1589 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/ir_model.py
+-rw-r--r--  2.0 unx       23 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/__init__.py
+-rw-r--r--  2.0 unx     1112 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/registry.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/__init__.py
+-rw-r--r--  2.0 unx      397 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/convert.py
+-rw-r--r--  2.0 unx      336 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/readme/CONTRIBUTORS.md
+-rw-r--r--  2.0 unx      677 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/readme/DESCRIPTION.md
+-rw-r--r--  2.0 unx      267 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/readme/ROADMAP.md
+-rw-r--r--  2.0 unx       69 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/readme/USAGE.md
+-rw-r--r--  2.0 unx      696 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/security/ir.model.access.csv
+-rw-r--r--  2.0 unx     9455 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/static/description/icon.png
+-rw-r--r--  2.0 unx    15067 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/static/description/index.html
+-rw-r--r--  2.0 unx      752 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/static/src/module_coverage_template.rst.mako
+-rw-r--r--  2.0 unx       26 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/tests/__init__.py
+-rw-r--r--  2.0 unx     1787 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/tests/test_module.py
+-rw-r--r--  2.0 unx      200 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/views/menu.xml
+-rw-r--r--  2.0 unx     2250 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/views/view_upgrade_analysis.xml
+-rw-r--r--  2.0 unx     2826 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/views/view_upgrade_comparison_config.xml
+-rw-r--r--  2.0 unx     2814 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/views/view_upgrade_record.xml
+-rw-r--r--  2.0 unx       82 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/wizards/__init__.py
+-rw-r--r--  2.0 unx     4527 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/wizards/upgrade_generate_record_wizard.py
+-rw-r--r--  2.0 unx     4066 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/wizards/upgrade_install_wizard.py
+-rw-r--r--  2.0 unx     1919 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/wizards/view_upgrade_generate_record_wizard.xml
+-rw-r--r--  2.0 unx     3454 b- defN 24-May-23 11:02 odoo/addons/upgrade_analysis/wizards/view_upgrade_install_wizard.xml
+-rw-r--r--  2.0 unx     5276 b- defN 24-May-23 11:02 odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       83 b- defN 24-May-23 11:02 odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 24-May-23 11:02 odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6021 b- defN 24-May-23 11:02 odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/RECORD
+54 files, 198644 bytes uncompressed, 55664 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -54,17 +54,14 @@
 
 Filename: odoo/addons/upgrade_analysis/odoo_patch/addons/mrp/__init__.py
 Comment: 
 
 Filename: odoo/addons/upgrade_analysis/odoo_patch/addons/point_of_sale/__init__.py
 Comment: 
 
-Filename: odoo/addons/upgrade_analysis/odoo_patch/addons/sale_quotation_builder/__init__.py
-Comment: 
-
 Filename: odoo/addons/upgrade_analysis/odoo_patch/addons/stock/__init__.py
 Comment: 
 
 Filename: odoo/addons/upgrade_analysis/odoo_patch/odoo/__init__.py
 Comment: 
 
 Filename: odoo/addons/upgrade_analysis/odoo_patch/odoo/models.py
@@ -90,24 +87,24 @@
 
 Filename: odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/__init__.py
 Comment: 
 
 Filename: odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/convert.py
 Comment: 
 
-Filename: odoo/addons/upgrade_analysis/readme/CONTRIBUTORS.rst
+Filename: odoo/addons/upgrade_analysis/readme/CONTRIBUTORS.md
 Comment: 
 
-Filename: odoo/addons/upgrade_analysis/readme/DESCRIPTION.rst
+Filename: odoo/addons/upgrade_analysis/readme/DESCRIPTION.md
 Comment: 
 
-Filename: odoo/addons/upgrade_analysis/readme/ROADMAP.rst
+Filename: odoo/addons/upgrade_analysis/readme/ROADMAP.md
 Comment: 
 
-Filename: odoo/addons/upgrade_analysis/readme/USAGE.rst
+Filename: odoo/addons/upgrade_analysis/readme/USAGE.md
 Comment: 
 
 Filename: odoo/addons/upgrade_analysis/security/ir.model.access.csv
 Comment: 
 
 Filename: odoo/addons/upgrade_analysis/static/description/icon.png
 Comment: 
@@ -147,20 +144,20 @@
 
 Filename: odoo/addons/upgrade_analysis/wizards/view_upgrade_generate_record_wizard.xml
 Comment: 
 
 Filename: odoo/addons/upgrade_analysis/wizards/view_upgrade_install_wizard.xml
 Comment: 
 
-Filename: odoo_addon_upgrade_analysis-16.0.1.0.2.dist-info/METADATA
+Filename: odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addon_upgrade_analysis-16.0.1.0.2.dist-info/WHEEL
+Filename: odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addon_upgrade_analysis-16.0.1.0.2.dist-info/top_level.txt
+Filename: odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addon_upgrade_analysis-16.0.1.0.2.dist-info/RECORD
+Filename: odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/upgrade_analysis/README.rst

```diff
@@ -3,89 +3,100 @@
 ================
 
 .. 
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
    !! This file is generated by oca-gen-addon-readme !!
    !! changes will be overwritten.                   !!
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-   !! source digest: sha256:47c0b46bc356790fb4c33f1147128f376d0f640d2015589cbae86ec0fdeb3e13
+   !! source digest: sha256:f5ec0738486de2c0128f10e4029e18956d4e92509fae8f60ed8c810097220dfe
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 
 .. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: Beta
 .. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 .. |badge3| image:: https://img.shields.io/badge/github-OCA%2Fserver--tools-lightgray.png?logo=github
-    :target: https://github.com/OCA/server-tools/tree/16.0/upgrade_analysis
+    :target: https://github.com/OCA/server-tools/tree/17.0/upgrade_analysis
     :alt: OCA/server-tools
 .. |badge4| image:: https://img.shields.io/badge/weblate-Translate%20me-F47D42.png
-    :target: https://translation.odoo-community.org/projects/server-tools-16-0/server-tools-16-0-upgrade_analysis
+    :target: https://translation.odoo-community.org/projects/server-tools-17-0/server-tools-17-0-upgrade_analysis
     :alt: Translate me on Weblate
 .. |badge5| image:: https://img.shields.io/badge/runboat-Try%20me-875A7B.png
-    :target: https://runboat.odoo-community.org/builds?repo=OCA/server-tools&target_branch=16.0
+    :target: https://runboat.odoo-community.org/builds?repo=OCA/server-tools&target_branch=17.0
     :alt: Try me on Runboat
 
 |badge1| |badge2| |badge3| |badge4| |badge5|
 
-This module provides the tool to generate the database analysis files that indicate how the Odoo data model and module data have changed between two versions of Odoo. Database analysis files for the core modules are included in the OpenUpgrade distribution so as a migration script developer you will not usually need to use this tool yourself. If you do need to run your analysis of a custom set of modules, please refer to the documentation here: https://doc.therp.nl/openupgrade/analysis.html
-
-This module is just a tool, a continuation of the old openupgrade_records in OpenUpgrade in previous versions. It's not recommended to have this module in a production database.
+This module provides the tool to generate the database analysis files
+that indicate how the Odoo data model and module data have changed
+between two versions of Odoo. Database analysis files for the core
+modules are included in the OpenUpgrade distribution so as a migration
+script developer you will not usually need to use this tool yourself. If
+you do need to run your analysis of a custom set of modules, please
+refer to the documentation here:
+https://doc.therp.nl/openupgrade/analysis.html
+
+This module is just a tool, a continuation of the old
+openupgrade_records in OpenUpgrade in previous versions. It's not
+recommended to have this module in a production database.
 
 **Table of contents**
 
 .. contents::
    :local:
 
 Usage
 =====
 
-`Usage instructions <https://oca.github.io/OpenUpgrade/analyse.html>`_
+`Usage instructions <https://oca.github.io/OpenUpgrade/analyse.html>`__
 
 Known issues / Roadmap
 ======================
 
-* Log removed modules in the module that owned them (#468)
-* Detect renamed many2many tables (#213)
-* Make sure that the ``migration_analysis.txt`` file is always generated in all cases. (See: https://github.com/OCA/OpenUpgrade/pull/3209#issuecomment-1157449981)
+-  Log removed modules in the module that owned them (#468)
+-  Detect renamed many2many tables (#213)
+-  Make sure that the ``migration_analysis.txt`` file is always
+   generated in all cases. (See:
+   https://github.com/OCA/OpenUpgrade/pull/3209#issuecomment-1157449981)
 
 Bug Tracker
 ===========
 
 Bugs are tracked on `GitHub Issues <https://github.com/OCA/server-tools/issues>`_.
 In case of trouble, please check there if your issue has already been reported.
 If you spotted it first, help us to smash it by providing a detailed and welcomed
-`feedback <https://github.com/OCA/server-tools/issues/new?body=module:%20upgrade_analysis%0Aversion:%2016.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.
+`feedback <https://github.com/OCA/server-tools/issues/new?body=module:%20upgrade_analysis%0Aversion:%2017.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.
 
 Do not contact contributors directly about support or help with technical issues.
 
 Credits
 =======
 
 Authors
-~~~~~~~
+-------
 
 * Therp BV
 * Opener B.V.
 * GRAP
 
 Contributors
-~~~~~~~~~~~~
+------------
 
-* Stefan Rijnhart <stefan@opener.amsterdam>
-* Holger Brunn <hbrunn@therp.nl>
-* Pedro M. Baeza <pedro.baeza@gmail.com>
-* Ferdinand Gassauer <gass@cc-l-12.chircar.at>
-* Florent Xicluna <florent.xicluna@gmail.com>
-* Miquel Raïch <miquel.raich@forgeflow.com>
-* Sylvain LE GAL <https://twitter.com/legalsylvain>
+-  Stefan Rijnhart <stefan@opener.amsterdam>
+-  Holger Brunn <hbrunn@therp.nl>
+-  Pedro M. Baeza <pedro.baeza@gmail.com>
+-  Ferdinand Gassauer <gass@cc-l-12.chircar.at>
+-  Florent Xicluna <florent.xicluna@gmail.com>
+-  Miquel Raïch <miquel.raich@forgeflow.com>
+-  Sylvain LE GAL <https://twitter.com/legalsylvain>
 
 Maintainers
-~~~~~~~~~~~
+-----------
 
 This module is maintained by the OCA.
 
 .. image:: https://odoo-community.org/logo.png
    :alt: Odoo Community Association
    :target: https://odoo-community.org
 
@@ -100,10 +111,10 @@
     :target: https://github.com/legalsylvain
     :alt: legalsylvain
 
 Current `maintainers <https://odoo-community.org/page/maintainer-role>`__:
 
 |maintainer-StefanRijnhart| |maintainer-legalsylvain| 
 
-This module is part of the `OCA/server-tools <https://github.com/OCA/server-tools/tree/16.0/upgrade_analysis>`_ project on GitHub.
+This module is part of the `OCA/server-tools <https://github.com/OCA/server-tools/tree/17.0/upgrade_analysis>`_ project on GitHub.
 
 You are welcome to contribute. To learn how please visit https://odoo-community.org/page/Contribute.
```

## odoo/addons/upgrade_analysis/__manifest__.py

```diff
@@ -1,15 +1,15 @@
 # Copyright 2011-2015 Therp BV <https://therp.nl>
 # Copyright 2016 Opener B.V. <https://opener.am>
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 {
     "name": "Upgrade Analysis",
     "summary": "Performs a difference analysis between modules"
     " installed on two different Odoo instances",
-    "version": "16.0.1.0.2",
+    "version": "17.0.1.0.0",
     "category": "Migration",
     "author": "Therp BV, Opener B.V., GRAP, Odoo Community Association (OCA)",
     "maintainers": ["StefanRijnhart", "legalsylvain"],
     "website": "https://github.com/OCA/server-tools",
     "data": [
         "security/ir.model.access.csv",
         "views/menu.xml",
```

## odoo/addons/upgrade_analysis/blacklist.py

```diff
@@ -1,8 +1,13 @@
-BLACKLIST_MODULES = []
+BLACKLIST_MODULES = [
+    "payment_alipay",
+    "payment_ogone",
+    "payment_payulatam",
+    "payment_payumoney",
+]
 
 # the hw_* modules are not affected by a migration as they don't
 # contain any ORM functionality, but they do start up threads that
 # delay the process and spit out annoying log messages continuously.
 
 # We also don't want to analyze tests modules
 BLACKLIST_MODULES_STARTS_WITH = ["hw_", "test_"]
```

## odoo/addons/upgrade_analysis/compare.py

```diff
@@ -10,15 +10,16 @@
 
 import collections
 import copy
 
 try:
     from odoo.addons.openupgrade_scripts import apriori
 except ImportError:
-    from dataclasses import dataclass, field as dc_field
+    from dataclasses import dataclass
+    from dataclasses import field as dc_field
 
     @dataclass
     class NullApriori:
         renamed_modules: dict = dc_field(default_factory=dict)
         merged_modules: dict = dc_field(default_factory=dict)
         renamed_models: dict = dc_field(default_factory=dict)
         merged_models: dict = dc_field(default_factory=dict)
@@ -111,26 +112,26 @@
 
 def fieldprint(old, new, field, text, reprs):
     fieldrepr = "{}".format(old["field"])
     if old["field"] not in ("_inherits", "_order"):
         fieldrepr += " ({})".format(old["type"])
     fullrepr = "{:<12} / {:<24} / {:<30}".format(old["module"], old["model"], fieldrepr)
     if not text:
-        text = "{} is now '{}' ('{}')".format(field, new[field], old[field])
+        text = f"{field} is now '{new[field]}' ('{old[field]}')"
         if field in ("column1", "column2"):
-            text += " [%s]" % old["table"]
+            text += f" [{old['table']}]"
         if field == "relation":
             text += " [nothing to do]"
-    reprs[module_map(old["module"])].append("{}: {}".format(fullrepr, text))
+    reprs[module_map(old["module"])].append(f"{fullrepr}: {text}")
     if field == "module":
-        text = "previously in module %s" % old[field]
+        text = f"previously in module {old[field]}"
         fullrepr = "{:<12} / {:<24} / {:<30}".format(
             new["module"], old["model"], fieldrepr
         )
-        reprs[module_map(new["module"])].append("{}: {}".format(fullrepr, text))
+        reprs[module_map(new["module"])].append(f"{fullrepr}: {text}")
 
 
 def report_generic(new, old, attrs, reprs):
     for attr in attrs:
         if attr == "required":
             if old[attr] != new["required"] and new["required"]:
                 text = "now required"
@@ -429,31 +430,31 @@
     sorted_records = sorted(
         old_records + new_records + moved_records + renamed_records + modified_records,
         key=lambda k: (k["model"], "old" in k, k["name"]),
     )
     for entry in sorted_records:
         content = ""
         if "old" in entry:
-            content = "DEL %(model)s: %(name)s" % entry
+            content = f"DEL {entry['model']}: {entry['name']}"
             if "moved" in entry:
-                content += " [moved to %(moved)s module]" % entry
+                content += f" [moved to {entry['moved']} module]"
             elif "renamed" in entry:
-                content += " [renamed to %(renamed)s module]" % entry
+                content += f" [renamed to {entry['renamed']} module]"
         elif "new" in entry:
-            content = "NEW %(model)s: %(name)s" % entry
+            content = f"NEW {entry['model']}: {entry['name']}"
             if "moved" in entry:
-                content += " [moved from %(moved)s module]" % entry
+                content += f" [moved from {entry['moved']} module]"
             elif "renamed" in entry:
-                content += " [renamed from %(renamed)s module]" % entry
+                content += f" [renamed from {entry['renamed']} module]"
         if "old" not in entry and "new" not in entry:
-            content = "%(model)s: %(name)s" % entry
+            content = f"{entry['model']}: {entry['name']}"
         if entry["domain"]:
             content += " (deleted domain)"
         if entry["definition"]:
-            content += " (changed definition: %(definition)s)" % entry
+            content += f" (changed definition: {entry['definition']})"
         if entry["noupdate"]:
             content += " (noupdate)"
         if entry["noupdate_switched"]:
             content += " (noupdate switched)"
         reprs[module_map(entry["module"])].append(content)
     return reprs
 
@@ -470,78 +471,75 @@
     obsolete_models = []
     for column in copy.copy(old_records):
         model = column["model"]
         if model in old_models:
             if model not in new_models:
                 if model_map(model) not in new_models:
                     obsolete_models.append(model)
-                    text = "obsolete model %s" % model
+                    text = f"obsolete model {model}"
                     if column["model_type"]:
-                        text += " [%s]" % column["model_type"]
+                        text += f" [{column['model_type']}]"
                     reprs[module_map(column["module"])].append(text)
                     reprs["general"].append(
-                        "obsolete model %s [module %s]"
-                        % (model, module_map(column["module"]))
+                        f"obsolete model {model} [module module_map(column['module'])]"
                     )
                 else:
                     moved_module = ""
                     if module_map(column["module"]) != new_models[model_map(model)]:
-                        moved_module = " in module %s" % new_models[model_map(model)]
+                        moved_module = f" in module {new_models[model_map(model)]}"
                     text = "obsolete model {} (renamed to {}{})".format(
                         model,
                         model_map(model),
                         moved_module,
                     )
                     if column["model_type"]:
-                        text += " [%s]" % column["model_type"]
+                        text += " [column['model_type']]"
                     reprs[module_map(column["module"])].append(text)
                     reprs["general"].append(
-                        "obsolete model %s (renamed to %s) [module %s]"
-                        % (model, model_map(model), module_map(column["module"]))
+                        f"obsolete model {model} (renamed to {model_map(model)}) "
+                        f"[module {module_map(column['module'])}]"
                     )
             else:
                 if module_map(column["module"]) != new_models[model]:
-                    text = "model {} (moved to {})".format(model, new_models[model])
+                    text = f"model {model} (moved to {new_models[model]})"
                     if column["model_type"]:
-                        text += " [%s]" % column["model_type"]
+                        text += " [column['model_type']]"
                     reprs[module_map(column["module"])].append(text)
-                    text = "model {} (moved from {})".format(model, old_models[model])
+                    text = f"model {model} (moved from {old_models[model]})"
                     if column["model_type"]:
-                        text += " [%s]" % column["model_type"]
+                        text += " [column['model_type']]"
 
     for column in copy.copy(new_records):
         model = column["model"]
         if model in new_models:
             if model not in old_models:
                 if inv_model_map(model) not in old_models:
-                    text = "new model %s" % model
+                    text = f"new model {model}"
                     if column["model_type"]:
-                        text += " [%s]" % column["model_type"]
+                        text += f" [{column['model_type']}]"
                     reprs[column["module"]].append(text)
                     reprs["general"].append(
                         "new model {} [module {}]".format(model, column["module"])
                     )
                 else:
                     moved_module = ""
                     if column["module"] != module_map(old_models[inv_model_map(model)]):
-                        moved_module = (
-                            " in module %s" % old_models[inv_model_map(model)]
-                        )
+                        moved_module = f" in module {old_models[inv_model_map(model)]}"
                     text = "new model {} (renamed from {}{})".format(
                         model,
                         inv_model_map(model),
                         moved_module,
                     )
                     if column["model_type"]:
-                        text += " [%s]" % column["model_type"]
+                        text += f" [{column['model_type']}]"
                     reprs[column["module"]].append(text)
                     reprs["general"].append(
-                        "new model %s (renamed from %s) [module %s]"
-                        % (model, inv_model_map(model), column["module"])
+                        f"new model {model} (renamed from {inv_model_map(model)}) "
+                        f"[module {column['module']}]"
                     )
             else:
                 if column["module"] != module_map(old_models[model]):
-                    text = "model {} (moved from {})".format(model, old_models[model])
+                    text = f"model {model} (moved from {old_models[model]})"
                     if column["model_type"]:
-                        text += " [%s]" % column["model_type"]
+                        text += f" [{column['model_type']}]"
                     reprs[column["module"]].append(text)
     return reprs
```

## odoo/addons/upgrade_analysis/upgrade_log.py

```diff
@@ -158,15 +158,15 @@
             "table": field.relation if field.type == "many2many" else "",
             "required": field.required and "required" or "",
             "stored": field.store and "stored" or "",
             "selection_keys": "",
             "hasdefault": hasdefault(field),
         }
         if field.type == "selection":
-            if isinstance(field.selection, (tuple, list)):
+            if isinstance(field.selection, tuple | list):
                 properties["selection_keys"] = str(
                     sorted(x[0] for x in field.selection)
                 )
             else:
                 properties["selection_keys"] = "function"
         elif field.type == "binary":
             properties["attachment"] = str(getattr(field, "attachment", False))
@@ -207,15 +207,15 @@
 
     :param module: The module that contains the xml_id
     :param xml_id: the xml_id, with or without 'module.' prefix
     """
     if not table_exists(cr, "upgrade_record"):
         return
     if "." not in xml_id:
-        xml_id = "{}.{}".format(module, xml_id)
+        xml_id = f"{module}.{xml_id}"
     cr.execute(
         "SELECT model FROM ir_model_data " "WHERE module = %s AND name = %s",
         xml_id.split("."),
     )
     record = cr.fetchone()
     if not record:
         _logger.warning("Cannot find xml_id %s", xml_id)
```

## odoo/addons/upgrade_analysis/i18n/upgrade_analysis.pot

```diff
@@ -1,14 +1,14 @@
 # Translation of Odoo Server.
 # This file contains the translation of the following modules:
 # 	* upgrade_analysis
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: Odoo Server 16.0\n"
+"Project-Id-Version: Odoo Server 17.0\n"
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Plural-Forms: \n"
@@ -217,24 +217,14 @@
 
 #. module: upgrade_analysis
 #: model:ir.model.fields,field_description:upgrade_analysis.field_ir_module_module__is_odoo_module
 msgid "Is Odoo Module"
 msgstr ""
 
 #. module: upgrade_analysis
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_analysis____last_update
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_attribute____last_update
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_comparison_config____last_update
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_generate_record_wizard____last_update
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard____last_update
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_record____last_update
-msgid "Last Modified on"
-msgstr ""
-
-#. module: upgrade_analysis
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_analysis__write_uid
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_attribute__write_uid
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_comparison_config__write_uid
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_generate_record_wizard__write_uid
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__write_uid
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_record__write_uid
 msgid "Last Updated by"
@@ -285,20 +275,24 @@
 #. module: upgrade_analysis
 #: model_terms:ir.ui.view,arch_db:upgrade_analysis.view_upgrade_record_search
 msgid "Modify Mode"
 msgstr ""
 
 #. module: upgrade_analysis
 #: model:ir.model,name:upgrade_analysis.model_ir_module_module
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__module_ids
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_record__module
 msgid "Module"
 msgstr ""
 
 #. module: upgrade_analysis
+#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__module_ids
+msgid "Modules"
+msgstr ""
+
+#. module: upgrade_analysis
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__module_qty
 msgid "Modules Quantity"
 msgstr ""
 
 #. module: upgrade_analysis
 #: model_terms:ir.ui.view,arch_db:upgrade_analysis.view_upgrade_generate_record_wizard_form
 msgid "Modules initialized and record created"
@@ -367,25 +361,14 @@
 #: model:ir.model.fields,help:upgrade_analysis.field_upgrade_record__mode
 msgid ""
 "Set to Create if a field is newly created in this module. If this module "
 "modifies an attribute of an existing field, set to Modify."
 msgstr ""
 
 #. module: upgrade_analysis
-#: model:ir.model.fields,field_description:upgrade_analysis.field_ir_module_module__smart_search
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_analysis__smart_search
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_attribute__smart_search
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_comparison_config__smart_search
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_generate_record_wizard__smart_search
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__smart_search
-#: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_record__smart_search
-msgid "Smart Search"
-msgstr ""
-
-#. module: upgrade_analysis
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_analysis__state
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_generate_record_wizard__state
 #: model:ir.model.fields,field_description:upgrade_analysis.field_upgrade_install_wizard__state
 msgid "State"
 msgstr ""
 
 #. module: upgrade_analysis
```

## odoo/addons/upgrade_analysis/models/upgrade_analysis.py

```diff
@@ -46,15 +46,16 @@
         readonly=True,
         required=True,
     )
 
     log = fields.Text(readonly=True)
     upgrade_path = fields.Char(
         compute="_compute_upgrade_path",
-        readonly=True,
+        readonly=False,
+        store=True,
         help=(
             "The base file path to save the analyse files of Odoo modules. "
             "Taken from Odoo's --upgrade-path command line option or the "
             "'scripts' subdirectory in the openupgrade_scripts addon."
         ),
     )
     write_files = fields.Boolean(
@@ -95,15 +96,15 @@
         else:
             full_path = os.path.join(
                 get_module_path(module_name), "migrations", version
             )
         if not os.path.exists(full_path):
             try:
                 os.makedirs(full_path)
-            except os.error:
+            except OSError:
                 return "ERROR: could not create migrations directory %s:\n" % (
                     full_path
                 )
         logfile = os.path.join(full_path, filename)
         try:
             f = open(logfile, "w")
         except Exception:
@@ -265,15 +266,14 @@
             )
 
         try:
             self.generate_noupdate_changes()
         except Exception as e:
             _logger.exception("Error generating noupdate changes: %s" % e)
             general_log += "ERROR: error when generating noupdate changes: %s\n" % e
-
         try:
             self.generate_module_coverage_file(no_changes_modules)
         except Exception as e:
             _logger.exception("Error generating module coverage file: %s" % e)
             general_log += "ERROR: error when generating module coverage file: %s\n" % e
 
         self.write(
@@ -570,15 +570,15 @@
                         x
                         for x in compare.apriori.renamed_modules
                         if compare.apriori.renamed_modules[x] == module
                     ][0]
                 )
             elif module in no_changes_modules:
                 status += "No DB layout changes. "
-            module_descriptions[module_description.ljust(49, " ")] = status.ljust(
+            module_descriptions[module_description.ljust(51, " ")] = status.ljust(
                 49, " "
             )
 
         rendered_text = file_template.render(
             start_version=start_version,
             end_version=end_version,
             module_descriptions=module_descriptions,
```

## odoo/addons/upgrade_analysis/models/upgrade_record.py

```diff
@@ -140,21 +140,21 @@
     @api.model
     def list_modules(self):
         """Return the set of covered modules"""
         self.env.cr.execute(
             """SELECT DISTINCT(module) FROM upgrade_record
             ORDER BY module"""
         )
-        return [module for module, in self.env.cr.fetchall()]
+        return [module for (module,) in self.env.cr.fetchall()]
 
     @staticmethod
     def _read_manifest(addon_dir):
         for manifest_name in MANIFEST_NAMES:
             if os.access(os.path.join(addon_dir, manifest_name), os.R_OK):
-                with open(os.path.join(addon_dir, manifest_name), "r") as f:
+                with open(os.path.join(addon_dir, manifest_name)) as f:
                     manifest_string = f.read()
                     return ast.literal_eval(manifest_string)
         raise ValidationError(
             _("No manifest found in %(addon_dir)s") % {"addon_dir": addon_dir}
         )
 
     @api.model
@@ -170,15 +170,15 @@
             if not manifest.get(key):
                 continue
             for xml_file in manifest[key]:
                 if not xml_file.lower().endswith(".xml"):
                     continue
                 parts = xml_file.split("/")
                 try:
-                    with open(os.path.join(addon_dir, *parts), "r") as xml_handle:
+                    with open(os.path.join(addon_dir, *parts)) as xml_handle:
                         files.append(xml_handle.read())
                 except UnicodeDecodeError:
                     _logger.warning(
                         "Encoding error: Unable to read %s",
                         os.path.join(addon_dir, *parts),
                     )
                     continue
```

## odoo/addons/upgrade_analysis/odoo_patch/odoo_patch.py

```diff
@@ -1,13 +1,13 @@
 import logging
 
 _logger = logging.getLogger(__name__)
 
 
-class OdooPatch(object):
+class OdooPatch:
     """Simple mechanism to apply a collection of monkeypatches using a
     context manager.
 
     Classes can register their monkeypatches by inheriting from this class.
     They need to define a `target` member, referring to the object or module
     that needs to be patched, and a list `method_names`. They also need to
     redefine those methods under the same name.
```

## odoo/addons/upgrade_analysis/odoo_patch/addons/__init__.py

```diff
@@ -1,4 +1,3 @@
 from . import mrp
 from . import point_of_sale
-from . import sale_quotation_builder
 from . import stock
```

## odoo/addons/upgrade_analysis/odoo_patch/odoo/models.py

```diff
@@ -13,11 +13,11 @@
         """Log data ids that are imported with `load`"""
         current_module = self.env.context["module"]
         for res in BaseModelPatch._convert_records._original_method(
             self, records, log=log
         ):
             _id, xid, _record, _info = res
             if xid:
-                xid = xid if "." in xid else "{}.{}".format(current_module, xid)
+                xid = xid if "." in xid else f"{current_module}.{xid}"
                 upgrade_log.log_xml_id(self.env.cr, current_module, xid)
 
             yield res
```

## odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/ir_model.py

```diff
@@ -19,22 +19,24 @@
             constraint[0]: cls._module
             for cls in reversed(type(model).mro())
             if not getattr(cls, "pool", None)
             for constraint in getattr(cls, "_local_sql_constraints", ())
         }
 
         data_list = []
-        for (key, definition, message) in model._sql_constraints:
-            conname = "%s_%s" % (model._table, key)
+        for key, definition, message in model._sql_constraints:
+            conname = f"{model._table}_{key}"
             module = constraint_module.get(key)
             record = self._reflect_constraint(
                 model, conname, "u", cons_text(definition), module, message
             )
             if record:
-                xml_id = "%s.constraint_%s" % (module, conname)
+                xml_id = f"{module}.constraint_{conname}"
                 data_list.append(dict(xml_id=xml_id, record=record))
-
-        self.env["ir.model.data"]._update_xmlids(data_list)
-        for data in data_list:
-            xml_id = data.get("xml_id")
-            module = xml_id.split(".")[0]
-            upgrade_log.log_xml_id(self.env.cr, module, xml_id)
+        if data_list:
+            self.env["ir.model.data"]._update_xmlids(data_list)
+            # Begin OpenUpgrade addition
+            for data in data_list:
+                xml_id = data.get("xml_id")
+                module = xml_id.split(".")[0]
+                upgrade_log.log_xml_id(self.env.cr, module, xml_id)
+            # End OpenUpgrade addition
```

## odoo/addons/upgrade_analysis/static/description/index.html

```diff
@@ -362,19 +362,28 @@
 <div class="document" id="upgrade-analysis">
 <h1 class="title">Upgrade Analysis</h1>
 
 <!-- !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 !! This file is generated by oca-gen-addon-readme !!
 !! changes will be overwritten.                   !!
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-!! source digest: sha256:47c0b46bc356790fb4c33f1147128f376d0f640d2015589cbae86ec0fdeb3e13
+!! source digest: sha256:f5ec0738486de2c0128f10e4029e18956d4e92509fae8f60ed8c810097220dfe
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! -->
-<p><a class="reference external image-reference" href="https://odoo-community.org/page/development-status"><img alt="Beta" src="https://img.shields.io/badge/maturity-Beta-yellow.png" /></a> <a class="reference external image-reference" href="http://www.gnu.org/licenses/agpl-3.0-standalone.html"><img alt="License: AGPL-3" src="https://img.shields.io/badge/licence-AGPL--3-blue.png" /></a> <a class="reference external image-reference" href="https://github.com/OCA/server-tools/tree/16.0/upgrade_analysis"><img alt="OCA/server-tools" src="https://img.shields.io/badge/github-OCA%2Fserver--tools-lightgray.png?logo=github" /></a> <a class="reference external image-reference" href="https://translation.odoo-community.org/projects/server-tools-16-0/server-tools-16-0-upgrade_analysis"><img alt="Translate me on Weblate" src="https://img.shields.io/badge/weblate-Translate%20me-F47D42.png" /></a> <a class="reference external image-reference" href="https://runboat.odoo-community.org/builds?repo=OCA/server-tools&amp;target_branch=16.0"><img alt="Try me on Runboat" src="https://img.shields.io/badge/runboat-Try%20me-875A7B.png" /></a></p>
-<p>This module provides the tool to generate the database analysis files that indicate how the Odoo data model and module data have changed between two versions of Odoo. Database analysis files for the core modules are included in the OpenUpgrade distribution so as a migration script developer you will not usually need to use this tool yourself. If you do need to run your analysis of a custom set of modules, please refer to the documentation here: <a class="reference external" href="https://doc.therp.nl/openupgrade/analysis.html">https://doc.therp.nl/openupgrade/analysis.html</a></p>
-<p>This module is just a tool, a continuation of the old openupgrade_records in OpenUpgrade in previous versions. It’s not recommended to have this module in a production database.</p>
+<p><a class="reference external image-reference" href="https://odoo-community.org/page/development-status"><img alt="Beta" src="https://img.shields.io/badge/maturity-Beta-yellow.png" /></a> <a class="reference external image-reference" href="http://www.gnu.org/licenses/agpl-3.0-standalone.html"><img alt="License: AGPL-3" src="https://img.shields.io/badge/licence-AGPL--3-blue.png" /></a> <a class="reference external image-reference" href="https://github.com/OCA/server-tools/tree/17.0/upgrade_analysis"><img alt="OCA/server-tools" src="https://img.shields.io/badge/github-OCA%2Fserver--tools-lightgray.png?logo=github" /></a> <a class="reference external image-reference" href="https://translation.odoo-community.org/projects/server-tools-17-0/server-tools-17-0-upgrade_analysis"><img alt="Translate me on Weblate" src="https://img.shields.io/badge/weblate-Translate%20me-F47D42.png" /></a> <a class="reference external image-reference" href="https://runboat.odoo-community.org/builds?repo=OCA/server-tools&amp;target_branch=17.0"><img alt="Try me on Runboat" src="https://img.shields.io/badge/runboat-Try%20me-875A7B.png" /></a></p>
+<p>This module provides the tool to generate the database analysis files
+that indicate how the Odoo data model and module data have changed
+between two versions of Odoo. Database analysis files for the core
+modules are included in the OpenUpgrade distribution so as a migration
+script developer you will not usually need to use this tool yourself. If
+you do need to run your analysis of a custom set of modules, please
+refer to the documentation here:
+<a class="reference external" href="https://doc.therp.nl/openupgrade/analysis.html">https://doc.therp.nl/openupgrade/analysis.html</a></p>
+<p>This module is just a tool, a continuation of the old
+openupgrade_records in OpenUpgrade in previous versions. It’s not
+recommended to have this module in a production database.</p>
 <p><strong>Table of contents</strong></p>
 <div class="contents local topic" id="contents">
 <ul class="simple">
 <li><a class="reference internal" href="#usage" id="toc-entry-1">Usage</a></li>
 <li><a class="reference internal" href="#known-issues-roadmap" id="toc-entry-2">Known issues / Roadmap</a></li>
 <li><a class="reference internal" href="#bug-tracker" id="toc-entry-3">Bug Tracker</a></li>
 <li><a class="reference internal" href="#credits" id="toc-entry-4">Credits</a><ul>
@@ -390,23 +399,25 @@
 <p><a class="reference external" href="https://oca.github.io/OpenUpgrade/analyse.html">Usage instructions</a></p>
 </div>
 <div class="section" id="known-issues-roadmap">
 <h1><a class="toc-backref" href="#toc-entry-2">Known issues / Roadmap</a></h1>
 <ul class="simple">
 <li>Log removed modules in the module that owned them (#468)</li>
 <li>Detect renamed many2many tables (#213)</li>
-<li>Make sure that the <tt class="docutils literal">migration_analysis.txt</tt> file is always generated in all cases. (See: <a class="reference external" href="https://github.com/OCA/OpenUpgrade/pull/3209#issuecomment-1157449981">https://github.com/OCA/OpenUpgrade/pull/3209#issuecomment-1157449981</a>)</li>
+<li>Make sure that the <tt class="docutils literal">migration_analysis.txt</tt> file is always
+generated in all cases. (See:
+<a class="reference external" href="https://github.com/OCA/OpenUpgrade/pull/3209#issuecomment-1157449981">https://github.com/OCA/OpenUpgrade/pull/3209#issuecomment-1157449981</a>)</li>
 </ul>
 </div>
 <div class="section" id="bug-tracker">
 <h1><a class="toc-backref" href="#toc-entry-3">Bug Tracker</a></h1>
 <p>Bugs are tracked on <a class="reference external" href="https://github.com/OCA/server-tools/issues">GitHub Issues</a>.
 In case of trouble, please check there if your issue has already been reported.
 If you spotted it first, help us to smash it by providing a detailed and welcomed
-<a class="reference external" href="https://github.com/OCA/server-tools/issues/new?body=module:%20upgrade_analysis%0Aversion:%2016.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**">feedback</a>.</p>
+<a class="reference external" href="https://github.com/OCA/server-tools/issues/new?body=module:%20upgrade_analysis%0Aversion:%2017.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**">feedback</a>.</p>
 <p>Do not contact contributors directly about support or help with technical issues.</p>
 </div>
 <div class="section" id="credits">
 <h1><a class="toc-backref" href="#toc-entry-4">Credits</a></h1>
 <div class="section" id="authors">
 <h2><a class="toc-backref" href="#toc-entry-5">Authors</a></h2>
 <ul class="simple">
@@ -432,14 +443,14 @@
 <p>This module is maintained by the OCA.</p>
 <a class="reference external image-reference" href="https://odoo-community.org"><img alt="Odoo Community Association" src="https://odoo-community.org/logo.png" /></a>
 <p>OCA, or the Odoo Community Association, is a nonprofit organization whose
 mission is to support the collaborative development of Odoo features and
 promote its widespread use.</p>
 <p>Current <a class="reference external" href="https://odoo-community.org/page/maintainer-role">maintainers</a>:</p>
 <p><a class="reference external image-reference" href="https://github.com/StefanRijnhart"><img alt="StefanRijnhart" src="https://github.com/StefanRijnhart.png?size=40px" /></a> <a class="reference external image-reference" href="https://github.com/legalsylvain"><img alt="legalsylvain" src="https://github.com/legalsylvain.png?size=40px" /></a></p>
-<p>This module is part of the <a class="reference external" href="https://github.com/OCA/server-tools/tree/16.0/upgrade_analysis">OCA/server-tools</a> project on GitHub.</p>
+<p>This module is part of the <a class="reference external" href="https://github.com/OCA/server-tools/tree/17.0/upgrade_analysis">OCA/server-tools</a> project on GitHub.</p>
 <p>You are welcome to contribute. To learn how please visit <a class="reference external" href="https://odoo-community.org/page/Contribute">https://odoo-community.org/page/Contribute</a>.</p>
 </div>
 </div>
 </div>
 </body>
 </html>
```

## odoo/addons/upgrade_analysis/static/src/module_coverage_template.rst.mako

```diff
@@ -1,12 +1,12 @@
 Module coverage ${start_version} -> ${end_version}
 ============================
 
 .. include:: coverage_legend.rst
 
-+-------------------------------------------------+----------------------+-------------------------------------------------+
-| Module                                          | Status               + Extra Information                               |
-+=================================================+======================+=================================================+
++---------------------------------------------------+----------------------+-------------------------------------------------+
+| Module                                            | Status               + Extra Information                               |
++===================================================+======================+=================================================+
 % for module, extra_information in module_descriptions.items():
 |${module}|                      |${extra_information}|
-+-------------------------------------------------+----------------------+-------------------------------------------------+
++---------------------------------------------------+----------------------+-------------------------------------------------+
 % endfor
```

## odoo/addons/upgrade_analysis/views/view_upgrade_analysis.xml

### odoo/addons/upgrade_analysis/views/view_upgrade_analysis.xml

```diff
@@ -15,22 +15,22 @@
     <field name="arch" type="xml">
       <form create="false">
         <header>
           <field name="state" widget="statusbar"/>
           <button name="analyze" string="Perform Analysis" type="object" icon="fa-cogs" colspan="2"/>
         </header>
         <sheet>
-          <group col="4" colspan="4">
-            <field name="config_id" attrs="{'readonly': [('state', '=', 'done')]}"/>
-            <field name="write_files" attrs="{'readonly': [('state', '=', 'done')]}"/>
-            <field name="upgrade_path" attrs="{'invisible': [('write_files', '=', False)]}"/>
-            <field name="analysis_date" attrs="{'invisible': [('analysis_date', '=', False)]}"/>
+          <group>
+            <field name="config_id" readonly="state == 'done'"/>
+            <field name="write_files" readonly="state == 'done'"/>
+            <field name="upgrade_path" invisible="not write_files"/>
+            <field name="analysis_date" invisible="not analysis_date"/>
           </group>
           <group string="Log">
-            <field name="log" nolabel="1" widget="ace" options="{'mode': 'txt'}"/>
+            <field name="log" nolabel="1" widget="ace" options="{'mode': 'txt'}" colspan="2"/>
           </group>
         </sheet>
       </form>
     </field>
   </record>
   <record id="action_upgrade_analysis_tree" model="ir.actions.act_window">
     <field name="name">Upgrade Analyses</field>
```

## odoo/addons/upgrade_analysis/views/view_upgrade_record.xml

### odoo/addons/upgrade_analysis/views/view_upgrade_record.xml

```diff
@@ -29,24 +29,24 @@
     </field>
   </record>
   <record id="view_upgrade_record_form" model="ir.ui.view">
     <field name="model">upgrade.record</field>
     <field name="arch" type="xml">
       <form>
         <sheet>
-          <group col="4" colspan="4">
+          <group>
             <field name="name"/>
             <field name="module"/>
             <field name="model"/>
             <field name="field"/>
             <field name="type"/>
             <field name="mode"/>
           </group>
           <group string="Attributes">
-            <field name="attribute_ids" nolabel="1" colspan="4">
+            <field name="attribute_ids" nolabel="1" colspan="2">
               <tree>
                 <field name="name"/>
                 <field name="value"/>
               </tree>
             </field>
           </group>
         </sheet>
```

## odoo/addons/upgrade_analysis/wizards/upgrade_install_wizard.py

```diff
@@ -20,14 +20,15 @@
     state = fields.Selection(
         [("draft", "Draft"), ("done", "Done")], readonly=True, default="draft"
     )
 
     module_ids = fields.Many2many(
         comodel_name="ir.module.module",
         domain=lambda x: x._module_ids_domain(),
+        string="Modules",
     )
 
     module_qty = fields.Integer(
         string="Modules Quantity", compute="_compute_module_qty"
     )
 
     @api.model
```

## odoo/addons/upgrade_analysis/wizards/view_upgrade_generate_record_wizard.xml

### odoo/addons/upgrade_analysis/wizards/view_upgrade_generate_record_wizard.xml

```diff
@@ -3,22 +3,23 @@
   <record id="view_upgrade_generate_record_wizard_form" model="ir.ui.view">
     <field name="model">upgrade.generate.record.wizard</field>
     <field name="arch" type="xml">
       <form>
         <header>
           <field name="state" widget="statusbar"/>
         </header>
-        <group states="draft" colspan="4">
-          <p>This will reinitialize all the modules installed on this database. Do not continue if you use this database in production.</p>
+        <group invisible="state != 'draft'">
+          <p colspan="2">This will reinitialize all the modules installed on this database. Do not continue if you use this database in production.</p>
         </group>
-        <group states="done" colspan="4">
+        <group invisible="state != 'done'">
           <p>Modules initialized and record created</p>
+          <p colspan="2">Modules initialized and record created</p>
         </group>
         <footer>
-          <button string="Continue" name="generate" type="object" states="draft" class="btn-primary"/>
+          <button string="Continue" name="generate" type="object" invisible="state != 'draft'" class="btn-primary"/>
           <button special="cancel" string="Close" class="btn-default"/>
         </footer>
       </form>
     </field>
   </record>
   <record id="action_upgrade_generate_record_wizard" model="ir.actions.act_window">
     <field name="name">Generate Records Wizard</field>
```

## odoo/addons/upgrade_analysis/wizards/view_upgrade_install_wizard.xml

### odoo/addons/upgrade_analysis/wizards/view_upgrade_install_wizard.xml

```diff
@@ -3,33 +3,33 @@
   <record id="view_upgrade_install_wizard_form" model="ir.ui.view">
     <field name="model">upgrade.install.wizard</field>
     <field name="arch" type="xml">
       <form>
         <header>
           <field name="state" widget="statusbar"/>
         </header>
-        <group states="draft">
-          <p class="alert alert-warning" role="alert">This will install the selected modules on the database. Do not continue if you use this database in production.</p>
+        <group invisible="state != 'draft'">
+          <p class="alert alert-warning" role="alert" colspan="2">This will install the selected modules on the database. Do not continue if you use this database in production.</p>
         </group>
-        <group states="done">
-          <p class="alert alert-info" role="alert">The modules have been installed successfuly</p>
+        <group invisible="state != 'done'">
+          <p class="alert alert-info" role="alert" colspan="2">The modules have been installed successfuly</p>
         </group>
-        <group col="4" states="draft">
+        <header invisible="state != 'draft'">
           <button name="select_installable_modules" type="object" string="All Modules"/>
           <button name="select_odoo_modules" type="object" string="All Odoo SA Modules" class="btn-primary"/>
           <button name="select_oca_modules" type="object" string="All OCA Modules"/>
           <button name="select_other_modules" type="object" string="All Other Modules"/>
-        </group>
-        <group states="draft">
+        </header>
+        <button name="unselect_modules" type="object" string="Clear the list" invisible="state != 'draft'"/>
+        <group invisible="state != 'draft'">
           <field name="module_qty"/>
           <field name="module_ids" widget="many2many_tags" options="{'no_create': True}"/>
-          <button name="unselect_modules" type="object" string="Clear the list"/>
         </group>
         <footer>
-          <button name="install_modules" type="object" class="btn-primary" string="Install Modules" states="draft"/>
+          <button name="install_modules" type="object" class="btn-primary" string="Install Modules" invisible="state != 'draft'"/>
           <button special="cancel" string="Close" class="btn-default"/>
         </footer>
       </form>
     </field>
   </record>
   <record id="action_upgrade_install_wizard" model="ir.actions.act_window">
     <field name="name">Install Modules Wizard</field>
```

## Comparing `odoo/addons/upgrade_analysis/readme/DESCRIPTION.rst` & `odoo/addons/upgrade_analysis/readme/DESCRIPTION.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,3 +1,12 @@
-This module provides the tool to generate the database analysis files that indicate how the Odoo data model and module data have changed between two versions of Odoo. Database analysis files for the core modules are included in the OpenUpgrade distribution so as a migration script developer you will not usually need to use this tool yourself. If you do need to run your analysis of a custom set of modules, please refer to the documentation here: https://doc.therp.nl/openupgrade/analysis.html
+This module provides the tool to generate the database analysis files
+that indicate how the Odoo data model and module data have changed
+between two versions of Odoo. Database analysis files for the core
+modules are included in the OpenUpgrade distribution so as a migration
+script developer you will not usually need to use this tool yourself. If
+you do need to run your analysis of a custom set of modules, please
+refer to the documentation here:
+<https://doc.therp.nl/openupgrade/analysis.html>
 
-This module is just a tool, a continuation of the old openupgrade_records in OpenUpgrade in previous versions. It's not recommended to have this module in a production database.
+This module is just a tool, a continuation of the old
+openupgrade_records in OpenUpgrade in previous versions. It's not
+recommended to have this module in a production database.
```

## Comparing `odoo_addon_upgrade_analysis-16.0.1.0.2.dist-info/METADATA` & `odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,111 +1,121 @@
 Metadata-Version: 2.1
-Name: odoo-addon-upgrade-analysis
-Version: 16.0.1.0.2
+Name: odoo-addon-upgrade_analysis
+Version: 17.0.1.0.0.6
+Requires-Python: >=3.10
+Requires-Dist: dataclasses
+Requires-Dist: mako
+Requires-Dist: odoo>=17.0a,<17.1dev
+Requires-Dist: odoorpc
+Requires-Dist: openupgradelib
 Summary: Performs a difference analysis between modules installed on two different Odoo instances
 Home-page: https://github.com/OCA/server-tools
+License: AGPL-3
 Author: Therp BV, Opener B.V., GRAP, Odoo Community Association (OCA)
 Author-email: support@odoo-community.org
-License: AGPL-3
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
-Classifier: Framework :: Odoo :: 16.0
+Classifier: Framework :: Odoo :: 17.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Requires-Python: >=3.10
-Requires-Dist: dataclasses
-Requires-Dist: mako
-Requires-Dist: odoo <16.1dev,>=16.0a
-Requires-Dist: odoorpc
-Requires-Dist: openupgradelib
 
 ================
 Upgrade Analysis
 ================
 
 .. 
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
    !! This file is generated by oca-gen-addon-readme !!
    !! changes will be overwritten.                   !!
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-   !! source digest: sha256:47c0b46bc356790fb4c33f1147128f376d0f640d2015589cbae86ec0fdeb3e13
+   !! source digest: sha256:f5ec0738486de2c0128f10e4029e18956d4e92509fae8f60ed8c810097220dfe
    !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 
 .. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: Beta
 .. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 .. |badge3| image:: https://img.shields.io/badge/github-OCA%2Fserver--tools-lightgray.png?logo=github
-    :target: https://github.com/OCA/server-tools/tree/16.0/upgrade_analysis
+    :target: https://github.com/OCA/server-tools/tree/17.0/upgrade_analysis
     :alt: OCA/server-tools
 .. |badge4| image:: https://img.shields.io/badge/weblate-Translate%20me-F47D42.png
-    :target: https://translation.odoo-community.org/projects/server-tools-16-0/server-tools-16-0-upgrade_analysis
+    :target: https://translation.odoo-community.org/projects/server-tools-17-0/server-tools-17-0-upgrade_analysis
     :alt: Translate me on Weblate
 .. |badge5| image:: https://img.shields.io/badge/runboat-Try%20me-875A7B.png
-    :target: https://runboat.odoo-community.org/builds?repo=OCA/server-tools&target_branch=16.0
+    :target: https://runboat.odoo-community.org/builds?repo=OCA/server-tools&target_branch=17.0
     :alt: Try me on Runboat
 
 |badge1| |badge2| |badge3| |badge4| |badge5|
 
-This module provides the tool to generate the database analysis files that indicate how the Odoo data model and module data have changed between two versions of Odoo. Database analysis files for the core modules are included in the OpenUpgrade distribution so as a migration script developer you will not usually need to use this tool yourself. If you do need to run your analysis of a custom set of modules, please refer to the documentation here: https://doc.therp.nl/openupgrade/analysis.html
-
-This module is just a tool, a continuation of the old openupgrade_records in OpenUpgrade in previous versions. It's not recommended to have this module in a production database.
+This module provides the tool to generate the database analysis files
+that indicate how the Odoo data model and module data have changed
+between two versions of Odoo. Database analysis files for the core
+modules are included in the OpenUpgrade distribution so as a migration
+script developer you will not usually need to use this tool yourself. If
+you do need to run your analysis of a custom set of modules, please
+refer to the documentation here:
+https://doc.therp.nl/openupgrade/analysis.html
+
+This module is just a tool, a continuation of the old
+openupgrade_records in OpenUpgrade in previous versions. It's not
+recommended to have this module in a production database.
 
 **Table of contents**
 
 .. contents::
    :local:
 
 Usage
 =====
 
-`Usage instructions <https://oca.github.io/OpenUpgrade/analyse.html>`_
+`Usage instructions <https://oca.github.io/OpenUpgrade/analyse.html>`__
 
 Known issues / Roadmap
 ======================
 
-* Log removed modules in the module that owned them (#468)
-* Detect renamed many2many tables (#213)
-* Make sure that the ``migration_analysis.txt`` file is always generated in all cases. (See: https://github.com/OCA/OpenUpgrade/pull/3209#issuecomment-1157449981)
+-  Log removed modules in the module that owned them (#468)
+-  Detect renamed many2many tables (#213)
+-  Make sure that the ``migration_analysis.txt`` file is always
+   generated in all cases. (See:
+   https://github.com/OCA/OpenUpgrade/pull/3209#issuecomment-1157449981)
 
 Bug Tracker
 ===========
 
 Bugs are tracked on `GitHub Issues <https://github.com/OCA/server-tools/issues>`_.
 In case of trouble, please check there if your issue has already been reported.
 If you spotted it first, help us to smash it by providing a detailed and welcomed
-`feedback <https://github.com/OCA/server-tools/issues/new?body=module:%20upgrade_analysis%0Aversion:%2016.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.
+`feedback <https://github.com/OCA/server-tools/issues/new?body=module:%20upgrade_analysis%0Aversion:%2017.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.
 
 Do not contact contributors directly about support or help with technical issues.
 
 Credits
 =======
 
 Authors
-~~~~~~~
+-------
 
 * Therp BV
 * Opener B.V.
 * GRAP
 
 Contributors
-~~~~~~~~~~~~
+------------
 
-* Stefan Rijnhart <stefan@opener.amsterdam>
-* Holger Brunn <hbrunn@therp.nl>
-* Pedro M. Baeza <pedro.baeza@gmail.com>
-* Ferdinand Gassauer <gass@cc-l-12.chircar.at>
-* Florent Xicluna <florent.xicluna@gmail.com>
-* Miquel Raïch <miquel.raich@forgeflow.com>
-* Sylvain LE GAL <https://twitter.com/legalsylvain>
+-  Stefan Rijnhart <stefan@opener.amsterdam>
+-  Holger Brunn <hbrunn@therp.nl>
+-  Pedro M. Baeza <pedro.baeza@gmail.com>
+-  Ferdinand Gassauer <gass@cc-l-12.chircar.at>
+-  Florent Xicluna <florent.xicluna@gmail.com>
+-  Miquel Raïch <miquel.raich@forgeflow.com>
+-  Sylvain LE GAL <https://twitter.com/legalsylvain>
 
 Maintainers
-~~~~~~~~~~~
+-----------
 
 This module is maintained by the OCA.
 
 .. image:: https://odoo-community.org/logo.png
    :alt: Odoo Community Association
    :target: https://odoo-community.org
 
@@ -120,12 +130,10 @@
     :target: https://github.com/legalsylvain
     :alt: legalsylvain
 
 Current `maintainers <https://odoo-community.org/page/maintainer-role>`__:
 
 |maintainer-StefanRijnhart| |maintainer-legalsylvain| 
 
-This module is part of the `OCA/server-tools <https://github.com/OCA/server-tools/tree/16.0/upgrade_analysis>`_ project on GitHub.
+This module is part of the `OCA/server-tools <https://github.com/OCA/server-tools/tree/17.0/upgrade_analysis>`_ project on GitHub.
 
 You are welcome to contribute. To learn how please visit https://odoo-community.org/page/Contribute.
-
-
```

## Comparing `odoo_addon_upgrade_analysis-16.0.1.0.2.dist-info/RECORD` & `odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,54 @@
-odoo/addons/upgrade_analysis/README.rst,sha256=TIiJHJyuA4EFhJK63dW5jHCIx-V-epDkCb7uaDbjjpg,4561
+odoo/addons/upgrade_analysis/README.rst,sha256=tn0jBATwQt-CmUTv6MpAQikvbDL29B0hHqy5Ea6okLI,4578
 odoo/addons/upgrade_analysis/__init__.py,sha256=1X8E6viDvX9QCI3au33OFkjFkJbFw6TazruSkrDurdI,140
-odoo/addons/upgrade_analysis/__manifest__.py,sha256=q8J6kN82HN8uow6PPysAFD7Mywfb0O3CFhji7PWubos,1077
-odoo/addons/upgrade_analysis/blacklist.py,sha256=BIu8cYUB6j3FYtSaRcs4nSxB6yUwyjhxzOaex1AiIHY,362
-odoo/addons/upgrade_analysis/compare.py,sha256=XSetlfvLS0LBy9nI5kF1gcneaaMo7kjd2uAwPz4KSoQ,20132
-odoo/addons/upgrade_analysis/upgrade_log.py,sha256=aUeWhlnpxJIF5lgHoLfbZTlqHpgXcK-GNsYs92IidGw,8297
+odoo/addons/upgrade_analysis/__manifest__.py,sha256=2TPFpeXvDNcWJ1V1EZyc6kNVAKu-7ZIwIKiBW4jiyXY,1077
+odoo/addons/upgrade_analysis/blacklist.py,sha256=h2b5VsBPF0Z6imWpZme37xZE-m0nmRdpzUbTWHW7u3E,456
+odoo/addons/upgrade_analysis/compare.py,sha256=r8S_JEwZFYwYqtS0AKK_c7jizG6Kg6fmSrspn0kafug,19987
+odoo/addons/upgrade_analysis/upgrade_log.py,sha256=POS59R1IbnrrMvKzWpcz1yNW_5oQ0skIhc6pDh8nruw,8286
 odoo/addons/upgrade_analysis/i18n/es_AR.po,sha256=fHZ_DD9rAwE5ecWSzlX3WMep0t3FG3I7Qsqnchq5f2Y,22496
 odoo/addons/upgrade_analysis/i18n/fr.po,sha256=uzNf1Vqaxcu3y6-CHg_IXUPFdNg6DHVOAB3mR75VDaY,20161
-odoo/addons/upgrade_analysis/i18n/upgrade_analysis.pot,sha256=oudXK6RkCZ2S6B3aoy7Mxf4moyBC8sJVYV8P8Rb6i6I,19925
+odoo/addons/upgrade_analysis/i18n/upgrade_analysis.pot,sha256=Hx2KXpgfF4Ui2Aj5W8_vZC9w5AMgRw5I8njKi4teWJE,18533
 odoo/addons/upgrade_analysis/models/__init__.py,sha256=V3z7qRHAST0ArkG6eGCgABdDHniOvY7Mcna8I4M5duk,163
 odoo/addons/upgrade_analysis/models/ir_module_module.py,sha256=Wy2bfWlulZ-ucpxh6flDgGcvCPBpeL1TztPCxW1x-9U,1031
-odoo/addons/upgrade_analysis/models/upgrade_analysis.py,sha256=6UBaqInIMil8iw9ZDiu9-qNLetFDxYwe6_UyxxEQ1u4,22546
+odoo/addons/upgrade_analysis/models/upgrade_analysis.py,sha256=nBDMvRAswBm283i9Ff5CHDuO74aIxJYNtu8sfl_zNO4,22565
 odoo/addons/upgrade_analysis/models/upgrade_attribute.py,sha256=j2K_dqArvAHThW51VWhiNSiyoy9g5BnPS01khhaaovw,536
 odoo/addons/upgrade_analysis/models/upgrade_comparison_config.py,sha256=2v-0S5vXoFZsL7e-wXlHdWdf3j5v222pYK5kKcbLCmk,3098
-odoo/addons/upgrade_analysis/models/upgrade_record.py,sha256=-z1YaxulCLJPD4Y6RgkHpndmoe3J9ytllKo1qFxBvyk,6006
+odoo/addons/upgrade_analysis/models/upgrade_record.py,sha256=dAtwYng98TJJclE04KMwMd2nuGMbEZMuQvGnXcABHV0,5998
 odoo/addons/upgrade_analysis/odoo_patch/__init__.py,sha256=dd3BGgBnbgdu740xmYrIfYX8F-S42Ia4m_JDFX5HHqA,65
-odoo/addons/upgrade_analysis/odoo_patch/odoo_patch.py,sha256=T3wGLqu3DtZPIFfwP9mVnZF1DbxkFryIYKc6bvDPLxA,1843
-odoo/addons/upgrade_analysis/odoo_patch/addons/__init__.py,sha256=sRS5k6qUboeeWteCHodbzgbGqrlPbG6EcDHMBnoEKnA,103
+odoo/addons/upgrade_analysis/odoo_patch/odoo_patch.py,sha256=bIScQP3UQAtOYnfPFNgkPOq6BIWh38nP-3AWiKhtXb8,1835
+odoo/addons/upgrade_analysis/odoo_patch/addons/__init__.py,sha256=k0e3fJGVpOVcCXMHcf2VcHNFcm6WU-mxcNDDdgTXyzc,66
 odoo/addons/upgrade_analysis/odoo_patch/addons/mrp/__init__.py,sha256=P3m4WfcD9qDPmFPiyKDjbEU-XcsqFQSoC9qKjKlJpm0,270
 odoo/addons/upgrade_analysis/odoo_patch/addons/point_of_sale/__init__.py,sha256=oM5n-sxc4Hl1l1Tm-pv6LVC19DMqYwznf4MXVl_K-Kg,371
-odoo/addons/upgrade_analysis/odoo_patch/addons/sale_quotation_builder/__init__.py,sha256=g2cNVF2vVkwFUmHM-hl3-lS22Rgj5MGc5NZAb7X_oTc,341
 odoo/addons/upgrade_analysis/odoo_patch/addons/stock/__init__.py,sha256=2QQ7l55w3aey4wynuOSx0ETZnG-Tz9u_B_EeDKSUmAg,259
 odoo/addons/upgrade_analysis/odoo_patch/odoo/__init__.py,sha256=P0ZkY7Ql1glqQNYEitW3cJFlD89_uz1Dg7FXW_QuSjE,84
-odoo/addons/upgrade_analysis/odoo_patch/odoo/models.py,sha256=BhN0_2AMJMI_PqmqnjTGTp2ZsJd-KC9zNSlB__YZrKI,739
+odoo/addons/upgrade_analysis/odoo_patch/odoo/models.py,sha256=LRAFdmyxHXyT1IgVQ_OgzcUEOWXwiUQ7xgdZkORgFkY,729
 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/__init__.py,sha256=9pIQnc7H3xgVNpi7n3I18hg04S4IkX5mnAfl9cv7RBE,19
 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/__init__.py,sha256=X9EJGOE2GtZbS0G82PtSXmWSZ_R8jEM0rlJTDliQjp4,21
 odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/__init__.py,sha256=V8hR-ja8zu7sRkJuB9_inZfZFWYcwxeQvG6GVWyN_yg,23
-odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/ir_model.py,sha256=w28WshZ2DEcHec555-r6uBqOii75aklfqSBirDOPjdI,1482
+odoo/addons/upgrade_analysis/odoo_patch/odoo/addons/base/models/ir_model.py,sha256=SajOomrzwsGPx0rUFhLUS8YhIXM98pdvziC-wbR2tVk,1589
 odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/__init__.py,sha256=ZMVa5M4OJIjWngqfYFqhva1pLHhv-TrO-FUtSs7Zwzs,23
 odoo/addons/upgrade_analysis/odoo_patch/odoo/modules/registry.py,sha256=VpujgZkFhccw0iVIIsMc85mnlXspUQf-sEgNaYo_Y3g,1112
 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/__init__.py,sha256=zJUx6tg2hBfTh6fQkU4JtHhC_0WRgfr81PIVua4SMA0,22
 odoo/addons/upgrade_analysis/odoo_patch/odoo/tools/convert.py,sha256=LinbMWmbr_G8KMfaNLyQAIL71thuH7YlSLCFGrNBrFk,397
-odoo/addons/upgrade_analysis/readme/CONTRIBUTORS.rst,sha256=40ZZbhFjmQBvBE1i_ISe1pQBFrDt7o-0i22_XsG2aaU,308
-odoo/addons/upgrade_analysis/readme/DESCRIPTION.rst,sha256=fTmsisjHxmm9Q5XjYJzS2I0C89_tHb6xlKv4HPbFf3o,675
-odoo/addons/upgrade_analysis/readme/ROADMAP.rst,sha256=sYjmNy1G_Ff37KIyZ1kqeLSPdQAG5xIEfrsU6kIaJbU,263
-odoo/addons/upgrade_analysis/readme/USAGE.rst,sha256=V8paWY9hBt0qz60d4UOVJRPtCiCR2aFxnCxRqwM7SiA,71
+odoo/addons/upgrade_analysis/readme/CONTRIBUTORS.md,sha256=u-jriLEBWR1ggHRLx_AlV_0d8-UUnRHIxOWa_Cxhf3Y,336
+odoo/addons/upgrade_analysis/readme/DESCRIPTION.md,sha256=NB1wxhB3b82i3WFxUfq1PheeXcrEzrvDiRGxbwNn7-4,677
+odoo/addons/upgrade_analysis/readme/ROADMAP.md,sha256=xNOwng8y76qNy5mQovxvuYL7tQgQ17S-5EZSNKPC7GA,267
+odoo/addons/upgrade_analysis/readme/USAGE.md,sha256=4I3nKlYKMMvrZQ03_34M4jaFERCPB5UqzY1mneHxy2U,69
 odoo/addons/upgrade_analysis/security/ir.model.access.csv,sha256=72UaOy9pjuAUMUICrj9cYpBBm65CbHSrn3WrgxNQ7Uc,696
 odoo/addons/upgrade_analysis/static/description/icon.png,sha256=6xBPJauaFOF0KDHfHgQopSc28kKvxMaeoQFQWZtfZDo,9455
-odoo/addons/upgrade_analysis/static/description/index.html,sha256=98QgN-Cou0bb-7L4sgYxWwbCiy1BbRJAiHJzxVH9iXE,15067
-odoo/addons/upgrade_analysis/static/src/module_coverage_template.rst.mako,sha256=Bs49LkFH1bxx_6FozpdPUEpiIx9tQz5SM-yUiw050ko,744
+odoo/addons/upgrade_analysis/static/description/index.html,sha256=cT9Wrl1hF8MIlpLhLkDSy_uKtVo46IlXh24cKRGRv9w,15067
+odoo/addons/upgrade_analysis/static/src/module_coverage_template.rst.mako,sha256=DndkkZW1buCqR_Gmt9F8iEmwFD96ztd5XUhDafWkosQ,752
 odoo/addons/upgrade_analysis/tests/__init__.py,sha256=vfUqzPeIroQ-zFgLEZ7RwslndWCR9eW87w3c0MD7mX4,26
 odoo/addons/upgrade_analysis/tests/test_module.py,sha256=RpSIlz7Hpu48MrN2CO0PSLP504NdaV6UNAgCQgGjYlk,1787
 odoo/addons/upgrade_analysis/views/menu.xml,sha256=Qz9pny7HLhLbkgIAPhIFN3NWgnrUwGlkMV4OFmt0DZE,200
-odoo/addons/upgrade_analysis/views/view_upgrade_analysis.xml,sha256=vSH9gJwVEFkxvDcDWnpPt_c2XG3nxcPOubjFgr4HzOc,2640
+odoo/addons/upgrade_analysis/views/view_upgrade_analysis.xml,sha256=5QnypjewfyqT8aITbIrOrvdDsAnQObjYkU1wgV0PhQI,2250
 odoo/addons/upgrade_analysis/views/view_upgrade_comparison_config.xml,sha256=pBTVmGOGkohO1tguxKFXAWGHkrSVJdok3jjuhERcGa4,2826
-odoo/addons/upgrade_analysis/views/view_upgrade_record.xml,sha256=oBxhlkz42bJxhrFMydpKpEDYt1sX0Z9WMipuA5Bpq2M,2834
+odoo/addons/upgrade_analysis/views/view_upgrade_record.xml,sha256=oH7i44cTERaDYRRQzcYUOtRvntBrhJJ9bxPdpl91L7k,2814
 odoo/addons/upgrade_analysis/wizards/__init__.py,sha256=6973yn8jkeAaHm-ofIILbHUCB6KQ7RUMSDCK0Xk18xE,82
 odoo/addons/upgrade_analysis/wizards/upgrade_generate_record_wizard.py,sha256=DTeLN_1rez_v82EA16H2Bsk4TGk9aA_n7Wn6_qQoKUE,4527
-odoo/addons/upgrade_analysis/wizards/upgrade_install_wizard.py,sha256=4g8E1EdR83R84hGVWHx45JVjnz8naQlBfvHNj5bNE6Q,4040
-odoo/addons/upgrade_analysis/wizards/view_upgrade_generate_record_wizard.xml,sha256=80IblSl5Jux1jYoh0bJGBJikNRk39HDgiRylMWPdkJo,1787
-odoo/addons/upgrade_analysis/wizards/view_upgrade_install_wizard.xml,sha256=_6uw3NVhdBp_gP5mybo--AI97n3_v6tIcyX2Z0WoCrE,3289
-odoo_addon_upgrade_analysis-16.0.1.0.2.dist-info/METADATA,sha256=dBHQwOSvv_e8fqi3BHt-Bz3U4K82YPdqSIg0vSxvUAQ,5278
-odoo_addon_upgrade_analysis-16.0.1.0.2.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-odoo_addon_upgrade_analysis-16.0.1.0.2.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo_addon_upgrade_analysis-16.0.1.0.2.dist-info/RECORD,,
+odoo/addons/upgrade_analysis/wizards/upgrade_install_wizard.py,sha256=ysFWUHxBYO4HKGO4SzwD_Tq0rNr9YUlUv73APpyfIto,4066
+odoo/addons/upgrade_analysis/wizards/view_upgrade_generate_record_wizard.xml,sha256=BUYgXSoebkDkezLQirUJIZbZxHuU3-gesUtOZ1eP00I,1919
+odoo/addons/upgrade_analysis/wizards/view_upgrade_install_wizard.xml,sha256=bKziKQUjgGfeXri_cj_0Vgkbj2M5I4IbX9xxlgoLEFI,3454
+odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/METADATA,sha256=oolP0nsBtOjHDi4kWyf1EIJWGq8tozU6qUMycl4kS3I,5276
+odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/WHEEL,sha256=8Rd4enx1PCuyDWP4SABqO5Fv8rpaknqp3VzjoFFLa6c,83
+odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/top_level.txt,sha256=QE6RBQ0QX5f4eFuUcGgU5Kbq1A_qJcDs-e_vpr6pmfU,4
+odoo_addon_upgrade_analysis-17.0.1.0.0.6.dist-info/RECORD,,
```

