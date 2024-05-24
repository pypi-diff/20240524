# Comparing `tmp/chemfusekit-1.1.0b3.tar.gz` & `tmp/chemfusekit-1.1.1b1.tar.gz`

## Comparing `chemfusekit-1.1.0b3.tar` & `chemfusekit-1.1.1b1.tar`

### file list

```diff
@@ -1,133 +1,133 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/.python-version
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/.releaserc.yml
--rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/CHANGELOG.md
--rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/cda_example_notebook.ipynb
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/requirements-dev.lock
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/requirements.lock
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/.github/workflows/gh_pages.yml
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/.github/workflows/release.yml
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/.github/workflows/thesis.yml
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/.github/workflows/unittest.yml
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/chemfusekit/__init__.py
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/chemfusekit/__utils.py
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/chemfusekit/knn.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/chemfusekit/lda.py
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/chemfusekit/lldf.py
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/chemfusekit/lr.py
--rw-r--r--   0        0        0     8825 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/chemfusekit/pca.py
--rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/chemfusekit/plsda.py
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/chemfusekit/svm.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/README.md
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/babel.config.js
--rw-r--r--   0        0        0     4025 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docusaurus.config.js
--rw-r--r--   0        0        0  1020872 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/package-lock.json
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/package.json
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/sidebars.js
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/complete-workflow.md
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/tutorial.md
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/knn/_category_.json
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/knn/knn.md
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/knn/knnsettings.md
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/lda/_category_.json
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/lda/lda.md
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/lda/ldasettings.md
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/lldf/_category_.json
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/lldf/lldf.md
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/lldf/lldfmodel.md
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/lldf/lldfsettings.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/lr/_category_.json
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/lr/lr.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/lr/lrsettings.md
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/pca/_category_.json
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/pca/pca.md
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/pca/pcasettings.md
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/plsda/_category_.json
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/plsda/plsda.md
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/plsda/plsdasettings.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/svm/_category_.json
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/svm/svm.md
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/docs/svm/svmsettings.md
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/src/components/HomepageFeatures/index.js
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/src/components/HomepageFeatures/styles.module.css
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/src/css/custom.css
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/src/pages/index.js
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/src/pages/index.module.css
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/src/pages/project.md
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/src/pages/project/continuous-integration.md
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/src/pages/project/process-model.md
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/src/pages/project/project-philosophy.md
--rw-r--r--   0        0        0    10945 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/src/pages/project/project-plan.md
--rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/src/pages/project/requirements-specification.md
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/src/pages/project/use-cases.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/static/.nojekyll
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/static/img/colab-logo.svg
--rw-r--r--   0        0        0    55746 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/static/img/docusaurus-social-card.jpg
--rw-r--r--   0        0        0    10723 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/static/img/docusaurus.png
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/static/img/favicon.ico
--rw-r--r--   0        0        0    23978 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/static/img/happy-woman.svg
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/static/img/logo.svg
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/docs/static/img/magnifying-glass.svg
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/Beartype.md
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/Constructors.md
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/Conventional Commits.md
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/Kanban.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/Logistic Regression.md
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/PCA-LR.md
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/PCA.md
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/PEP coding standards.md
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/SVM.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/To do.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/Use Case Diagram.md
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/kNN.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/.obsidian/app.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/.obsidian/appearance.json
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/.obsidian/community-plugins.json
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/.obsidian/core-plugins-migration.json
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/.obsidian/core-plugins.json
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/.obsidian/daily-notes.json
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/.obsidian/templates.json
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/.obsidian/workspace.json
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/.obsidian/plugins/calendar/data.json
--rw-r--r--   0        0        0   141498 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/.obsidian/plugins/calendar/main.js
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/.obsidian/plugins/calendar/manifest.json
--rw-r--r--   0        0        0   723669 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/.obsidian/plugins/obsidian-kanban/main.js
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/.obsidian/plugins/obsidian-kanban/manifest.json
--rw-r--r--   0        0        0    53515 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/.obsidian/plugins/obsidian-kanban/styles.css
--rw-r--r--   0        0        0   294758 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/.obsidian/plugins/obsidian-plantuml/main.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/.obsidian/plugins/obsidian-plantuml/manifest.json
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/.obsidian/plugins/obsidian-plantuml/styles.css
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/Devlog/2024-04-19.md
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/Devlog/2024-04-20.md
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/Devlog/2024-04-22.md
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/Devlog/2024-04-23.md
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/Devlog/2024-05-06.md
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/Devlog/2024-05-07.md
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/Devlog/2024-05-08.md
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/Devlog/2024-05-09.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/Devlog/2024-05-17.md
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/Devlog/2024-05-18.md
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/Templates/Daily devlog.md
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/UML/Components.md
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/UML/Process state machine.md
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/UML/Sequence.md
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/notes/UML/Use cases.md
--rw-r--r--   0        0        0   590311 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/tests/qepas.xlsx
--rw-r--r--   0        0        0    18770 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/tests/rt.xlsx
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/tests/test_knn.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/tests/test_lda.py
--rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/tests/test_lldf.py
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/tests/test_lr.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/tests/test_pca.py
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/tests/test_plsda.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/tests/test_svm.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/thesis/0-header.md
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/thesis/1-abstract.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/thesis/2-index.md.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/thesis/3-intro.md
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/thesis/999-ringraziamenti.md
--rw-r--r--   0        0        0    21285 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/thesis/logo-unibg.png
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/.gitignore
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/pyproject.toml
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/readme.md
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 chemfusekit-1.1.0b3/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/.python-version
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/.releaserc.yml
+-rw-r--r--   0        0        0     9311 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/CHANGELOG.md
+-rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/cda_example_notebook.ipynb
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/requirements-dev.lock
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/requirements.lock
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/.github/workflows/gh_pages.yml
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/.github/workflows/thesis.yml
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/chemfusekit/__init__.py
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/chemfusekit/__utils.py
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/chemfusekit/knn.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/chemfusekit/lda.py
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/chemfusekit/lldf.py
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/chemfusekit/lr.py
+-rw-r--r--   0        0        0     8825 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/chemfusekit/pca.py
+-rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/chemfusekit/plsda.py
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/chemfusekit/svm.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/README.md
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/babel.config.js
+-rw-r--r--   0        0        0     4025 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docusaurus.config.js
+-rw-r--r--   0        0        0  1020872 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/package-lock.json
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/package.json
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/sidebars.js
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/complete-workflow.md
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/tutorial.md
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/knn/_category_.json
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/knn/knn.md
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/knn/knnsettings.md
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/lda/_category_.json
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/lda/lda.md
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/lda/ldasettings.md
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/lldf/_category_.json
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/lldf/lldf.md
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/lldf/lldfmodel.md
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/lldf/lldfsettings.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/lr/_category_.json
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/lr/lr.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/lr/lrsettings.md
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/pca/_category_.json
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/pca/pca.md
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/pca/pcasettings.md
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/plsda/_category_.json
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/plsda/plsda.md
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/plsda/plsdasettings.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/svm/_category_.json
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/svm/svm.md
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/svm/svmsettings.md
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/components/HomepageFeatures/index.js
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/components/HomepageFeatures/styles.module.css
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/css/custom.css
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/pages/index.js
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/pages/index.module.css
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/pages/project.md
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/pages/project/continuous-integration.md
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/pages/project/process-model.md
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/pages/project/project-philosophy.md
+-rw-r--r--   0        0        0    10945 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/pages/project/project-plan.md
+-rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/pages/project/requirements-specification.md
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/pages/project/use-cases.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/static/.nojekyll
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/static/img/colab-logo.svg
+-rw-r--r--   0        0        0    55746 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/static/img/docusaurus-social-card.jpg
+-rw-r--r--   0        0        0    10723 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/static/img/docusaurus.png
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/static/img/favicon.ico
+-rw-r--r--   0        0        0    23978 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/static/img/happy-woman.svg
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/static/img/logo.svg
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/static/img/magnifying-glass.svg
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Beartype.md
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Constructors.md
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Conventional Commits.md
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Kanban.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Logistic Regression.md
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/PCA-LR.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/PCA.md
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/PEP coding standards.md
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/SVM.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/To do.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Use Case Diagram.md
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/kNN.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/app.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/appearance.json
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/community-plugins.json
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/core-plugins-migration.json
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/core-plugins.json
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/daily-notes.json
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/templates.json
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/workspace.json
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/plugins/calendar/data.json
+-rw-r--r--   0        0        0   141498 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/plugins/calendar/main.js
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/plugins/calendar/manifest.json
+-rw-r--r--   0        0        0   723669 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/plugins/obsidian-kanban/main.js
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/plugins/obsidian-kanban/manifest.json
+-rw-r--r--   0        0        0    53515 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/plugins/obsidian-kanban/styles.css
+-rw-r--r--   0        0        0   294758 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/plugins/obsidian-plantuml/main.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/plugins/obsidian-plantuml/manifest.json
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/plugins/obsidian-plantuml/styles.css
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Devlog/2024-04-19.md
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Devlog/2024-04-20.md
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Devlog/2024-04-22.md
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Devlog/2024-04-23.md
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Devlog/2024-05-06.md
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Devlog/2024-05-07.md
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Devlog/2024-05-08.md
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Devlog/2024-05-09.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Devlog/2024-05-17.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Devlog/2024-05-18.md
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Templates/Daily devlog.md
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/UML/Components.md
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/UML/Process state machine.md
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/UML/Sequence.md
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/UML/Use cases.md
+-rw-r--r--   0        0        0   590311 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/tests/qepas.xlsx
+-rw-r--r--   0        0        0    18770 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/tests/rt.xlsx
+-rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/tests/test_knn.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/tests/test_lda.py
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/tests/test_lldf.py
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/tests/test_lr.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/tests/test_pca.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/tests/test_plsda.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/tests/test_svm.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/thesis/0-header.md
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/thesis/1-abstract.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/thesis/2-index.md.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/thesis/3-intro.md
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/thesis/999-ringraziamenti.md
+-rw-r--r--   0        0        0    21285 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/thesis/logo-unibg.png
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/.gitignore
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/pyproject.toml
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/readme.md
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/PKG-INFO
```

### Comparing `chemfusekit-1.1.0b3/.releaserc.yml` & `chemfusekit-1.1.1b1/.releaserc.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/CHANGELOG.md` & `chemfusekit-1.1.1b1/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,51 @@
+## [1.1.1-beta.1](https://github.com/f-aguzzi/tesi/compare/v1.1.0...v1.1.1-beta.1) (2024-05-23)
+
+
+### Bug Fixes
+
+* wrong training procedure in SVM ([74d1741](https://github.com/f-aguzzi/tesi/commit/74d1741743f53eea6cc2d9002005c6426bf4f0d0))
+
+
+### CI
+
+* **release:** 1.1.0-beta.3 [skip ci] ([96988ac](https://github.com/f-aguzzi/tesi/commit/96988acbfd0f015c03385f74f14ea26e98a9b4b2))
+
 ## [1.1.0-beta.3](https://github.com/f-aguzzi/tesi/compare/v1.1.0-beta.2...v1.1.0-beta.3) (2024-05-23)
 
 
+### Features
+
+* beartype integration ([2f823ce](https://github.com/f-aguzzi/tesi/commit/2f823cebee0cb8006523d9e0d6aaa673484bd928)), closes [#7](https://github.com/f-aguzzi/tesi/issues/7)
+
+
 ### Bug Fixes
 
+
 * wrong training procedure in SVM ([74d1741](https://github.com/f-aguzzi/tesi/commit/74d1741743f53eea6cc2d9002005c6426bf4f0d0))
 
+* add missing checks to LLDFSettings ([3d57752](https://github.com/f-aguzzi/tesi/commit/3d577527eefd0b183a66c378d53cb1f1ee506343)), closes [#20](https://github.com/f-aguzzi/tesi/issues/20)
+
+
+### chore
+
+* **thesis:** set up build system (merge from [#22](https://github.com/f-aguzzi/tesi/issues/22)) ([0b13ed3](https://github.com/f-aguzzi/tesi/commit/0b13ed346448f0eeefecbc6fd051eb7c98919650))
+
+
+### Refactor
+
+* extract split tests and graphs (merge [#23](https://github.com/f-aguzzi/tesi/issues/23)) ([6865c88](https://github.com/f-aguzzi/tesi/commit/6865c88d70b650de5e8440807b0194022a15dc0e))
+
+
+### CI
+
+* **release:** 1.1.0-beta.1 [skip ci] ([2deffcc](https://github.com/f-aguzzi/tesi/commit/2deffcc4c8a29d09a4a644558e491d770f71f6dc)), closes [#7](https://github.com/f-aguzzi/tesi/issues/7)
+* **release:** 1.1.0-beta.2 [skip ci] ([25704dc](https://github.com/f-aguzzi/tesi/commit/25704dc4eb0cbc249bbf85611c5dfe257ebccc30)), closes [#20](https://github.com/f-aguzzi/tesi/issues/20) [#22](https://github.com/f-aguzzi/tesi/issues/22) [#23](https://github.com/f-aguzzi/tesi/issues/23)
+
+
 ## [1.1.0-beta.2](https://github.com/f-aguzzi/tesi/compare/v1.1.0-beta.1...v1.1.0-beta.2) (2024-05-20)
 
 
 ### Bug Fixes
 
 * add missing checks to LLDFSettings ([3d57752](https://github.com/f-aguzzi/tesi/commit/3d577527eefd0b183a66c378d53cb1f1ee506343)), closes [#20](https://github.com/f-aguzzi/tesi/issues/20)
```

### Comparing `chemfusekit-1.1.0b3/cda_example_notebook.ipynb` & `chemfusekit-1.1.1b1/cda_example_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/requirements-dev.lock` & `chemfusekit-1.1.1b1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/requirements.lock` & `chemfusekit-1.1.1b1/requirements.lock`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/.github/workflows/gh_pages.yml` & `chemfusekit-1.1.1b1/.github/workflows/gh_pages.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/.github/workflows/pylint.yml` & `chemfusekit-1.1.1b1/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/.github/workflows/release.yml` & `chemfusekit-1.1.1b1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/.github/workflows/thesis.yml` & `chemfusekit-1.1.1b1/.github/workflows/thesis.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/.github/workflows/unittest.yml` & `chemfusekit-1.1.1b1/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/chemfusekit/__utils.py` & `chemfusekit-1.1.1b1/chemfusekit/__utils.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/chemfusekit/knn.py` & `chemfusekit-1.1.1b1/chemfusekit/knn.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/chemfusekit/lda.py` & `chemfusekit-1.1.1b1/chemfusekit/lda.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/chemfusekit/lldf.py` & `chemfusekit-1.1.1b1/chemfusekit/lldf.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/chemfusekit/lr.py` & `chemfusekit-1.1.1b1/chemfusekit/lr.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/chemfusekit/pca.py` & `chemfusekit-1.1.1b1/chemfusekit/pca.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/chemfusekit/plsda.py` & `chemfusekit-1.1.1b1/chemfusekit/plsda.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/chemfusekit/svm.py` & `chemfusekit-1.1.1b1/chemfusekit/svm.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/README.md` & `chemfusekit-1.1.1b1/docs/README.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/docusaurus.config.js` & `chemfusekit-1.1.1b1/docs/docusaurus.config.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/package-lock.json` & `chemfusekit-1.1.1b1/docs/package-lock.json`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/package.json` & `chemfusekit-1.1.1b1/docs/package.json`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/sidebars.js` & `chemfusekit-1.1.1b1/docs/sidebars.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/docs/complete-workflow.md` & `chemfusekit-1.1.1b1/docs/docs/complete-workflow.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/docs/tutorial.md` & `chemfusekit-1.1.1b1/docs/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/docs/knn/knn.md` & `chemfusekit-1.1.1b1/docs/docs/knn/knn.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/docs/knn/knnsettings.md` & `chemfusekit-1.1.1b1/docs/docs/knn/knnsettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/docs/lda/lda.md` & `chemfusekit-1.1.1b1/docs/docs/lda/lda.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/docs/lda/ldasettings.md` & `chemfusekit-1.1.1b1/docs/docs/lda/ldasettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/docs/lldf/lldf.md` & `chemfusekit-1.1.1b1/docs/docs/lldf/lldf.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/docs/lldf/lldfsettings.md` & `chemfusekit-1.1.1b1/docs/docs/lldf/lldfsettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/docs/lr/lr.md` & `chemfusekit-1.1.1b1/docs/docs/lr/lr.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/docs/lr/lrsettings.md` & `chemfusekit-1.1.1b1/docs/docs/lr/lrsettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/docs/pca/pca.md` & `chemfusekit-1.1.1b1/docs/docs/pca/pca.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/docs/pca/pcasettings.md` & `chemfusekit-1.1.1b1/docs/docs/pca/pcasettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/docs/plsda/plsda.md` & `chemfusekit-1.1.1b1/docs/docs/plsda/plsda.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/docs/plsda/plsdasettings.md` & `chemfusekit-1.1.1b1/docs/docs/plsda/plsdasettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/docs/svm/svm.md` & `chemfusekit-1.1.1b1/docs/docs/svm/svm.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/docs/svm/svmsettings.md` & `chemfusekit-1.1.1b1/docs/docs/svm/svmsettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/src/components/HomepageFeatures/index.js` & `chemfusekit-1.1.1b1/docs/src/components/HomepageFeatures/index.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/src/css/custom.css` & `chemfusekit-1.1.1b1/docs/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/src/pages/index.js` & `chemfusekit-1.1.1b1/docs/src/pages/index.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/src/pages/project/continuous-integration.md` & `chemfusekit-1.1.1b1/docs/src/pages/project/continuous-integration.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/src/pages/project/process-model.md` & `chemfusekit-1.1.1b1/docs/src/pages/project/process-model.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/src/pages/project/project-philosophy.md` & `chemfusekit-1.1.1b1/docs/src/pages/project/project-philosophy.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/src/pages/project/project-plan.md` & `chemfusekit-1.1.1b1/docs/src/pages/project/project-plan.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/src/pages/project/requirements-specification.md` & `chemfusekit-1.1.1b1/docs/src/pages/project/requirements-specification.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/src/pages/project/use-cases.md` & `chemfusekit-1.1.1b1/docs/src/pages/project/use-cases.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/static/img/colab-logo.svg` & `chemfusekit-1.1.1b1/docs/static/img/colab-logo.svg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/static/img/docusaurus-social-card.jpg` & `chemfusekit-1.1.1b1/docs/static/img/docusaurus-social-card.jpg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/static/img/docusaurus.png` & `chemfusekit-1.1.1b1/docs/static/img/docusaurus.png`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/static/img/favicon.ico` & `chemfusekit-1.1.1b1/docs/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/static/img/happy-woman.svg` & `chemfusekit-1.1.1b1/docs/static/img/happy-woman.svg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/static/img/logo.svg` & `chemfusekit-1.1.1b1/docs/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/docs/static/img/magnifying-glass.svg` & `chemfusekit-1.1.1b1/docs/static/img/magnifying-glass.svg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/Beartype.md` & `chemfusekit-1.1.1b1/notes/Beartype.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/Constructors.md` & `chemfusekit-1.1.1b1/notes/Constructors.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/Conventional Commits.md` & `chemfusekit-1.1.1b1/notes/Conventional Commits.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/Kanban.md` & `chemfusekit-1.1.1b1/notes/Kanban.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/Use Case Diagram.md` & `chemfusekit-1.1.1b1/notes/Use Case Diagram.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/.obsidian/core-plugins-migration.json` & `chemfusekit-1.1.1b1/notes/.obsidian/core-plugins-migration.json`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/.obsidian/workspace.json` & `chemfusekit-1.1.1b1/notes/.obsidian/workspace.json`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/.obsidian/plugins/calendar/main.js` & `chemfusekit-1.1.1b1/notes/.obsidian/plugins/calendar/main.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/.obsidian/plugins/obsidian-kanban/main.js` & `chemfusekit-1.1.1b1/notes/.obsidian/plugins/obsidian-kanban/main.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/.obsidian/plugins/obsidian-kanban/styles.css` & `chemfusekit-1.1.1b1/notes/.obsidian/plugins/obsidian-kanban/styles.css`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/.obsidian/plugins/obsidian-plantuml/main.js` & `chemfusekit-1.1.1b1/notes/.obsidian/plugins/obsidian-plantuml/main.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/.obsidian/plugins/obsidian-plantuml/styles.css` & `chemfusekit-1.1.1b1/notes/.obsidian/plugins/obsidian-plantuml/styles.css`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/Devlog/2024-04-19.md` & `chemfusekit-1.1.1b1/notes/Devlog/2024-04-19.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/Devlog/2024-04-20.md` & `chemfusekit-1.1.1b1/notes/Devlog/2024-04-20.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/Devlog/2024-04-22.md` & `chemfusekit-1.1.1b1/notes/Devlog/2024-04-22.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/Devlog/2024-04-23.md` & `chemfusekit-1.1.1b1/notes/Devlog/2024-04-23.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/Devlog/2024-05-06.md` & `chemfusekit-1.1.1b1/notes/Devlog/2024-05-06.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/Devlog/2024-05-07.md` & `chemfusekit-1.1.1b1/notes/Devlog/2024-05-07.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/Devlog/2024-05-08.md` & `chemfusekit-1.1.1b1/notes/Devlog/2024-05-08.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/Devlog/2024-05-09.md` & `chemfusekit-1.1.1b1/notes/Devlog/2024-05-09.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/Devlog/2024-05-17.md` & `chemfusekit-1.1.1b1/notes/Devlog/2024-05-17.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/Devlog/2024-05-18.md` & `chemfusekit-1.1.1b1/notes/Devlog/2024-05-18.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/UML/Process state machine.md` & `chemfusekit-1.1.1b1/notes/UML/Process state machine.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/UML/Sequence.md` & `chemfusekit-1.1.1b1/notes/UML/Sequence.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/notes/UML/Use cases.md` & `chemfusekit-1.1.1b1/notes/UML/Use cases.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/tests/qepas.xlsx` & `chemfusekit-1.1.1b1/tests/qepas.xlsx`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/tests/rt.xlsx` & `chemfusekit-1.1.1b1/tests/rt.xlsx`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/tests/test_knn.py` & `chemfusekit-1.1.1b1/tests/test_knn.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/tests/test_lda.py` & `chemfusekit-1.1.1b1/tests/test_lda.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/tests/test_lldf.py` & `chemfusekit-1.1.1b1/tests/test_lldf.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/tests/test_lr.py` & `chemfusekit-1.1.1b1/tests/test_lr.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/tests/test_pca.py` & `chemfusekit-1.1.1b1/tests/test_pca.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/tests/test_plsda.py` & `chemfusekit-1.1.1b1/tests/test_plsda.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/tests/test_svm.py` & `chemfusekit-1.1.1b1/tests/test_svm.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/thesis/0-header.md` & `chemfusekit-1.1.1b1/thesis/0-header.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/thesis/1-abstract.md` & `chemfusekit-1.1.1b1/thesis/1-abstract.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/thesis/logo-unibg.png` & `chemfusekit-1.1.1b1/thesis/logo-unibg.png`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/pyproject.toml` & `chemfusekit-1.1.1b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "chemfusekit"
-version = "1.1.0b3"
+version = "1.1.1b1"
 description = "A minimal Python / Jupyter Notebook / Colab library for data fusion and chemometrical analysis."
 authors = [
     { name = "Federico Aguzzi", email = "62149513+f-aguzzi@users.noreply.github.com" }
 ]
 dependencies = [
     "numpy>=1.26.4",
     "scipy>=1.13.0",
```

### Comparing `chemfusekit-1.1.0b3/readme.md` & `chemfusekit-1.1.1b1/readme.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.0b3/PKG-INFO` & `chemfusekit-1.1.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: chemfusekit
-Version: 1.1.0b3
+Version: 1.1.1b1
 Summary: A minimal Python / Jupyter Notebook / Colab library for data fusion and chemometrical analysis.
 Author-email: Federico Aguzzi <62149513+f-aguzzi@users.noreply.github.com>
 Requires-Python: >=3.8
 Requires-Dist: beartype>=0.18.5
 Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: openpyxl>=3.1.2
```

